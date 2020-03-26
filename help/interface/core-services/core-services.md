---
description: Experience Cloud를 구현하고 관리자가 됩니다. 이 프로세스는 고객 속성 및 대상과 같은 핵심 서비스 기능에 대한 솔루션을 현대화합니다.
keywords: core services;customer attributes
seo-description: Experience Cloud를 구현하고 관리자가 됩니다. 이 프로세스는 고객 속성 및 대상과 같은 핵심 서비스 기능에 대한 솔루션을 현대화합니다.
seo-title: 핵심 서비스용 Experience Cloud 솔루션을 사용하도록 설정
solution: Experience Cloud
title: 핵심 서비스용 솔루션을 사용하도록 설정
uuid: 5820060f-9b18-4339-81e0-401d964f7a03
translation-type: tm+mt
source-git-commit: f7ec8bf6087a18be41c9efbf05f60e6cfd24e566

---


# 핵심 서비스용 솔루션을 사용하도록 설정

기존 고객의 경우 고객 속성 및 대상과 같은 기능을 사용할 수 있도록 솔루션 구현을 현대화하고 Experience Cloud를 구현하는 방법을 알아봅니다. 이를 위해 다음을 수행합니다.

1. [Experience Cloud에 참여 및 관리자 되기](#section_2423F0BD3DF642658103310EE5EA6154)
1. [Experience Cloud ID 서비스 구현](#section_3C9F6DF37C654D939625BB4D485E4354)
1. [보고서 세트를 Experience Cloud 조직에 매핑](#section_7B08516B01BA421681DF03D0E86CE3BA)
1. [Analytics AppMeasurement 코드 업데이트](#section_1798D9D0F05C47E29816AC4EEB9A0913)
1. [Adobe Target 구현 업데이트](#section_C2F4493C7A36406DAE2266B429A4BD24)
1. [핵심 서비스 구현 확인](#section_E641782A0F4F44AF8C9C91216BE330D5)
1. [사용자 및 제품 관리](#section_B6E95F4E0E12483CB9DA99CBC0C5A4AF)
1. [핵심 서비스 사용 시작](#section_960C06093623462E8EA247B3E97274A1)

## 1단계. Experience Cloud에 참여 및 관리자 되기 {#section_2423F0BD3DF642658103310EE5EA6154}

Experience Cloud에 참여하기 위해 수행할 작업:

![](assets/step1_icon.png) 적절한 Adobe Analytics 또는 Adobe Target SKU가 있는지 확인합니다.

* **Adobe Analytics:** Standard 또는 Premium(이전 SKU가 [!DNL SiteCatalyst] 아님).
* **Adobe Target:** Standard 또는 Premium.

>[!NOTE]
>
>의 [!DNL Target]경우 에서 at.js로 마이그레이션합니다 [!DNL mbox.js]. See [Upgrading from at.js 1. x to at.js 2. x](https://docs.adobe.com/content/help/en/target/using/implement-target/client-side/upgrading-from-atjs-1x-to-atjs-20.html).

![](assets/step2_icon.png) 구현을 현대화하고 관리자가 프로비저닝되도록 합니다.

1. Experience Cloud ID 서비스 [배포의 아래 [!UICONTROL 단계를 따르십시오]](../core-services/core-services.md#section_3C9F6DF37C654D939625BB4D485E4354).
1. 계정 관리자에게 문의하여 Experience Cloud의 프로비저닝 프로세스를 시작합니다.

![](assets/step3_icon.png)[!UICONTROL  Admin Console에서 사용자 및 제품 관리].

### 관리자 로그인

After you are an administrator, you can log in at [experiencecloud.adobe.com](https://experiencecloud.adobe.com).

Experience Cloud 메뉴 탐색에 **[!UICONTROL 관리]** 링크가 표시됩니다.

도움이 필요한 경우 [Experience Cloud 사용자 및 제품 관리](../admin-getting-started/admin-getting-started.md#topic_3FCB4099640647E3B2411ADBFCE81909)를 참조하십시오.

### 사용자 로그인

Experience Cloud에 로그인하려면 사용자가 다음을 수행해야 합니다.

1. Adobe ID(또는 회사의 Enterprise ID)가 있어야 합니다.
1. Sign in at [experiencecloud.adobe.com](https://experiencecloud.adobe.com).
1. 기업 그룹에 매핑된 솔루션 그룹에 속합니다.
1. 필요한 경우 솔루션 계정을 해당 Adobe ID에 연결합니다(아래 설명).

![](assets/step4_icon.png) 선택 사항: 기존 사용자 계정을 연결합니다.

대부분의 경우 이전에 Analytics > 관리 도구에서 관리했던 Analytics 그룹과 같은 솔루션 그룹의 [!UICONTROL 구성원인] 사용자가 [!UICONTROL 있습니다].

이러한 그룹을 Experience Cloud 엔터프라이즈 그룹에 매핑하면 해당 사용자는 솔루션 계정 자격 증명을 Adobe ID에 수동으로 연결해야 합니다.

Experience [Cloud에서 계정 연결 참조](../admin-getting-started/organizations.md#topic_C31CB834F109465A82ED57FF0563B3F1)

>[!NOTE]
>
>엔터프라이즈 및 솔루션 그룹이 매핑되면 새로운 사용자가 자동으로 연결됩니다. (솔루션 자격 증명은 자동으로 생성되어 Adobe ID에 연결됩니다.)

다음 섹션에서는 구현을 현대화하는 방법에 대해 설명합니다. 구현을 현대화하면 Experience Cloud의 핵심 서비스가 활성화됩니다.

## 2단계. Experience [!UICONTROL Platform Launch] 또는 [!UICONTROL 다이내믹 태그 관리를 사용하여 Experience Cloud]ID [!UICONTROL 서비스] 구현 {#section_3C9F6DF37C654D939625BB4D485E4354}

Experience [!UICONTROL Cloud ID 서비스는] 솔루션 간 통합에 대한 공통 ID를 제공합니다. 고객 속성을 통해 업로드된 CRM 데이터를 기반으로 크로스 도메인 방문자 식별과 크로스 디바이스/브라우저 타깃팅 및 개인화 경로를 [!UICONTROL 제공합니다].

Experience Cloud 핵심 서비스를 활성화하는 가장 간단한 방법은 Experience Platform Launch의 Experience Cloud ID 서비스 확장 [](https://docs.adobe.com/content/help/en/launch/using/implement/solutions/idservice-save.html) 기능을 [!UICONTROL 통해 또는 다이내믹 태그 관리의 ECID]도구를 통해 Analytics 및 Adobe Target에 대해 자동으로 활성화하는 [!UICONTROL 것입니다]. (Experience Platform Launch가 적극 권장됩니다.)

![](assets/menu-activation-shell.png)

전체 Experience Cloud ID 서비스 도움말(이전 방문자 ID)을 보려면 [여기로](https://docs.adobe.com/content/help/en/id-service/using/home.html)이동하십시오.

**Experience Platform[!UICONTROL Launch]또는 다이내믹 태그[!UICONTROL 관리를 사용하지 않습니까]?**

If you are not using [!UICONTROL Experience Platform Launch] or [!UICONTROL Dynamic Tag Management], manually implement the ID service via the JavaScript Deployment ([!DNL VisitorAPI.js]), as follows:

| 작업 | 설명 |
| -----------| ---------- |  
| [Analytics용 Experience Cloud ID 서비스 구현](https://docs.adobe.com/content/help/en/id-service/using/implementation/setup-analytics.html) | 추가 [고객 ID를 설정하는 것도 좋습니다](https://docs.adobe.com/content/help/en/id-service/using/reference/authenticated-state.html). 이러한 ID는 각 방문자와 연결되며 Experience Cloud에서 현재 및 향후 기능을 활성화합니다. |
| 기존 [!DNL s_code]를 버전 H.27.3 이상으로 업데이트하거나 기존 [!DNL AppMeasurement.js]를 버전 1.4 이상으로 업데이트합니다. | 이러한 파일은 Analytics 관리 도구의 코드 [관리자에서](https://docs.adobe.com/content/help/en/analytics/admin/admin-tools/code-manager-admin.html) 다운로드할 수 있습니다.  ( [자세한](https://docs.adobe.com/content/help/en/analytics/implementation/javascript-implementation/javascript-implementation-overview.html) 정보가 필요한 경우 JavaScript 구현 안내서를 사용할 수 [!DNL AppMeasurement.js]있습니다.) |
| Analytics에 대한 고객 ID 동기화 | See [Analytics - synching the customer ID](../core-services/core-services.md#section_AD473A6A21C1446498E700363F9A8437) (below). |

## Analytics &amp; Adobe Target - synching the customer ID {#section_AD473A6A21C1446498E700363F9A8437}

Experience Cloud ID 서비스 설정의 일부로, Adobe는 Analytics에 대해 [!DNL Target] 권장하며 [고객 ID를 Experience Cloud와](https://docs.adobe.com/content/help/en/id-service/using/reference/authenticated-state.html) 동기화할 것을 권장합니다.

In Adobe Target, the `mbox3rdpartyid` needs to get the customer ID and send it to [!DNL Target]. (고객 [속성](https://docs.adobe.com/content/help/en/target/using/audiences/visitor-profiles/working-with-customer-attributes.html) 작업을 참조하십시오 [!DNL Target].)

방문자가 웹 사이트에서 인증을 받거나 다른 방법으로 식별되면 구현에서 해당 개인의 CRM 고객 ID를 페이지나 앱에 노출해야 합니다. 그런 다음 적절한 함수 호출을 사용하여 고객 ID를 Experience Cloud와 동기화할 수 있습니다. 이 동기화는 방문자의 CRM 고객 ID를 Experience Cloud에 저장하고 해당 고객의 속성을 Experience Cloud에서 사용할 수 있도록 활성화합니다.

예를 들어 CRM 시스템에서 Bob의 고객 ID가 `52mc210tr42`라고 가정해봅시다. Bob이 사용자 사이트에서 인증을 받으면, 사용자는 이 ID를 페이지에 제공하고 다음 두 가지 방법 중 하나로 해당 ID를 사용하여 동기화해야 합니다.

* 방문자 ID 서비스를 사용하여 `visitor.setCustomerIDs({"crm_id":"52mc210tr42"})`를 호출합니다. 또는,
* prop 또는 eVar *`Customer ID (52mc210tr42)`* 에서 을 채웁니다.

고객 ID는 고객 ID가 알려지는 모든 [!DNL Analytics] 서버 호출에서 설정되어야 합니다.

### Mobile SDK

Android *및 iOS Mobile* 애플리케이션에서 추가 고객 ID를 설정하는 방법에 대한 구문 예는 [Experience Cloud](https://docs.adobe.com/content/help/en/mobile-services/android/overview.html) ID [서비스](https://docs.adobe.com/content/help/en/mobile-services/ios/overview.html) 섹션을참조하십시오.

### 이전 데이터의 속성 활성화

고객 속성 데이터는 방문자가 로그인한 후에 사용할 수 있습니다. 최신 Experience Cloud ID 서비스를 아직 구현하지 않았으며, 이전에 prop 또는 eVar에서 고객 ID를 추적한 적이 있는 경우, Experience Cloud에 내역 로그인을 보내는 프로세스를 요청할 수 있습니다. 이 프로세스를 통해 고객 속성을 즉시 사용할 수 있습니다.

내역 데이터를 활성화하려면 고객 지원 센터에 문의하십시오.

## 3단계. Map report suites to an Experience Cloud Organization {#section_7B08516B01BA421681DF03D0E86CE3BA}

Experience Cloud 서비스(예: Experience Cloud ID [!UICONTROL 서비스]및 사람 서비스)는 개별 Analytics 보고서 세트 대신 Experience Cloud 조직과 연결됩니다. 이러한 서비스가 올바르게 작동하도록 하려면 각 Analytics 보고서 세트를 Experience Cloud 조직에 매핑해야 합니다.

[조직에 보고서 세트 매핑](report-suite-mapping.md)을 확인하십시오.

## 4단계. (Adobe Analytics) Update your Analytics AppMeasurement code {#section_1798D9D0F05C47E29816AC4EEB9A0913}

지역 데이터 수집(RDC)에서 작업 중인지 확인합니다. 데이터 수집 도메인이 [!DNL omtrdc.net]이거나 CNAME이 [!DNL omtrdc.net]으로 매핑된 경우 RDC를 사용해야 합니다. 자세한 [내용은 RDC로](https://docs.adobe.com/content/help/en/analytics/technotes/rdc/regional-data-collection.html) 전환을 참조하십시오. 퍼스트 파티 쿠키를 사용하는 경우, 데이터 수집 CNAME [및 도메인 간 추적에](https://docs.adobe.com/content/help/en/id-service/using/reference/analytics-reference/cname.html) 대한 자세한 내용은 CNAME 및 Experience Cloud ID 서비스를 참조하십시오.

방문자 API를 비롯한 JavaScript 라이브러리를 업데이트하여 Analytics 구현을 현대화하는 것이 좋습니다. Dynamic Tag Management에서 [!DNL Adobe Analytics] 도구를 추가하고 구성 방법으로 *`Automatic`*&#x200B;을 지정하는 간편한 방법입니다.

In [!UICONTROL Dynamic Tag Management], click **[!UICONTROL <Web Property Name>]**>**[!UICONTROL &#x200B;개요&#x200B;]**>**[!UICONTROL &#x200B;도구&#x200B;]**추가 >**[!UICONTROL  Adobe ]**Analytics. 배포[정보는 다이내믹](https://docs.adobe.com/content/help/en/dtm/using/tools/analytics-dtm.html)태그 관리의 Adobe Analytics 설정을 참조하십시오.

## 5단계. (Adobe Target) Update your Adobe Target implementation {#section_C2F4493C7A36406DAE2266B429A4BD24}

* Adobe Experience Platform Launch에서 Adobe [Target 확장](https://docs.adobe.com/content/help/en/launch/using/extensions-ref/adobe-extension/targetv2-extension/adobe-target-extension-v2.html) 기능을 추가하면 라이브러리 검색이 자동으로 수행됩니다. 또한 Experience Platform Launch를 사용하여 [Adobe Target(및 기타 솔루션)용 Experience Cloud ID 서비스 확장을](https://docs.adobe.com/content/help/en/launch/using/extensions-ref/adobe-extension/id-service-extension/overview.html) 설정할 [!UICONTROL 수 있습니다]. Adobe [!UICONTROL Target에서] 핵심 서비스를 사용하려면 Experience Cloud ID 서비스 **업데이트가** 필요합니다. 다이내믹 태그 관리를 사용하는 [!UICONTROL 경우]Adobe Target [도구를](https://docs.adobe.com/content/help/en/dtm/using/tools/target.html)추가합니다. 다이내믹 태그 관리를 사용하여 [!UICONTROL Adobe] Target용 Experience Cloud ID 서비스를 배포할 수도 있습니다.)
* Experience Platform Launch 또는 [!UICONTROL 다이내믹 태그 관리를] 사용하지 않는 [!UICONTROL 경우]mbox 라이브러리를 [수동으로](https://docs.adobe.com/content/help/en/target/using/implement-target/client-side/mbox-implement/target-download-config-mbox.html) 업데이트하십시오.
* Request access to use Adobe Analytics as the reporting source for [!DNL Adobe Target]. [!DNL Target] 및 데이터가 처리 중에 동일한 서버 호출에 결합되므로 방문자가 두 솔루션 간에 연결됩니다. [!DNL Analytics] See [Analytics for Target Implementation](https://docs.adobe.com/content/help/en/target/using/integrate/a4t/a4t.html).

   >[!IMPORTANT]
   >
   >모든 Analytics 고객은 이미 고객 속성과 같은 핵심 서비스에 대해 프로비저닝되었습니다. Analytics 사용자가 아닌 경우 고객 지원 센터에 문의하여 제공받을 수 있도록 요청하십시오.

## Step 6. 핵심 서비스 구현 확인 {#section_E641782A0F4F44AF8C9C91216BE330D5}

다음 프로세스를 사용하여 Experience Cloud ID 서비스가 사이트에서 올바르게 구현되었는지 확인하십시오.

1. Experience Cloud ID Service에 대한 요청을 볼 수 있도록 사이트에 대한 쿠키를 지웁니다. 요청은 첫 번째 방문에서 수행된 후 매주 방문자당 약 1번씩 수행됩니다.
1. Using a packet analyzer or the network panel in a web browser debugger, look for a request going to [!DNL dpm.demdex.net].
1. 이 응답에는 `d_mid` 및 값이 포함됩니다(예: `_setMarketingCloudFields({"d_mid":"4235...`).
1. Analytics 요청에 `mid` 매개 변수(Experience Cloud ID)가 포함되어 있는지 확인합니다. 유예 기간 동안(활성화된 경우) 매개 변수(Analytics 방문자 ID)도 `aid` 표시됩니다.

Experience Cloud ID가 포함된 예상 응답:

![](assets/mac_id_response.png)

Experience Cloud ID를 포함하는 Analytics 이미지 요청( `mid` 또는 _방문자 ID라고도 함_):

![](assets/mid.png)

mbox 요청의 Experience Cloud ID:

![](assets/mbox_request.png)

### 유예 기간이란 무엇입니까?

Experience Cloud ID 서비스를 배포한 후 새 방문자가 더 이상 데이터 수집 서버에서 Analytics Experience Cloud ID를 받지 않습니다. 사이트의 섹션이 아직 Experience Cloud ID 서비스를 구현하지 않은 경우 방문자가 이러한 섹션으로 이동하면 Experience Cloud ID가 인식되지 않으며 방문자에게 이전 Analytics 방문자 ID가 할당됩니다. 이로 인해 중복 방문 및 잘못된 기여도 분석과 같은 잠재적인 문제가 발생할 수 있습니다.

예를 들어 사이트의 지원 섹션이 별도의 CMS에서 관리되는 경우 이 섹션에 대해 다른 Analytics JavaScript 파일이 있을 수 있습니다. ID 서비스를 지원 사이트에 배포하기 전에 기본 사이트에 Experience Cloud ID를 배포하는 경우 새 방문자가 지원 섹션을 방문할 때 이전 Analytics ID를 받고 두 사이트 섹션을 모두 포함하는 방문이 서로 다른 방문으로 보고됩니다.

여러 JavaScript 파일 또는 기타 기술(예: Flash)을 사용하는 사이트에 Experience Cloud ID 서비스를 배포하면 사이트의 모든 부분에서 동시에 Experience Cloud ID 서비스를 활성화해야 하므로 조정 문제가 발생할 수 있습니다. 유예 기간을 구성하면 새 방문자가 ID 서비스에서 Analytics 방문자 ID를 계속 받게 되므로 방문자는 업그레이드되지 않은 사이트 섹션에서 일관되게 식별되어 방문자 ID 서비스를 사용할 수 있습니다.

## 7단계. 사용자 및 제품 관리 {#section_B6E95F4E0E12483CB9DA99CBC0C5A4AF}

Once you are up and running, navigate to the [Admin Console](https://adminconsole.adobe.com/), where you can manage users and product profiles.

![](assets/menu-administration-shell.png)

[Experience Cloud 사용자 및 제품 관리](../admin-getting-started/admin-getting-started.md#topic_3FCB4099640647E3B2411ADBFCE81909)를 참조하십시오.

### 사용자 특성

<!-- <p> 
 <note type="important">
  To use the Customer Attributes feature, users must belong to the 
  <span class="term"> Adobe Customer Attributes</span> group, and to solution-level groups (Analytics or Adobe Target). 
 </note> </p> 
 -->

Users that are added to the [!UICONTROL Customer Attributes] group will see the [!UICONTROL Customer Attributes] menu item on the left side of the Experience Cloud interface.

## 8단계. Begin using core services {#section_960C06093623462E8EA247B3E97274A1}

다음 핵심 서비스 기능을 활용할 수 있습니다.

![](assets/menu-audiences-shell.png)

### [!UICONTROL 사람] > [!UICONTRO전체 고객 속성]

CRM(고객 관계 관리) 데이터베이스에서 엔터프라이즈 고객 데이터를 캡처하는 경우, 이 데이터를 Experience Cloud의 고객 속성 데이터 소스에 업로드할 수 있습니다. 업로드했으면 [!DNL Adobe Analytics] 및 [!DNL Adobe Target]의 데이터를 활용합니다.

[고객 속성](../attributes/attributes.md#concept_ACFEE7C8B8E94875BA0825CDF4913AF1)을 참조하십시오

### [!UICONTROL 사람] > [!UICONTROL 대상 라이브러리]

Experience Cloud [!UICONTROL Audiences] is the interface that lets you create audiences, combine existing audiences to create composite audiences, and view all shared audiences.

[대상](../audience-library/audience-library.md#topic_679810123CAA4E0CA4FA3417FB0100C7)을 참조하십시오

## 데이터 저장 및 개인 정보 공개

Adobe [!DNL Experience Cloud] 내의 실시간 대상 프로파일링 및 기타 핵심 서비스를 활용하는 경우, 이러한 서비스의 사용이 데이터가 상주하는 데이터 센터(및 국가)에 영향을 줄 수 있습니다. Specifically, because the core services of the Adobe [!DNL Experience Cloud] leverage Adobe Audience Manager, data used within the [!UICONTROL People] service must reside within Audience Manager servers in the United States.

When leveraging core services made available via the [!UICONTROL People] service, the types of data sent from other Adobe products to audience management are:

* [!DNL Analytics] 키/값 쌍(props, eVars, list vars 등). 기본적으로 로그 줄에는 IP의 마지막 8진수를 포함하는 IP 주소가 포함됩니다(IP 주소가 Adobe [!DNL Analytics] 내의 IP 난독화 설정에 따라 수정되지 않았다고 가정).
* 방문자가 Audience Manager에 설정된 규칙을 기반으로 자격을 평가하는 트레이트 및 세그먼트
* (선택 사항) 하나 이상의 ID. ID 서비스의 구현에 따라 CRM ID 또는 해시된 이메일 주소와 같은 하나 이상의 ID를 전송할 수도 있습니다. 이 데이터가 Adobe [!DNL Analytics]로 전송되면 Adobe 고객 관리로 전달됩니다. 개인 데이터는 Adobe [!DNL Analytics]에 제공하지 않는 것이 좋습니다. 대신 단방향 해시를 사용하여 데이터를 Adobe로 보내기 전에 마스크를 적용합니다.
* 백엔드 세그먼트 공유 기능을 통해 [!DNL Analytics]에서 시작된 세그먼트
* demdex.net 쿠키는 타사 쿠키가 차단되지 않은 경우에 설정됩니다. The `AMCV_###@AdobeOrg` first-party cookie is always set with the Experience Cloud ID Service.

이러한 모든 데이터 요소는 로그 파일 형식으로 Adobe Audience Manager에 전달됩니다. Audience Manager는 미국 내에서 이 데이터를 처리하고 저장합니다. Audience Manager는 미국 외부에서 이 데이터를 저장하거나 처리하는 옵션을 제공하지 않습니다.

### 쿠키 및 옵트아웃

실시간 대상 프로파일링을 사용할 때 [!DNL Analytics] 및 [!DNL Target]에 사용되는 쿠키 외에, Audience Manager 쿠키가 활용됩니다.

적절한 옵트아웃 기능을 제공하려는 경우 사이트 방문자가 기존 옵트아웃 프로세스에 Audience Manager 옵트아웃을 추가해야 합니다.

자세한 [내용은 Adobe Experience Cloud - Adobe 옵트아웃](https://docs.adobe.com/content/help/en/analytics/implementation/javascript-implementation/data-collection/opt-out.html) 구현을 참조하십시오.

도메인 [간 추적을 활성화하려면 데이터 수집](https://docs.adobe.com/content/help/en/id-service/using/reference/analytics-reference/cname.html) CNAME 및 도메인 간 추적을 참조하십시오.
