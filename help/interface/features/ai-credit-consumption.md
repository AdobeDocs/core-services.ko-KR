---
title: 에이전트 작업 및 AI 크레딧 사용량
description: Experience Cloud 애플리케이션의 에이전트 작업 및 AI 크레딧 사용량에 대해 알아봅니다.
solution: Experience Cloud
topic: Artificial Intelligence
feature: Agentic AI, AI Tools
role: Admin, User
level: Intermediate
hidefromtoc: true
index: false
source-git-commit: 4f738324ee18bbb63ae8c1d45907ecaf05230b34
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 13%

---

# 에이전트 작업 및 AI 신용 소비

Experience Cloud 애플리케이션의 아젠틱 AI 작업 및 AI 신용 사용에 대해 알아봅니다.

## 에이전트 작업

_에이전트 작업_&#x200B;은(는) 고객 입력에 따라 특정 결과를 얻기 위해 에이전트가 실행하는 일련의 작업 및 작업입니다.

AI Assistant를 통해 자연어 프롬프트를 사용하면 에이전트에게 특정 작업을 수행하도록 요청할 수 있습니다. 이러한 입력을 기반으로 Agent Orchestrator은 관련 Experience Cloud 애플리케이션 내에서 각 단계를 실행하도록 적절한 에이전트를 조정합니다.

## AI 크레딧

_AI 크레딧_&#x200B;은 에이전트 작업의 실행을 수량화하는 사용 기반 지표입니다. AI 크레딧이 [AI 우선 애플리케이션](/help/interface/features/agentic-ai.md)에 적용되지 않습니다.

## AI 신용 소비

AI 크레딧 사용은 실행된 작업의 복잡성과 가치에 따라 달라질 수 있습니다.

* 간단한(종종 단일 단계) 작업은 더 적은 크레딧을 사용합니다
* 복잡한(종종 여러 단계) 작업이 더 많은 크레딧을 소비함
* 고급 추론, 유효성 검사, 다중 에이전트 조정 또는 통합과 관련된 작업은 더 많은 크레딧을 사용합니다.

### 예상 AI 크레딧 소비율

| 에이전트 | 작업 | 지원되는 애플리케이션 | 예상 AI 점수 |
|------|-----|------------------------|----------------------|
| Audience 에이전트 | 대상자/계정 관념화 | <ul><li>Real-Time CDP</li><li>Adobe Journey Optimizer</li></ul> | 50 |
| Audience 에이전트 | 지식 기반 대상/계정 생성 | <ul><li>Real-Time CDP</li><li>Adobe Journey Optimizer</li></ul> | 150 |
| Audience 에이전트 | 대상자/계정 관리 | <ul><li>Real-Time CDP</li><li>Adobe Journey Optimizer</li></ul> | 25 |
| Audience 에이전트 | 대상/계정 분석 | <ul><li>Real-Time CDP</li><li>Adobe Journey Optimizer</li></ul> | 25 |
| Audience 에이전트 | 구매 그룹 관념화 | <ul><li>Adobe Journey Optimizer (B2B)</li></ul> | 25 |
| Data Insights Agent | 데이터 분석 및 시각화 | <ul><li>Customer Journey Analytics</li></ul> | 25 |
| Journey Agent | 여정 관념화 | <ul><li>Adobe Journey Optimizer (B2B)</li></ul> | 25 |
| Journey Agent | 여정 생성 | <ul><li>Adobe Journey Optimizer (B2B, B2C)</li></ul> | 30 |
| Journey Agent | 여정 분석 | <ul><li>Adobe Journey Optimizer (B2B, B2C)</li></ul> | 50 |
| Journey Agent | 여정 관리 | <ul><li>Adobe Journey Optimizer (B2B, B2C)</li></ul> | 25 |
| 제품 지원 에이전트 | 지식 기반 문제 해결 | <ul><li>여러 Experience Cloud 애플리케이션</li></ul> | 0 |
| 제품 지원 에이전트 | 지원 사례 만들기 및 추적 | <ul><li>여러 Experience Cloud 애플리케이션</li></ul> | 10 |
| 콘텐츠 관리자 에이전트 | 콘텐츠 검색 | <ul><li>Adobe Experience Manager 클라우드 서비스</li></ul> | 5 |
| 콘텐츠 관리자 에이전트 | 콘텐츠 업데이트 및 최적화 | <ul><li>Adobe Experience Manager 클라우드 서비스</li></ul> | 10 |
| 브랜드 경험 에이전트 | 배포 지원 | <ul><li>Adobe Experience Manager 클라우드 서비스</li></ul> | 5 |
| 브랜드 경험 에이전트 | 사이트 현대화 | <ul><li>Adobe Experience Manager 클라우드 서비스</li></ul> | 100 |

>[!NOTE]
>
>실제 AI 크레딧 소비는 실행된 단계 수와 단계당 반복 횟수에 따라 달라질 수 있습니다.
