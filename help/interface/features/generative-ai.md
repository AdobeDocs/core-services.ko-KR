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
source-git-commit: bc1f602df5a4b6f2d6eb9a3b00f2756a09d97e2b
workflow-type: tm+mt
source-wordcount: '1662'
ht-degree: 4%

---


# Experience Cloud 애플리케이션의 AI

이 페이지는 Experience Cloud 애플리케이션이 생성 AI를 사용하는 방법과 애플리케이션별 정보를 찾을 수 있는 위치를 이해하는 데 도움이 됩니다. 질문, 프롬프트, 입력 및 출력 모델 클래스에 대해 알아봅니다.

## 생성 AI 및 AI Assistant 정보

생성 AI는 다음과 같은 새로운 콘텐츠를 _생성_&#x200B;하고 사용자의 진술과 질문(프롬프트)에 _응답_&#x200B;할 수 있는 유형의 인공 지능입니다.

* **만들기:** AI가 교육 및 입력 프롬프트를 기반으로 처음부터 새 콘텐츠(텍스트, 이미지, 음악 또는 비디오)를 생성하는 기능을 나타냅니다. 이 기능은 생성 AI의 _생성_ 측면입니다.

* **응답:** AI가 특정 질문, 문 또는 프롬프트에 대한 답변 또는 반응을 제공하는 것으로, 일반적으로 지식 또는 추론 기능을 기반으로 합니다.

특정 Experience Cloud 애플리케이션은 생성 AI를 활용하여 신규 사용자가 제품 지식을 빠르게 습득하고 숙련된 사용자가 몇 시간이 아닌 몇 초 만에 운영 통찰력을 발견할 수 있도록 지원합니다.

### AI 어시스턴트

[AI Assistant](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/landing)은(는) Experience Platform 및 관련 애플리케이션에서 지원되는 대화 도구입니다. 워크플로우를 가속화하거나, 제품 지식을 개선하거나, 문제를 해결하거나, 정보를 검색하는 데 사용합니다. AI Assistant를 사용하면 몇 시간이 아니라 몇 초 만에 작동 인사이트를 확인할 수 있습니다.

모든 제품 지식 답변은 확인할 수 있으며 Experience League의 제품 설명서에 대한 링크를 통해 인용됩니다. [AI Assistant를 최대한 활용하기 위해 AI Assistant 및 목표 기반 프롬프트 유형에 대해 알아봅니다](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home).

## AI를 사용하는 Experience Cloud 애플리케이션

서브헤드 버전(완료되지 않음)...

* [GenStudio for Performance Marketing](#gspm)
* [Experience Manager Sites(Cloud Service)](#aem-sites)
* 추가 정보...

### GenStudio for Performance Marketing {#gspm}

[GenStudio for Performance Marketing](https://experienceleague.adobe.com/ko/docs/genstudio-for-performance-marketing/user-guide/home)은(는) 생성형 AI 기반 플랫폼입니다. 콘텐츠 생성 라이프사이클에 마케팅 콘텐츠가 생성, 검토, 공유 및 분석되는 방식을 전환하는 생성 AI 기능을 주입합니다.

_GenStudio for Performance Marketing 만들기_&#x200B;는 Adobe GenAI의 기능을 활용하여 마케터와 분산 팀이 우수한 성능의 브랜드 내 경험을 만들 수 있도록 합니다. 콘텐츠 생성 대상:

* 이메일
* 메타 광고
* LinkedIn 광고
* 광고 표시
* 배너

예, 고객 담당자 및 제품에 대한 설명, 브랜드 지침을 사용하여 GenStudio for Performance Marketing에서 브랜드에 대해 교육할 수 있습니다. [자세히 알아보기](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/create/overview)

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



테이블 버전...

## AI를 사용하는 Experience Cloud 애플리케이션

Experience Cloud 애플리케이션이 생성 AI 또는 AI Assistant를 사용하는 방법과 Adobe Firefly 지원 여부에 대해 알아봅니다.

| 애플리케이션 | 생성 AI 사용 방법 | 예시 | Adobe Firefly? |
|----------|------------|-----------|----------------|
| GenStudio for Performance Marketing | [GenStudio for Performance Marketing](https://experienceleague.adobe.com/ko/docs/genstudio-for-performance-marketing/user-guide/home)은(는) 생성형 AI 기반 플랫폼입니다. 콘텐츠 생성 라이프사이클에 마케팅 콘텐츠가 생성, 검토, 공유 및 분석되는 방식을 전환하는 생성 AI 기능을 주입합니다.<br>예, 고객 담당자 및 제품에 대한 설명, 브랜드 지침을 사용하여 브랜드에 대한 GenStudio for Performance Marketing을 교육할 수 있습니다. | _GenStudio for Performance Marketing 만들기_&#x200B;를 통해 이메일, 메타 광고, LinkedIn 광고, 디스플레이 광고 및 배너에 대한 콘텐츠를 생성할 수 있습니다. <br>**입력:** <ul><li>템플릿을 사용하여 콘텐츠 작성 프로세스를 시작합니다. </li><li>브랜드, 제품, 가상 사용자(지침) 및 콘텐츠(자산)와 같은 매개 변수를 추가하여 생성된 경험을 구체화합니다. </li><li>생성하려는 컨텍스트 또는 경험을 설명하는 설명 프롬프트를 입력합니다. [자세히 알아보기...](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/create/overview)</li></ul> | 예 |
| Adobe Experience Manager Sites(Cloud Service) | AEM Sites은 [변형 생성](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations)을 사용합니다. <br>변형 생성은 생성 AI를 사용하여 프롬프트에 따라 콘텐츠 변형을 만듭니다. 이러한 프롬프트는 Adobe에서 제공하거나 사용자가 생성 및 관리합니다. | 변형을 만든 후에는 웹 사이트의 콘텐츠를 사용하고 Edge Delivery Services의 실험 기능을 사용하여 성공을 측정할 수 있습니다. <br>**입력:** 입력 필드에는 생성할 변형 수, 대상 Source/대상 대상, 추가 컨텍스트 및 고객 기반 프롬프트가 포함됩니다. <ul><li>[Adobe 프롬프트 템플릿](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#get-started) </li><li>[사용자 생성 프롬프트](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#create-prompt)</li></ul> **출력:** 생성된 콘텐츠/마켓 카피. Firefly의 생성 AI 기능을 사용하여 Adobe Express에서 이미지를 생성하는 옵션도 있습니다. [이미지 생성](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#generate-image)을 참조하세요. | 예 |
| Adobe Journey Optimizer | Journey Optimizer은 두 가지 수준의 질문으로 [AI Assistant](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home)를 사용합니다.<ul><li>**제품 지식** - 제품 insight에 대한 Adobe 데이터 저장소(예: Experience League 제품 설명서)를 쿼리합니다. 이 출력은 고객을 구분하지 않습니다. </li><li>**Operational Insights(Beta)** - 고객의 샌드박스로 분할된 여정에 대한 중앙 집중식 운영 데이터가 포함된 고객별 Operational Insights 데이터 저장소를 쿼리합니다. 비즈니스 개체에서만 메타데이터를 가져오고 샌드박스 내의 데이터에 액세스하지 않습니다.</li></ul> | <ul><li>**제품 정보 입력:** 하나의 Adobe Journey Optimizer 샌드박스에서 사용할 수 있는 라이브 활동 수는 몇 개입니까?</li><li>**제품 지식 출력:** 제품 지식은 Experience League(공개 설명서)에서 가져옵니다. </li><li>**Operational Insights 입력:** 지난 7일 동안 만들어진 여정 수는 몇 개입니까? </li><li>**Operational Insights 출력:** Operational Insights 출력은 고객의 비즈니스 개체에서 가져온 메타데이터에 따라 다릅니다. 여정 는 AJO에서 사용할 수 있는 유일한 개체이며 메타데이터는 현재 샌드박스에서 가져옵니다. </li></ul> [AI 길잡이 작업](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/ai-assistant) 및 [필드 준비](https://fieldreadiness-adobe.highspot.com/items/6661f1c132683fd5e6a8adf4?lfrm=srp.1#11)를 참조하십시오. | 아니요 |
| Journey Optimizer: _Prime_ 및 _Ultimate_ | [Content Accelerator용 AI Assistant](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative)은(는) 텍스트 및 이미지에 대한 사전 예방적 콘텐츠 변형 제안을 제공합니다. 이메일, 푸시, 웹 및 SMS 채널에 사용 가능합니다. 이 새로운 기능은 프롬프트 기반 텍스트 및 이미지 생성을 제공합니다. | <ul><li> **전자 메일** - 전체 전자 메일, 텍스트만 또는 이미지만 생성합니다. [자세히 알아보기...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-email) </li><li> **푸시 알림** - 전체 푸시 알림, 텍스트만 또는 이미지만 생성합니다. [자세히 알아보기...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-push) </li><li> **SMS** - 전체 SMS 또는 텍스트만 생성합니다. [자세히 알아보기](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-sms) </li><li> **웹 페이지** - 웹 페이지 이미지 또는 웹 페이지 텍스트를 생성합니다. [자세히 알아보기...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-web) </li><li> **콘텐츠** - 다양한 메시징 캠페인에 대한 콘텐츠를 생성합니다. [자세히 알아보기...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-experimentation)</li></ul> **참고:** AJO Prime 및 Ultimate의 Content Accelerator에서 출력되는 내용은 손실됩니다. | 예 |
| Journey Optimizer B2B 에디션 | 한 가지 질문 클래스로 [AI Assistant](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/get-started/ai-assistant)을(를) 사용합니다. <br> **제품 지식** - 제품 insight에 대한 Adobe 데이터 저장소(예: Experience League 제품 설명서)를 쿼리합니다. 이 출력은 고객을 구분하지 않습니다. | <ul><li>**입력:** 계정 여정에서 전자 메일을 보내는 방법</li><li>**출력:** 제품 지식을 Experience League(공개 설명서)에서 가져옵니다. [자세히 알아보기...](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/get-started/ai-assistant)</li></ul> | 아니요 |
| Campaign 관리 클라우드 서비스 | [콘텐츠 가속기를 위한 AI 도우미](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-gs) 마케팅 목표를 기반으로 개인화되고, 매력적이며, 효과적인 콘텐츠를 자동으로 생성합니다. 이 콘텐츠는 이메일, SMS, 푸시 등 여러 채널에서 브랜드 윤곽선 스타일, 레이아웃, 색조 등에 최적화된 콘텐츠입니다. | <ul><li> **전자 메일** - 전체 전자 메일, 텍스트만 또는 이미지만 생성합니다. [자세히 알아보기](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-content) </li><li> **SMS** - 전체 SMS 또는 텍스트만 생성합니다. [자세히 알아보기...](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-sms) </li><li> **푸시** - 매력적인 메시지를 만들고 콘텐츠를 생성합니다. [자세히 알아보기...](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-push) </li></ul> **참고:** Campaign Managed Cloud Services의 Content Accelerator에서 출력되는 내용은 손실되지 않습니다. | 예 |
| Customer Journey Analytics | CJA은 [AI Assistant](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/ai-assistant)를 사용하여 Experience League에서 제품 지식과 통찰력을 찾는 데 도움을 줍니다. <br>예를 들어, 새로운 사용자는 이를 사용하여 Customer Journey Analytics 개념을 학습하고 익숙하지 않은 제품 및 기능을 온보딩할 수 있습니다. <br>숙련된 사용자가 AI Assistant를 사용하여 보다 고급 사용 사례나 팁과 요령을 제시하고 빠른 속도로 작업을 수행할 수 있습니다. 개념을 이해하고, 문제를 해결하거나, 정보를 검색할 수 있습니다. [자세히 알아보기...](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/ai-assistant#knowledge) | <ul><li>**제품 지식 입력:** 계산된 지표를 작성하는 방법 </li><li> **제품 지식 출력:** 제품 지식은 Experience League(공개 설명서)에서 가져옵니다. </li></ul> | 아니요 |
| Customer Journey Analytics | [지능형 캡션](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/visualizations/intelligent-captions)은(는) Workspace 시각화의 선 시각화에 자연어 인사이트를 제공합니다. | <ul><li>**입력:** 선 시각화. **지능형 캡션**&#x200B;을 클릭하면 이러한 선 시각화에 따라 캡션이 자동으로 생성됩니다. </li><li> **출력:** 자동 생성된 자연어 캡션</li></ul> | 아니요 |
| Real-Time CDP | [AI Assistant](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home)를 사용하여 Experience League에서 제품 지식과 통찰력을 찾는 데 도움을 줍니다. 이 서비스는 데이터베이스를 쿼리하고 데이터베이스의 데이터를 사람이 읽을 수 있는 답변으로 변환합니다. 두 가지 클래스의 질문: <br> **제품 지식** - 제품 insight에 대한 Adobe 데이터 저장소(예: Experience League 제품 설명서)를 쿼리합니다. 이 출력은 고객을 구분하지 않습니다. <br> **Operational Insights(Beta)** - 고객의 AEP 샌드박스로 분할된 중앙 집중식 운영 데이터가 포함된 고객별 Operational Insights 데이터 저장소를 쿼리합니다. 속성, 대상, 데이터 흐름, 데이터 세트, 대상, 스키마 및 소스에서만 메타데이터를 가져오고 샌드박스 내의 데이터에 액세스하지 않습니다. <br>예를 들어 대상 [!DNL AI Assistant]에 대한 쿼리의 경우 대상 이름 및 기타 관련 메타데이터에는 액세스할 수 있지만 해당 대상 내의 프로필에는 액세스할 수 없습니다. | <ul><li>**제품 지식 입력:** 프로필 풍부성은 어떻게 계산됩니까? </li><li>**제품 지식 출력:** 제품 지식은 Experience League(공개 설명서)에서 가져옵니다. </li><li> **Operational Insights 입력:** 보유한 데이터 세트 수 </li><li> **Operational Insights 출력:** Operational Insights 출력은 고객의 비즈니스 개체(특성, 대상, 데이터 흐름, 데이터 세트, 대상, 스키마 및 원본)에서 가져온 메타데이터에 따라 다르며, 쿼리된 데이터가 포함된 특정 UI 페이지에 대한 링크를 포함합니다. </li></ul>예를 들어, [Experience Platform의 AI Assistant](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home)에서 _제품 지식_ 및 _Operational Insights_ 입력 테이블을 참조하십시오. | 아니요 |
| Marketo | [Dynamic Chat](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview)은(는) 사용자 지정 및 사전 승인된 질문과 답변과 대화 요약으로 AI 지원 대화를 만듭니다 | <ul><li> **질문 생성:** 콘텐츠를 추출하여 질문/응답을 생성하는 데 사용할 URL을 제공합니다. </li><li> **대화 요약:** 대화 요약을 생성합니다. </li></ul> [자세히 알아보기...](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/generative-ai/response-library) | 아니요 |
| Workfront | Workfront의 [AI Assistant](https://experienceleague.adobe.com/en/docs/workfront/using/basics/ai-assistant/ai-assistant-overview)는 자연어 대화에서 인앱 정보와 제안을 제공하여 작업을 완수하도록 도와줍니다. AI Assistant는 다음 기능을 제공합니다. 프로젝트/작업/문제/문서를 요약하고, Experience League의 Workfront 설명서에서 가져온 지침 또는 참조 정보를 제공하며, 계산된 사용자 정의 필드에 대한 공식을 생성하거나 구체화합니다. | <ul><li>**프로젝트 입력 요약:** 이 프로젝트 요약 </li><li> **프로젝트 출력 요약:** 프로젝트의 목적과 상태에 대한 간단한 설명을 반환하고 완료되었으며 아직 보류 중인 작업의 예를 제공하고 몇 가지 추가 세부 정보와 메모를 제공합니다.</li><li> **수식 입력 생성/세분화:** &quot;잘못된 식 오류를 제거하려면 이 수식을 다시 작성하십시오.&quot; </li><li> **수식 출력 생성/세분화:** 생성 또는 세분화된 수식. </li></ul>**참고:** AI Assistant는 수식의 크기와 복잡성에 따라 수정된 수식을 생성하는 데 몇 분 정도 걸릴 수 있습니다. | 아니요 |
