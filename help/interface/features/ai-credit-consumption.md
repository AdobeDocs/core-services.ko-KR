---
title: 에이전트 작업 및 AI 크레딧 사용량
description: Experience Cloud 애플리케이션의 에이전트 작업 및 AI 크레딧 사용률에 대해 알아봅니다.
solution: Experience Cloud
topic: Artificial Intelligence
feature: Agentic AI, AI Tools
role: Admin, User
level: Intermediate
source-git-commit: bb6adf13bed37d4a885b5baec28199efade592e1
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 3%

---

# Adobe Experience Platform 에이전트 작업 및 AI 크레딧 소비

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
| ------ |-----|------------------------|----------------------|----------------|
| Audience 에이전트 | 대상자/계정 관념화 | <ul><li>Real-Time CDP (B2B, B2C 및 B2P 에디션)</li><li>Adobe Journey Optimizer(B2C Edition)</li></ul> | 50 | <ul><li>부유한 구매자를 위한 필드 표시</li><li>고객 환경 설정과 관련된 모든 필드 찾기</li></ul> |
| Audience 에이전트 | 지식 기반 대상/계정 생성 | <ul><li>Real-Time CDP (B2B, B2C 및 B2P 에디션)</li><li>Adobe Journey Optimizer(B2C Edition)</li></ul> | 150 | <ul><li>California에 거주하는 사람들로 구성된 대상자 만들기</li><li>이번 분기에 1,000달러 이상을 지출한 VIP 멤버 대상 생성</li><li>의류 항목을 구매했지만 지난 60일 동안 구매하지 않은 사용자의 대상을 작성합니다</li></ul> |
| Audience 에이전트 | 대상자 / 계정 관리 | <ul><li>Real-Time CDP (B2B, B2C 및 B2P 에디션)</li><li>Adobe Journey Optimizer(B2C Edition)</li></ul> | 25 | <ul><li>중복 대상이 있습니까?</li><li>5명의 가장 큰 대상자를 보여 주세요.</li><li>대상에 활성화되지 않은 대상자 표시</li><li>라이브 여정에 사용된 모든 대상 나열</li></ul> |
| Audience 에이전트 | 대상자/계정 분석 | <ul><li>Real-Time CDP (B2B, B2C 및 B2P 에디션)</li><li>Adobe Journey Optimizer(B2C Edition)</li></ul> | 25 | <ul><li>지난 주에 20% 이상 증가한 대상은 무엇입니까?</li><li>30일 전의 값과 비교하여 대상 &quot;충성도 플래티넘&quot;은 얼마나 변경되었습니까?</li><li>가장 빠르게 성장하는 대상자는 어디입니까?</li></ul> |
| Audience 에이전트 | 구매 그룹 관념화 | <ul><li>Adobe Journey Optimizer(B2B edition)</li></ul> | 25 | <ul><li>어떤 계정이 이 제품에 대한 의도를 보여 줍니까?</li><li>XYZ의 제품 의도에 따라 최고의 사용자를 보여 주십시오.</li><li>5명 이상의 회원을 보유한 구매 그룹은 무엇입니까?</li></ul> |
| Data Insights Agent | 데이터 분석 및 시각화 | <ul><li>Customer Journey Analytics (B2C 및 B2B 에디션)</li></ul> | 25 | <ul><li>7월의 주문 트렌드</li><li>지역별 매출을 표시합니다.</li><li>3월부터 6월까지 성별 주문을 표시합니다.</li><li>6월 수익별 상위 10개 SKU는 무엇입니까?</li><li>연간 월별 구매 비율</li><li>제품 범주별 매출 점유율</li></ul> |
| Journey Agent | 여정 관념화 | <ul><li>Adobe Journey Optimizer(B2B edition)</li></ul> | 25 | <ul><li>웹 사이트의 콘텐츠에 관여하는 사람들을 중심으로 내 솔루션을 위한 목적으로 공백 계정에 대한 여정을 만듭니다.</li></ul> |
| Journey Agent | 여정 생성 | <ul><li>Adobe Journey Optimizer (B2B 및 B2C 에디션)</li></ul> | 30 | <ul><li>지난 7일 동안 첫 구매를 완료하지 않은 사용자에게 미리 알림을 보낼 여정을 생성합니다</li><li>사용자가 첫 번째 구매를 완료하면 3일 후 이메일을 통해 SMS 확인 및 후속 혜택 설명을 보냅니다</li></ul> |
| Journey Agent | 여정 분석 | <ul><li>Adobe Journey Optimizer (B2B 및 B2C 에디션)</li></ul> | 50 | <ul><li>7월 4일 여정 캠페인에 대한 노드별 폴아웃을 분석하려고 합니다.</li><li>여정 X에 대해 일정 충돌이 있습니까</li><li>여정 X에 대한 대상 겹침 충돌 표시</li></ul> |
| Journey Agent | 여정 관리 | <ul><li>Adobe Journey Optimizer (B2B 및 B2C 에디션)</li></ul> | 25 | <ul><li>라이브 여정 수는 몇 개입니까?</li><li>대상 X를 사용하여 모든 여정을 나열합니다.</li><li>현재 테스트 모드에 있는 모든 여정 나열</li></ul> |
| 제품 지원 에이전트 | 지식 기반 문제 해결 | <ul><li>Real-Time CDP (B2B, B2C 및 B2P 에디션)</li><li>Adobe Journey Optimizer (B2C 및 B2B 에디션)</li><li>Customer Journey Analytics (B2C 및 B2B 에디션)</li></ul> | 0 | <ul><li>라이선스 사용 대시보드와 Experience Platform 홈 페이지에서 프로필 카운트가 다른 이유는 무엇입니까?</li><li>여정이 트리거되지 않는 이유는 무엇입니까?</li><li>Adobe Experience Platform은 어떻게 실시간 경험을 생성합니까?</li><li>Adobe Experience Platform에서 경고를 구성하고 사용하는 방법은 무엇입니까?</li><li>Adobe Experience Platform 활성화의 평균 프로필 풍부도 제한은 얼마입니까?</li></ul> |
| 제품 지원 에이전트 | 지원 사례 만들기 및 추적 | <ul><li>Real-Time CDP (B2B, B2C 및 B2P 에디션)</li>Adobe Journey Optimizer (B2C 및 B2B 에디션)<li>Customer Journey Analytics (B2C 및 B2B 에디션)</li><li>Adobe Experience Manager</li></ul> | 10 | <ul><li>실패한 세분화 작업에 대한 새 지원 티켓 만들기</li><li>E-001772068표 상태가 어떻게 되나요?</li></ul> |
| 콘텐츠 관리자 에이전트 | 콘텐츠 검색 | <ul><li>Adobe Experience Manager 클라우드 서비스</li></ul> | 5 | <ul><li>WKND 오퍼 캠페인을 만들기 위한 콘텐츠 조각을 표시합니다.</li><li>제품 패키징 PNG 이미지를 찾아보십시오.</li><li>WKND 폴더에 태그가 지정된 Office 이미지를 표시합니다.</li><li>WKND 폴더에 svgs가 있습니까?</li><li>대출 신청서 양식 모두 보여 주세요.</li><li>직원 온보딩 양식을 찾고 있습니다.</li></ul> |
| 콘텐츠 관리자 에이전트 | <ul><li>콘텐츠 업데이트</li><li>콘텐츠 최적화</li><li>Forms 제작</li></ul> | <ul><li>Adobe Experience Manager 클라우드 서비스</li></ul> | 10 | <ul><li>80% 품질의 2000px 렌디션을 JPEG으로 만듭니다.</li><li>Instagram 스토리에 대한 렌디션을 만듭니다.</li><li>이미지 위에 30% 할인 그래픽이 있는 이미지를 중앙에서 100px에 배치합니다.</li><li>PNG의 배경색을 PNG로 #ff8932.</li></ul> |
| 브랜드 경험 에이전트 | <ul><li>경험 지원</li><li>배포 지원</li></ul> | <ul><li>Adobe Experience Manager 클라우드 서비스</li></ul> | 5 | <ul><li>실패한 내 파이프라인 문제 해결</li><li>주 프로그램에 대해 실패한 내 파이프라인을 나열합니다.</li><li>&quot;개발 파이프라인&quot;이라는 실패한 내 파이프라인을 분석합니다.</li><li>파이프라인 실행 문제 1234567</li></ul> |
| 브랜드 경험 에이전트 | 사이트 현대화 | Adobe Experience Manager 클라우드 서비스 | 100 | <ul><li>페이지 마이그레이션 https://wknd-trendsetters.site</li></ul> |

>[!NOTE]
>
>실제 AI 크레딧 소비는 실행된 단계 수와 단계당 반복 횟수에 따라 달라질 수 있습니다.

## 이 항목에 대한 추가 도움말

* [Experience Cloud의 아젠틱 AI](/help/interface/features/agentic-ai.md)
* [Adobe Experience Platform 에이전트 사용 바인딩된 평가판](https://experienceleague.adobe.com/en/docs/experience-cloud-ai/experience-cloud-ai/agents/trial)