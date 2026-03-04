---
title: 에이전트 작업 및 AI 크레딧 사용량
description: Experience Cloud 애플리케이션의 에이전트 작업 및 AI 크레딧 사용률에 대해 알아봅니다.
solution: Experience Cloud
topic: Artificial Intelligence
feature: Agentic AI, AI Tools
role: Admin, User
level: Intermediate
source-git-commit: 1897e2162ba53ebc43a78877a61ebf4370127631
workflow-type: tm+mt
source-wordcount: '1001'
ht-degree: 4%

---

# Adobe Experience Platform 에이전트 작업 및 AI 크레딧 소비

업데이트 날짜: **2026년 3월 4일 목요일**

Experience Cloud 애플리케이션의 아젠틱 AI 작업 및 AI 신용 사용에 대해 알아봅니다. 기존 Experience Cloud 애플리케이션에서 Agentic AI 기능을 활성화하는 방법에 대한 자세한 내용은 [Experience Cloud의 Agentic AI](agentic-ai.md#existing-apps)를 참조하십시오.

## 에이전트 작업

_에이전트 작업_&#x200B;은(는) 고객 입력의 지시에 따라 특정 결과를 얻기 위해 에이전트가 실행하는 일련의 작업 및 작업입니다.

AI Assistant를 통해 자연어 프롬프트를 사용하면 에이전트에게 특정 작업을 수행하도록 요청할 수 있습니다. 이러한 입력을 기반으로 Agent Orchestrator은 관련 Experience Cloud 애플리케이션 내에서 각 단계를 실행하도록 적절한 에이전트를 조정합니다.

## AI 크레딧

_AI 크레딧_&#x200B;은 에이전트 작업의 실행을 수량화하는 사용 기반 지표입니다. AI 크레딧이 [AI 우선 애플리케이션](/help/interface/features/agentic-ai.md)에 적용되지 않습니다.

## AI 신용 소비

AI 크레딧 사용은 실행된 작업의 복잡성과 가치에 따라 달라질 수 있습니다.

* 간단한(종종 단일 단계) 작업은 더 적은 크레딧을 사용합니다
* 복잡한(종종 여러 단계) 작업이 더 많은 크레딧을 소비함
* 고급 추론, 유효성 검사, 다중 에이전트 조정 또는 통합과 관련된 작업은 더 많은 크레딧을 사용합니다.

### 예상 AI 크레딧 소비율

| 에이전트 | 작업 | 지원되는 애플리케이션 | 예상 AI 점수 | 샘플 프롬프트 |
| ------ | ----- | ------------------------ | ----------------------- | ----------------- |
| Audience 에이전트 | 대상자/계정 관념화 | <ul><li>Real-Time CDP (B2B, B2C 및 B2P 에디션)</li><li>Adobe Journey Optimizer(B2C Edition)</li></ul> | 50 | <ul><li>_부유한 구매자를 위한 필드 표시_</li><li>_고객 환경 설정과 관련된 모든 필드 찾기_</li></ul> |
| Audience 에이전트 | 지식 기반 대상/계정 생성 | <ul><li>Real-Time CDP (B2B, B2C 및 B2P 에디션)</li><li>Adobe Journey Optimizer(B2C Edition)</li></ul> | 150 | <ul><li>_캘리포니아에 거주하는 사람들로 구성된 대상자를 만듭니다_</li><li>_이번 분기에 1,000달러 이상 지출한 VIP 회원의 대상자 생성_</li><li>_의류 항목을 구입했지만 지난 60일 동안 구입하지 않은 사용자를 대상으로 대상 만들기_</li></ul> |
| Audience 에이전트 | 대상자 / 계정 관리 | <ul><li>Real-Time CDP (B2B, B2C 및 B2P 에디션)</li><li>Adobe Journey Optimizer(B2C Edition)</li></ul> | 25 | <ul><li>_중복 대상이 있습니까?_</li><li>_가장 큰 대상자 5명을 표시합니다._</li><li>_대상에 대해 활성화되지 않은 대상 표시_</li><li>_라이브 여정에 사용된 모든 대상 나열_</li></ul> |
| Audience 에이전트 | 대상자/계정 분석 | <ul><li>Real-Time CDP (B2B, B2C 및 B2P 에디션)</li><li>Adobe Journey Optimizer(B2C Edition)</li></ul> | 25 | <ul><li>_지난 주에 20% 이상 증가한 대상은 무엇입니까?_</li><li>_30일 전 값과 비교하여 대상 &quot;단골 플래티넘&quot;이 얼마나 변경되었습니까?_</li><li>_가장 빠르게 성장하는 대상자는 무엇입니까?_</li></ul> |
| Audience 에이전트 | 구매 그룹 관념화 | <ul><li>Adobe Journey Optimizer(B2B edition)</li></ul> | 25 | <ul><li>_이 제품에 대한 의도를 표시하는 계정은 무엇입니까?_</li><li>_XYZ의 제품 의도로 최상위 사용자를 보여 주십시오._</li><li>_5명 이상의 회원이 있는 구매 그룹_</li></ul> |
| Data Insights Agent | 데이터 분석 및 시각화 | <ul><li>Customer Journey Analytics (B2C 및 B2B 에디션)</li></ul> | 25 | <ul><li>_7월 주문 트렌드_</li><li>_지역별 매출을 표시합니다._</li><li>_3월부터 6월까지 성별 주문 표시_</li><li>_6월 수익별 상위 10개 SKU는 무엇입니까_</li><li>_연간 월별 구매 비율_</li><li>_제품 범주별 매출 점유율_</li></ul> |
| Journey Agent | 여정 관념화 | <ul><li>Adobe Journey Optimizer(B2B edition)</li></ul> | 25 | <ul><li>_웹 사이트에서 콘텐츠에 관여하는 사람들에게 초점을 맞추어 내 솔루션을 위한 여정을 만들어 스페이스 계정을 만드세요_</li></ul> |
| Journey Agent | 여정 생성 | <ul><li>Adobe Journey Optimizer (B2B 및 B2C 에디션)</li></ul> | 30 | <ul><li>_지난 7일 동안 첫 구매를 완료하지 않은 사용자에게 미리 알림을 보낼 여정을 생성합니다._</li><li>_사용자가 첫 구매를 완료하면 3일 후 이메일로 SMS 확인 및 후속 혜택 설명을 보내세요_</li></ul> |
| Journey Agent | 여정 분석 | <ul><li>Adobe Journey Optimizer (B2B 및 B2C 에디션)</li></ul> | 50 | <ul><li>_7월 4일 여정에 대한 노드별 폴아웃을 분석하려고 합니다._</li><li>_여정 X에 대해 일정 충돌이 있습니까_</li><li>_여정 X에 대한 대상 겹침 표시_</li></ul> |
| Journey Agent | 여정 관리 | <ul><li>Adobe Journey Optimizer (B2B 및 B2C 에디션)</li></ul> | 25 | <ul><li>_라이브 여정이 몇 개나 있습니까?_</li><li>_대상 X를 사용하여 모든 여정 나열._</li><li>_현재 테스트 모드에 있는 모든 여정 나열_</li></ul> |
| 제품 지원 에이전트 | 지식 기반 문제 해결 | <ul><li>Real-Time CDP (B2B, B2C 및 B2P 에디션)</li><li>Adobe Journey Optimizer (B2C 및 B2B 에디션)</li><li>Customer Journey Analytics (B2C 및 B2B 에디션)</li></ul> | 0 | <ul><li>_라이선스 사용 대시보드와 Experience Platform 홈 페이지에서 프로필 수가 다른 이유는 무엇입니까?_</li><li>_여정이 트리거되지 않는 이유는 무엇입니까?_</li><li>_Adobe Experience Platform에서 실시간 경험을 만드는 방법은 무엇입니까?_</li><li>_Adobe Experience Platform에서 경고를 구성하고 사용하는 방법은 무엇입니까?_</li><li>_Adobe Experience Platform 활성화의 평균 프로필 풍부도 제한은 얼마입니까?_</li></ul> |
| 제품 지원 에이전트 | 지원 사례 만들기 및 추적 | <ul><li>Real-Time CDP (B2B, B2C 및 B2P 에디션)</li>Adobe Journey Optimizer (B2C 및 B2B 에디션)<li>Customer Journey Analytics (B2C 및 B2B 에디션)</li><li>Adobe Experience Manager</li></ul> | 10 | <ul><li>_실패한 세분화 작업에 대한 새 지원 티켓 만들기_</li><li>_티켓 전자 메일의 001772068이 무엇입니까?_</li></ul> |
| 콘텐츠 관리자 에이전트 | 콘텐츠 검색 | <ul><li>Adobe Experience Manager</li></ul> | 5 | <ul><li>_WKND 오퍼 캠페인을 만들기 위한 콘텐츠 조각을 표시합니다._</li><li>_제품 패키지 PNG 이미지를 찾습니다._</li><li>_WKND 폴더에 태그가 지정된 Office 이미지를 표시합니다._</li><li>_WKND 폴더에 svgs가 있습니까?_</li><li>_대출 신청서 양식을 모두 표시합니다._</li><li>_직원 온보딩 양식을 찾고 있습니다._</li></ul> |
| 콘텐츠 관리자 에이전트 | <ul><li>콘텐츠 최적화</li></ul> | <ul><li>Adobe Experience Manager Assets 및 Dynamic Media</li></ul> | 10 | <ul><li>_2000px 렌디션을 JPEG으로 80% 품질로 만듭니다._</li><li>_Instagram 스토리에 대한 렌디션을 만듭니다._</li><li>_이미지 위에 30% 할인 그래픽으로 이미지를 오버레이하여 중앙에서 100px를 배치합니다._</li><li>_PNG의 배경색을 #ff8932._</li></ul> |
| 브랜드 거버넌스 에이전트 | <ul><li>브랜드 정책 확인</li></ul><ul><li>Content Hub을 사용한 권한</li></ul><ul><li>파이프라인 문제 해결</li></ul> | <ul><li>Adobe Experience Manager Sites(브랜드 정책)</li></ul><ul><li>Adobe Experience Manager Assets</li></ul> | 25 | <ul><li>_이 페이지가 내 브랜드와 일치합니까?`https://www.website/en.html`_</li><li>_기존 Content Hub ABAC 규칙 모두 표시_</li><li>_내 자산이 곧 만료됩니까?_</li></ul> |
| 브랜드 경험 에이전트 | <ul><li>콘텐츠 업데이트</li><li>Forms 제작</li><li>파이프라인 문제 해결</li></ul> | <ul><li>Adobe Experience Manager 클라우드 서비스</li><li>Adobe Experience Manager Sites</li><li>Adobe Experience Manager Forms</li></ul> | 50 | <ul><li>_이름, 전자 메일 및 메시지 필드가 있는 연락처 양식을 만듭니다_</li><li>_실패한 파이프라인 문제 해결_</li><li>_주 프로그램에 대해 실패한 파이프라인을 나열합니다._</li></ul> |

>[!NOTE]
>
>실제 AI 크레딧 소비는 실행된 단계 수와 단계당 반복 횟수에 따라 달라질 수 있습니다.

## 이 항목에 대한 추가 도움말

* [Experience Cloud의 아젠틱 AI](/help/interface/features/agentic-ai.md)
* [Adobe Experience Platform 에이전트 사용 바인딩된 평가판](https://experienceleague.adobe.com/ko/docs/experience-cloud-ai/experience-cloud-ai/agents/trial)
