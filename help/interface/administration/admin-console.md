---
title: 사용자 및 제품 라이선스 관리
description: Admin Console for Experience Cloud 애플리케이션에서 사용자 및 제품 라이선스를 관리합니다.
application: Experience Cloud
index: true
feature: Admin Console
topic: Administration
role: Admin
level: Experienced
exl-id: c82821c4-aa5d-48ae-8bef-5937fede8db2
source-git-commit: 4b9318849f76941cb59ab5e9ca08045705c8ec46
workflow-type: tm+mt
source-wordcount: '728'
ht-degree: 4%

---

# 사용자 관리 및 제품 라이선스

이 페이지에서는 일반적인 사용자 및 제품 관리 설명서에 대한 링크와 함께 Experience Cloud 관리자를 위한 정보를 제공합니다.

모든 Adobe 애플리케이션에 적용할 수 있는 일반 ID 관리 도움말은 [Enterprise 및 Teams 관리 가이드](https://helpx.adobe.com/kr/enterprise/admin-guide.html)를 참조하십시오.

## Admin Console의 관리자 역할

Admin Console은 세 가지 기본 관리 역할을 제공하며, 각 역할에는 특정 수준의 액세스 및 책임이 있습니다.

| 역할 | 설명 |
| ------- | ------- |
| 시스템 관리자 | 전체 액세스 - 콘솔의 모든 측면을 관리합니다. <br>주요 책임: <br><ul><li>사용자를 추가, 제거 및 관리합니다.</li><li>제품 라이선스를 할당 및 취소합니다.</li><li>ID 및 인증 설정 구성</li><li>청구 정보를 보고 관리합니다.</li><li>추가 관리자 및 위임 역할을 설정합니다.</li></ul> **최적의 대상:** IT 관리자 또는 팀이 전체 조직의 Adobe 환경을 감독하는 데 도움이 됩니다. |
| 제품 관리자 | 제품별 관리 - 특정 Adobe 제품에 대한 액세스 및 권한을 제어합니다.<br>주요 책임:<ul><li>특정 제품에 대한 라이센스를 할당하고 관리합니다.</li><li>제품 프로필을 만들고 관리합니다.</li><li>할당된 제품 내에서 사용자를 추가하거나 제거합니다.</li></ul>   **Marketo Engage 또는 Adobe Creative Cloud과 같은 특정 소프트웨어를 관리하는 팀/사용자에 대한 최적의 용도:** |
| 제품 프로필 관리자 | 세분화된 역할 관리 - 제품 내의 사용자 그룹 및 권한 관리에 중점을 둡니다.<br>주요 책임:<ul><li>제품 프로필을 만들고 관리합니다.</li><li>프로필 내에서 권한 및 기능 액세스 권한을 할당합니다.</li><li>프로필 내에 사용자를 추가하거나 제거합니다.</li></ul> **가장 적합한 대상:** 부서 팀장 또는 팀 관리자가 전문화된 요구 사항을 가진 소규모 그룹을 감독합니다. <br> 관리자는 조직의 요구 사항에 따라 역할을 결합하여 유연성을 높일 수 있습니다. |

## Experience Cloud용 Admin Console

Experience Cloud 응용 프로그램에 대한 ID 및 제품 라이선스를 관리하려면 [Admin Console](https://adminconsole.adobe.com/enterprise/)&#x200B;(으)로 이동하십시오.

다음은 Admin Console에서 관리자로 시작할 때 필요할 수 있는 리소스입니다.

### 리소스 설정

| 도움말 링크 | 설명 |
| ------- | ------- |
| [ID 및 SSO(Single Sign-On) 설정](https://helpx.adobe.com/kr/enterprise/using/set-up-identity.html) | **[!UICONTROL Admin Console]** > **[!UICONTROL 설정]** <br> SSO(Single Sign-On)를 사용하거나 사용하지 않고 다른 ID 유형의 사용자 계정을 설정하는 방법을 알아봅니다. Adobe 소프트웨어에 대한 SSO를 설정하고, SAML 설정을 구성하고, 가장 일반적인 질문과 오류를 살펴봅니다. |
| [디렉터리 트러스트를 통해 조직 설정](https://helpx.adobe.com/enterprise/using/directory-trust.html) | 다른 조직에서 이미 요청한 도메인에 대해 사용자를 인증합니다. 조직을 찾고 전환하는 방법에 대한 자세한 내용은 [Experience Cloud의 조직](organizations.md)을 참조하세요. |
| [인증 설정(enterprise)](https://helpx.adobe.com/enterprise/using/authentication-settings.html) | Admin Console은 안전 및 보안을 보장하기 위해 여러 암호 보호 수준 및 정책을 지원합니다. 암호 보호 수준을 사용하여 조직의 모든 사용자에게 적용하도록 지정할 수 있습니다. |
| [개인 정보 및 보안 연락처](https://helpx.adobe.com/enterprise/using/security-contacts.html) | 조직 및 사용자의 데이터를 보호합니다. 소프트웨어 솔루션과 관련된 보안 사고가 발생하면 해당 규정 준수 담당자에게 알림이 전송됩니다. 기업은 데이터 보호, 무결성 및 기타 규정 준수 관련 업무를 담당하는 인력을 보유하고 있습니다. 따라서 보안 사고 발생 시 신속한 알림을 받을 수 있도록 이러한 담당자에 대한 연락처 정보가 매우 중요합니다. |

### 사용자 관리

| 도움말 링크 | 설명 |
| ------- | ------- |
| [여러 사용자 관리](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) | **[!UICONTROL Admin Console]** > **[!UICONTROL 사용자]** <br>Admin Console에 CSV 일괄 업로드를 통해 여러 사용자를 관리하는 방법에 대해 알아봅니다. |
| [ID 유형](https://helpx.adobe.com/kr/enterprise/using/identity.html) | ID 유형을 사용하면 조직이 사용자의 계정 및 데이터를 다양한 수준으로 제어할 수 있습니다. 선택한 ID 모델은 조직이 자산을 저장하고 공유하는 방식에 영향을 줍니다. Federated ID 및 Enterprise ID 모델은 조직에서 만들고 관리하는 반면 Adobe ID는 개인이 만들고 관리합니다. |
| [사용자 동기화 도구](https://helpx.adobe.com/enterprise/using/user-sync.html)&#x200B;(UST) | Adobe 사용자 동기화 도구는 조직의 ID 관리 시스템(예: Active Directory)과 Adobe Admin Console 간의 사용자 데이터 동기화를 자동화하는 데 사용되는 데스크탑 애플리케이션입니다. 관리자는 이 도구를 사용하여 Adobe 제품 전반에 대한 사용자 프로비저닝, 업데이트 및 비활성화를 간소화할 수 있습니다. |
| [사용자 세부 정보 보기(관리 도구)](admin-tool-experience-cloud.md) | [!UICONTROL 관리 도구]에서 모든 Experience Cloud 사용자 및 정책을 세부 정보와 함께 정렬 및 필터링 가능한 목록으로 봅니다. |

### 보고서 및 로그

| 도움말 링크 | 설명 |
| ------- |------- |
| [감사 로그](https://helpx.adobe.com/enterprise/using/audit-logs.html) | **[!UICONTROL 인사이트]** > **[!UICONTROL 로그]** > **[!UICONTROL 감사 로그]** <br> Admin Console에서 변경한 모든 내용을 추적합니다. |


## 애플리케이션별 리소스

이러한 링크는 특정 Experience Cloud 애플리케이션에 대한 관리 정보를 찾는 데 도움이 됩니다.

<!-- | Application | Link to resource|
| ------- | ------- |
|  [!DNL Analytics] <p>Customer Journey Analytics| [Analytics in the Adobe Admin Console overview](https://experienceleague.adobe.com/en/docs/analytics/admin/admin-console/home) <p>[Administration requirements](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/workspace-faq/frequently-asked-questions-analysis-workspace) |
| [!DNL Audience Manager] | [Audience Manager user migration to Admin Console](https://experienceleague.adobe.com/en/docs/audience-manager/user-guide/features/administration/admin-console-migration) |
| [!DNL Campaign] v8 |  [Get started with permissions](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/gs-permissions) |
| [!DNL Campaign Standard] to [!DNL Campaign v8] | [User access management from Campaign Standard to Campaign V8](https://experienceleague.adobe.com/en/docs/campaign-web/acs-to-ac/user-management-acs) |
| [!DNL Commerce] | [Configure the Commerce Admin Integration with Adobe ID](https://experienceleague.adobe.com/en/docs/commerce-admin/start/admin/ims/adobe-ims-config) |
| [!DNL Dynamic Media Classic] | [Administration setup](https://experienceleague.adobe.com/en/docs/dynamic-media-classic/using/setup/administration-setup#user_administration) |
| [!DNL Experience Manager as a Cloud Service] |  [Accessing the Admin Console](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/onboarding/journey/admin-console) |
| [!DNL Experience Platform] <p>[!DNL Data Collection] | [Access control UI overview](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/ui/overview) <p>[Permission management for data collection in Experience Platform](https://experienceleague.adobe.com/en/docs/experience-platform/collection/permissions)|
| [!DNL GenStudio for Performance Marketing] | [Provision Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/intro/product-provisioning) |
| [!DNL Journey Optimizer] | [Manage users and roles](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/access-control/permissions) |
| [!DNL Journey Optimizer B2B Edition] | [User management](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/admin/user-management) |
|[!DNL  Journey Orchestration] | [Access management](https://experienceleague.adobe.com/en/docs/journeys/using/starting-with-journeys/access-management) |
| [!DNL Marketo Engage] | [Understanding Marketo Subscription and User Migration to the Adobe Admin Console](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console) |
| [!DNL Marketo Measure] | [Adobe Admin Console Setup](https://experienceleague.adobe.com/en/docs/marketo-measure/using/configuration-and-setup/getting-started-with-marketo-measure/adobe-admin-console-setup) |
| [!DNL Mix Modeler] | [Access controls](https://experienceleague.adobe.com/en/docs/mix-modeler/using/data-governance/access-controls) |
| [!DNL Pass] | [Get started with Account IQ](https://experienceleague.adobe.com/en/docs/pass/aiq-help/get-started) |
| [!DNL Target] | [Administrator first steps](https://experienceleague.adobe.com/en/docs/target/using/administer/start-target) <p> [User management](https://experienceleague.adobe.com/en/docs/target/using/administer/manage-users/user-management) |
| [!DNL Workfront] | [Manage users in the Adobe Admin Console](https://experienceleague.adobe.com/en/docs/workfront/using/administration-and-setup/add-users/create-manage-users/admin-console) |

 -->

* [Analytics](https://experienceleague.adobe.com/en/docs/analytics/admin/admin-console/home)
* [Customer Journey Analytics](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/workspace-faq/frequently-asked-questions-analysis-workspace)
* [Audience Manager](https://experienceleague.adobe.com/en/docs/audience-manager/user-guide/features/administration/admin-console-migration)
* [Campaign v8](https://experienceleague.adobe.com/ko/docs/campaign/campaign-v8/admin/permissions/gs-permissions)
* [Campaign Standard](https://experienceleague.adobe.com/en/docs/campaign-web/acs-to-ac/user-management-acs)
* [상거래](https://experienceleague.adobe.com/en/docs/commerce-admin/start/admin/ims/adobe-ims-config)
* [Dynamic Media Classic](https://experienceleague.adobe.com/en/docs/dynamic-media-classic/using/setup/administration-setup#user_administration)
* [Experience Manager as a Cloud Service](https://experienceleague.adobe.com/ko/docs/experience-manager-cloud-service/content/onboarding/journey/admin-console)
* [Experience Platform](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/ui/overview) 및 [데이터 수집](https://experienceleague.adobe.com/en/docs/experience-platform/collection/permissions)
* [GenStudio for Performance Marketing](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/intro/product-provisioning)
* [Journey Optimizer](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/access-control/permissions)
* [Journey Optimizer B2B edition](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/admin/user-management)
* [Journey Orchestration](https://experienceleague.adobe.com/en/docs/journeys/using/starting-with-journeys/access-management)
* [Marketo Engage](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console)
* [Marketo Measure](https://experienceleague.adobe.com/en/docs/marketo-measure/using/configuration-and-setup/getting-started-with-marketo-measure/adobe-admin-console-setup)
* [Mix Modeler](https://experienceleague.adobe.com/en/docs/mix-modeler/using/data-governance/access-controls)
* [Adobe Pass](https://experienceleague.adobe.com/en/docs/pass/aiq-help/get-started)
* [Target](https://experienceleague.adobe.com/en/docs/target/using/administer/start-target)
* [Workfront](https://experienceleague.adobe.com/en/docs/workfront/using/administration-and-setup/add-users/create-manage-users/admin-console)

모든 Adobe 응용 프로그램에 대한 대부분의 관리 콘솔 도움말은 [Enterprise 및 Teams 관리 안내서](https://helpx.adobe.com/kr/enterprise/admin-guide.html)에 설명되어 있습니다.
