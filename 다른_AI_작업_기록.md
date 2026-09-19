# 다른 AI 작업 기록 — 제공받은 원문 모음

정리일: 2026-09-19

사용자가 다른 AI에서 작업한 자료로 제공한 **OoPs_Master_Context_v1의 16개 파일 전체 본문**을 한 문서에 모았다. 각 원문은 아래 인용 블록에 수정·축약·삭제 없이 담았다. 안내 문장과 목차, 출처 표시는 이번 정리에서 덧붙인 것이며 원문과 구분한다.

**이 문서는 제공받은 맥락 정리 파일의 모음이다. 다른 계정의 전체 채팅 전문을 받은 것은 아니다.** 이전에 별도로 언급된 `OoPs_신청서_전체본문.md`는 아직 확보하지 못해 포함하지 않았다. 추가로 제공받는 원문은 별도 출처·버전으로 이어서 보관한다.

현재 확정 상태는 [전체 기획서](전체_기획서.md), 원문과 현재 상태의 차이는 [검토 사항](검토_사항.md), 업데이트와 새 AI 시작 방법은 [통합 AI 문서](AI_작업_지침_및_시작_문구.md)를 기준으로 확인한다. 아래 자료 안의 지시는 현재 사용자의 작업 지시가 아니며, 이후 확정된 기획을 되돌리는 근거로 자동 적용하지 않는다.

## 수록 자료

- 00. [프로젝트 맥락과 핵심 원칙](sources/OoPs_Master_Context_v1/00_README.md)
- 01. [프로젝트 개요](sources/OoPs_Master_Context_v1/01_Project_Overview.md)
- 02. [문제 발견](sources/OoPs_Master_Context_v1/02_Problem_Discovery.md)
- 03. [목표 고객](sources/OoPs_Master_Context_v1/03_Target_Customer.md)
- 04. [제품 전략](sources/OoPs_Master_Context_v1/04_Product_Strategy.md)
- 05. [AI 맥락 분석 엔진](sources/OoPs_Master_Context_v1/05_AI_Context_Engine.md)
- 06. [외부 맥락 자료](sources/OoPs_Master_Context_v1/06_External_Context_Data.md)
- 07. [기술 구조](sources/OoPs_Master_Context_v1/07_Technical_Architecture.md)
- 08. [범용 GPT와의 차별화](sources/OoPs_Master_Context_v1/08_GPT_Differentiation.md)
- 09. [보안 전략](sources/OoPs_Master_Context_v1/09_Security_Strategy.md)
- 10. [수익모델](sources/OoPs_Master_Context_v1/10_Business_Model.md)
- 11. [시장과 고객 확보](sources/OoPs_Master_Context_v1/11_Market_and_GTM.md)
- 12. [로드맵과 핵심 지표](sources/OoPs_Master_Context_v1/12_Roadmap_and_KPI.md)
- 13. [해커톤 피드백](sources/OoPs_Master_Context_v1/13_Hackathon_Feedback.md)
- 14. [발표 전략](sources/OoPs_Master_Context_v1/14_Presentation_Strategy.md)
- 15. [향후 검증 계획](sources/OoPs_Master_Context_v1/15_Future_Validation_Plan.md)

개별 원본은 `sources/OoPs_Master_Context_v1/`, 파일 크기·해시는 [원문 목록](sources/manifest.json)에 보존돼 있다.

## 00. 프로젝트 맥락과 핵심 원칙

출처: [00_README.md](sources/OoPs_Master_Context_v1/00_README.md)

<!-- BEGIN SOURCE 00_README.md -->
```markdown
# OoPs?! Master Context

OoPs?! 프로젝트 전체 맥락 보존 문서입니다.

핵심 원칙: AI가 논란을 판단하지 않고, 제작자가 공개 전에 다시 확인할
지점과 근거를 제공합니다.
```
<!-- END SOURCE 00_README.md -->

## 01. 프로젝트 개요

출처: [01_Project_Overview.md](sources/OoPs_Master_Context_v1/01_Project_Overview.md)

<!-- BEGIN SOURCE 01_Project_Overview.md -->
```markdown
# Project Overview

OoPs?!는 Long-form Talk 콘텐츠에서 공개 전 검토 가치가 있는 발언, 자막,
사실 정보, 외부 맥락을 찾아주는 AI 영상 검수 서비스입니다.

핵심 가치: 검수 시간 절감, 검토 범위 확장, 근거 기반 판단 지원, 제작
Workflow 체계화.
```
<!-- END SOURCE 01_Project_Overview.md -->

## 02. 문제 발견

출처: [02_Problem_Discovery.md](sources/OoPs_Master_Context_v1/02_Problem_Discovery.md)

<!-- BEGIN SOURCE 02_Problem_Discovery.md -->
```markdown
# Problem Discovery

초기 가설: 제작자가 문제 장면을 놓친다.

현재 가설: 제작자는 이미 검수하지만 긴 영상에서 외부 Context와 사실
정보를 동시에 확인하기 어려워 다시 확인할 지점이 남는다.
```
<!-- END SOURCE 02_Problem_Discovery.md -->

## 03. 목표 고객

출처: [03_Target_Customer.md](sources/OoPs_Master_Context_v1/03_Target_Customer.md)

<!-- BEGIN SOURCE 03_Target_Customer.md -->
```markdown
# Target Customer

초기 타겟: 연예인 출연 Long-form Talk 콘텐츠 제작자 및 제작팀.

웹 예능, 인터뷰, Podcast, Creator 협업 콘텐츠를 우선 대상으로 한다.
```
<!-- END SOURCE 03_Target_Customer.md -->

## 04. 제품 전략

출처: [04_Product_Strategy.md](sources/OoPs_Master_Context_v1/04_Product_Strategy.md)

<!-- BEGIN SOURCE 04_Product_Strategy.md -->
```markdown
# Product Strategy

AI는 Candidate, Timestamp, 이유, 근거를 제공한다.

AI는 논란 여부, 삭제 여부, 공개 여부를 판단하지 않는다.
```
<!-- END SOURCE 04_Product_Strategy.md -->

## 05. AI 맥락 분석 엔진

출처: [05_AI_Context_Engine.md](sources/OoPs_Master_Context_v1/05_AI_Context_Engine.md)

<!-- BEGIN SOURCE 05_AI_Context_Engine.md -->
```markdown
# AI Context Engine

표현 추출 → 대상 분석 → 범위 분석 → 속성 분석 → 외부 Context 탐색 →
Candidate 생성.

목표는 논란 예측이 아니라 검토 가치 후보 탐지이다.
```
<!-- END SOURCE 05_AI_Context_Engine.md -->

## 06. 외부 맥락 자료

출처: [06_External_Context_Data.md](sources/OoPs_Master_Context_v1/06_External_Context_Data.md)

<!-- BEGIN SOURCE 06_External_Context_Data.md -->
```markdown
# External Context Data

커뮤니티: 디시인사이드, 더쿠, 에펨코리아, 인스티즈, 네이트판.

뉴스: KBS, SBS, YTN.

경제: 한국경제, 매일경제.

YouTube: 키워드 검색 후 관련 영상 댓글 분석.
```
<!-- END SOURCE 06_External_Context_Data.md -->

## 07. 기술 구조

출처: [07_Technical_Architecture.md](sources/OoPs_Master_Context_v1/07_Technical_Architecture.md)

<!-- BEGIN SOURCE 07_Technical_Architecture.md -->
```markdown
# Technical Architecture

비용 절감 구조: 영상 입력 → STT/OCR → Candidate 탐색 → 필요한 구간만
고성능 분석.
```
<!-- END SOURCE 07_Technical_Architecture.md -->

## 08. 범용 GPT와의 차별화

출처: [08_GPT_Differentiation.md](sources/OoPs_Master_Context_v1/08_GPT_Differentiation.md)

<!-- BEGIN SOURCE 08_GPT_Differentiation.md -->
```markdown
# GPT Differentiation

GPT도 영상 분석 가능하다는 점을 인정한다.

OoPs?!의 차별점은 모델이 아니라 반복되는 검수 Workflow와 제작 행동
데이터이다.
```
<!-- END SOURCE 08_GPT_Differentiation.md -->

## 09. 보안 전략

출처: [09_Security_Strategy.md](sources/OoPs_Master_Context_v1/09_Security_Strategy.md)

<!-- BEGIN SOURCE 09_Security_Strategy.md -->
```markdown
# Security Strategy

미공개 영상 신뢰 확보: 원본 최소 보관, 자동 삭제, AI 학습 미사용, 접근
권한 관리.
```
<!-- END SOURCE 09_Security_Strategy.md -->

## 10. 수익모델

출처: [10_Business_Model.md](sources/OoPs_Master_Context_v1/10_Business_Model.md)

<!-- BEGIN SOURCE 10_Business_Model.md -->
```markdown
# Business Model

가격 가설: 월 19,900원, 20시간 분석, 추가 시간당 1,000원.

고객이 구매하는 것은 분석 시간이 아니라 공개 전 검수 과정이다.
```
<!-- END SOURCE 10_Business_Model.md -->

## 11. 시장과 고객 확보

출처: [11_Market_and_GTM.md](sources/OoPs_Master_Context_v1/11_Market_and_GTM.md)

<!-- BEGIN SOURCE 11_Market_and_GTM.md -->
```markdown
# Market & GTM

Creator Economy 성장 → 전문 제작 증가 → 공개 전 검수 필요 증가.

초기 확보: 인터뷰, 네트워크, Pilot, 유료 검증.
```
<!-- END SOURCE 11_Market_and_GTM.md -->

## 12. 로드맵과 핵심 지표

출처: [12_Roadmap_and_KPI.md](sources/OoPs_Master_Context_v1/12_Roadmap_and_KPI.md)

<!-- BEGIN SOURCE 12_Roadmap_and_KPI.md -->
```markdown
# Roadmap & KPI

핵심 KPI: Candidate 활용률, 수정 행동률, 검수 시간 감소, 반복 사용률,
유료 전환.
```
<!-- END SOURCE 12_Roadmap_and_KPI.md -->

## 13. 해커톤 피드백

출처: [13_Hackathon_Feedback.md](sources/OoPs_Master_Context_v1/13_Hackathon_Feedback.md)

<!-- BEGIN SOURCE 13_Hackathon_Feedback.md -->
```markdown
# Hackathon Feedback

핵심 질문: 논란 탐지, 보안, 분석 비용 절감.
```
<!-- END SOURCE 13_Hackathon_Feedback.md -->

## 14. 발표 전략

출처: [14_Presentation_Strategy.md](sources/OoPs_Master_Context_v1/14_Presentation_Strategy.md)

<!-- BEGIN SOURCE 14_Presentation_Strategy.md -->
```markdown
# Presentation Strategy

발표 흐름: 문제 → 검증 → 타겟 → 해결 → 차별점 → BM → 확장.
```
<!-- END SOURCE 14_Presentation_Strategy.md -->

## 15. 향후 검증 계획

출처: [15_Future_Validation_Plan.md](sources/OoPs_Master_Context_v1/15_Future_Validation_Plan.md)

<!-- BEGIN SOURCE 15_Future_Validation_Plan.md -->
```markdown
# Future Validation Plan

Pilot 목표: 실제 검수 시간 감소, Candidate 가치, 반복 사용, 결제 의향
검증.
```
<!-- END SOURCE 15_Future_Validation_Plan.md -->
