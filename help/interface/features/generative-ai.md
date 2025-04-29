---
title: Experience Cloud 애플리케이션의 AI
description: 생성 AI와 Experience Cloud 애플리케이션에서 genAI 및  [!DNL AI Assistant]을(를) 사용하는 방법에 대해 알아봅니다.
solution: Experience Cloud
feature: AI Assistant, Generative AI
topic: Administration
role: Admin
level: Intermediate
exl-id: bdc51956-82aa-4aae-b627-a2018f80b5f5
source-git-commit: d84fcf64b7019f0146340a423e8e20a932cd7874
workflow-type: tm+mt
source-wordcount: '1168'
ht-degree: 3%

---

# Experience Cloud 제품의 AI

이 페이지에서는 생성 AI를 지원하는 제품, [!DNL AI Assistant] 및 Adobe Firefly의 호환 여부를 확인할 수 있습니다. Experience Cloud에서 AI를 사용하는 방법에 대한 제품별 도움말 리소스 링크를 찾을 수도 있습니다.

**생성 AI 정보**

생성 AI는 단순히 질문에 대한 답변 이상의 역할을 하는 인공 지능의 한 종류이다. _콘텐츠를 만들고_&#x200B;질문 또는 구문(_프롬프트_)에 대한 응답을 _생성하고_&#x200B;할 수 있습니다.

* **만들기:** 교육 및 입력 프롬프트에 따라 처음부터 콘텐츠(텍스트, 이미지, 음악 또는 비디오)를 생성하는 기능입니다. 이 기능은 생성 AI의 _생성_ 측면입니다.

* **응답 생성:** AI는 일반적으로 사용 가능한 데이터 및 지식 저장소를 기반으로 프롬프트에 대한 답변이나 반응을 제공합니다.

**[!DNL AI Assistant]란?**

[!DNL AI Assistant]은(는) Experience Platform 및 관련 응용 프로그램에서 지원되는 대화 도구입니다. 이를 통해 _제품 지식_&#x200B;을 빠르게 습득하고 지원되는 응용 프로그램에서 거의 즉시 _운영 통찰력_&#x200B;을 습득할 수 있습니다.

* **제품 기술 자료:** 제품 기술 자료는 Experience League 설명서에 나와 있는 개념과 주제를 참조합니다. Experience League의 응답은 확인 가능하며 링크로 인용됩니다. [!DNL AI Assistant]을(를) 최대한 활용하기 위해 [목표 기반 프롬프트](https://experienceleague.adobe.com/ko/docs/experience-platform/ai-assistant/home)의 유형에 대해 알아봅니다.

* **Operational Insights:** Operational Insights는 카운트, 조회 및 계보 영향을 포함하여 AI Assistant가 메타 데이터 개체(특성, 대상, 데이터 흐름, 데이터 세트, 대상, 여정, 스키마 및 원본)에 대해 생성하는 답변을 참조합니다. AI Assistant를 사용하면 몇 시간이 아닌 몇 초 만에 작동 인사이트를 확인할 수 있습니다.

[자세히 알아보기](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/landing)

<!-- **Your data remains yours**

In AI Assistant, security is the priority:

* Customer data is not used to train language models.
* AI Assistant looks at only the documents that you tell it to. You are in control.
* Your people can use AI Assistant only on documents they can access.
* It's audit-ready: Responses are attributable to source documents.
* Enterprise controls are in place to manage who has AI access in the company.
 -->

## Experience Cloud 제품의 AI 가용성

Experience Cloud 제품의 생성 AI 또는 [!DNL AI Assistant] 지원에 대해 알아봅니다. Adobe Firefly에 대한 지원도 표시됩니다.

* [[!DNL GenStudio for Performance Marketing]](#gspm)
* [[!DNL Experience Manager Sites]](#aem-sites)
* [[!DNL Journey Optimizer]](#journey-optimizer)
* [[!DNL Journey Optimizer] B2B edition](#ajo-b2b)
* [[!DNL Campaign] 관리 클라우드 서비스](#campaign-cs)
* [[!DNL Customer Journey Analytics]](#cja)
* [[!DNL Customer Journey Analytics]](#cja-captions)
* [[!DNL Real-Time CDP]](#rtcdp)
* [[!DNL Marketo]](#marketo)
* [[!DNL Workfront]](#workfront)

## Adobe GenStudio for Performance Marketing {#gspm}

[!DNL GenStudio for Performance Marketing]은(는) 브랜드 표준을 준수하고 엔터프라이즈 정책을 준수하는 마케팅 콘텐츠를 생성하고 관리할 수 있는 AI 기반 플랫폼입니다. 이메일, 메타 광고, LinkedIn 광고, 디스플레이 광고 및 배너에 대한 콘텐츠를 생성합니다.

예, 고객 담당자 및 제품에 대한 설명, 브랜드 지침을 사용하여 GenStudio for Performance Marketing에서 브랜드에 대한 교육을 실시할 수도 있습니다.

[자세히 알아보기](https://experienceleague.adobe.com/ko/docs/genstudio-for-performance-marketing/user-guide/home)

Adobe Firefly과의 호환성: **예**

## Adobe [!DNL Experience Manager Sites] {#aem-sites}

AEM Sites에서는 _[!UICONTROL 변형 생성]_&#x200B;을 사용할 수 있습니다. 이 기능은 생성 인공 지능을 사용하여 입력 프롬프트에 따라 콘텐츠 변형을 만듭니다. 프롬프트는 Adobe에서 제공하거나 사용자가 생성 및 관리합니다.

변형을 만든 후에는 웹 사이트의 콘텐츠를 사용하고 Edge Delivery Services의 [실험](https://www.aem.live/docs/experimentation) 기능을 사용하여 성공을 측정할 수 있습니다. Firefly의 생성 AI 기능을 사용하여 Adobe Express에서 이미지를 생성하는 옵션도 있습니다.

**입력 및 출력 예**

입력 필드는 다음과 같습니다.

* 생성할 변형 수
* Audience Source
* 대상 타겟
* 추가 컨텍스트
* 고객 중심 프롬프트

출력은 생성된 콘텐츠 또는 마켓 카피입니다.

[변형 생성에 대해 자세히 알아보기](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations-integrated-editor)

Adobe Firefly과의 호환성: **예**

## Adobe [!DNL Journey Optimizer] {#journey-optimizer}

[!DNL Journey Optimizer]&#x200B;(AJO)에서 [AI Assistant](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/ai-assistant)를 사용하여 _제품 지식_ 및 _작동 인사이트_(베타)를 얻을 수 있습니다.

### AJO에서 AI Assistant를 사용하는 예

다음은 제품 지식에 대한 예제 입력입니다.

* _하나의 Journey Optimizer 샌드박스에서 몇 개의 라이브 활동을 사용할 수 있습니까?_

  출력은 Experience League 및 기타 Adobe 데이터 저장소에서 생성됩니다.

다음은 작동 인사이트에 대한 예제 입력입니다.

* _지난 7일 동안 만들어진 여정 수는 몇 개입니까?_

  출력의 경우 AI Assistant는 고객별 데이터 저장소를 쿼리합니다. 데이터 저장소에 [!UICONTROL 여정]에 대한 중앙 집중식 운영 데이터가 포함되어 있습니다. 이 기능은 고객을 구분하지 않으며 비즈니스 개체에서만 메타데이터를 가져옵니다. 샌드박스 내의 데이터에 액세스하지 않습니다.

[자세히 알아보기](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/ai-assistant).

Adobe Firefly과의 호환성: **아니요**

### 콘텐츠 생성을 위한 AI 지원(AJO Prime 및 Ultimate) {#ajo-prime}

AJO _Prime_ 및 _Ultimate_&#x200B;에서 콘텐츠 생성에 [콘텐츠 생성](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative)을 사용하여 텍스트 및 이미지에 대한 사전 예방적 콘텐츠 변형 제안을 가져올 수 있습니다.

이 기능은 이메일, 푸시 알림, 웹 페이지, 콘텐츠 및 SMS 채널에 사용할 수 있습니다. 프롬프트 기반 텍스트 및 이미지 생성을 제공합니다. AJO Prime 및 Ultimate의 콘텐츠 생성 출력은 손실됩니다.

[자세히 알아보기](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative)

Adobe Firefly과의 호환성: **예**

## [!DNL Journey Optimizer B2B Edition] {#ajo-b2b}

Journey Optimizer B2B edition은 [!DNL AI Assistant]을(를) 사용하여 제품 지식을 지원합니다.

입력 예:

* _계정 여정에서 전자 메일을 보내는 방법_

  제품 지식 출력은 Experience League에서 가져옵니다.

[자세히 알아보기](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/ai-assistant/ai-assistant-overview)

Adobe Firefly과의 호환성: **아니요**

## [!DNL Campaign] 관리 클라우드 서비스 {#campaign-cs}

Campaign 관리 클라우드 서비스는 콘텐츠 생성에 [!DNL AI Assistant]을(를) 사용합니다. 이 기능을 사용하면 마케팅 목표를 기반으로 개인화되고, 매력적이며, 효과적인 콘텐츠를 자동 생성할 수 있으며, 브랜드 윤곽선 스타일, 레이아웃, 색조 등에 최적화된 콘텐츠를 사용할 수 있습니다. 이메일, SMS 및 푸시와 같은 채널에서 사용할 수 있습니다.

**참고:** Campaign Managed Cloud Services에서 콘텐츠 생성의 출력은 손실됩니다.

[자세히 알아보기](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-gs)

Adobe Firefly과의 호환성: **예**

## [!DNL Customer Journey Analytics] {#cja}

Customer Journey Analytics은 [!DNL AI Assistant]을(를) 사용하여 Experience League에서 제품 지식과 통찰력을 찾는 데 도움을 줍니다.

신규 사용자인 경우 Customer Journey Analytics 개념을 빠르게 학습하고 제품 및 기능을 온보딩하십시오. 예:

* _계정 여정에서 전자 메일을 보내는 방법_

숙련된 사용자는 고급 사용 사례를 얻거나 빠른 속도로 작업을 수행하는 전략을 학습합니다. 개념을 빠르게 이해하고, 문제를 해결하거나, 정보를 검색할 수 있다.

[자세히 알아보기](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/cja-b2c-overview/ai-assistant)

Adobe Firefly과의 호환성: **아니요**

## [!DNL Customer Journey Analytics] {#cja-captions}

[!DNL Customer Journey Analytics]의 _지능형 캡션_&#x200B;을(를) 사용하여 가장 자주 사용되는 Workspace 시각화에 대한 자연어 통찰력을 얻을 수 있습니다. 지능형 캡션은 다른 사용자와 공유하기 위해 서사와 컨텍스트가 필요한 분석가에게 이상적입니다. 비즈니스 사용자는 이를 사용하여 높은 수준의 아이디어를 빠르게 발견할 수 있습니다.

예:

* **입력:** CJA에서 지원되는 시각화(선, 영역, 막대 차트, 흐름 또는 폴아웃 포함)를 실행한 다음 **[!UICONTROL 지능형 캡션]**&#x200B;을 클릭합니다.

* **출력:** 컨텍스트 및 키 변환을 보여 주는 자동 생성된 자연어 캡션을 봅니다. 그런 다음 생성된 데이터를 검토, 복사 및 조직과 공유하는 등의 작업을 수행할 수 있습니다. [방법 보기](https://video.tv.adobe.com/v/3420131/?quality=12&learn=on#_blank)

[자세히 알아보기](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/visualizations/intelligent-captions)

Adobe Firefly과의 호환성: **아니요**

## [!DNL Real-Time CDP] {#rtcdp}

Real-Time CDP은 [!DNL AI Assistant]을(를) 사용하여 Experience League의 제품 지식을 지원합니다. 또한 운영 통찰력(베타 버전)도 제공합니다. [!DNL AI Assistant]은(는) AEP 샌드박스에서 분할된 중앙 운영 데이터를 포함하는 고객별 operational insights 데이터 저장소를 쿼리합니다. 시스템은 속성, 대상, 데이터 흐름, 데이터 세트, 대상, 스키마 및 소스에서만 메타데이터를 가져오고 샌드박스 내의 데이터에 액세스하지 않습니다.

예를 들어 대상자에 대해 쿼리하는 경우 [!DNL AI Assistant]은(는) 대상자의 이름 및 기타 관련 메타데이터에는 액세스할 수 있지만 해당 대상자 내의 프로필에는 액세스할 수 없습니다.

[자세히 알아보기](https://experienceleague.adobe.com/ko/docs/experience-platform/ai-assistant/home)

Adobe Firefly과의 호환성: **아니요**

## [!DNL Marketo] {#marketo}

Adobe Dynamic Chat의 생성 AI 기반 기능을 사용하면 판매 에이전트의 생산성을 최적화하고, 웹 사이트 방문자의 의도에 대한 통찰력을 얻고, 방문자 질문에 안전한 방식으로 응답할 수 있습니다. 질문, 답변 및 대화 요약을 사전 승인할 수 있습니다.

[자세히 알아보기](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/generative-ai/overview)

Adobe Firefly과의 호환성: **아니요**

## [!DNL Workfront] {#workfront}

[!DNL Workfront]의 [!DNL AI Assistant]은(는) 인앱 정보와 제안을 제공하여 작업을 완수하도록 도와줍니다. 다음과 같은 작업을 수행할 수 있습니다.

* 일부 객체의 요약을 가져와 객체의 의도 또는 세부 사항을 개략적으로 볼 수 있습니다.
* 질문하고 [!DNL AI Assistant]이(가) Experience League에서 답을 찾도록 하세요.
* 프롬프트에 따라 생성된 공식을 가져옵니다. 계산된 필드에서 잘못된 사용자 정의 표현식의 오류를 해결할 수도 있습니다.
* 프로젝트, 작업 및 문제를 찾습니다.

[자세히 알아보기](https://experienceleague.adobe.com/en/docs/workfront/using/basics/ai-assistant/ai-assistant-overview)

Adobe Firefly과의 호환성: **아니요**
