---
description: Experience Cloud를 구현하고 관리자가 됩니다. 이 프로세스는 고객 속성 및 대상과 같은 핵심 서비스 기능에 대한 솔루션을 현대화합니다.
keywords: 핵심 서비스, 고객 속성
seo-description: Experience Cloud를 구현하고 관리자가 됩니다. 이 프로세스는 고객 속성 및 대상과 같은 핵심 서비스 기능에 대한 솔루션을 현대화합니다.
seo-title: 핵심 서비스용 Experience Cloud 솔루션을 사용하도록 설정
solution: Experience Cloud
title: 핵심 서비스용 솔루션을 사용하도록 설정
uuid: 5820060f-9b18-4339-81e0-401d964f7a03
translation-type: tm+mt
source-git-commit: c0ba39895218769e27ab99568387eb91310a574c

---


# 핵심 서비스용 솔루션을 사용하도록 설정

Experience Cloud를 구현하고 관리자가 됩니다. 이 프로세스는 고객 속성 및 대상과 같은 핵심 서비스 기능에 대한 솔루션을 현대화합니다.

<!-- <p>https://marketing-beta.adobe.com/resources/help/core/core-services.html </p> 
<p>https://adobe.sharepoint.com/sites/AGSConsulting/CoreServices/PA/_layouts/15/start.aspx#/ </p> -->

<!-- Core services architecture and data flow wiki: https://wiki.corp.adobe.com/pages/viewpage.action?pageId=1004285689 -->

## 1단계. Experience Cloud에 참여 및 관리자 되기 {#section_2423F0BD3DF642658103310EE5EA6154}

Experience Cloud에 참여하기 위해 수행할 작업:

![](assets/step1_icon.png) 적절한 Adobe Analytics 또는 Adobe Target SKU가 있는지 확인합니다.

* **Adobe Analytics:** Standard 또는 Premium(이전SiteCatalyst SKU 아님).
* **Adobe Target:** Standard 또는 Premium.

>[!NOTE]
>
>For Target, [migrate to at.js from mbox.js](https://marketing.adobe.com/resources/help/en_US/target/ov2/t_target-migrate-atjs.html).

![](assets/step2_icon.png) 구현을 현대화하고 관리자가 프로비저닝되도록 합니다.


1. [Experience Cloud ID 서비스 배포](../core-services/core-services.md#section_3C9F6DF37C654D939625BB4D485E4354)에서 아래 단계를 수행합니다.
1. 계정 관리자에게 문의하여 Experience Cloud에 대한 프로비저닝 프로세스를 시작합니다.

![](assets/step3_icon.png) Admin Console에서 사용자 및 제품 관리.

**관리자 액세스**

After you are an administrator, you can log in at [experiencecloud.adobe.com](https://experiencecloud.adobe.com).

Experience Cloud 메뉴 탐색에 **[!UICONTROL 관리]링크가 표시됩니다.**

도움이 필요한 경우 [Experience Cloud 사용자 및 제품 관리](../admin-getting-started/admin-getting-started.md#topic_3FCB4099640647E3B2411ADBFCE81909)를 참조하십시오.

**사용자 액세스**

Experience Cloud에 로그인하려면 사용자가 다음을 수행해야 합니다.


1. Adobe ID를 보유합니다.
1. Sign in at [experiencecloud.adobe.com](https://experiencecloud.adobe.com).
1. 엔터프라이즈 그룹에 매핑된 솔루션 그룹에 속합니다.
1. 필요한 경우 솔루션 계정을 Adobe ID에 연결합니다(아래에 설명).

![](assets/step4_icon.png) 선택 사항: 기존 사용자 계정을 연결합니다.

Analytics &gt; 관리 도구에서 관리한 Analytics 그룹처럼 이미 솔루션 그룹의 구성원인 사용자가 있을 수 있습니다.

이러한 그룹을 Experience Cloud 엔터프라이즈 그룹에 매핑하면 그러한 사용자가 해당 솔루션 계정 자격 증명을 해당 Adobe ID에 수동으로 링크해야 합니다.

[Experience Cloud에서 계정 링크](../admin-getting-started/organizations.md#topic_C31CB834F109465A82ED57FF0563B3F1)를 참조하십시오.

> [!NOTE]
> 
> 엔터프라이즈 및 솔루션 그룹이 매핑되면 새로운 사용자가 자동으로 연결됩니다. (솔루션 자격 증명은 자동으로 만들어지고 해당 Adobe ID에 연결됩니다.)

다음 섹션에서는 구현을 현대화하는 방법을 설명합니다. 구현을 현대화하면 Experience Cloud에서 핵심 서비스가 활성화됩니다.

## 2단계. Dynamic Tag Manager 또는 Experience Platform Launch를 사용하여 Experience Cloud ID 서비스 구현{#section_3C9F6DF37C654D939625BB4D485E4354}

Experience Cloud 핵심 서비스를 사용하는 가장 간단한 방법은 다이내믹 태그 관리자에서 [Experience Cloud ID 서비스 도구](https://docs.adobe.com/content/help/en/id-service/using/implementation-guides/standard.html)를 통해 Analytics 및 Target에 대해 자동으로 활성화하는 것입니다. (또는 Experience Platform Launch)

![](assets/menu-activation-shell.png)

For complete Experience Cloud ID service help (formerly, visitor ID), go [here](https://docs.adobe.com/content/help/en/id-service/using/home.html).

또한 차세대 태그 관리 제품은 ](https://docs.adobelaunch.com/getting-started)Launch, Adobe 제공[입니다.

**Dynamic Tag Management 또는 Launch를 사용하지 않습니까?**

Dynamic Tag Management를 사용하지 않는 경우 다음과 같이 JavaScript 배포([!DNL VisitorAPI.js])를 사용하여 ID 서비스를 수동으로 구현합니다.

1. [Analytics에 대한 Experience Cloud ID 서비스 구현](https://docs.adobe.com/content/help/en/id-service/using/implementation-guides/setup-analytics.html)에 설명된 단계를 수행합니다.

   추가 [고객 ID](https://docs.adobe.com/content/help/en/id-service/using/reference/authenticated-state.html)를 설정하는 것도 좋습니다. 이러한 ID는 각 방문자와 연결되며 Experience Cloud 핵심 서비스의 현재 및 향후 기능을 활성화합니다.

1. 기존 [!DNL s_code]를 버전 H.27.3 이상으로 업데이트하거나 기존 [!DNL AppMeasurement.js]를 버전 1.4 이상으로 업데이트합니다.

   이러한 파일은 Analytics 관리 도구의 [코드 관리자](https://docs.adobe.com/content/help/en/analytics/admin/admin-tools/code-manager-admin.html)에서 다운로드할 수 있습니다.

   ([에 대한 추가 정보가 필요한 경우 ](https://docs.adobe.com/content/help/en/analytics/implementation/javascript-implementation/javascript-implementation-overview.html)JavaScript 구현[!DNL AppMeasurement.js] 안내서를 이용할 수 있습니다.)

1. Analytics에 대한 고객 ID를 동기화합니다. [Analytics - 고객 ID 동기화](../core-services/core-services.md#section_AD473A6A21C1446498E700363F9A8437)(아래)를 참조하십시오.

## Analytics 및 Target - 고객 ID 동기화 {#section_AD473A6A21C1446498E700363F9A8437}

Experience Cloud ID 서비스 설정의 일부로, Analytics 및 Target에 대해 [고객 ID](https://docs.adobe.com/content/help/en/id-service/using/reference/authenticated-state.html)를 Experience Cloud와 동기화하는 것이 좋습니다.

Target에서 [!DNL mbox3rdpartyid]는 고객 ID를 가져와서 Target에 보내야 합니다. (Target에서 [고객 속성 작업](https://docs.adobe.com/content/help/en/target/using/audiences/visitor-profiles/working-with-customer-attributes.html)을 참조하십시오.)

방문자가 사용자의 웹 사이트에서 인증을 받거나 다른 방식으로 식별될 경우 페이지나 앱에 해당 개인의 CRM 고객 ID가 제공되어야 합니다. 그러면 해당 기능 호출을 사용하여 고객 ID를 Experience Cloud와 동기화할 수 있습니다. 이와 같이 동기화가 진행되면 방문자의 CRM 고객 ID가 Experience Cloud에 저장되고 Experience Cloud에서 사용할 해당 고객의 특성이 활성화됩니다.

예를 들어 CRM 시스템에서 Bob의 고객 ID가 `52mc210tr42`라고 가정해봅시다. Bob이 사용자 사이트에서 인증을 받으면, 사용자는 이 ID를 페이지에 제공하고 다음 두 가지 방법 중 하나로 해당 ID를 사용하여 동기화해야 합니다.

* 방문자 ID 서비스를 사용하여 `visitor.setCustomerIDs({"crm_id":"52mc210tr42"})`를 호출합니다. 또는,
* prop 또는 eVar에서  *`Customer ID (52mc210tr42)`* 를 입력합니다.


고객 ID는 고객 ID가 알려지는 모든 [!DNL Analytics] 서버 호출에서 설정되어야 합니다.

**Mobile SDK**

Android *및 iOS Mobile 애플리케이션에서 추가 고객 ID를 설정하는 방법에 대한 구문 예는 Experience Cloud ID 서비스*[](https://docs.adobe.com/content/help/en/mobile-services/android/overview.html) 섹션을 [참조하십시오](https://docs.adobe.com/content/help/en/mobile-services/ios/overview.html) .

**이전 데이터의 속성 활성화**

고객 속성 데이터는 방문자가 로그인한 후에 사용할 수 있습니다. 최신 Experience Cloud ID 서비스를 아직 구현하지 않았으며 이전에 prop 또는 eVar에서 고객 ID를 추적해온 경우 Experience Cloud에 내역 로그인을 전송하는 프로세스를 요청할 수 있습니다. 이 프로세스를 진행하면 고객 속성을 바로 사용할 수 있습니다.

이전 데이터를 활성화하려면 고객 지원 센터에 문의하십시오.

## 3단계. 보고서 세트를 Experience Cloud 조직에 매핑 {#section_7B08516B01BA421681DF03D0E86CE3BA}

Experience Cloud 서비스(예: Experience Cloud ID 서비스 및 사용자)는 개별 보고서 세트 대신 Experience Cloud 조직과 연결되어 있습니다. 이러한 서비스가 올바르게 작동하도록 하려면 각 Analytics 보고서 세트를 Experience Cloud 조직에 매핑해야 합니다.

[조직에 보고서 세트 매핑](report-suite-mapping.md)을 확인하십시오.

## 4단계. (Adobe Analytics) Analytics AppMeasurement 코드 현대화 {#section_1798D9D0F05C47E29816AC4EEB9A0913}

지역 데이터 수집(RDC)에서 작업 중인지 확인합니다. 데이터 수집 도메인이 [!DNL omtrdc.net]이거나 CNAME이 [!DNL omtrdc.net]으로 매핑된 경우 RDC를 사용해야 합니다. 자세한 내용은 [RDC로 전환](https://docs.adobe.com/content/help/en/analytics/technotes/rdc/regional-data-collection.html)을 참조하십시오. If you are using first-party cookies, refer to [CNAME and the Experience Cloud ID Service](https://docs.adobe.com/content/help/en/id-service/using/reference/analytics-reference/cname.html) for information about data collection CNAMEs and cross-domain tracking.

방문자 API를 비롯한 JavaScript 라이브러리를 업데이트하여 Analytics 구현을 현대화하는 것이 좋습니다. Dynamic Tag Management에서 [!DNL Adobe Analytics] 도구를 추가하고 구성 방법으로 *`Automatic`*&#x200B;을 지정하는 간편한 방법입니다.

Dynamic Tag Management에서 **[!UICONTROL <Web Property Name>]**&gt;**[!UICONTROL 개요]**&gt;**[!UICONTROL 도구 추가]**&gt;**[!UICONTROL Adobe Analytics]**를 클릭합니다. 배포 정보에 대해서는 다이내믹 태그 관리에서[Adobe Analytics 설정](https://docs.adobe.com/content/help/en/dtm/using/tools/analytics-dtm.html)을 참조하십시오.

## 5단계. (Adobe Target) Adobe Target 구현 현대화 {#section_C2F4493C7A36406DAE2266B429A4BD24}

* 다이내믹 태그 관리에 [Adobe Target 도구를](https://docs.adobe.com/content/help/en/dtm/using/tools/target.html) 추가합니다. 그러면 라이브러리 검색이 자동이 됩니다. Dynamic Tag Management에서 **[!UICONTROL <Web Property Name>]**&gt;**[!UICONTROL 개요]**&gt;**[!UICONTROL 도구 추가]**&gt;**[!UICONTROL Adobe Target]**를 클릭합니다.**&#x200B;참고:**Dynamic Tag Management를 사용하여 Target(및 기타 솔루션)에 대해 Experience Cloud ID 서비스를 배포할 수도 있습니다. Target에서 핵심 서비스를 사용하려면 Experience Cloud ID 서비스 업데이트가**&#x200B;필요합니다&#x200B;**.
* 다이내믹 태그 관리를 사용하지 않는 경우 수동으로 [mbox 라이브러리를 업데이트](https://docs.adobe.com/content/help/en/target/using/implement-target/client-side/mbox-implement/target-download-config-mbox.html)하십시오.
* 액세스를 요청하여 Adobe Target에 대한 보고 소스로 Adobe Analytics를 사용합니다. Target 및 Analytics 데이터가 처리 중에 동일한 서버 호출에 결합되므로 방문자가 두 솔루션 간에 연결됩니다. [Target 구현을 위해 Analytics 사용](https://docs.adobe.com/content/help/en/target/using/integrate/a4t/a4t.html)을 참조하십시오.
* 
   >[!IMPORTANT]
   >
   >모든 Analytics 고객에게 고객 속성과 같은 핵심 서비스가 공급됩니다. Analytics 사용자가 아닌 경우 고객 지원 센터에 문의하여 제공받을 수 있도록 요청하십시오.

## Step 6. 핵심 서비스 구현 확인 {#section_E641782A0F4F44AF8C9C91216BE330D5}

다음 프로세스에 따라 사이트에서 Experience Cloud ID 서비스가 올바르게 구현되도록 합니다.

1. Experience Cloud ID 서비스에 대한 요청을 볼 수 있게 사이트에 대한 쿠키를 지웁니다. 이 요청은 첫 번째 방문에서 수행된 후 매주 방문자마다 거의 한 번씩 수행됩니다.1. 패킷 분석기 또는 웹 브라우저 디버거의 네트워크 패널을 사용하여 [!DNL dpm.demdex.net]으로 진행되는 요청을 찾습니다.
1. 이 응답에는 `d_mid` 및 값이 포함됩니다(예: `_setMarketingCloudFields({"d_mid":"4235...`).
1. Analytics 요청에 mid 매개 변수(Marketing Cloud ID)가 포함되어 있는지 확인합니다. 유예 기간(활성화된 경우) 동안 aid 매개 변수(Analytics 방문자 ID)도 표시되어야 합니다.

Experience Cloud ID가 포함된 예상 응답은 다음과 같습니다.

![](assets/mac_id_response.png)

Experience Cloud ID(mid)가 포함된 Analytics 이미지 요청:

![](assets/mid.png)

mbox 요청의 Experience Cloud ID:

![](assets/mbox_request.png)

**유예 기간이란?**

방문자 ID 서비스를 배포한 후에 새 방문자는 더 이상 데이터 수집 서버에서 Analytics 방문자 ID를 받지 않습니다. 사이트의 섹션에 방문자 ID 서비스가 아직 구현되지 않은 경우 방문자가 이러한 섹션으로 이동하면 Experience Cloud ID는 인식되지 않으며 방문자에게 이전 Analytics 방문자 ID가 할당됩니다. 이로 인해 중복 방문 및 잘못된 특성을 포함한 잠재적 문제가 발생할 수 있습니다.

예를 들어 사이트의 지원 섹션에 별도의 CMS에서 관리되는 경우 이 섹션에 대해 다른 Analytics JavaScript 파일을 보유할 수 있습니다. 지원 사이트에 방문자 ID 서비스를 배포하기 전에 기본 사이트에 방문자 ID를 배포하는 경우 새 방문자가 지원 섹션을 방문할 때 이전 Analytics ID를 받게 되며 두 사이트 섹션에 걸쳐 진행되는 방문이 다른 방문으로 보고됩니다.

여러 JavaScript 파일 또는 기타 기술(예: Flash)을 사용하는 사이트에 방문자 ID 서비스를 배포하면 동시에 사이트의 모든 부분에서 해당 방문자 ID 서비스를 설정해야 하므로 조정 문제가 발생할 수 있습니다. 유예 기간을 구성하면 새 방문자가 방문자 ID 서비스에서 Analytics 방문자 ID를 계속 받게 되므로 방문자는 업그레이드되지 않은 사이트의 섹션에서 일관되게 식별되므로 방문자 ID 서비스를 사용할 수 있습니다.

## 7단계. 사용자 및 제품 관리 {#section_B6E95F4E0E12483CB9DA99CBC0C5A4AF}

Admin Console을 실행 중이면 사용자 및 제품 프로필을 관리할 수 있는 **[!UICONTROL 관리]** &gt; **[!UICONTROL Admin Console 시작]**&#x200B;으로 이동합니다.

![](assets/menu-administration-shell.png)

[Experience Cloud 사용자 및 제품 관리](../admin-getting-started/admin-getting-started.md#topic_3FCB4099640647E3B2411ADBFCE81909)를 참조하십시오.

**고객 속성**

<!-- <p> 
 <note type="important">
  To use the Customer Attributes feature, users must belong to the 
  <span class="term"> Adobe Customer Attributes</span> group, and to solution-level groups (Analytics or Target). 
 </note> </p> 
 -->

고객 속성 그룹에 추가된 사용자의 경우 Experience Cloud 인터페이스 왼쪽에 [!UICONTROL 고객 속성] 메뉴 항목이 표시됩니다

## 8단계. 핵심 서비스 사용 시작 {#section_960C06093623462E8EA247B3E97274A1}

다음 핵심 서비스 기능을 활용할 수 있습니다.

![](assets/menu-audiences-shell.png)

**사람 &gt; 고객 속성**

CRM(고객 관계 관리) 데이터베이스에서 엔터프라이즈 고객 데이터를 캡처하는 경우, 이 데이터를 Experience Cloud의 고객 속성 데이터 소스에 업로드할 수 있습니다. 업로드했으면 [!DNL Adobe Analytics] 및 [!DNL Adobe Target]의 데이터를 활용합니다.

[고객 속성](../attributes/attributes.md#concept_ACFEE7C8B8E94875BA0825CDF4913AF1)을 참조하십시오

**사람 &gt; 대상 라이브러리**

Experience Cloud 대상은 대상을 만들고, 기존 대상을 결합하여 복합 대상을 만들고, 모든 공유 대상을 볼 수 있는 인터페이스입니다.

[대상](../audience-library/audience-library.md#topic_679810123CAA4E0CA4FA3417FB0100C7)을 참조하십시오

<!-- aam_mc.xml -->

## 데이터 저장 및 개인 정보 공개 정보

Adobe [!DNL Experience Cloud] 내의 실시간 대상 프로파일링 및 기타 핵심 서비스를 활용하는 경우, 이러한 서비스의 사용이 데이터가 상주하는 데이터 센터(및 국가)에 영향을 줄 수 있습니다. 특히, Adobe [!DNL Experience Cloud]의 핵심 서비스는 Adobe Audience Manager를 활용하므로, 사용자 핵심 서비스 내에서 사용된 데이터는 미국의 Audience Manager 서버 내에 상주해야 합니다.

사용자 핵심 서비스를 통해 사용할 수 있는 핵심 서비스를 활용할 때 다른 Adobe 제품에서 대상 관리로 전송되는 데이터 유형은 다음과 같습니다.

* [!DNL Analytics] 키/값 쌍(props, eVars, list vars 등). 기본적으로 로그 줄에는 IP의 마지막 8진수를 포함하는 IP 주소가 포함됩니다(IP 주소가 Adobe [!DNL Analytics] 내의 IP 난독화 설정에 따라 수정되지 않았다고 가정).
* 방문자가 Audience Manager에서 설정된 규칙에 따라 자격을 평가하는 트레이트 및 세그먼트
* (선택 사항) 하나 이상의 ID. ID 서비스 구현에 따라, CRM ID 또는 해시된 이메일 주소와 같은 하나 이상의 ID를 전송할 수도 있습니다. 이 데이터가 Adobe [!DNL Analytics]로 전송되면 Adobe 고객 관리로 전달됩니다. 개인 데이터는 Adobe [!DNL Analytics]에 제공하지 않는 것이 좋습니다. 개인 데이터의 경우 Adobe로 전송하기 전에 단방향 해시를 사용해서 익명을 사용하는 것이 좋습니다.
* 백엔드 세그먼트 공유 기능을 통해 [!DNL Analytics]에서 시작된 세그먼트
* demdex.net 쿠키는 타사 쿠키가 차단되지 않은 경우에 설정됩니다. `AMCV_###@AdobeOrg` 자사 쿠키는 항상 Experience Cloud ID(이전의 방문자 ID 서비스)를 사용하여 설정됩니다.


이러한 모든 데이터 요소는 로그 파일 형식에서 Adobe Audience Manager로 전달됩니다. Audience Manager는 미국 내에서 이 데이터를 처리하고 저장합니다. Audience Manager는 미국 외부에서 이 데이터를 저장하고 처리하기 위한 옵션을 제공하지 않습니다.

**쿠키 및 옵트아웃**

실시간 대상 프로파일링을 사용할 때 [!DNL Analytics] 및 [!DNL Target]에 사용되는 쿠키 외에, Audience Manager 쿠키가 활용됩니다.

적절한 옵트아웃 기능을 제공하려는 경우 사이트 방문자가 기존 옵트아웃 프로세스에 Audience Manager 옵트아웃을 추가해야 합니다.

지침은 [Adobe Experience Cloud - Adobe 옵트아웃 구현](https://docs.adobe.com/content/help/en/analytics/implementation/javascript-implementation/data-collection/opt-out.html)을 참조하십시오.

도메인 간 추적을 사용하려면 [데이터 수집 CNAME 및 도메인 간 추적](https://docs.adobe.com/content/help/en/id-service/using/reference/analytics-reference/cname.html)을 참조하십시오.
