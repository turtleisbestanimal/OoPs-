# 자료 목록과 읽기 상태

## 사용자 첨부 자료 — 모두 대기

처음 목록 조회에서 아래 16개 파일의 이름과 크기를 확인했다. 이후 실제 본문을 읽기 전에 해당 폴더가 없어졌다. 따라서 **목록 확인만 했고 본문은 읽지 않았다.** 접근 권한을 받은 뒤에도 경로에 파일이 없었다. 사용자에게 현재 위치를 요청했다.

원래 폴더: `/Users/turtleisbestanimal/Downloads/OoPs_Master_Context_v1/`

- 00_README.md
- 01_Project_Overview.md
- 02_Problem_Discovery.md
- 03_Target_Customer.md
- 04_Product_Strategy.md
- 05_AI_Context_Engine.md
- 06_External_Context_Data.md
- 07_Technical_Architecture.md
- 08_GPT_Differentiation.md
- 09_Security_Strategy.md
- 10_Business_Model.md
- 11_Market_and_GTM.md
- 12_Roadmap_and_KPI.md
- 13_Hackathon_Feedback.md
- 14_Presentation_Strategy.md
- 15_Future_Validation_Plan.md

별도 첨부: `/Users/turtleisbestanimal/Downloads/OoPs_신청서_전체본문.md` (목록에서 20,289바이트 확인, 본문 미열람)

파일을 확보하면 원본 바이트 그대로 `sources/`에 보관하고 경로·크기·SHA-256·열람 결과를 기록한다. 현재는 원문 사본도 해시도 없다.

## 현재 대화

- 사용자가 제공한 사업·제품·팀·일정 설명과 이미지, 문서 작성 선호를 요약했다.
- 별도 원본 채팅 내보내기는 제공받지 않았다. 요약을 전체 대화 전문이라고 표시하지 않는다.
- 인터뷰·해커톤 성과·분석 사례·비용 수치는 사용자가 제공한 진술이다. 외부 검증 완료로 표시하지 않는다.

## 백엔드 참고 저장소

- 저장소: https://github.com/LikeLionHGU/oops_backend
- 코드 기준: `e6b7003` (main, 2026-08-20 커밋). 2026-09-19 원격 fetch로 확인.
- 이번에 전문을 읽은 비교 문서: `docs/프로젝트-현황-정리.md`, `docs/기획서-구현-격차분석.md`.
- 부분 확인 문서: `docs/API명세-구현-대조표.md`, `docs/개발자-인수인계.md`.
- 설정·코드 근거: `oops-backend/src/main/resources/application.yml`, `application-local.yml`, `oops-backend/build.gradle`, `oops-analysis/app/config.py`, `app/stt.py`, `app/ocr.py`, `requirements-core.txt`, `requirements-ocr.txt`, `OpenAiClient.java`, `StorageCleanupScheduler.java` 등.
- 저장소 조회는 운영 서버 로그인·실행 검증과 다르다. 확인 범위를 넘는 운영 상태는 미확인이다.

## 기획 기준 저장소

- 사용자가 이번 작업 도중 지정: https://github.com/turtleisbestanimal/OoPs-
- 초기 커밋: `57a5228`. 파일 목록은 `README.md` 하나였다.
- 이후 기획 맥락·검토 목록·작업 기록은 이 저장소에 모은다.
