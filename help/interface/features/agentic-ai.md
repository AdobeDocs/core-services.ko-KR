---
title: Experience Cloud 애플리케이션의 Agentic AI
description: Experience Cloud 애플리케이션에서 Agentic AI를 사용할 수 있는 위치를 알아봅니다.
solution: Experience Cloud
landing-page-name: ai
landing-page-breadcrumb-title: AI Documentation
topic: Artificial Intelligence
feature: Agentic AI, AI Tools
role: Admin, User
level: Intermediate
exl-id: c1a8f9a7-4752-4040-b5f0-dc775417f536
source-git-commit: e63dd988abba199049da2b3620eed9ebf51043d1
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 5%

---

# Experience Cloud의 Experience Platform 에이전트

업데이트됨: **2025년 12월 2일**

Adobe [!DNL Experience Platform] [Agent Orchestrator](https://experienceleague.adobe.com/ko/docs/experience-cloud-ai/experience-cloud-ai/home) 및 Adobe Experience Platform 에이전트를 사용하면 Experience Cloud 애플리케이션에서 에이전트 기능을 사용할 수 있습니다.

다음을 통해 이러한 에이전트 기능에 액세스할 수 있습니다.

* [기존 [!DNL Experience Cloud] 앱](#existing-apps): 이러한 응용 프로그램은 자체적으로 작동하지만 Experience Platform Agent Orchestrator 및 에이전트를 활성화하면 이러한 응용 프로그램에서 실행되는 기존 작업 및 워크플로의 효율성이 향상되고 이를 활용하는 팀의 생산성이 향상됩니다. 현재 라이선스가 부여된 Experience Cloud 애플리케이션에서 이러한 에이전트 기능을 활성화하려면 Agent Orchestrator 라이선스도 구매해야 합니다.

* [AI-first [!DNL Experience Cloud] 앱](#ai-first-apps): 이러한 응용 프로그램은 핵심 요소에 있는 생성 또는 아젠틱 AI로 빌드됩니다. 이들은 주요 작업에 생성 AI 또는 아젠틱 AI를 사용하며, 아젠틱 기능은 이미 AI 우선 애플리케이션 라이선스에 포함되어 있으며 Agent Orchestrator 라이선스가 필요하지 않습니다.

## 기존 [!DNL Experience Cloud]개 응용 프로그램

다음은 기존 experience cloud 애플리케이션에서 사용할 수 있고 Agent Orchestrator 라이선스에서 활성화된 Experience Platform 에이전트 목록입니다.

| 에이전트 이름 | 가용성 | 기능 | 지원되는 애플리케이션 |
|---|----------|----------|----------|
| [Audience Agent](https://experienceleague.adobe.com/ko/docs/experience-cloud-ai/experience-cloud-ai/agents/audience) | 사용 가능 | 자연어 프롬프트를 사용하여 팀이 대상을 만들고, 관리하고, 최적화할 수 있도록 함으로써 보다 쉽고, 효율적이며, 시장 출시 속도를 높일 수 있습니다. | <ul><li>Real-Time CDP (B2B 및 B2C 에디션)</li><li>Adobe Journey Optimizer (B2B 및 B2C 에디션)</li></ul> |
| [콘텐츠 최적화 에이전트](https://experienceleague.adobe.com/ko/docs/experience-manager-cloud-service/content/ai-in-aem/business-agents/content-optimization/using) | 사용 가능 | 자연어 프롬프트를 사용하여 소스 에셋에서 시각적 콘텐츠 변형을 쉽게 만들 수 있습니다. | <ul><li>Adobe Experience Manager([OpenAPI를 사용하는 Dynamic Media](https://experienceleague.adobe.com/ko/docs/experience-manager-cloud-service/content/assets/dynamicmedia/dynamic-media-open-apis/dynamic-media-open-apis-overview) 사용)</li></ul> |
| [Data Insights Agent](https://experienceleague.adobe.com/ko/docs/analytics-platform/using/cja-overview/cja-b2c-overview/data-analysis-ai) | 사용 가능 | 데이터에 대한 데이터 질문에 신속하게 답변할 수 있습니다. 데이터 보기의 구성 요소를 사용하고 실제 데이터를 사용하여 Analysis Workspace에서 관련 시각화를 구축합니다. | <ul><li>Customer Journey Analytics</li></ul> |
| [개발 에이전트](https://experienceleague.adobe.com/ko/docs/experience-manager-cloud-service/content/ai-in-aem/business-agents/development/overview) | 사용 가능 | AEM CS 개발자와 기술 관리자가 근본 원인을 분석하고 수정 사항을 제시하여 Cloud Manager 파이프라인의 빌드 단계 오류를 해결할 수 있도록 지원합니다. | <ul><li>AEM Cloud Service 및 Adobe Managed Services의 AI 지원</li></ul> |
| [검색 에이전트](https://experienceleague.adobe.com/ko/docs/experience-manager-cloud-service/content/ai-in-aem/business-agents/discovery/using) | 사용 가능 | 이미지, 비디오, 텍스트 기반 문서, 콘텐츠 조각 및 양식에서 Experience Manager 콘텐츠를 즉시 찾아 표시하도록 간소화된 자연어 프롬프트를 통해 작성 속도를 높이고 검색 속도를 높입니다. | <ul><li>Adobe Experience Manager 클라우드 서비스</li></ul> |
| [Experience Production Agent](https://experienceleague.adobe.com/ko/docs/experience-manager-cloud-service/content/ai-in-aem/business-agents/production/overview) | 사용 가능 | CMS에서 많은 노력과 대량의 작업을 자동화합니다. 이 에이전트는 길고 수동적인 프로세스를 모든 경험을 최신 상태로 일관되게 유지하는 빠른 AI 지원 워크플로우로 전환하여 비즈니스의 목표 달성에 도움이 됩니다. | <ul><li>Adobe Experience Manager 클라우드 서비스 및 Edge Delivery Services</li></ul> |
| [거버넌스 에이전트](https://experienceleague.adobe.com/ko/docs/experience-manager-cloud-service/content/ai-in-aem/business-agents/governance/overview) | 사용 가능 | Experience Manager 전반에 걸쳐 보안, 규정 및 브랜드 정책을 시행하여 브랜드 무결성 및 규정 준수를 보호합니다. 이 에이전트는 브랜드 거버넌스를 적용하여 시각적 및 메시징 표준을 관리합니다. 또한 세분화된 권한을 사용하여 액세스 및 콘텐츠 변경을 관리하고 DRM을 통합하여 라이선싱 및 사용 제한을 유지합니다. | <ul><li>Adobe Experience Manager Sites</li><li>Adobe Experience Manager Assets</li><li>Adobe Experience Manager Forms </li></ul> |
| [Journey Agent](https://experienceleague.adobe.com/ko/docs/experience-cloud-ai/experience-cloud-ai/agents/ajo-agent-analyze) | 사용 가능 | 팀이 규모에 맞게 멀티 터치 고객 여정을 신속하게 만들고, 분석하고, 최적화할 수 있도록 합니다. | <ul><li>Adobe Journey Optimizer (B2B 및 B2C 에디션)</li></ul> |
| [제품 지원 에이전트](https://experienceleague.adobe.com/ko/docs/experience-platform/ai-assistant/new-features/customer-support) | 사용 가능 | 워크플로우를 종료하지 않고 지원 문제를 해결하고, 고객 지원 티켓을 만들고, AI Assistant를 사용하여 사례 진행 상황을 추적합니다. | <ul><li>Real-Time CDP (B2B 및 B2C 에디션)</li><li>Adobe Journey Optimizer (B2B 및 B2C 에디션)</li><li>Adobe Journey Optimizer B2B edition</li><li>Customer Journey Analytics</li><li>Adobe Experience Manager</li></ul> |

<!-- | Agent name  | Availability | Capabilities | Supported applications   |
|---|----------|----------|----------|
| [Audience Agent](https://experienceleague.adobe.com/ko/docs/experience-cloud-ai/experience-cloud-ai/agents/audience)  | Available | Empower your teams to create, manage, and optimize audiences using natural language prompts for greater ease, efficiency, and speed to market. | <ul><li>Real-Time CDP (B2B and B2C editions)</li><li>Adobe Journey Optimizer (B2B and B2C editions)</li></ul> |
| [Data Insights Agent](https://experienceleague.adobe.com/ko/docs/analytics-platform/using/cja-overview/cja-b2c-overview/data-analysis-ai)  | Available | Quickly answers data questions about your data. It builds relevant visualizations in Analysis Workspace using components from your data view and using your actual data. | <ul><li>Customer Journey Analytics</li></ul>  |
| [Journey Agent](https://experienceleague.adobe.com/ko/docs/experience-cloud-ai/experience-cloud-ai/agents/ajo-agent-analyze) | Available | Enable your teams to quickly create, analyze, and optimize multi-touch customer journeys at scale. | <ul><li>Adobe Journey Optimizer (B2B and B2C editions)</li></ul>    |
| [Product Support Agent](https://experienceleague.adobe.com/ko/docs/experience-platform/ai-assistant/new-features/customer-support) | Available | Troubleshoot support issues without leaving your workflows, create customer support tickets, and track case progress using AI Assistant. | <ul><li>Real-Time CDP (B2B and B2C editions)</li><li>Adobe Journey Optimizer (B2B and B2C editions)</li><li>Adobe Journey Optimizer B2B Edition</li><li>Customer Journey Analytics</li><li>Adobe Experience Manager</li></ul>  | -->


## AI 우선 Experience Cloud 애플리케이션

다음은 AI 우선 애플리케이션에서 사용할 수 있으며 이러한 AI 우선 애플리케이션에 라이센스를 부여하여 사용할 수 있는 Experience Platform 에이전트 목록입니다.

| 에이전트 이름 | 가용성 | 기능 | 지원되는 애플리케이션 |
|---|----------|----------|----------|
| [실험 에이전트](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/content-experiment/experiment/experiment-accelerator-security) | 사용 가능 | 인사이트를 자동화, 분석 및 합성하므로 수작업 프로세스를 줄이면서 중앙 집중식 작업 공간에서 영향력이 큰 실험 및 성장 기회를 신속하게 식별할 수 있습니다. | <ul><li>AJO Experimentation Accelerator</li></ul> |
| [LLM 최적화 에이전트](https://experienceleague.adobe.com/ko/docs/llm-optimizer/using/home) | 사용 가능 | AI 기반 검색 환경에서 가시성, 정확성 및 영향력을 강화하고, AI가 생성한 답변에서 브랜드 존재에 대한 통찰력을 제공하고, 규범적인 콘텐츠 권장 사항을 제공하고, 최적화 수정 사항을 자동화합니다. | <ul><li>Adobe LLM Optimizer</li></ul> |
| [Site Optimization Agent](https://experienceleague.adobe.com/ko/docs/experience-manager-sites-optimizer/content/home) | 사용 가능 | 향상된 웹 사이트를 자동으로 감지하고 배포하여 비즈니스 효과를 극대화합니다. 생성 AI와 여러 모니터링 기술을 사용하면 사이트 트래픽 획득, 참여 등을 향상시킬 수 있습니다 | <ul><li>AEM Sites Optimizer</li></ul> |

<!-- | Agent name  | Availability | Capabilities | Supported applications   |
|---|----------|----------|----------|
| [Content Optimization Agent](https://experienceleague.adobe.com/ko/docs/experience-manager-cloud-service/content/ai-in-aem/business-agents/content-optimization/using) | Available | Simplify creating visual content variants from source assets using natural language prompts.|  <ul><li>Adobe Experience Manager (with [Dynamic Media with OpenAPI](https://experienceleague.adobe.com/ko/docs/experience-manager-cloud-service/content/assets/dynamicmedia/dynamic-media-open-apis/dynamic-media-open-apis-overview))</li></ul>  |
| [Development Agent](https://experienceleague.adobe.com/ko/docs/experience-manager-cloud-service/content/ai-in-aem/business-agents/development/overview) | Available | Helps AEM CS developers and technical administrators troubleshoot build-step failures in the Cloud Manager pipeline by analyzing the root cause and suggesting fixes.|  <ul><li>AI Assistant in AEM Cloud Service and Adobe Managed Services</li></ul>  |
| [Discovery Agent](https://experienceleague.adobe.com/ko/docs/experience-manager-cloud-service/content/ai-in-aem/business-agents/discovery/using) | Available | Speed authoring and boost discovery with simplified natural-language prompts to instantly find and surface Experience Manager content across images, videos, text-based documents, content fragments, and forms.|  <ul><li>Adobe Experience Manager Cloud Services</li></ul>  |
| [Experience Production Agent](https://experienceleague.adobe.com/ko/docs/experience-manager-cloud-service/content/ai-in-aem/business-agents/production/overview) | Available | Automates high-effort and high-volume tasks in the CMS. This agent turns manual, lengthy processes into fast, AI-assisted workflows that keep every experience current and consistent, helping your business achieve your goals.|  <ul><li>Adobe Experience Manager Cloud Services and Edge Delivery Services</li></ul>  |
| [Experimentation Agent](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/content-experiment/experiment/experiment-accelerator-security) | Available | Automate, analyze, and synthesize insights, so you can quickly identify high-impact experiments and growth opportunities from a centralized workspace — all while reducing manual processes.  | <ul><li>AJO Experimentation Accelerator</li></ul>   |
| [Governance Agent](https://experienceleague.adobe.com/ko/docs/experience-manager-cloud-service/content/ai-in-aem/business-agents/governance/overview) | Available | Safeguard brand integrity and compliance by enforcing security, regulatory, and brand policies across Experience Manager. This agent applies brand governance to maintain visual and messaging standards. It uses granular permissions to manage access and content changes, and incorporates DRM to uphold licensing and usage constraints. |  <ul><li>Adobe Experience Manager Sites</li><li>Adobe Experience Manager Assets</li><li>Adobe Experience Manager Forms </li></ul>  |
| [LLM Optimization Agent](https://experienceleague.adobe.com/ko/docs/llm-optimizer/using/home) | Available | Enhance visibility, accuracy, and influence in AI-driven search environments, provide insights into brand presence in AI-generated answers, offer prescriptive content recommendations, and automate optimization fixes. | <ul><li>Adobe LLM Optimizer</li></ul>   |
| [Site Optimization Agent](https://experienceleague.adobe.com/ko/docs/experience-manager-sites-optimizer/content/home) | Available | Maximize business impact by automatically detecting and deploying website enhancements. Using generative AI and multiple monitoring technologies, you can increase site traffic acquisition, engagement, and more | <ul><li>AEM Sites Optimizer</li></ul> | -->

## 이 항목에 대한 추가 도움말

* Experience Cloud의 [AI](https://experienceleague.adobe.com/ko/docs/ai) 설명서 홈

[!BADGE Adobe for Business에 대해 자세히 알아보기]{type=Informative url="https://business.adobe.com/kr/products/experience-platform/agent-orchestrator.html" tooltip="Business.adobe.com으로 이동"}
