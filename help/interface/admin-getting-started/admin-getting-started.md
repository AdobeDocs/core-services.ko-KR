---
description: Admin Console 로그인, Experience Cloud 사용자 권한 및 제품 프로필 관리, 브라우저 지원에 대한 자세한 내용을 살펴보십시오.
keywords: core services
seo-description: Admin Console 로그인, Experience Cloud 사용자 권한 및 제품 프로필 관리, 브라우저 지원에 대한 자세한 내용을 살펴보십시오.
seo-title: Experience Cloud 사용자 및 제품 관리
solution: Experience Cloud
title: Experience Cloud 사용자 및 제품 관리
uuid: aea4e4c3-f543-4e8d-b553-d838418477d6
translation-type: tm+mt
source-git-commit: 14d6e0ae15b023ad4dd3f8aca0606f26b39a21e9

---


# Experience Cloud 사용자 및 제품 관리 {#topic_3FCB4099640647E3B2411ADBFCE81909}

Admin Console 로그인, Experience Cloud 사용자 권한 및 제품 프로필 관리, 브라우저 지원에 대한 자세한 내용을 살펴보십시오.

<!-- Beginning April 16, 2020, new organizations created in the Admin Console will block Adobe ID (type 1) identity types. Starting 16 Apr 2020 , newly created orgs will block the addition of Adobe ID/Type1 accounts.Migration for Orgs that have CCE/DX overlapping contracts will happen starting on  26 Apr 2020 (Gov't & Commercial Orgs) (~600 Orgs) Majority of EC customers will be migrated after July 2020. (~15k Orgs)https://wiki.corp.adobe.com/pages/viewpage.action?spaceKey=engage&title=Type2e+DX+GTM-->

>[!IMPORTANT]
>
>Admin Console에서 사용자 관리는 새 용어, 인터페이스 및 탐색을 소개합니다. 다음 정보는 이러한 변경 사항에 대해 설명하고 추가 도움말 자료에 대한 링크를 제공합니다. This help supplements the information in the [Enterprise Administration User Guide](https://helpx.adobe.com/enterprise/managing/user-guide.html) for all Adobe cloud products.

## Experience Cloud 사용자 관리의 새로운 기능 {#concept_06A0A13362F644FB90F947238407637A}

Adobe Experience Cloud 사용자 관리의 최신 기능에 대해 알아보십시오.

## Admin Console에 로그인 {#section_705072FD4EBE4B70BC69EC81F2BB8669}

관리자는 더 이상 솔루션의 사용자를 관리하지 않습니다. 이제 Experience Cloud에 대한 사용자 및 제품 관리가 관리 콘솔에서 수행됩니다.

**Admin Console에 로그인하려면**

1. Navigate to [https://adminconsole.adobe.com/enterprise/](https://adminconsole.adobe.com/enterprise/#).
1. Adobe ID [또는 Enterprise ID](https://helpx.adobe.com/enterprise/help/identity.html) 및 암호를 입력합니다.

Alternatively, from the Experience Cloud menu ( ![](assets/menu-icon.png)), click **[!UICONTROL Administration]** > **[!UICONTROL Launch Admin Console]**.

**관련 도움말**

[Creative Cloud](https://helpx.adobe.com/enterprise/using/users.html) 및 Document Cloud 관리 사용 안내서 일부 정보는 ID 유형 [관리와 같이 Experience Cloud 사용자 관리와 관련이 있습니다](https://helpx.adobe.com/enterprise/help/identity.html).

[로그인 및 프로필 설정을](../admin-getting-started/getting-started-experience-cloud.md#topic_AC564B6795334DE39359ADD87F52F2E0) 관리하여 암호, 조직 및 알림을 관리합니다.

## 제품 프로필 및 그룹 {#section_AB50558124D541CF80A0D3D76D35A4BF}

제품 프로필을 추가하면 이전에 그룹을 사용하여 솔루션 제품 및 서비스를 관리하던 방식이 달라졌습니다. 관리 콘솔에서 권한은 사용자에게 할당할 수 있는 제품 및 서비스 그룹인 제품 프로필을 기반으로 합니다.

예를 들어 Analytics에서는 보고서 세트, 지표, 차원 등과 함께 분석 작업 공간 및 리포트 빌더와 같은 보고 도구 모음을 구성할 수 있습니다. 프로필에 제품 프로필을 추가하여 사용자에게 제품 프로필에 대한 권한을 부여할 수 있습니다. See [Assign Analytics access permissions to a product profile](../admin-getting-started/admin-getting-started.md#task_040673FE3E3E429B9531FBCB8B6A4391).

**관련 도움말**

[제한된 관리 권한 위임](../admin-getting-started/admin-getting-started.md#task_3A072C4AA9734BC59FFA7E015271BC7E)

## Analytics {#section_97DE101F92CD494AB073893680992F1A}

Admin Console에서 Analytics 사용자 및 제품 권한을 관리합니다.

[제품 프로필에 Analytics 액세스 권한을 지정](../admin-getting-started/admin-getting-started.md#task_040673FE3E3E429B9531FBCB8B6A4391)합니다(이 페이지에서).

**사용자 계정 마이그레이션**

Analytics 사용자 ID 마이그레이션 도구는 Analytics 관리자가 Analytics 사용자 관리에서 [Adobe Admin Console](https://adminconsole.adobe.com/enterprise/)/로 사용자 계정을 마이그레이션하도록 지원하는 데 사용할 수 있습니다.

계정 마이그레이션이 단계적으로 고객에게 배포되고 있습니다. Adobe will notify and assist you when it is your time to migrate existing user accounts from **[!UICONTROL Admin Tools]** > **[!UICONTROL User Management]** to the Admin Console.

After the migration, users sign in using their Adobe ID (or Enterprise ID) and authenticate to their Experience Cloud solutions and services at [experiencecloud.adobe.com](https://experiencecloud.adobe.com). 사용자가 이전 계정([!DNL my.omniture.com] 및 [!DNL sc.omniture.com])을 통해 로그인하려고 하면 [!DNL experiencecloud.adobe.com]으로 리디렉션됩니다.

**관련 도움말**

[Analytics 사용자 ID 마이그레이션](https://docs.adobe.com/content/help/en/analytics/admin/user-product-management/user-management/migrate-users/c-migration-tool.html)

## Target - 제품 프로필과 작업 공간 {#section_3860AF177C9E4C7E9C390D36A414F353}

Target에서 작업 공간은 제품 프로필입니다. 이를 통해 조직은 특정 사용자 집합을 특정 속성 집합에 할당할 수 있습니다. 여러 가지 방식에서 작업 공간은 Adobe Analytics의 보고서 세트와 비슷합니다.

다음을 참조하십시오.
* [Enterprise 사용자 권한](https://docs.adobe.com/content/help/en/target/using/administer/manage-users/enterprise/property-channel.html)
* [제품 및 프로필 관리](https://helpx.adobe.com/enterprise/using/manage-products-and-profiles.html)
* 비디오:Adobe [Admin Console에서 타겟 작업 영역을 구성하는 방법](https://helpx.adobe.com/target/kb/how-to-configure-target-workspaces-in-adobe-admin-console0.html)

## 캠페인 - 제품 프로필, 임차인 및 보안 그룹 {#section_09CDF75366444CF5810CF321B7C712F3}

Campaign의 *테넌트가* 관리 콘솔 제품 페이지에 *제품으로* 표시됩니다.

*보안 그룹이* 제품 프로필로 표시됩니다.

보안 [그룹 및 보안 그룹에 사용자](https://helpx.adobe.com/campaign/standard/administration/using/managing-groups-and-users.html) 지정에 대한 자세한 내용은 그룹 및 사용자 관리를 참조하십시오.

## Experience Platform Launch {#section_F2DA6778DD2D48AA8F794041971EE6B1}

경험 플랫폼 시작은 관리 콘솔의 제품 페이지에 표시됩니다. Launch 제품 프로필에 다른 솔루션 및 서비스를 포함할 수 있습니다.

관리 [콘솔의](https://docs.adobelaunch.com/launch-reference/administration/user-permissions) 사용자 권한에 대한 자세한 내용은 사용자 관리를 참조하고, 프로필에 권한 할당을 비롯한 론치별 옵션을 설정합니다.

## Dynamic Tag Manager {#section_3A41CF2BD5994B9891537D063571D4ED}

사용자를 Dynamic Tag Management에 초대하고, 사용자 역할을 지정하고, 사용자를 그룹에 추가합니다.

See [Users and Permissions](https://docs.adobe.com/content/help/en/dtm/using/admin/users.html) for information about how to invite users to Dynamic Tag Management and assign user roles and add users to groups.

## Audience Manager {#section_C31E3FA8A1E14463B1B3E07235F1983C}

Audience Manager 사용자를 만들어 그룹에 할당합니다. 한도(트레이트, 세그먼트, 대상 및 AlgoModel)를 볼 수도 있습니다.

Audience [Manager](https://docs.adobe.com/content/help/en/dtm/using/admin/users.html) 도움말의 관리를 참조하십시오.

## Experience Cloud 제품 관리 {#task_16335111C52D40E9BAC73D0699584DBF}

제품 프로필을 만들어 권한 그룹에 지정합니다.

사용자를 조직에 초대하면 사용자에게 제품 및 제품 프로필에 대한 액세스 권한을 부여할 수 있습니다. 제한된 관리 권한을 사용자에게 위임할 수도 있습니다. 마찬가지로 사용자 그룹을 만든 다음 제품 프로필에 그룹을 추가하여 액세스를 활성화할 수 있습니다.

1. In the [Admin Console](https://adminconsole.adobe.com/enterprise/), click **[!UICONTROL Products]**.
1. **[!UICONTROL 새 프로필]**&#x200B;을 클릭합니다.
1. 프로필 세부 사항을 구성한 후 **[!UICONTROL 다음]**&#x200B;을 클릭합니다.
1. **[!UICONTROL 완료를 클릭합니다]**.

다음에서 추가 도움말을 참조하십시오.

* [제품 및 프로필 관리](https://helpx.adobe.com/enterprise/using/manage-products-and-profiles.html)
* [Target 도움말의](https://docs.adobe.com/content/help/en/target/using/administer/manage-users/enterprise/property-channel.html) Enterprise 사용자 권한을 참조하십시오.
* 비디오:Adobe [Admin Console에서 타겟 작업 영역을 구성하는 방법](https://helpx.adobe.com/target/kb/how-to-configure-target-workspaces-in-adobe-admin-console0.html)

## 제품 프로필에 Analytics 액세스 권한 지정 {#task_040673FE3E3E429B9531FBCB8B6A4391}

제품 프로필에 Analytics 보고서 액세스 권한(보고서 세트, 지표, 차원 등)을 지정합니다.

예를 들면 특정 지표와 차원(eVars 등)에 대한 권한 및 세그먼트나 계산된 지표 생성과 같은 기능을 사용하여 여러 Analytics 도구([!UICONTROL Analysis Workspace], [!UICONTROL Reports &amp; Analytics], [!UICONTROL Report Builder])를 포함하는 제품 프로필을 만들 수 있습니다.

1. Sign in to the [Admin Console](https://adminconsole.adobe.com/enterprise), then click **[!UICONTROL Products]** (or click your product name).
1. 그런 다음 제품 프로필에서 **[!UICONTROL 권한]**(관리자만 사용 가능)을 클릭합니다.
1. 프로필의 권한 구성:

| 요소 | 설명 |
|--- |--- |
| 보고서 세트 | 특정 보고서 세트에 대한 권한을 활성화합니다. |
| 지표 | 트래픽, 전환, 사용자 지정 이벤트, 솔루션 이벤트, 컨텐츠 인식 등에 대한 권한을 활성화합니다. |
| 차원 | eVar, 트래픽 보고서, 솔루션 보고서 및 경로 지정 보고서를 포함하여 세분된 수준에서 사용자 액세스를 사용자 지정합니다. |
| 보고서 세트 도구 | 웹 서비스, 보고서 세트 관리, 도구 및 보고서, 대시보드 항목에 대한 사용자 권한을 활성화합니다. |
| Analytics 도구 | 일반 항목(청구, 로그 등), 회사 관리, 도구, 웹 서비스 액세스, Report Builder 및 Data Connectors 통합에 대한 사용자 권한을 활성화합니다. 관리 콘솔 사용자 지정 카테고리의 회사 설정이 Analytics 도구로 이동되었습니다. |

## 사용자에게 관리자 역할 위임 {#task_3A072C4AA9734BC59FFA7E015271BC7E}

관리 콘솔에서 조직의 다른 사람에게 제한된 관리 권한을 위임할 수 있습니다. 위임된 역할을 통해 최종 사용자에 대한 소프트웨어 액세스를 관리하고 액세스 배포 기능을 제공하며 지원 위임자의 역할을 수행할 수 있습니다.

예를 들어 다음 작업을 수행할 수 있습니다.

* 크리에이티브 감독이 Creative Cloud에 대한 액세스 권한을 부여할 수 있습니다.
* 마케팅 이사가 Experience Cloud에 대한 액세스 권한을 부여할 수 있습니다.
* 이 두 역할을 별도로 유지하여 서로의 역할을 무시하지 않도록 합니다.

이러한 역할을 사용하면 필요 이상의 기능을 제공하지 않고도 다른 사람에게 관리를 동시에 위임할 수 있습니다.

1. Admin Console에서 **[!UICONTROL 사용자]**&#x200B;를 클릭한 다음 사용자 이름을 클릭합니다.
1. **[!UICONTROL 관리 권한 편집]**&#x200B;을 클릭합니다.
1.  사용자의 관리 권한을 구성합니다. 
1. **[!UICONTROL 다음]**&#x200B;을 클릭하여 설정을 검토한 다음 **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

## 지원되는 브라우저 및 시스템 요구 사항 {#concept_CDC4371EB9BF433E9534F8716DC8A088}

Experience Cloud에서 지원되는 브라우저입니다.

Experience Cloud 지원 브라우저에는 다음이 포함됩니다.

* [!DNL Microsoft Edge] (Microsoft는 Internet Explorer 8, 9 및 10에 대한 지원을 [](https://www.microsoft.com/en-us/WindowsForBusiness/End-of-IE-support) 종료했습니다. 따라서 Adobe는 이러한 특정 버전의 Internet Explorer에 대해 보고된 문제는 수정하지 않습니다.)
* [!DNL Google Chrome]
* [!DNL Firefox]
* [!DNL Safari]
* [!DNL Opera]

**참고:** Experience Cloud 인터페이스는 이러한 브라우저를 지원하지만 개별 솔루션은 모든 브라우저를 지원하지 않을 수 있습니다. (예: [Analytics](https://docs.adobe.com/content/help/en/analytics/admin/sys-reqs.html)는 [!DNL Opera]를 지원하지 않으며, [Target](https://docs.adobe.com/help/en/target/using/implement-target/before-implement/supported-browsers.html)은 [!DNL Safari]를 지원하지 않습니다.)

**솔루션 및 제품 요구 사항**

* [Analytics](https://docs.adobe.com/content/help/en/analytics/admin/sys-reqs.html)
* [Report Builder](https://docs.adobe.com/content/help/en/analytics/analyze/report-builder/report-builder-setup/system-requirements.html)
* [Adobe Target](https://docs.adobe.com/help/en/target/using/implement-target/before-implement/supported-browsers.html)
