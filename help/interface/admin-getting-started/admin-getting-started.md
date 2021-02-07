---
description: Adobe Experience Cloud 사용자 권한 및 제품 프로필을 관리하는 방법을 알아보십시오. Adobe Admin Console 로그인 및 Experience Cloud 브라우저 지원에 대한 자세한 내용을 살펴보십시오.
solution: Admin
title: '사용자 및 제품 관리 방법 '
index: true
translation-type: ht
source-git-commit: 119bbd98e78fe55ae30ef874e2125fa196221363
workflow-type: ht
source-wordcount: '1421'
ht-degree: 100%

---


# Experience Cloud 사용자 및 제품 관리 {#topic_3FCB4099640647E3B2411ADBFCE81909}

Admin Console에 로그인, Experience Cloud 사용자 권한과 제품 프로필 관리 및 브라우저 지원 방법에 대해 알아봅니다.

>[!IMPORTANT]
>
>Admin Console에서 사용자 관리는 새 용어, 인터페이스 및 탐색을 소개합니다. 다음 정보는 이러한 변경 사항에 대해 설명하고 추가 도움말 자료에 대한 링크를 제공합니다. 이 도움말은 [Enterprise Administration 사용 안내서](https://helpx.adobe.com/kr/enterprise/managing/user-guide.html)에 있는 모든 Adobe 클라우드 제품에 대한 정보를 보완합니다.

## Experience Cloud 사용자 관리의 새로운 기능 {#concept_06A0A13362F644FB90F947238407637A}

Adobe Experience Cloud 사용자 및 제품 관리의 최신 기능에 대해 알아보십시오.

<!-- ### Business ID type

Adobe is introducing an identity type called Business ID. This identity type improves the control of user and product management. Adobe is migrating all Adobe IDs (owned by individuals) that are used for business to the new enterprise Business IDs owned by your organization.

If you are an existing Experience Cloud customer, Adobe will migrate all your users with Adobe IDs in the Admin Console to Business IDs. If you are a new enterprise or teams customer, you will add users to the Admin Console using one of the available identity types: Business ID, Enterprise ID, or Federated ID.

What to do

* Your users will need to accept Terms of Use (TOU) changes prior to accounts being migrated to Type2e. 
* Users that belong to multiple organizations might see a Profile Selection screen during the login workflow and need to select the correct one. This ensures that they are logging into the correct organization. (There might be multiple profiles to choose from if a user was a member of multiple organizations before the migration.)

Beginning May 2020, enterprise administrators cannot use the Adobe ID for new organizations created in the Admin Console. Latest: https://wiki.corp.adobe.com/pages/viewpage.action?spaceKey=engage&title=Type2e+DX+GTM-->

### 관리 도구

관리자는 관리 도구에서 모든 Experience Cloud 사용자 목록과 세부 사항을 정렬 및 필터링 가능한 목록으로 볼 수 있습니다. [관리 도구에서 Experience Cloud 사용자 보기](admin-tool-experience-cloud.md)를 참조하십시오.

## Admin Console에 로그인 {#section_705072FD4EBE4B70BC69EC81F2BB8669}

관리자는 더 이상 특정 제품 솔루션으로 사용자를 관리하지 않습니다. 이제 Experience Cloud의 사용자 및 제품 관리는 Admin Console에서 이루어집니다.

Admin Console에 로그인하려면,

1. [https://adminconsole.adobe.com/enterprise/](https://adminconsole.adobe.com/enterprise/#)로 이동합니다.
1. [Adobe ID나 Enterprise ID](https://helpx.adobe.com/kr/enterprise/help/identity.html)와 암호를 입력합니다.

또는 Experience Cloud 메뉴(![](assets/menu-icon.png))에서 **[!UICONTROL 관리]** > **[!UICONTROL Admin Console 시작]**&#x200B;을 클릭합니다.

**관련 도움말**

Creative Cloud 및 Document Cloud에 대한 [관리 사용 안내서](https://helpx.adobe.com/kr/enterprise/using/users.html). 일부 정보는 [ID 유형 관리](https://helpx.adobe.com/kr/enterprise/help/identity.html)와 같이, Experience Cloud 사용자 관리와 관련이 있습니다.

[로그인 및 프로필 설정 관리](../admin-getting-started/getting-started-experience-cloud.md#topic_AC564B6795334DE39359ADD87F52F2E0).

## 제품 프로필 및 그룹 {#section_AB50558124D541CF80A0D3D76D35A4BF}

제품 프로필을 추가하면 그룹을 사용하여 솔루션 제품 및 서비스를 관리하던 이전 방식에서 변경될 것임을 나타냅니다. Admin Console에서 권한은 사용자에게 지정할 수 있는 제품 및 서비스 그룹인 제품 프로필을 기반으로 합니다.

예를 들면 Analytics에서 보고서 세트, 지표, 차원 등과 함께 Analysis Workspace 및 Report Builder와 같은 보고 도구의 컬렉션을 구성할 수 있습니다. 프로필에 사용자를 추가하여 제품 프로필에 대한 권한을 부여할 수 있습니다. 이 페이지에서.[제품 프로필에 Analytics 액세스 권한을 지정](../admin-getting-started/admin-getting-started.md#task_040673FE3E3E429B9531FBCB8B6A4391)을 참조하십시오.

**관리 권한 위임**

이 페이지에서 [제한된 관리 권한 위임](../admin-getting-started/admin-getting-started.md#task_3A072C4AA9734BC59FFA7E015271BC7E)을 참조하십시오.

## Analytics {#section_97DE101F92CD494AB073893680992F1A}

Admin Console에서 Analytics 사용자 및 제품 권한을 관리합니다.

[제품 프로필에 Analytics 액세스 권한을 지정](../admin-getting-started/admin-getting-started.md#task_040673FE3E3E429B9531FBCB8B6A4391)합니다(이 페이지에서).

**사용자 계정 마이그레이션**

Analytics 사용자 ID 마이그레이션 도구는 Analytics 관리자가 Analytics 사용자 관리에서 [Adobe Admin Console](https://adminconsole.adobe.com/enterprise/)로 사용자 계정을 마이그레이션하도록 지원하는 데 사용할 수 있습니다.

계정 마이그레이션이 단계적으로 고객에게 배포되고 있습니다. Adobe에서는 기존 사용자 계정을 **[!UICONTROL 관리 도구]** > **[!UICONTROL 사용자 관리]**&#x200B;에서 Admin Console로 마이그레이션할 때 사용자에게 알리고 지원합니다.

마이그레이션 후 사용자는 Adobe ID(또는 Enterprise ID)를 사용하여 로그인하고 [experiencecloud.adobe.com](https://experiencecloud.adobe.com)에서 해당 Experience Cloud 솔루션 및 서비스를 인증합니다. 사용자가 이전 계정([!DNL my.omniture.com] 및 [!DNL sc.omniture.com])을 통해 로그인하려고 하면 [!DNL experiencecloud.adobe.com]으로 리디렉션됩니다.

**관련 도움말**

[Analytics 사용자 ID 마이그레이션](https://docs.adobe.com/content/help/ko-KR/analytics/admin/user-product-management/user-management/migrate-users/c-migration-tool.html)

## Adobe Target - 제품 프로필과 작업 공간 {#section_3860AF177C9E4C7E9C390D36A414F353}

Adobe Target에서 작업 공간은 제품 프로필입니다. 이를 통해 조직에서는 특정 사용자 세트를 특정 속성 세트에 할당할 수 있습니다. 여러 가지 방식에서 작업 공간은 Adobe Analytics의 보고서 세트와 비슷합니다.

다음을 참조하십시오.

* [Enterprise 사용자 권한](https://docs.adobe.com/content/help/ko-KR/target/using/administer/manage-users/enterprise/property-channel.html)
* [제품 및 프로필 관리](https://helpx.adobe.com/kr/enterprise/using/manage-products-and-profiles.html)
* 비디오: [Adobe Admin Console에서 Adobe Target 작업 공간을 구성하는 방법](https://helpx.adobe.com/kr/target/kb/how-to-configure-target-workspaces-in-adobe-admin-console0.html)

## 캠페인 - 제품 프로필, 테넌트 및 보안 그룹 {#section_09CDF75366444CF5810CF321B7C712F3}

Campaign의 *테넌트*&#x200B;는 Admin Console 제품 페이지에서 *제품*&#x200B;으로 표시됩니다.

*보안 그룹*&#x200B;은 제품 프로필로 표시됩니다.

보안 그룹과 보안 그룹에 사용자를 지정하는 것에 대한 자세한 내용은 [그룹 및 사용자 관리](https://helpx.adobe.com/kr/campaign/standard/administration/using/managing-groups-and-users.html)를 참조하십시오.

## Experience Platform Launch {#section_F2DA6778DD2D48AA8F794041971EE6B1}

Experience Platform Launch는 Admin Console에서 제품 페이지에 표시됩니다. Launch 제품 프로필에 다른 솔루션 및 서비스를 포함할 수 있습니다.

[사용자 관리](https://docs.adobelaunch.com/launch-reference/administration/user-permissions)를 참조하여 Admin Console에서의 사용자 권한에 대해 알아보고, 프로필에 권한 지정을 포함하여 Launch 관련 옵션을 설정합니다.

## Experience Manager as a Cloud Service

Adobe Enterprise 고객은 Adobe Admin Console에서 IMS 조직으로 표시됩니다. 이것은 Adobe 고객이 사용자 및 그룹에 대한 제품 권한을 관리하는 데 사용하는 포털입니다. AEM 고객은 Adobe Admin Console을 사용하여 AEM as a Cloud Service에 대한 제품 권한 및 IMS 인증을 관리할 수 있습니다.

[AEM as a Cloud Service를 위한 IMS 지원](https://docs.adobe.com/content/help/ko-KR/experience-manager-cloud-service/security/ims-support.html#managing-products-and-user-access-in-admin-console)을 참조하십시오.

## Experience Platform Launch {#section_3A41CF2BD5994B9891537D063571D4ED}

사용자를 [!UICONTROL Platform Launch]에 초대하고 사용자 역할과 권한을 할당합니다.

[사용자 권한](https://experienceleague.adobe.com/docs/launch/using/admin/user-permissions.html?lang=ko-KR#admin)을 참조하십시오.

## Audience Manager {#section_C31E3FA8A1E14463B1B3E07235F1983C}

Audience Manager 사용자를 만들고 그룹에 지정합니다. 제한(트레이트, 세그먼트, 대상 및 [!DNL AlgoModel])을 볼 수도 있습니다.

Audience Manager 도움말의 [관리](https://docs.adobe.com/content/help/ko-KR/dtm/using/admin/users.html)를 참조하십시오.

## Experience Cloud 제품 관리 {#task_16335111C52D40E9BAC73D0699584DBF}

제품 프로필을 작성하여 권한 그룹에 지정합니다.

사용자를 조직에 초대할 때 사용자에게 제품 및 제품 프로필에 대한 액세스 권한을 제공할 수 있습니다. 제한된 관리 권한을 사용자에게 위임할 수도 있습니다. 마찬가지로 사용자 그룹을 작성한 후, 제품 프로필에 액세스할 수 있는 그룹을 추가할 수 있습니다.

1. [Admin Console](https://adminconsole.adobe.com/enterprise/)에서 **[!UICONTROL 제품]**&#x200B;을 클릭합니다.
1. **[!UICONTROL 새 프로필]**&#x200B;을 클릭합니다.
1. 프로필 세부 사항을 구성한 후 **[!UICONTROL 다음]**&#x200B;을 클릭합니다.
1. **[!UICONTROL 완료]**&#x200B;를 클릭합니다.

다음에서 추가 도움말을 참조하십시오.

* [제품 및 프로필 관리](https://helpx.adobe.com/kr/enterprise/using/manage-products-and-profiles.html)
* 자세한 내용은 Target 도움말의 [Enterprise 사용자 권한](https://docs.adobe.com/content/help/ko-KR/target/using/administer/manage-users/enterprise/property-channel.html)을 참조하십시오.
* 비디오: [Adobe Admin Console에서 Adobe Target 작업 공간을 구성하는 방법](https://helpx.adobe.com/kr/target/kb/how-to-configure-target-workspaces-in-adobe-admin-console0.html)

## 제품 프로필에 Analytics 액세스 권한 지정 {#task_040673FE3E3E429B9531FBCB8B6A4391}

제품 프로필에 Analytics 보고서 액세스 권한(보고서 세트, 지표, 차원 등)을 지정합니다.

예를 들면 특정 지표와 차원(eVars 등)에 대한 권한 및 세그먼트나 계산된 지표 생성과 같은 기능을 사용하여 여러 Analytics 도구([!UICONTROL Analysis Workspace], [!UICONTROL Reports &amp; Analytics], [!UICONTROL Report Builder])를 포함하는 제품 프로필을 만들 수 있습니다.

1. [Admin Console](https://adminconsole.adobe.com/enterprise)에 로그인한 다음 **[!UICONTROL 제품]**(또는 제품 이름)을 클릭합니다.
1. 그런 다음 제품 프로필에서 **[!UICONTROL 권한]**(관리자만 사용 가능)을 클릭합니다.
1. 프로필의 권한 구성:

| 요소 | 설명 |
|--- |--- |
| 보고서 세트 | 특정 보고서 세트에 대한 권한을 사용하도록 설정합니다. |
| 지표 | 트래픽, 전환, 사용자 지정 이벤트, 솔루션 이벤트, 컨텐츠 인식 등에 대한 권한을 활성화합니다. |
| 차원 | eVar, 트래픽 보고서, 솔루션 보고서 및 경로 보고서를 포함하여 세분된 수준에서 사용자 액세스를 사용자 지정합니다. |
| 보고서 세트 도구 | 웹 서비스, 보고서 세트 관리, 도구 및 보고서, 대시보드 항목에 대한 사용자 권한을 활성화합니다. |
| Analytics 도구 | 일반 항목(청구, 로그 등), 회사 관리, 도구, 웹 서비스 액세스, Report Builder 및 Data Connectors 통합에 대한 사용자 권한을 활성화합니다. 관리 콘솔 사용자 지정 카테고리의 회사 설정이 Analytics 도구로 이동되었습니다. |

## 사용자에게 관리자 역할 위임 {#task_3A072C4AA9734BC59FFA7E015271BC7E}

Admin Console에서 조직의 다른 사용자에게 제한된 관리 권한을 위임할 수 있습니다. 위임된 역할을 통해 사용자는 최종 사용자에 대한 소프트웨어 액세스를 관리하고, 액세스 배포 기능을 제공하고, 지원 위임자 역할을 할 수 있습니다.

예를 들어 다음 작업을 수행할 수 있습니다.

* 제작 감독이 Creative Cloud에 대한 액세스 권한을 부여하도록 할 수 있습니다.
* 마케팅 관리자가 Experience Cloud에 대한 액세스 권한을 부여하도록 할 수 있습니다.
* 이러한 두 역할이 서로의 역할을 넘지 않도록 구분합니다.

이러한 역할을 사용하면 필요 이상으로 더 많은 기능을 제공하지 않고 다른 사람에게 관리를 동시에 위임할 수 있습니다.

1. Admin Console에서 **[!UICONTROL 사용자]**&#x200B;를 클릭한 다음 사용자 이름을 클릭합니다.
1. **[!UICONTROL 관리 권한 편집]**&#x200B;을 클릭합니다.
1.  사용자의 관리 권한을 구성합니다. 
1. **[!UICONTROL 다음]**&#x200B;을 클릭하여 설정을 검토한 다음 **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

## 지원되는 브라우저 및 시스템 요구 사항 {#concept_CDC4371EB9BF433E9534F8716DC8A088}

Experience Cloud에서 지원되는 브라우저입니다.

* [!DNL Microsoft Edge] (Microsoft에서는 Internet Explorer 8, 9 및 10에 대한 [지원을 종료](https://www.microsoft.com/en-us/WindowsForBusiness/End-of-IE-support)했습니다. 따라서 Adobe에서는 이러한 버전의 Internet Explorer에 대해 보고된 문제는 수정하지 않습니다.)
* [!DNL Google Chrome]
* [!DNL Firefox]
* [!DNL Safari]
* [!DNL Opera]

**참고:** Experience Cloud 인터페이스는 이러한 브라우저를 지원하지만 개별 솔루션은 모든 브라우저를 지원하지 않을 수 있습니다. (예를 들어 [Analytics](https://docs.adobe.com/content/help/ko-KR/analytics/admin/sys-reqs.html)는 [!DNL Opera]를 지원하지 않으며, [Adobe Target](https://docs.adobe.com/help/ko-KR/target/using/implement-target/before-implement/supported-browsers.html)은 [!DNL Safari]를 지원하지 않습니다.)

### 솔루션 및 제품 요구 사항

* [Analytics](https://docs.adobe.com/content/help/ko-KR/analytics/admin/sys-reqs.html)
* [Report Builder](https://docs.adobe.com/content/help/ko-KR/analytics/analyze/report-builder/report-builder-setup/system-requirements.html)
* [Adobe Target](https://docs.adobe.com/help/ko-KR/target/using/implement-target/before-implement/supported-browsers.html)
