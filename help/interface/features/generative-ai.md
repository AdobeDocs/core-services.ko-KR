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
source-git-commit: d54af09033b1a0727e9b7aa3dbf4a9be6003a8ea
workflow-type: tm+mt
source-wordcount: '1371'
ht-degree: 3%

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

**입력:** 입력 필드는 다음과 같습니다.

* 생성할 변형 수
* Audience Source
* 대상 타겟
* 추가 컨텍스트
* 고객 중심 프롬프트

**출력:** 생성된 콘텐츠/마켓 카피. Firefly의 생성 AI 기능을 사용하여 Adobe Express에서 이미지를 생성하는 옵션도 있습니다.

자세한 내용은 [이미지 생성](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#generate-image)을 참조하세요.

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

Customer Journey Analytics은 [AI Assistant](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/ai-assistant)를 사용하여 Experience League에서 제품 지식과 통찰력을 찾는 데 도움을 줍니다.

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

* 응답: _Operational Insights 출력은 고객의 비즈니스 개체(특성, 대상, 데이터 흐름, 데이터 세트, 대상, 스키마 및 원본)에서 가져온 메타데이터에 따라 다르며, 쿼리된 데이터가 포함된 특정 UI 페이지에 대한 링크를 포함합니다._

자세한 예제는 [Experience Platform의 AI Assistant](https://experienceleague.adobe.com/ko/docs/experience-platform/ai-assistant/home)에서 _제품 지식_ 및 _Operational Insights_ 입력 테이블을 참조하십시오.

**Firefly 호환:** 아니요

## Marketo의 Dynamic Chat {#marketo}

[Dynamic Chat](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview)은(는) 사용자 지정 및 사전 승인된 질문과 답변과 대화 요약으로 AI 지원 대화를 만듭니다 |<ul><li> **질문 생성:** 콘텐츠를 추출하여 질문/응답을 생성하는 데 사용할 URL을 제공합니다. </li><li> **대화 요약:** 대화 요약을 생성합니다. </li></ul> [자세히 알아보기...](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/generative-ai/response-library)  | 아니요 |

## Workfront의 AI 지원 {#workfront}

Workfront의 [AI Assistant](https://experienceleague.adobe.com/en/docs/workfront/using/basics/ai-assistant/ai-assistant-overview)는 자연어 대화에서 인앱 정보와 제안을 제공하여 작업을 완수하도록 도와줍니다. AI Assistant는 다음 기능을 제공합니다. 프로젝트/작업/문제/문서를 요약하고, Experience League의 Workfront 설명서에서 가져온 지침 또는 참조 정보를 제공하며, 계산된 사용자 정의 필드에 대한 공식을 생성하거나 구체화합니다.  | <ul><li>**프로젝트 입력 요약:** 이 프로젝트 요약 </li><li> **프로젝트 출력 요약:** 프로젝트의 목적과 상태에 대한 간단한 설명을 반환하고 완료되었으며 아직 보류 중인 작업의 예를 제공하고 몇 가지 추가 세부 정보와 메모를 제공합니다.</li><li> **수식 입력 생성/세분화:** &quot;잘못된 식 오류를 제거하려면 이 수식을 다시 작성하십시오.&quot; </li><li> **수식 출력 생성/세분화:** 생성 또는 세분화된 수식. </li></ul>**참고:** AI Assistant는 수식의 크기와 복잡성에 따라 수정된 수식을 생성하는 데 몇 분 정도 걸릴 수 있습니다. | 아니요  |


<!-- ## Experience Cloud applications that use AI

Learn how Experience Cloud applications use generative AI or AI Assistant, and whether Adobe Firefly is supported. 

| Application | How Generative AI Is Used | Examples | Adobe Firefly? |
|----------|------------|-----------|----------------|
| GenStudio for Performance Marketing | [GenStudio for Performance Marketing](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home) is a generative AI-driven platform. It infuses the content creation lifecycle with generative AI capabilities that transform how marketing content is created, reviewed, shared, and analyzed.<br>You can train GenStudio for Performance Marketing on your brand using examples, descriptions of customer personas and products, and brand guidelines. |_GenStudio for Performance Marketing Create_ lets you generate content for emails, Meta ads, LinkedIn ads, display ads, and banners. <br>**Inputs:** <ul><li>Use templates to start the content creation process. </li><li>Add parameters like Brands, Products, and Personas (guidelines) and Content (assets) to shape the generated experience. </li><li>Enter descriptive prompts that describe the context or experience you intend to generate. [Learn more...](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/create/overview)</li></ul> |Yes |
|Adobe Experience Manager Sites (Cloud Service)  | AEM Sites uses [Generate Variations](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations). <br>Generate Variations uses generative AI to create content variations based on prompts. These prompts are either provided by Adobe or created and managed by users. |After creating variations, you can use the content on your website and measure its success using the Experimentation functionality of Edge Delivery Services. <br>**Input:** Input fields include Number of Variations to generate; Audience Source / Audience Target; Additional Context, and customer-driven prompts. <ul><li>[Adobe prompt template](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#get-started) </li><li>[User generated prompt](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#create-prompt)</li></ul> **Output:** Generated Content / Market Copy. You also have the option to generate images in Adobe Express using the generative AI capabilities of Firefly. See [Generate Image](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#generate-image). | Yes|
| Adobe Journey Optimizer |Journey Optimizer uses [AI Assistant](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home) with two classes of questions:<ul><li>**Product knowledge** - Queries Adobe data stores (such as Experience League product documentation) for product insight. This output is customer agnostic. </li><li>**Operational Insights (Beta)** - queries a customer-specific operational insights data store that contains centralized operational data about Journeys, partitioned by the customer's sandbox. Pulls metadata only from business objects and does not access data within the sandbox.</li></ul>|<ul><li>**Product Knowledge Input:** How many live activities can I have in one Adobe Journey Optimizer sandbox?</li><li>**Product Knowledge Output:** Product Knowledge pulls from Experience League (public documentation). </li><li>**Operational Insights Input:** How many Journeys have been created in the last seven days? </li><li>**Operational Insights Output:** Operational Insights output depends on metadata pulled from customer's business objects. Journeys is the only object available in AJO, and metadata is pulled from the current sandbox. </li></ul> See [Work with the AI Assistant](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/ai-assistant) and [Field Readiness](https://fieldreadiness-adobe.highspot.com/items/6661f1c132683fd5e6a8adf4?lfrm=srp.1#11) | No |
| Journey Optimizer: _Prime_ and _Ultimate_  | [AI Assistant for Content Accelerator](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative) brings proactive content variation suggestions for text and images. It is available for email, push, web and SMS channels. This new capability provides prompt-based text and image generation. |<ul><li> **Email** - generate a full email, text only or image only. [Learn more...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-email) </li><li> **Push Notification** - Generate a full push notification, text only or image only. [Learn more...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-push) </li><li> **SMS** - Generate a full SMS, or text only. [Learn more](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-sms) </li><li> **Webpage** - Generate web page images or web page text. [Learn more...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-web) </li><li> **Content** - Generate content for various messaging campaigns. [Learn more...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-experimentation)</li></ul> **Note:** Output from Content Accelerator in AJO Prime and Ultimate is indemnified. | Yes   |
| Journey Optimizer B2B Edition  | Uses [AI Assistant](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/get-started/ai-assistant) with one class of questions: <br> **Product knowledge** - Queries Adobe data stores (such as Experience League product documentation) for product insight. This output is customer agnostic. | <ul><li>**Input:** How do I send an email in an account journey?</li><li>**Output:** Product Knowledge pulls from Experience League (public documentation). [Learn more...](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/get-started/ai-assistant)</li></ul>   | No   |
| Campaign Managed Cloud Services | [AI Assistant for Content Accelerator](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-gs) auto-generates personalized, engaging, and effective content based on the marketing objective with content optimized for brand outlined styles, layouts, tone, and more across channels like Email, SMS, Push. |<ul><li> **Email** - Generate a full email, text only or image only. [Learn more](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-content) </li><li> **SMS** - Generate full SMS or text only. [Learn more...](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-sms) </li><li> **Push** - Craft compelling messaging and generate content. [Learn more...](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-push) </li></ul> **Note:** Output from Content Accelerator in Campaign Managed Cloud Services is indemnified. | Yes  |
| Customer Journey Analytics   | CJA uses [AI Assistant](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/ai-assistant) to help you discover product knowledge and insights from Experience League. <br>For example, new users can use it to learn Customer Journey Analytics concepts and onboard yourself to products and features that you are unfamiliar with. <br>Experienced users can use AI Assistant to present more advanced use cases or tips and tricks and perform tasks at a fast pace. Understand concepts, troubleshoot problems, or search for information. [Learn more...](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/ai-assistant#knowledge) | <ul><li>**Product Knowledge Input:** How do I build a calculated metric? </li><li> **Product Knowledge Output:** Product Knowledge pulls from Experience League (public documentation). </li></ul> | No |
| Customer Journey Analytics    | [Intelligent Captions](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/visualizations/intelligent-captions) provides natural-language insights for line visualizations in Workspace visualizations.| <ul><li>**Input:** Line visualizations. Captions are auto-generated based on such line visualizations when you click **Intelligent captions**. </li><li> **Output:** Auto-generated natural-language captions.</li></ul>  | No             |
| Real-Time CDP |Uses [AI Assistant](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home) to help you discover product knowledge and insights from Experience League. It queries a database and translates data from the database into a human-readable answer. Two classes of questions: <br> **Product knowledge** - Queries Adobe data stores (such as Experience League product documentation) for product insight. This output is customer agnostic. <br> **Operational Insights (Beta)** - Queries a customer-specific operational insights data store that contains centralized operational data, partitioned by the customer's AEP sandbox. Pulls metadata only from Attributes, Audiences, Dataflows, Datasets, Destinations, Schemas, and Sources, and does not access data within the sandbox. <br>For example, for a query about an audience [!DNL AI Assistant] can access the name of the audience and other associated metadata but cannot access the profiles within that audience. | <ul><li>**Product Knowledge Input:** How is profile richness calculated? </li><li>**Product Knowledge Output:** Product Knowledge pulls from Experience League (public documentation). </li><li> **Operational Insights Input:** How many datasets do I have? </li><li> **Operational Insights Output:** Operational Insights output depends on metadata pulled from Customer's business objects (Attributes, Audiences, Dataflows, Datasets, Destinations, Schemas, and Sources), and includes a link to specific UI page containing queried data. </li></ul>For examples, see the _Product Knowledge_ and _Operational Insights_ input tables in [AI Assistant in Experience Platform](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home)  | No |
| Marketo  | [Dynamic Chat](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview) creates AI-assisted conversations with customized and pre-approved questions and answers, as well as conversation summary |<ul><li> **Generate Questions:** Provide URLs from which content is extracted and used to generate questions / responses. </li><li> **Conversation Summary:** Generates a summary of a chat conversation. </li></ul> [Learn more...](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/generative-ai/response-library)  | No |
| Workfront | [AI Assistant](https://experienceleague.adobe.com/en/docs/workfront/using/basics/ai-assistant/ai-assistant-overview) in Workfront helps you accomplish your work by offering in-app information and suggestions in a natural-language conversation. AI Assistant offers the following functionality: Summarizes projects/tasks/issues/documents, provides instructions or reference information pulled from the Workfront documentation on Experience League, generates or refines formulas for calculated custom fields.  | <ul><li>**Summarize Project Input:** Summarize this project </li><li> **Summarize Project Output:** Returns brief descriptions of the project's purpose and status, gives examples of tasks that are completed and that are still pending, and provides some additional details and notes.</li><li> **Generate/Refine Formula Input:** "Rewrite this formula to remove the invalid expression error." </li><li> **Generate/Refine Formula Output:** Generated or refined formula. </li></ul>**Note:** AI Assistant may take a few moments to generate the revised formula, depending on the size and complexity of the formula. | No  | -->
