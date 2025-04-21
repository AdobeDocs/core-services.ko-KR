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
source-git-commit: 4f51bc948f3d109f8c1211fda44adee17cc05170
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 6%

---

# Experience Cloud 애플리케이션의 AI

이 페이지는 생성 AI와 Experience Cloud 애플리케이션에서 이를 사용하는 방법을 이해하는 데 도움이 됩니다. 생성 AI, AI Assistant를 사용하는 제품 기능과 Adobe Firefly 지원 여부를 알아봅니다.

## 생성 AI 및 AI Assistant 정보

생성 AI는 단순히 질문에 대한 답변 이상의 역할을 하는 인공 지능의 한 종류이다. _콘텐츠를 만들고_ _프롬프트_(질문 및 문)에 대해 _응답_&#x200B;합니다.

* **만들기:** AI가 교육 및 입력 프롬프트를 기반으로 처음부터 새 콘텐츠(텍스트, 이미지, 음악 또는 비디오)를 생성하는 기능을 나타냅니다. 이 기능은 생성 AI의 _생성_ 측면입니다.

* **응답:** AI가 특정 질문, 문 또는 프롬프트에 대한 답변 또는 반응을 제공하는 것으로, 일반적으로 지식 또는 추론 기능을 기반으로 합니다.

특정 Experience Cloud 애플리케이션은 생성 AI를 활용하여 신규 사용자가 제품 지식을 빠르게 습득하고 숙련된 사용자가 몇 시간이 아닌 몇 초 만에 운영 통찰력을 발견할 수 있도록 지원합니다.

### AI 어시스턴트

[AI Assistant](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/landing)은(는) Experience Platform 및 관련 애플리케이션에서 지원되는 대화 도구입니다. 워크플로우를 가속화하거나, 제품 지식을 개선하거나, 문제를 해결하거나, 정보를 검색하는 데 사용합니다. AI Assistant를 사용하면 몇 시간이 아니라 몇 초 만에 작동 인사이트를 확인할 수 있습니다.

모든 제품 지식 답변은 확인할 수 있으며 Experience League의 제품 설명서에 대한 링크를 통해 인용됩니다. [AI Assistant를 최대한 활용하기 위해 AI Assistant 및 목표 기반 프롬프트 유형에 대해 알아봅니다](https://experienceleague.adobe.com/ko/docs/experience-platform/ai-assistant/home).

## AI를 사용하는 Experience Cloud 애플리케이션

* [Adobe GenStudio for Performance Marketing](#gspm)
* [Adobe Experience Manager Sites(Cloud Service)](#aem-sites)
* [Adobe Journey Optimizer](#journey-optimizer)
* [Adobe Journey Optimizer Prime 및 Ultimate](#ajo-prime-ultimate)
* [Journey Optimizer B2B 에디션](#ajo-b2b)

### GenStudio for Performance Marketing {#gspm}

[GenStudio for Performance Marketing](https://experienceleague.adobe.com/ko/docs/genstudio-for-performance-marketing/user-guide/home)은(는) 캠페인 자산을 만들고, 전달하고, 최적화할 수 있는 생성 AI 기반 플랫폼입니다. AI의 생성 기능은 마케팅 콘텐츠가 생성, 검토, 공유 및 분석되는 방식을 전환합니다.

기능 _GenStudio for Performance Marketing 만들기_(또는 간단히 _만들기_)을 사용하면 마케터와 분산 팀이 고성능의 브랜드 내 경험을 만들 수 있습니다. 다음에 대한 콘텐츠를 생성할 수 있습니다.

* 이메일
* 메타 광고
* LinkedIn 광고
* 광고 표시
* 배너

예, 고객 담당자 및 제품에 대한 설명, 브랜드 지침을 사용하여 GenStudio for Performance Marketing에서 브랜드에 대한 교육을 실시할 수도 있습니다. [자세히 알아보기...](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/create/overview)

**Adobe Firefly과의 호환성:** 예정

### Experience Manager Sites {#aem-sites}

AEM Sites은 [변형 생성](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations)을 사용합니다. 변형 생성 은 생성 AI를 사용하여 프롬프트에 따라 콘텐츠 변형을 만듭니다. 이러한 프롬프트는 [Adobe](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#get-started)에서 제공하거나 [사용자](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#create-prompt)에서 만들고 관리합니다.

변형을 만든 후에는 웹 사이트의 콘텐츠를 사용하고 Edge Delivery Services의 실험 기능을 사용하여 성공을 측정할 수 있습니다.

**입력:** 입력 필드는 다음과 같습니다.

* 생성할 변형 수
* Audience Source
* 대상 타겟
* 추가 컨텍스트
* 고객 중심 프롬프트

**출력:** 생성된 콘텐츠/마켓 카피. Firefly의 생성 AI 기능을 사용하여 Adobe Express에서 이미지를 생성하는 옵션도 있습니다.

[이미지 생성](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#generate-image)을 참조하세요.

**Adobe Firefly과의 호환성:** 예

## Journey Optimizer {#journey-optimizer}

Journey Optimizer은 두 가지 수준의 질문으로 [AI Assistant](https://experienceleague.adobe.com/ko/docs/experience-platform/ai-assistant/home)를 사용합니다.

**제품 지식** - 제품 insight에 대한 Adobe 데이터 저장소(예: Experience League 제품 설명서)를 쿼리합니다. 이 출력은 고객을 구분하지 않습니다. 예:

* 하나의 Adobe Journey Optimizer 샌드박스에서 몇 개의 라이브 활동을 가질 수 있습니까?

**Operational Insights(Beta)** - 고객의 샌드박스로 분할된 여정에 대한 중앙 집중식 운영 데이터가 포함된 고객별 Operational Insights 데이터 저장소를 쿼리합니다. 비즈니스 개체에서만 메타데이터를 가져오고 샌드박스 내의 데이터에 액세스하지 않습니다.

* 지난 7일 동안 얼마나 많은 여정이 생성되었습니까?

Operational Insights 출력은 고객의 비즈니스 개체에서 가져온 메타데이터에 따라 다릅니다.

여정은 Journey Optimizer에서 AI Assistant에 사용할 수 있는 유일한 개체이며 메타데이터는 현재 샌드박스에서 가져옵니다.

자세한 내용은 [AI 도우미와 함께 작업](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/ai-assistant) 및 [필드 준비](https://fieldreadiness-adobe.highspot.com/items/6661f1c132683fd5e6a8adf4?lfrm=srp.1#11)를 참조하십시오.

**Adobe Firefly과의 호환성:** 아니요

## Journey Optimizer Prime 및 Ultimate {#ajo-prime-ultimate}

Journey Optimizer Prime 및 Ultimate에서는 [AI Assistant for Content Accelerator](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative)를 사용하여 텍스트 및 이미지에 대한 사전 예방적 콘텐츠 변형 제안을 제공합니다.

이 기능은 이메일, 푸시, 웹 및 SMS 채널에 사용할 수 있습니다. 프롬프트 기반 텍스트 및 이미지 생성을 제공합니다.

**전자 메일** - 전체 전자 메일, 텍스트만 또는 이미지만 생성합니다. [자세히 알아보기...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-email)

**푸시 알림** - 전체 푸시 알림, 텍스트만 또는 이미지만 생성합니다. [자세히 알아보기...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-push)

**SMS** - 전체 SMS 또는 텍스트만 생성합니다. [자세히 알아보기](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-sms)

**웹 페이지** - 웹 페이지 이미지 또는 웹 페이지 텍스트를 생성합니다. [자세히 알아보기...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-web)

**콘텐츠** - 다양한 메시징 캠페인에 대한 콘텐츠를 생성합니다. [자세히 알아보기...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-experimentation)

**참고:** AJO Prime 및 Ultimate의 Content Accelerator에서 출력되는 내용은 손실됩니다.

**Adobe Firefly과의 호환성:** 예

## Journey Optimizer B2B 에디션 {#ajo-b2b}

제품 정보 프롬프트에 [AI Assistant](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/get-started/ai-assistant)을 사용합니다.

**제품 지식** - 제품 insight에 대한 Adobe 데이터 저장소(예: Experience League 제품 설명서)를 쿼리합니다. 이 출력은 고객을 구분하지 않습니다. | <ul><li>**입력:** 계정 여정에서 전자 메일을 보내는 방법</li><li>**출력:** 제품 지식을 Experience League(공개 설명서)에서 가져옵니다. [자세히 알아보기...](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/get-started/ai-assistant)</li></ul>   | 아니요   |

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
