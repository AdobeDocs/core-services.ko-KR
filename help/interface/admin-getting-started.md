---
title: 사용자 및 제품 관리
description: Admin Console에 로그인하고 Experience Cloud 사용자 권한 및 제품(제품 프로필)을 관리합니다. Experience Cloud 사용자에게 관리 권한을 위임하는 방법과 Experience Cloud에 대한 브라우저 지원에 대해 알아보십시오.
solution: Admin
index: true
feature: Admin Console
topic: Administration
role: Admin
level: Experienced
exl-id: af9eda5b-d984-44b7-a7b3-52dfc4e03d8f
source-git-commit: f229ec33ff721527e6a4c920ea63eabb4102935a
workflow-type: tm+mt
source-wordcount: '1582'
ht-degree: 74%

---

# 에서 사용자 및 제품 관리 [!DNL Experience Cloud]

Admin Console에 로그인, Experience Cloud 사용자 권한과 제품 프로필 관리 및 브라우저 지원 방법에 대해 알아봅니다.

>[!IMPORTANT]
>
>다음 정보는 특히 Experience Cloud 애플리케이션에 대한 것입니다. 이 정보는 모든 Adobe 클라우드 제품에 대한 [Enterprise 관리 사용 안내서](https://helpx.adobe.com/kr/enterprise/admin-guide.html)의 광범위한 관리 정보를 보완합니다.

관리 도구에서 모든 Experience Cloud 사용자 목록과 세부 사항을 정렬 및 필터링 가능한 목록으로 볼 수 있습니다. [관리 도구에서 Experience Cloud 사용자 보기](admin-tool-experience-cloud.md)를 참조하십시오.

## 프로비저닝 업데이트 알림{#provisioning}

업데이트 날짜: **2022년 7월 20일**

>[!IMPORTANT]
>
>Experience Cloud 프로비저닝에 대한 다음 알림을 검토하십시오.

Adobe는 모든 Experience Cloud 고객이 일부 Experience Cloud 제품 간의 상호 운용성을 지원하는 기본 기능을 이용할 수 있도록 프로비저닝을 업데이트하고 있습니다. 사용자는 자신의 Experience Cloud 조직에 새로운 자격으로 추가되고 [!UICONTROL 데이터 수집]이 포함 서비스로 제공되는 Adobe Experience Platform을 이용하게 됩니다.

Adobe Experience Platform [!UICONTROL Data Collection]에는 단순화된 범용 태그 관리를 위한 [태그](https://experienceleague.adobe.com/en/docs/tags)가 포함되어 있으며, 신뢰할 수 있고 강력하며 완벽한 스트리밍 데이터 인프라를 제공합니다. 태그는 고객 경험 데이터 수집을 단순화하고 경험 전달을 간소화합니다.

**의 변경 사항[!DNL Admin Console]**

관리자는에 대한 변경 사항이나 추가 사항을 볼 수 있습니다. [!DNL Admin Console] 다음과 같이:

* Admin Console의 Adobe Experience Platform 제품 카드에는 다음이 포함됩니다.

   * 장소
   * 보증
   * ID 네임스페이스
   * 샌드박스
   * 경험 데이터 모델
   * 스키마
   * 데이터스트림
   * 방문자 ID

  현재 Experience Platform을 사용하지 않는 조직의 경우 _Adobe Experience Platform_ 의 제품 [!DNL Admin Console]위에 나열된 기능을 포함합니다.

  현재 Experience Platform을 사용하는 조직의 경우, 이제 _장소_&#x200B;가 Experience Platform 카드로 통합됩니다.

* Adobe Experience Platform Data Collection(이전의 Launch) 및 개인정보 보호는 다른 Experience Platform 기능과 별도의 제품 카드로 계속 표시됩니다.

새로운 기능에 대한 자세한 내용은 Experience League의 해당 페이지를 참조하십시오.

* [데이터 수집](https://experienceleague.adobe.com/docs/discontinued/using/reports-and-analytics.html)
* [장소](https://experienceleague.adobe.com/en/docs/places/using/home)
* [보증](https://experienceleague.adobe.com/docs/platform-learn/implement-mobile-sdk/app-implementation/assurance.html?lang=ko-KR)
* [ID 네임스페이스](https://experienceleague.adobe.com/docs/experience-platform/identity/home.html?lang=ko-KR)
* [샌드박스](https://experienceleague.adobe.com/docs/experience-platform/sandbox/home.html?lang=ko-KR)
* [경험 데이터 모델](https://experienceleague.adobe.com/docs/experience-platform/xdm/home.html?lang=ko-KR)
* [스키마](https://experienceleague.adobe.com/docs/experience-platform/xdm/schema/composition.html?lang=ko-KR)
* [데이터스트림](https://experienceleague.adobe.com/docs/experience-platform/edge/datastreams/overview.html?lang=ko-KR)
* [방문자 ID](https://experienceleague.adobe.com/docs/core-services/interface/services/core-services.html?lang=ko-KR#section_3C9F6DF37C654D939625BB4D485E4354)
* [개인정보 보호](https://experienceleague.adobe.com/docs/experience-platform/privacy/home.html?lang=ko-KR)

## Experience Cloud 사용자 인증 (마이그레이션 예정){#migration}

2022년 2월부터 Adobe는 조직이 개별 프로필에 대한 비즈니스 권한을 보다 효율적으로 관리할 수 있도록 프로필 관리 시스템을 업데이트합니다. 따라서 개별 Adobe ID(Type1)에 해당하는 개인 프로필을 보유하고 있는 모든 사용자는 새 비즈니스 프로필로 마이그레이션됩니다. 이 프로필은 _Business ID_(Type2e)에 해당합니다.

다음을 참조하십시오 [Adobe의 ID 유형 [!DNL Admin Console]](https://helpx.adobe.com/kr/enterprise/using/identity.html) id 유형에 대한 자세한 내용

### 마이그레이션 프로세스

마이그레이션 시간이 되면 조직 관리자는 사용자의 마이그레이션 30일 전에 알림 이메일을 수신하게 됩니다.

* 마이그레이션은 조직의 주요 시간대 또는 주말을 기준으로 오후 10시에서 오전 6시 사이로 예약됩니다.
* 마이그레이션하는 동안 약 15분 동안 Experience Cloud 애플리케이션에 액세스할 수 없으며 [!DNL Admin Console] 최대 30분 동안 액세스할 수 없습니다. 그렇지 않으면 이 마이그레이션이 원활하게 이루어집니다.

### 마이그레이션 후 변경 사항

[!DNL Admin Console]

* 여러 계정을 보유한 관리자는에 로그인할 때 프로필 선택기가 표시됩니다 [!DNL Admin Console].
* 개별 Adobe ID 사용자가 Business ID로 업데이트됩니다.
* Business ID 디렉터리가에 추가됩니다. **[!UICONTROL 설정]** > **[!UICONTROL 신원]** > **[!UICONTROL 디렉터리]**.

  ![[!DNL Admin Console] ID - 비즈니스 ID](assets/identity-home.png)

### 마이그레이션 후 로그인

로그인 경험은 이 업데이트로 인해 변경되지 않습니다.

1. 동일한 자격 증명을 사용하여 `experience.adobe.com`에 로그인합니다.

1. Business ID와 연결된 새 프로필이 생성됩니다. **[!UICONTROL 지금 가입]** 또는 **[!UICONTROL 건너뛰기]**&#x200B;를 선택하라는 메시지가 표시됩니다.

1. 옵션 중 하나를 선택하면 기존의 랜딩 페이지 경험이 구축됩니다.

1. Adobe 프로필은 각 비즈니스 플랜과 연결되어 있으며 추가 Adobe 클라우드 서비스(Creative Cloud 및 Document Cloud)에서 생성된 에셋을 구성하는 기능을 제공합니다.

자세한 내용은 [Adobe 프로필 소개](https://helpx.adobe.com/kr/enterprise/kb/introducing-adobe-profiles.html)를 참조하십시오.

## 제품 프로필이란? {#section_AB50558124D541CF80A0D3D76D35A4BF}

_[!UICONTROL 제품 프로필]_ 는 사용자에게 할당할 수 있는 제품 및 서비스 그룹입니다. Experience Cloud에서 권한은 사용자가 아닌 제품 프로필을 기반으로 합니다. (그러나 특정 사용자에게 관리 권한을 위임할 수 있습니다.)

예를 들면 Analytics에서 보고서 세트, 지표 및 차원과 함께 Analysis Workspace 및 Report Builder와 같은 보고 도구의 컬렉션을 구성할 수 있습니다. 프로필에 사용자를 추가하여 제품 프로필에 대한 권한을 부여할 수 있습니다.

* 이 페이지에서 [제품 프로필에 Analytics 액세스 권한을 지정](admin-getting-started.md#task_040673FE3E3E429B9531FBCB8B6A4391) 을 참조하십시오.
* 이 페이지에서 [사용자에게 관리자 역할 위임](#delegate-rights) 을 참조하십시오.

## Manage Experience Cloud 제품 프로필 {#task_16335111C52D40E9BAC73D0699584DBF}

제품 프로필을 만들어 권한 그룹에 지정할 수 있습니다.

사용자를 조직에 초대할 때 사용자에게 제품 및 제품 프로필에 대한 액세스 권한을 제공할 수 있습니다. 제한된 관리 권한을 사용자에게 위임할 수도 있습니다. 마찬가지로 사용자 그룹을 작성한 후, 제품 프로필에 액세스할 수 있는 그룹을 추가할 수 있습니다.

1. 다음에서 [[!DNL Admin Console]](https://adminconsole.adobe.com/enterprise/), 선택 **[!UICONTROL 제품]**.
1. 조직 이름을 선택합니다.
1. **[!UICONTROL 새 프로필]**&#x200B;을 선택합니다.
1. 프로필 세부 사항을 구성한 다음 **[!UICONTROL 저장]**&#x200B;을 선택합니다.

자세한 내용 및 Creative Cloud와 Document Cloud 제품 관리에 대한 도움말은 [관리 사용 안내서](https://helpx.adobe.com/kr/enterprise/using/users.html)의 [ID](https://helpx.adobe.com/kr/enterprise/using/identity.html)를 참조하십시오.

**관련 도움말**

* [사용자 관리](https://helpx.adobe.com/kr/enterprise/using/users.html) 위치: [!DNL Admin Console]
* [제품 및 프로필 관리](https://helpx.adobe.com/kr/enterprise/using/manage-products.html) 위치: [!DNL Admin Console].
* 자세한 내용은 Target 도움말의 [Enterprise 사용자 권한](https://experienceleague.adobe.com/docs/target/using/administer/manage-users/enterprise/property-channel.html?lang=ko)을 참조하십시오.
* 비디오: [Adobe에서 Adobe Target 작업 공간을 구성하는 방법 [!DNL Admin Console]](https://experienceleague.adobe.com/docs/experience-cloud-kcs/kbarticles/KA-17521.html?lang=ko-KR)

## 사용자에게 관리자 역할 위임 {#delegate-rights}

위치 [!DNL Admin Console], 조직의 다른 사용자에게 제한된 관리 권한을 위임할 수 있습니다. 위임된 역할을 통해 사용자는 최종 사용자에 대한 소프트웨어 액세스를 관리하고, 액세스 배포 기능을 제공하고, 지원 위임자 역할을 할 수 있습니다.

예를 들어 다음 작업을 수행할 수 있습니다.

* 제작 감독이 Creative Cloud에 대한 액세스 권한을 부여하도록 할 수 있습니다.
* 마케팅 관리자가 Experience Cloud 액세스 권한을 부여하도록 허용합니다.
* 이러한 두 역할이 서로의 역할을 넘지 않도록 구분합니다.

이러한 역할을 사용하면 필요 이상으로 더 많은 기능을 제공하지 않고 다른 사람에게 관리를 동시에 위임할 수 있습니다.

1. 다음에서 [!DNL Admin Console], 선택 **[!UICONTROL 사용자]**&#x200B;을 클릭한 다음 사용자 이름을 선택합니다.

   ![의 관리 권한 [!DNL Admin Console]](assets/edit-admin-rights.png)

1. **[!UICONTROL 관리 권한 편집]**&#x200B;을 선택합니다.

   ![에서 관리 권한 편집 [!DNL Admin Console]](assets/edit-admin-rights-page.png)

1. 사용자의 관리 권한을 지정합니다.
1. **[!UICONTROL 저장]**&#x200B;을 선택합니다.

## Analytics 사용자 및 제품 관리 {#section_97DE101F92CD494AB073893680992F1A}

제품 프로필에 Analytics 보고서 액세스 권한(보고서 세트, 지표, 차원 등)을 지정할 수 있습니다.

예를 들면 여러 Analytics 도구([!UICONTROL Analysis Workspace], [!UICONTROL Reports &amp; Analytics] 및 [!UICONTROL Report Builder])가 포함된 제품 프로필을 만들 수 있습니다. 이러한 프로필에는 특정 지표 및 차원(eVar 포함)에 대한 권한과 세그먼트 또는 계산된 지표 생성과 같은 기능이 포함됩니다.

1. 에 로그인 [[!DNL Admin Console]](https://adminconsole.adobe.com/enterprise)을 선택한 다음 을 선택합니다. **[!UICONTROL 제품]**.
1. [!UICONTROL 제품] 페이지에서 해당 제품을 선택한 다음 **[!UICONTROL 권한]** (관리자만 사용 가능)을 선택합니다.
1. 프로필의 권한 구성:

| 요소 | 설명 |
|--- |--- |
| 보고서 세트 | 특정 보고서 세트에 대한 권한을 사용하도록 설정합니다. |
| 지표 | 트래픽, 전환, 사용자 정의 이벤트, 애플리케이션 이벤트, 콘텐츠 인식 등에 대한 권한을 활성화합니다. |
| 차원 | eVar, 트래픽 보고서, 애플리케이션 보고서 및 경로 보고서를 포함하여 세분된 수준에서 사용자 액세스를 사용자 정의합니다. |
| 보고서 세트 도구 | 웹 서비스, 보고서 세트 관리, 도구 및 보고서, 대시보드 항목에 대한 사용자 권한을 활성화합니다. |
| Analytics 도구 | 일반 항목(청구, 로그 등), 회사 관리, 도구, 웹 서비스 액세스, Report Builder 및 Data Connectors 통합에 대한 사용자 권한을 활성화합니다. 사용자 지정의 회사 설정 [!DNL Admin Console] 범주가 Analytics 도구로 이동되었습니다. |

**사용자 계정 마이그레이션**

Analytics 사용자 ID 마이그레이션 도구는 Analytics 관리자가 Analytics 사용자 관리에서 로 사용자 계정을 마이그레이션하도록 지원하는 데 사용할 수 있습니다. [Adobe [!DNL Admin Console]](https://adminconsole.adobe.com/enterprise/).

계정 마이그레이션이 단계적으로 고객에게 배포되고 있습니다. Adobe은 기존 사용자 계정을 마이그레이션할 때 사용자에게 알리고 지원합니다. **[!UICONTROL 관리 도구]** > **[!UICONTROL 사용자 관리]** (으)로 [!DNL Admin Console].

마이그레이션 후 사용자는 Adobe ID(또는 Enterprise ID)를 사용하여 로그인하고 [experience.adobe.com](https://experience.adobe.com)에서 해당 Experience Cloud 애플리케이션 및 서비스를 인증합니다. 사용자가 이전 계정([!DNL my.omniture.com], [!DNL sc.omniture.com] 및 [!DNL experiencecloud.adobe.com])을 통해 로그인하려고 하면 [!DNL experience.adobe.com]으로 리디렉션됩니다.

**관련 도움말**

* [의 분석 [!DNL Admin Console]](https://experienceleague.adobe.com/docs/analytics/admin/admin-console/home.html?lang=ko-KR)
* [Analytics 사용자 ID 마이그레이션](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/user-product-management/migrate-users/c-migration-tool.html?lang=ko)

## Adobe Target 관리 - 제품 프로필과 작업 공간 {#section_3860AF177C9E4C7E9C390D36A414F353}

Adobe Target에서 작업 공간은 제품 프로필입니다. 이를 통해 조직에서는 특정 사용자 세트를 특정 속성 세트에 할당할 수 있습니다. 여러 가지 방식에서 작업 영역은 Adobe Analytics의 보고서 세트와 비슷합니다.

다음을 참조하십시오.

* [Enterprise 사용자 권한](https://experienceleague.adobe.com/docs/target/using/administer/manage-users/enterprise/property-channel.html?lang=ko)
* [제품 및 프로필 관리](https://helpx.adobe.com/kr/enterprise/using/manage-products.html)
* 비디오: [Adobe에서 Adobe Target 작업 공간을 구성하는 방법 [!DNL Admin Console]](https://experienceleague.adobe.com/docs/experience-cloud-kcs/kbarticles/KA-17521.html?lang=ko-KR)

## 캠페인 제품 프로필, 테넌트 및 보안 그룹 관리 {#section_09CDF75366444CF5810CF321B7C712F3}

Campaign의 *테넌트*&#x200B;는 Admin Console 제품 페이지에서 *제품*&#x200B;으로 표시됩니다.

*보안 그룹*&#x200B;은 제품 프로필로 표시됩니다.

보안 그룹과 보안 그룹에 사용자를 지정하는 것에 대한 자세한 내용은 [그룹 및 사용자 관리](https://experienceleague.adobe.com/docs/campaign-standard/using/administrating/users-and-security/managing-groups-and-users.html?lang=ko-KR) 를 참조하십시오.

## Experience Platform 데이터 수집 관리 {#section_F2DA6778DD2D48AA8F794041971EE6B1}

Experience Platform [!UICONTROL 데이터 수집]은 [!UICONTROL Admin Console]의 [!UICONTROL 제품] 페이지에 표시됩니다. 데이터 수집 제품 프로필에 다른 애플리케이션과 서비스를 포함할 수 있습니다.

사용자를 [!UICONTROL Platform 데이터 수집]에 초대하고 사용자 역할과 권한을 할당하십시오.

다음을 참조하십시오 [사용자 권한](https://experienceleague.adobe.com/docs/experience-platform/tags/admin/user-permissions.html?lang=ko-KR) 의 사용자 권한에 대한 자세한 내용은 [!DNL Admin Console] 프로필에 대한 권한 설정에 대해 설명합니다.

## Experience Manager as a Cloud Service

Adobe 엔터프라이즈 고객은 Adobe에서 조직으로 표시됩니다 [!DNL Admin Console]. Experience Manager 고객은 Adobe을 사용할 수 있습니다 [!DNL Admin Console] as a Experience Manager에 대한 제품 자격 및 IMS 인증을 관리하려면 [!UICONTROL Cloud Service].

[Experience Manager as a Cloud Service를 위한 IMS 지원](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/security/ims-support.html?lang=ko)을 참조하십시오.

## Audience Manager {#section_C31E3FA8A1E14463B1B3E07235F1983C}

Audience Manager 사용자를 만들고 그룹에 지정합니다. 제한(트레이트, 세그먼트, 대상 및 [!DNL AlgoModel])을 볼 수도 있습니다.

Audience Manager 도움말의 [관리](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/administration/administration-overview.html?lang=ko-KR)를 참조하십시오.

## Experience Cloud에서 지원되는 브라우저

* [!DNL Microsoft® Edge] (Microsoft®는 Internet Explorer 8, 9 및 10에 대한 [지원을 종료](https://www.microsoft.com/ko-kr/WindowsForBusiness/End-of-IE-support)했습니다. 따라서 Adobe는 이러한 버전의 Internet Explorer에 대해 보고된 문제는 수정하지 않습니다.)
* [!DNL Google Chrome]
* [!DNL Firefox]
* [!DNL Safari]
* [!DNL Opera]

**참고:** Experience Cloud 인터페이스는 이러한 브라우저를 지원하지만 개별 애플리케이션이 모든 브라우저를 지원하는 것은 아닙니다. (예를 들어 [Analytics](https://experienceleague.adobe.com/docs/analytics/admin/admin-overview/sys-reqs.html?lang=ko)는 [!DNL Opera]를 지원하지 않으며, [!DNL Adobe Target]은 [!DNL Safari]를 지원하지 않습니다.)

### 솔루션 및 제품 요구 사항

* [Analytics](https://experienceleague.adobe.com/docs/analytics/admin/admin-overview/sys-reqs.html?lang=ko)
* [Report Builder](https://experienceleague.adobe.com/docs/analytics/analyze/report-builder/report-builder-setup/system-requirements.html?lang=ko)
