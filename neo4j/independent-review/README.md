# Neo4j 독립 점검 규칙

2026-10-29 사용자 확정 내용. 공통 기준 21개 각각에 진행 최소 정보·제외 조건·정보 부족 시 중단 범위를 추가한다. 공통 실행 원칙은 서버 코드·공통 프롬프트에서 관리한다. 이 폴더는 기준 데이터와 적재·조회 도구이며 AI 분석 엔진이 아니다.

## 데이터와 연결

- 대상 RuleSet: `ruleset:oops:all:0.4-draft`
- 독립 규칙 버전: `independent-review/1.0`
- 연결: `Criterion -HAS_REVIEW_GATE-> ReviewGate -HAS_CONTENT-> ContentBody`
- 본문: `minimum_information`, `exclusion_conditions`, `missing_information_scope`
- 규칙 21개, 본문 21개, 연결 42개를 추가한다. 기존 공통·추가 기준과 과거 사례 노드/본문을 변경하지 않는다.
- 기존 공통 본문은 Criterion의 직접 HAS_CONTENT로 계속 조회한다. 추가 기준은 독립 점검 통과 후에만 조회하며, 중단한 판단 범위를 상세 검토에도 전달한다.
- 진행 판정은 위험 확정이나 사용자 노출 승인이 아니다. 상세 검토·근거 검증을 거쳐야 한다.

## 파일

- `review_gate_rules.json`: 21개 확정 문안과 추가 노드·관계. 세 본문은 전체 기획서 표와 일치한다.
- `migrate_review_gates.py`: 기존 DB에 추가하는 전용 도구. DB 전체 재적재가 아니다.
- `read_rules.cypher`, `read_selected_rule.cypher`: 실제 세 규칙 본문 조회.
- `test_migration.py`: 오프라인 동작 계약 시험. 실제 DB/Cypher 통합 시험을 대신하지 않는다.

## 적용

사용자에게 제공하는 `oops-neo4j-all-review-rules.zip`은 기존 전체 자료와 이 규칙을 합친 통합 실행 묶음이다. 기존 `oops-neo4j-all`과 같은 상위 폴더에 압축을 풀고 새 폴더에서 `bash start.sh`를 실행한다. 기존 `.env`와 Docker 프로젝트·볼륨을 재사용한다. ZIP에는 비밀번호가 포함되지 않는다.

기존 DB에 전체 기준이 있으면 원래 자료는 읽기 검증만 하고 규칙 42개 노드·42개 관계만 한 트랜잭션에서 추가한다. 새 DB라면 기존 전체 자료를 먼저 적재하고 규칙을 추가한다. 규칙이 이미 정확히 있으면 재실행은 변경 없이 검증한다. 기존 규칙이 일부만 있거나 수동 수정된 경우 덮어쓰기 없이 중단한다. 적용 중 DB를 동시에 편집하지 않는다.

별도 서버에서 이 폴더만 적용할 때는 기존 전체 자료와 `OoPsEntity.id` 고유 제약이 있는 DB를 대상으로, Neo4j Python driver가 설치된 환경에서 `NEO4J_URI`, `NEO4J_USER`, `NEO4J_PASSWORD`, 선택 `NEO4J_DATABASE`를 환경변수로 설정한다. 자격 증명을 Git이나 명령 예시에 기록하지 않는다.

```bash
python migrate_review_gates.py          # 파일만 검증, DB 연결/쓰기 없음
python migrate_review_gates.py --apply  # 기존 DB에 추가, 기존 본문 덮어쓰기 없음
python migrate_review_gates.py --verify # DB 읽기 검증만 수행
python -m unittest -v test_migration
```

적용 로그의 `review_gate_bodies_read: 21`, `review_gate_fields_verified: 63`, `original_common_text_preserved: true`를 확인한다. 노트북 DB 실행을 확인하기 전에는 적재 완료로 기록하지 않는다. DB에 데이터가 추가돼도 기존 2단계 AI 서비스가 자동으로 독립 점검을 실행하지는 않는다. 백엔드 전달서의 흐름을 별도로 구현해야 한다.

기존 자료에서 수정한 본문은 유지되지만 새 규칙과의 의미적 정합성까지 적재 도구가 판정하지는 않는다. 기준 편집 이력이 있으면 서비스 투입 전 해당 조합을 검토한다.

## 공식 구현 참고

- https://neo4j.com/docs/python-manual/current/transactions/
- https://neo4j.com/docs/cypher-manual/current/clauses/merge/
