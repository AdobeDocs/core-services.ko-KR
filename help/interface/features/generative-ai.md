---
title: Experience Cloud 애플리케이션의 AI
description: Experience Cloud 애플리케이션이 생성 AI 및 AI Assistant를 사용하는 방법을 알아봅니다.
solution: Experience Cloud
feature: AI Assistant, Generative AI
topic: Administration
role: Admin
level: Intermediate
hide: false
hidefromtoc: true
index: n
exl-id: bdc51956-82aa-4aae-b627-a2018f80b5f5
source-git-commit: c6285bb87885d020275c6c0b4c003e912026ad20
workflow-type: tm+mt
source-wordcount: '1314'
ht-degree: 4%

---

# Experience Cloud 애플리케이션의 AI

이 페이지는 생성 AI와 Experience Cloud 애플리케이션에서 이를 사용하는 방법을 이해하는 데 도움이 됩니다. 생성 AI, AI Assistant를 사용하는 제품 기능과 Adobe Firefly 지원 여부를 알아봅니다.

## 생성 AI 및 AI Assistant 정보

생성 AI는 단순히 질문에 대한 답변 이상의 역할을 하는 인공 지능의 한 종류이다. _콘텐츠를 만들고_ _프롬프트_(질문 및 문)에 대해 _응답_&#x200B;합니다.

* **만들기:** AI가 교육 및 입력 프롬프트를 기반으로 처음부터 새 콘텐츠(텍스트, 이미지, 음악 또는 비디오)를 생성하는 기능을 나타냅니다. 이 기능은 생성 AI의 _생성_ 측면입니다.

* **응답:** AI가 특정 프롬프트에 대한 답변이나 반응을 제공하는 것으로, 일반적으로 지식 또는 추론 기능을 기반으로 합니다.

Experience Cloud을 처음 사용하는 경우 생성 AI를 사용하여 제품 지식을 빠르게 얻을 수 있습니다. 숙련된 사용자는 시간이 아닌 초 단위로 운영 통찰력을 발견할 수 있습니다.

### AI 어시스턴트

[AI Assistant](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/landing)은(는) Experience Platform 및 관련 애플리케이션에서 지원되는 대화 도구입니다. 워크플로우를 가속화하거나, 제품 지식을 개선하거나, 문제를 해결하거나, 정보를 검색하는 데 사용합니다. 특정 애플리케이션에서 AI Assistant를 사용하여 운영 통찰력을 즉시 발견할 수 있습니다.

Experience League의 제품 지식 응답은 링크를 통해 확인할 수 있고 인용됩니다. AI Assistant를 최대한 활용하기 위해 [목표 기반 프롬프트](https://experienceleague.adobe.com/ko/docs/experience-platform/ai-assistant/home)의 유형에 대해 알아봅니다.

## AI를 지원하는 기능이 있는 애플리케이션

* [GenStudio for Performance Marketing](#gspm)
* [AEM Sites(Cloud Service)에서 변형 생성](#aem-sites)
* [Journey Optimizer의 AI 어시스턴트](#journey-optimizer)
* [Adobe Journey Optimizer Prime 및 Ultimate](#ajo-prime-ultimate)
* [Journey Optimizer B2B 에디션](#ajo-b2b)
* [Journey Optimizer Prime 및 Ultimate의 AI 지원](#ajo-prime-ultimate)
* [Journey Optimizer B2B edition의 AI 지원](#ajo-b2b)
* [Campaign Managed Cloud Services의 AI 지원](#campaign-cs)
* [Customer Journey Analytics의 AI 지원](#cja)
* [Customer Journey Analytics의 지능형 캡션](#cja-captions)
* [Real-Time CDP의 AI 지원](#rtcdp)
* [Marketo의 Dynamic Chat](#marketo)
* [Workfront의 AI 지원](#workfront)

### GenStudio for Performance Marketing {#gspm}

[GenStudio for Performance Marketing](https://experienceleague.adobe.com/ko/docs/genstudio-for-performance-marketing/user-guide/home)은(는) 기능이 아니라 생성 AI 기반 플랫폼입니다. AI의 생성 기능은 마케팅 콘텐츠가 생성, 검토, 공유 및 분석되는 방식을 전환합니다.

[만들기](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/create/overview) 홈에서 고성능의 브랜드 내 경험을 만들 수 있습니다. 콘텐츠 생성 대상:

* 이메일
* 메타 광고
* LinkedIn 광고
* 광고 표시
* 배너

예, 고객 담당자 및 제품에 대한 설명, 브랜드 지침을 사용하여 GenStudio for Performance Marketing에서 브랜드에 대한 교육을 실시할 수도 있습니다. [자세히 알아보기...](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/create/overview)

**Adobe Firefly과 호환:** 예정

### Experience Manager Sites에서 변형 생성 {#aem-sites}

AEM Sites에서 [변형 생성](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations)은(는) 생성 AI를 사용하여 프롬프트에 따라 콘텐츠 변형을 만듭니다. 이러한 프롬프트는 [Adobe](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#get-started)에서 제공하거나 [사용자](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#create-prompt)에서 만들고 관리합니다.

변형을 만든 후에는 웹 사이트의 콘텐츠를 사용하고 Edge Delivery Services의 실험 기능을 사용하여 성공을 측정할 수 있습니다.

### 입력 및 출력 필드

입력 필드는 다음과 같습니다.

* 생성할 변형 수
* Audience Source
* 대상 타겟
* 추가 컨텍스트
* 고객 중심 프롬프트

출력은 생성된 콘텐츠 또는 마켓 카피입니다.

Firefly의 생성 AI 기능을 사용하여 Adobe Express에서 이미지를 생성하는 옵션도 있습니다. [자세히 알아보기...](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#generate-image)

**Adobe Firefly 호환:** 예

## Journey Optimizer의 AI 어시스턴트 {#journey-optimizer}

Journey Optimizer에서 AI Assistant를 통해 제품 지식과 운영 통찰력을 얻을 수 있습니다.

**제품 정보:** AI Assistant가 제품 insight에 대한 Adobe 데이터 저장소(예: Experience League 제품 설명서)에 대해 쿼리합니다. 결과는 고객이 알 수 없습니다.

예:

* _하나의 Adobe Journey Optimizer 샌드박스에서 몇 개의 라이브 활동을 사용할 수 있습니까?_

**Operational Insights(Beta)** - AI Assistant는 여정에 대한 중앙 집중식 운영 데이터가 포함된 고객별 Operational Insights 데이터 저장소를 쿼리하고 고객의 샌드박스로 분할합니다. 이 기능은 비즈니스 개체에서만 메타데이터를 가져오고 샌드박스 내의 데이터에 액세스하지 않습니다.

예제 프롬프트:

* _지난 7일 동안 만들어진 여정 수는 몇 개입니까?_

Operational Insights 출력은 고객의 비즈니스 개체에서 가져온 메타데이터에 따라 다릅니다. 이 출력은 고객을 구분하지 않습니다.

_여정_&#x200B;은(는) Journey Optimizer에서 AI Assistant에 사용할 수 있는 유일한 개체이며 현재 샌드박스에서 메타데이터를 가져옵니다. [추가 정보...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/ai-assistant).

**Adobe Firefly과 호환:** 아니요

## Journey Optimizer Prime 및 Ultimate의 AI 지원 {#ajo-prime-ultimate}

Journey Optimizer Prime 및 Ultimate에서는 [AI Assistant for Content Accelerator](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative)를 사용하여 텍스트 및 이미지에 대한 사전 예방적 콘텐츠 변형 제안을 제공합니다.

이 기능은 [이메일](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-email), [푸시 알림](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-push), [웹 페이지](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-web), [콘텐츠](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-experimentation) 및 [SMS](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-sms) 채널에서 사용할 수 있습니다. 프롬프트 기반 텍스트 및 이미지 생성을 제공합니다.

**참고:** AJO Prime 및 Ultimate의 Content Accelerator에서 출력되는 내용은 손실됩니다.

**Adobe Firefly 호환:** 예

## Journey Optimizer B2B edition의 AI 지원 {#ajo-b2b}

Journey Optimizer B2B edition은 제품 정보 프롬프트에 따라 [AI Assistant](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/ai-assistant/ai-assistant-overview)를 사용하여 제품 지식을 지원합니다.

**제품 지식** - 제품 insight에 대한 Adobe 데이터 저장소(예: Experience League 제품 설명서)를 쿼리합니다. 이 출력은 고객을 구분하지 않습니다.

* **입력:** 계정 여정에서 전자 메일을 보내는 방법

* **출력:** 제품 지식을 Experience League(공개 설명서)에서 가져옵니다. [자세히 알아보기...](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/ai-assistant/question-guidance)

**Adobe Firefly과 호환:** 아니요

## Campaign Managed Cloud Services의 AI 지원 {#campaign-cs}

Campaign Managed Cloud Services는 [콘텐츠 가속기용 AI 도우미](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-gs)를 사용합니다. 이 기능을 사용하면 마케팅 목표를 기반으로 개인화되고, 매력적이며, 효과적인 콘텐츠를 자동 생성할 수 있으며, 브랜드 윤곽선 스타일, 레이아웃, 색조 등에 최적화된 콘텐츠를 사용할 수 있습니다. [이메일](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-content), [SMS](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-sms), [푸시](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-push) 등의 채널에서 사용할 수 있습니다.

**참고:** Campaign Managed Cloud Services의 Content Accelerator에서 출력되는 내용은 손실되지 않습니다.

**Adobe Firefly 호환:** 예

## Customer Journey Analytics의 AI 지원 {#cja}

Customer Journey Analytics은 [AI Assistant](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/cja-b2c-overview/ai-assistant)를 사용하여 Experience League에서 제품 지식과 통찰력을 찾는 데 도움을 줍니다.

**예제 프롬프트:** 계산된 지표를 만들려면 어떻게 해야 합니까?

새로운 사용자는 이를 사용하여 Customer Journey Analytics 개념을 학습하고 익숙하지 않은 제품 및 기능을 온보딩할 수 있습니다.

숙련된 사용자가 AI 어시스턴트를 활용해 보다 고급 사용 사례나 팁과 요령을 제시하고 빠른 속도로 작업을 수행할 수 있다. 개념을 이해하고, 문제를 해결하거나, 정보를 검색할 수 있습니다. [자세히 알아보기...](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/ai-assistant#knowledge)

**Adobe Firefly과 호환:** 아니요

## Customer Journey Analytics의 지능형 캡션 {#cja-captions}

Customer Journey Analytics의 [지능형 캡션](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/visualizations/intelligent-captions)은(는) 가장 자주 사용되는 Workspace 시각화에 대한 자연어 통찰력을 제공합니다.

**Adobe Firefly과 호환:** 아니요

## Real-Time CDP의 AI 지원 {#rtcdp}

Real-Time CDP은 [AI Assistant](https://experienceleague.adobe.com/ko/docs/experience-platform/ai-assistant/home)를 사용하여 Experience League에서 제품 지식과 통찰력을 찾는 데 도움을 줍니다. 질문에 대한 [팁을 얻으세요](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/questions).

또한 운영 통찰력(베타 버전)도 제공합니다. AI Assistant는 고객의 AEP 샌드박스로 분할되어 중앙 집중식 운영 데이터가 포함된 고객별 운영 통찰력 데이터 스토어를 쿼리합니다. 속성, 대상, 데이터 흐름, 데이터 세트, 대상, 스키마 및 소스에서만 메타데이터를 가져오고 샌드박스 내의 데이터에 액세스하지 않습니다.

예를 들어 대상자에 대한 쿼리의 경우 [!DNL AI Assistant]은(는) 대상자의 이름 및 기타 관련 메타데이터에는 액세스할 수 있지만 해당 대상자 내의 프로필에는 액세스할 수 없습니다.

예:

* 입력: _보유 데이터 세트 수?_

* 응답: Operational Insights 출력은 고객의 비즈니스 개체(속성, 대상, 데이터 흐름, 데이터 세트, 대상, 스키마 및 소스)에서 가져온 메타데이터에 따라 다르며, 쿼리된 데이터가 포함된 특정 UI 페이지에 대한 링크를 포함합니다.

자세한 예제는 [Experience Platform의 AI Assistant](https://experienceleague.adobe.com/ko/docs/experience-platform/ai-assistant/home)에서 _제품 지식_ 및 _Operational Insights_ 입력 테이블을 참조하십시오.

**Firefly 호환:** 아니요

## Marketo의 Dynamic Chat {#marketo}

Adobe Dynamic Chat의 생성 AI 기반 기능을 사용하면 판매 에이전트의 생산성을 최적화하고, 웹 사이트 방문자의 의도에 대한 통찰력을 얻고, 방문자 질문에 안전한 방식으로 응답할 수 있습니다. 질문, 답변 및 대화 요약을 사전 승인할 수 있습니다. [자세히 알아보기...](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/generative-ai/overview)

**Firefly 호환:** 아니요

## Workfront의 AI 지원 {#workfront}

Workfront의 AI Assistant는 인앱 정보 및 제안 사항을 제공하여 작업을 완수하도록 도와줍니다. 다음과 같은 작업을 수행할 수 있습니다.

* 일부 객체의 요약을 가져와 객체의 의도 또는 세부 사항을 개략적으로 볼 수 있습니다.
* 질문하고 [!DNL AI Assistant]이(가) Experience League에서 답을 찾도록 하세요.
* 프롬프트에 따라 생성된 공식을 가져옵니다. 계산된 필드에서 잘못된 사용자 정의 표현식의 오류를 해결할 수도 있습니다.
* 프로젝트, 작업 및 문제를 찾습니다.

[자세히 알아보기...](https://experienceleague.adobe.com/en/docs/workfront/using/basics/ai-assistant/ai-assistant-overview)

**Firefly 호환:** 아니요
