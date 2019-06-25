---
description: Admin Console에 로그인 및 Experience Cloud 사용자 권한 및 제품 프로필 관리 방법에 대해 알아봅니다.
keywords: 핵심 서비스
seo-description: Admin Console에 로그인 및 Experience Cloud 사용자 권한 및 제품 프로필 관리 방법에 대해 알아봅니다.
seo-title: Experience Cloud 사용자 및 제품 관리
solution: Marketing Cloud
title: Experience Cloud 사용자 및 제품 관리
uuid: aea4e4c3-f543-4e8d-b553-d838418477d6
translation-type: ht
source-git-commit: 979b2202a70e2a5362aa86a65a17d7c4279b3a1a

---


# Experience Cloud 사용자 및 제품 관리 {#topic_3FCB4099640647E3B2411ADBFCE81909}

Admin Console에 로그인 및 Experience Cloud 사용자 권한 및 제품 프로필 관리 방법에 대해 알아봅니다.


<!-- marketing-cloud-identity-management.xml -->

<!-- user_mgmt_admin.xml -->

<!-- domain change for 2018 
<ul id="ul_6654B3993EBE4DE0A3FBCFA5173A52D1"> 
 <li id="li_BE41EB31960B4C079E864FAA2E322BB4"> Private Beta - Support new domain alongside old domain for selected customers (June, 2018) </li> 
 <li id="li_0513CA457FAA4F37A9D5E514DEAF2067"> General Rollout - Serve both old and new domains seamlessly for all customers (Aug, 2018) </li> 
 <li id="li_AB89A6D00A274EB7863D0243757322DE"> Public Beta - Drive solution teams and customers to switch references from old domain to new domain (Aug - Oct, 2018) </li> 
 <li id="li_6FED48B1F361493082102E823EA335F4"> General Availability - Redirect all old domain requests to new domain (Oct, 2018) </li> 
</ul> -->

>[!IMPORTANT]
>
>Admin Console에서 사용자 관리는 새 용어, 인터페이스 및 탐색을 소개합니다. 다음 정보는 이러한 변경 사항에 대해 설명하고 추가 도움말 자료에 대한 링크를 제공합니다. 이 도움말은 [Enterprise Administration 사용 안내서](https://helpx.adobe.com/kr/enterprise/managing/user-guide.html)에 있는 모든 Adobe 클라우드 제품에 대한 정보를 보완합니다.

## Experience Cloud 사용자 관리의 새로운 기능 {#concept_06A0A13362F644FB90F947238407637A}

Adobe Experience Cloud 사용자 관리의 최신 기능에 대해 알아보십시오.


## Admin Console에 로그인 {#section_705072FD4EBE4B70BC69EC81F2BB8669}

관리자는 더 이상 솔루션으로 사용자를 관리하지 않습니다. 이제 Experience Cloud에 대한 사용자 및 제품 관리가 Admin Console에서 발생합니다.

**Admin Console에 로그인하려면**

1. [https://adminconsole.adobe.com/enterprise/]()로 이동합니다.
1. [Adobe ID 또는 Enterprise ID](https://helpx.adobe.com/kr/enterprise/help/identity.html) 및 암호를 입력합니다.


또는 Experience Cloud 메뉴(![](assets/menu-icon.png))에서 **[!UICONTROL 관리]&gt;****Admin Console 시작[!UICONTROL 을 클릭합니다]**.

**관련 도움말**

Creative Cloud 및 Document Cloud의 경우 [관리 사용 안내서](https://helpx.adobe.com/kr/enterprise/using/users.html)를 참조하십시오. 일부 정보는 [ID 유형 관리](https://helpx.adobe.com/kr/enterprise/help/identity.html)와 같은 Experience Cloud 사용자 관리와 관련되어 있습니다.

암호, 조직 및 알림을 관리하려면 [로그인 및 프로필 설정 관리](../admin-getting-started/getting-started-experience-cloud.md#topic_AC564B6795334DE39359ADD87F52F2E0)합니다.

## 제품 프로필 및 그룹 {#section_AB50558124D541CF80A0D3D76D35A4BF}

제품 프로필을 추가하면 그룹을 사용하여 솔루션 제품 및 서비스를 관리하던 이전 방식에서 변경될 것임을 나타냅니다. Admin Console에서 권한은 사용자에게 지정할 수 있는 제품 및 서비스 그룹인 제품 프로필을 기반으로 합니다.

예를 들면 Analytics에서 보고서 세트, 지표, 차원 등과 함께 Analysis Workspace 및 Report Builder와 같은 보고 도구의 컬렉션을 구성할 수 있습니다. 프로필에 사용자를 추가하여 제품 프로필에 대한 권한을 부여할 수 있습니다. 자세한 내용은 [제품 프로필에 Analytics 액세스 권한 지정](../admin-getting-started/admin-getting-started.md#task_040673FE3E3E429B9531FBCB8B6A4391).

**관련 도움말**

[제한된 관리 권한 위임](../admin-getting-started/admin-getting-started.md#task_3A072C4AA9734BC59FFA7E015271BC7E)

## Analytics {#section_97DE101F92CD494AB073893680992F1A}

Admin Console에서 Analytics 사용자 및 제품 권한을 관리합니다.

[제품 프로필에 Analytics 액세스 권한을 지정](../admin-getting-started/admin-getting-started.md#task_040673FE3E3E429B9531FBCB8B6A4391)합니다(이 페이지에서).

**사용자 계정 마이그레이션**

Analytics 사용자 ID 마이그레이션 도구는 Analytics 관리자가 Analytics 사용자 관리에서 [Adobe Admin Console](https://adminconsole.adobe.com/enterprise/)로 사용자 계정을 마이그레이션하도록 지원하는 데 사용할 수 있습니다.

계정 마이그레이션이 단계적으로 고객에게 배포되고 있습니다. Adobe에서는 기존 사용자 계정을 **[!UICONTROL 관리 도구]** &gt; **[!UICONTROL 사용자 관리]** 에서 Admin Console로 마이그레이션할 때 사용자에게 알리고 지원합니다.

마이그레이션 후 사용자는 Adobe ID(또는 Enterprise ID)를 사용하여 로그인하고 [marketing.adobe.com](https://marketing.adobe.com)에서 해당 Experience Cloud 솔루션 및 서비스를 인증합니다. 사용자가 이전 계정([!DNL my.omniture.com] 및 [!DNL sc.omniture.com])을 통해 로그인하려고 하면 [!DNL marketing.adobe.com]으로 리디렉션됩니다.

**관련 도움말**

[Analytics 사용자 ID 마이그레이션](https://marketing.adobe.com/resources/help/ko_KR/experience-cloud/admin-console/analytics-migration/)

## Target - 제품 프로필과 작업 공간 {#section_3860AF177C9E4C7E9C390D36A414F353}

Target에서 작업 공간은 제품 프로필입니다. 이를 통해 조직에서는 특정 사용자 세트를 특정 속성 세트에 할당할 수 있습니다. 여러 가지 방식에서 작업 공간은 Adobe Analytics의 보고서 세트와 비슷합니다.

다음을 참조하십시오.
* [Enterprise 사용자 권한](https://marketing.adobe.com/resources/help/ko_KR/target/target/property_channel.html)
* [제품 및 프로필 관리](https://helpx.adobe.com/kr/enterprise/using/manage-products-and-profiles.html)
* 비디오: [Adobe Admin Console에서 Target 작업 공간 구성 방법](https://helpx.adobe.com/kr/target/kb/how-to-configure-target-workspaces-in-adobe-admin-console0.html)




## 캠페인 - 제품 프로필, 임차인 및 보안 그룹 {#section_09CDF75366444CF5810CF321B7C712F3}

캠페인의 *임차인*은 Admin Console 제품 페이지에서 *제품*으로 표시됩니다.

*보안 그룹*은 제품 프로필로 표시됩니다.

보안 그룹 및 보안 그룹에 대한 사용자 지정에 대한 정보는 [그룹 및 사용자 관리](https://helpx.adobe.com/kr/campaign/standard/administration/using/managing-groups-and-users.html)를 참조하십시오.

## Experience Platform Launch {#section_F2DA6778DD2D48AA8F794041971EE6B1}

Experience Platform Launch는 Admin Console에서 제품 페이지에 표시됩니다. Launch 제품 프로필에 다른 솔루션 및 핵심 서비스를 포함할 수 있습니다.

Admin Console의 사용자 권한 및 Launch 전용 옵션 설정(프로필에 권한 할당 포함)에 대한 자세한 내용은 [사용자 관리](https://marketing.adobe.com/resources/help/ko_KR/experience-cloud/launch/user-management.html)를 참조하십시오.

## Dynamic Tag Manager {#section_3A41CF2BD5994B9891537D063571D4ED}

사용자를 Dynamic Tag Management에 초대하고, 사용자 역할을 지정하고, 사용자를 그룹에 추가합니다.

Dynamic Tag Management에 사용자 초대, 사용자 역할 할당 및 그룹에 사용자 추가 방법에 대한 자세한 내용은 [사용자 및 권한](https://marketing.adobe.com/resources/help/ko_KR/dtm/users.html)을 참조하십시오.

## Audience Manager {#section_C31E3FA8A1E14463B1B3E07235F1983C}

Audience Manager 사용자를 만들고 그룹에 지정합니다. 제한(트레이트, 세그먼트, 대상 및 AlgoModel)을 볼 수도 있습니다.

Audience Manager 도움말에서 [관리](https://marketing.adobe.com/resources/help/ko_KR/aam/c_administration.html)를 참조하십시오.

## Experience Cloud 제품 관리 {#task_16335111C52D40E9BAC73D0699584DBF}

제품 프로필을 작성하여 권한 그룹에 지정합니다.

사용자를 조직에 초대할 때 사용자에게 제품 및 제품 프로필에 대한 액세스 권한을 제공할 수 있습니다. 제한된 관리 권한을 사용자에게 위임할 수도 있습니다. 마찬가지로 사용자 그룹을 작성한 후, 제품 프로필에 액세스할 수 있는 그룹을 추가할 수 있습니다.

1. [Admin Console](https://adminconsole.adobe.com/enterprise/)에서 **[!UICONTROL 제품]** 을 클릭합니다.
1. **[!UICONTROL 새 프로필]** 을 클릭합니다.
1. 프로필 세부 사항을 구성한 후 **[!UICONTROL 다음]** 을 클릭합니다.
1. **[!UICONTROL 완료를 클릭합니다]**.

다음에서 추가 도움말을 참조하십시오.

* [제품 및 프로필 관리](https://helpx.adobe.com/kr/enterprise/using/manage-products-and-profiles.html)
* 자세한 내용은 Target에서 [Enterprise 사용자 권한](https://marketing.adobe.com/resources/help/ko_KR/target/target/property_channel.html)을 참조하십시오.
* 비디오: [Adobe Admin Console에서 Target 작업 공간 구성 방법](https://helpx.adobe.com/kr/target/kb/how-to-configure-target-workspaces-in-adobe-admin-console0.html)


## 제품 프로필에 Analytics 액세스 권한 지정 {#task_040673FE3E3E429B9531FBCB8B6A4391}

제품 프로필에 Analytics 보고서 액세스 권한(보고서 세트, 지표, 차원 등)을 지정합니다.

예를 들면 특정 지표와 차원(eVars 등)에 대한 권한 및 세그먼트나 계산된 지표 생성과 같은 기능을 사용하여 여러 Analytics 도구([!UICONTROL Analysis Workspace], [!UICONTROL Reports &amp; Analytics], [!UICONTROL Report Builder])를 포함하는 제품 프로필을 만들 수 있습니다.

1. [Admin Console](https://adminconsole.adobe.com/enterprise)에 로그인한 다음 **[!UICONTROL 제품]**(또는 제품 이름)을 클릭합니다.
1. 그런 다음 제품 프로필에서 **[!UICONTROL 권한]**(관리자만 사용 가능)을 클릭합니다.
1. 프로필의 권한 구성:


| 요소 | 설명 |
|--- |--- |
| 보고서 세트 | 특정 보고서 세트에 대한 권한을 사용하도록 설정합니다. |
| 지표 | 트래픽, 전환, 사용자 지정 이벤트, 솔루션 이벤트, 내용 인식 등에 대한 권한을 활성화합니다. |
| 차원 | eVar, 트래픽 보고서, 솔루션 보고서 및 경로 지정 보고서를 포함하여 세분화된 수준에서 사용자 액세스를 사용자 지정합니다. |
| 보고서 세트 도구 | 웹 서비스, 보고서 세트 관리, 도구 및 보고서, 대시보드 항목에 대한 사용자 권한을 활성화합니다. |
| Analytics 도구 | 일반 항목(청구, 로그 등), 회사 관리, 도구, 웹 서비스 액세스, Report Builder 및 Data Connectors 통합에 대한 사용자 권한을 활성화합니다. 관리 콘솔 사용자 지정 카테고리의 회사 설정이 Analytics 도구로 이동되었습니다. |



## 사용자에게 관리자 역할 위임 {#task_3A072C4AA9734BC59FFA7E015271BC7E}


<!-- t_admin-roles.xml -->
Admin Console에서 조직의 다른 사용자에게 제한된 관리 권한을 위임할 수 있습니다. 위임된 역할을 통해 사용자는 최종 사용자에 대한 소프트웨어 액세스를 관리하고, 액세스 배포 기능을 제공하고, 지원 위임자 역할을 할 수 있습니다.

예를 들어 다음 작업을 수행할 수 있습니다.

* 제작 감독이 Creative Cloud에 대한 액세스 권한을 부여하도록 할 수 있습니다.
* 마케팅 관리자가 Experience Cloud에 대한 액세스 권한을 부여하도록 할 수 있습니다.
* 이러한 두 역할이 서로의 역할을 넘지 않도록 구분합니다.


이러한 역할을 사용하면 필요 이상으로 더 많은 기능을 제공하지 않고 다른 사람에게 관리를 동시에 위임할 수 있습니다.

1. Admin Console에서 **[!UICONTROL 사용자]** 를 클릭한 다음 사용자 이름을 클릭합니다.
1. **[!UICONTROL 관리 권한 편집]** 을 클릭합니다.
1.  사용자의 관리 권한을 구성합니다. 
1. **[!UICONTROL 다음]** 을 클릭하여 설정을 검토한 다음 **[!UICONTROL 저장]** 을 클릭합니다.

## 지원되는 브라우저 및 시스템 요구 사항 {#concept_CDC4371EB9BF433E9534F8716DC8A088}

Experience Cloud에서 지원되는 브라우저입니다.


<!-- browsers.xml -->
**Experience Cloud 핵심 서비스**

* Microsoft의 최신 Internet Explorer입니다. (Microsoft는 Internet Explorer 8, 9 및 10의 [지원을 종료](https://www.microsoft.com/ko-kr/WindowsForBusiness/End-of-IE-support)합니다. 따라서 Adobe에서는 이러한 버전의 Internet Explorer에 대해 보고된 문제는 수정하지 않습니다.)
* Google Chrome
* Mozilla Firefox
* Apple Safari


**솔루션 및 제품 요구 사항**

* [Analysis Workspace 및 Reports &amp; Analytics](https://marketing.adobe.com/resources/help/ko_KR/sc/user/?f=requirements)(Adobe Social 포함)
* [Report Builder](https://marketing.adobe.com/resources/help/ko_KR/arb/?f=system_requirements)
* [Ad Hoc Analysis](https://marketing.adobe.com/resources/help/ko_KR/dsc/index.html?f=c_sys_reqs)
* [Data Workbench](https://marketing.adobe.com/resources/help/ko_KR/insight/install/?f=c_Data_Workbench_Client_install)
* [Adobe Target](https://marketing.adobe.com/resources/help/ko_KR/target/ov/?f=r_supported_browsers)
* [Adobe Audience Manager](https://marketing.adobe.com/resources/help/ko_KR/aam/?f=c_supported_browsers)
* [Adobe Campaign Standard](https://helpx.adobe.com/kr/campaign/standard/start/using/compatible-browsers.html)
* [Adobe Campaign Classic](https://helpx.adobe.com/kr/campaign/kb/compatibility-matrix.html)
