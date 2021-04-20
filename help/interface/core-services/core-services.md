---
description: 교차 솔루션 서비스를 위한 Adobe Analytics 및 Adobe Target 솔루션을 현대화합니다. Experience Cloud 서비스를 사용하는 방법을 알아봅니다.
keywords: 핵심 서비스, 고객 속성
solution: Experience Cloud
title: 교차 솔루션 서비스용 솔루션을 사용하도록 설정
index: true
feature: Customer Attributes
topic: Administration
role: Administrator
level: Experienced
translation-type: ht
source-git-commit: 042f7caed2f1bace05f59c6c2824c286a13934fe
workflow-type: ht
source-wordcount: '2369'
ht-degree: 100%

---


# Experience Cloud 서비스에 대한 구현 활성화

최근 Experience Platform Launch를 사용하여 Experience Cloud을 구현한 경우 고객 속성 및 Experience Cloud 대상에 대해 이미 설정되어 있습니다. Admin Console에서 사용자와 제품을 관리할 수도 있습니다.

기존 고객의 경우 솔루션 구현을 현대화하고 Experience Cloud을 구현해야 할 수 있습니다. 이를 통해 Adobe Analytics, Audience Manager 및 Adobe Target에서 고객 속성 및 대상 기능을 활용할 수 있습니다. 이를 구현하려면 다음 작업을 수행합니다.

1. [Experience Cloud에 참여 및 관리자 되기](#section_2423F0BD3DF642658103310EE5EA6154)
1. [Experience Cloud ID 서비스 구현](#section_3C9F6DF37C654D939625BB4D485E4354)
1. [보고서 세트를 Experience Cloud 조직에 매핑](#section_7B08516B01BA421681DF03D0E86CE3BA)
1. [Analytics AppMeasurement 코드 업데이트](#section_1798D9D0F05C47E29816AC4EEB9A0913)
1. [Adobe Target 구현 업데이트](#section_C2F4493C7A36406DAE2266B429A4BD24)
1. [구현 확인](#section_E641782A0F4F44AF8C9C91216BE330D5)
1. [사용자 및 제품 관리](#section_B6E95F4E0E12483CB9DA99CBC0C5A4AF)
1. [속성 및 대상 데이터 공유 시작](#section_960C06093623462E8EA247B3E97274A1)

## Experience Cloud에 참여 및 관리자 되기 {#section_2423F0BD3DF642658103310EE5EA6154}

Experience Cloud에 참여하기 위해 수행할 작업:

1. 적절한 Adobe Analytics 또는 Adobe Target SKU가 있는지 확인합니다.

   * **Adobe Analytics:** Standard 또는 Premium(이전 [!DNL SiteCatalyst] SKU 아님).
   * **Adobe Target:** Standard 또는 Premium.

   >[!NOTE]
   >
   >[!DNL Target]의 경우 [!DNL mbox.js]에서 at.js로 마이그레이션하십시오. [at.js 1.x에서 at.js 2. x로 업그레이드](https://docs.adobe.com/content/help/ko-KR/target/using/implement-target/client-side/upgrading-from-atjs-1x-to-atjs-20.html)를 참조하십시오.

1. 구현을 현대화하고 관리자가 프로비저닝되도록 합니다.

   * [[!UICONTROL Experience Cloud ID 서비스]](../core-services/core-services.md#section_3C9F6DF37C654D939625BB4D485E4354) 구현에서 아래 절차를 따르십시오.
   * 계정 관리자에게 문의하여 Experience Cloud에 대한 프로비저닝 프로세스를 시작합니다.

1. [!UICONTROL Admin Console]에서 사용자 및 제품 관리.

### 관리자 로그인

관리자가 되면 [marketing.adobe.com](https://experiencecloud.adobe.com)에 로그인할 수 있습니다.

Experience Cloud 메뉴 탐색에 **[!UICONTROL 관리]** 링크가 표시됩니다.

자세한 내용은 [Experience Cloud 사용자 및 제품 관리](../admin-getting-started/admin-getting-started.md#topic_3FCB4099640647E3B2411ADBFCE81909)를 참조하십시오.

### 사용자 로그인

Experience Cloud에 로그인하려면 귀하의 사용자는

* Adobe ID(또는 회사의 Enterprise ID)가 있어야 합니다.
* [experiencecloud.adobe.com](https://experiencecloud.adobe.com)에서 로그인합니다.
* 엔터프라이즈 그룹에 매핑된 솔루션 그룹에 속합니다.
* 필요한 경우 솔루션 계정을 Adobe ID에 연결합니다(아래에 설명).

### 선택 사항: 기존 사용자 계정을 연결합니다.

[!UICONTROL Analytics] > [!UICONTROL 관리 도구]에서 이전에 관리한 Analytics 그룹처럼 이미 솔루션 그룹의 구성원인 사용자가 있을 것입니다.

이러한 그룹을 Experience Cloud 엔터프라이즈 그룹에 매핑하면 그러한 사용자가 해당 솔루션 계정 자격 증명을 해당 Adobe ID에 수동으로 링크해야 합니다.

[Experience Cloud에서 계정 연결](../admin-getting-started/organizations.md#topic_C31CB834F109465A82ED57FF0563B3F1)을 참조하십시오.

>[!NOTE]
>
>엔터프라이즈 및 솔루션 그룹이 매핑되면 새로운 사용자가 자동으로 연결됩니다. (솔루션 자격 증명은 자동으로 만들어지고 해당 Adobe ID에 연결됩니다.)

다음 섹션에서는 구현을 현대화하는 방법을 설명합니다. 구현을 현대화하면 Experience Cloud에서 핵심 서비스가 활성화됩니다.

## [!UICONTROL Experience Cloud ID 서비스] 구현 {#section_3C9F6DF37C654D939625BB4D485E4354}

[!UICONTROL Experience Cloud ID 서비스]에서는 교차 솔루션 통합을 위한 공통 ID를 제공하고 [!UICONTROL 고객 속성]을 통해 업로드된 CRM 데이터를 기반으로 도메인 간 방문자 식별 및 장치/브라우저 간 타깃팅 및 개인화를 위한 경로를 제공합니다.

Experience Cloud 핵심 서비스를 활성화하는 가장 간단한 방법은 [Experience Platform Launch](https://experienceleague.adobe.com/docs/launch/using/extensions-ref/adobe-extension/id-service-extension/overview.html?lang=ko-KR#extensions-ref)에서 [!UICONTROL Experience Cloud ID 서비스 확장]을 통해 Analytics 및 Adobe Target에 대해 자동으로 활성화하는 것입니다.

전체 Experience Cloud ID 서비스 도움말(이전의 방문자 ID)를 보려면 [여기](https://experienceleague.adobe.com/docs/id-service/using/intro/overview.html?lang=ko-KR#intro)로 이동하십시오.

**[!UICONTROL Experience Platform Launch]나 [!UICONTROL Dynamic Tag Management]를 사용하지 않습니까?**

[!UICONTROL Experience Platform Launch]나 [!UICONTROL Dynamic Tag Management]를 사용하지 않는 경우 다음과 같이 JavaScript 배포([!DNL VisitorAPI.js])를 사용하여 ID 서비스를 수동으로 구현하십시오.

| 작업 | 설명 |
| -----------| ---------- |  
| [Analytics용 Experience Cloud ID 서비스 구현](https://docs.adobe.com/content/help/ko-KR/id-service/using/implementation/setup-analytics.html) | [고객 ID](https://docs.adobe.com/content/help/ko-KR/id-service/using/reference/authenticated-state.html)를 추가적으로 설정하는 것도 좋습니다. 이러한 ID는 각 방문자와 연결되며 Experience Cloud의 현재 및 향후 기능을 활성화합니다. |
| 기존 [!DNL s_code]를 버전 H.27.3 이상으로 업데이트하거나 기존 [!DNL AppMeasurement.js]를 버전 1.4 이상으로 업데이트합니다. | 이러한 파일은 Analytics 관리 도구의 [코드 관리자](https://docs.adobe.com/content/help/ko-KR/analytics/admin/admin-tools/code-manager-admin.html)에서 다운로드할 수 있습니다. ([!DNL AppMeasurement.js]에 대한 자세한 내용이 필요한 경우 [JavaScript 구현](https://docs.adobe.com/content/help/ko-KR/analytics/implementation/javascript-implementation/javascript-implementation-overview.html) 안내서를 사용할 수 있습니다.) |
| Analytics에 대한 고객 ID 동기화 | [Analytics - 고객 ID 동기화](../core-services/core-services.md#section_AD473A6A21C1446498E700363F9A8437)(아래)를 참조하십시오. |

### Analytics 및 Adobe Target - 고객 ID 동기화 {#section_AD473A6A21C1446498E700363F9A8437}

Experience Cloud ID 서비스 설정의 일부로, Analytics 및 [!DNL Target]에 대해 [고객 ID](https://docs.adobe.com/content/help/ko-KR/id-service/using/reference/authenticated-state.html)를 Experience Cloud와 동기화하는 것이 좋습니다.

Adobe Target에서 `mbox3rdpartyid`는 고객 ID를 가져와서 [!DNL Target]에 보내야 합니다. ([!DNL Target]에서 [고객 속성 사용](https://docs.adobe.com/content/help/ko-KR/target/using/audiences/visitor-profiles/working-with-customer-attributes.html)을 참조하십시오.)

방문자가 사용자의 웹 사이트에서 인증을 받거나 다른 방식으로 식별될 경우 페이지나 앱에 해당 개인의 CRM 고객 ID가 제공되어야 합니다. 그러면 해당 기능 호출을 사용하여 고객 ID를 Experience Cloud와 동기화할 수 있습니다. 이와 같이 동기화가 진행되면 방문자의 CRM 고객 ID가 Experience Cloud에 저장되고 Experience Cloud에서 사용할 해당 고객의 속성이 활성화됩니다.

예를 들어 CRM 시스템에서 Bob의 고객 ID가 `52mc210tr42`라고 가정해봅시다. Bob이 사용자 사이트에서 인증을 받으면, 사용자는 이 ID를 페이지에 제공하고 다음 두 가지 방법 중 하나로 해당 ID를 사용하여 동기화해야 합니다.

* 방문자 ID 서비스를 사용하여 `visitor.setCustomerIDs({"crm_id":"52mc210tr42"})`를 호출합니다. 또는,
* prop 또는 eVar에서 *`Customer ID (52mc210tr42)`*&#x200B;를 입력합니다.

고객 ID는 고객 ID가 알려지는 모든 [!DNL Analytics] 서버 호출에서 설정되어야 합니다.

### Mobile SDK

[Android](https://docs.adobe.com/content/help/ko-KR/mobile-services/android/overview.html) 및 [iOS](https://docs.adobe.com/content/help/ko-KR/mobile-services/ios/overview.html) 모바일 애플리케이션에서 추가 고객 ID 설정 방법에 대한 구문 예가 필요하면 *Experience Cloud ID 서비스* 섹션을 참조하십시오.

### 이전 데이터의 속성 활성화

고객 특성 데이터는 방문자가 로그인한 후에 사용할 수 있습니다. 최신 Experience Cloud ID 서비스를 아직 구현하지 않았으며 이전에 prop 또는 eVar에서 고객 ID를 추적해온 경우 Experience Cloud에 내역 로그인을 전송하는 프로세스를 요청할 수 있습니다. 이 프로세스를 진행하면 고객 속성을 바로 사용할 수 있습니다.

이전 데이터를 활성화하려면 고객 지원 센터에 문의하십시오.

## 보고서 세트를 Experience Cloud 조직에 매핑 {#section_7B08516B01BA421681DF03D0E86CE3BA}

>[!NOTE]
>
>보고서 세트 매핑 기능은 2020년 11월에 더 이상 사용되지 않습니다. 문의 사항이 있으면 고객 지원팀에 문의하십시오.

Experience Cloud 서비스(예: Experience Cloud ID 서비스, [!UICONTROL People 서비스])는 개별 Analytics 보고서 세트가 아니라 Experience Cloud 조직과 연결되어 있습니다. 이러한 서비스가 올바르게 작동하도록 하려면 각 Analytics 보고서 세트를 Experience Cloud 조직에 매핑해야 합니다.

[조직에 보고서 세트 매핑](report-suite-mapping.md)을 확인하십시오.

## Analytics AppMeasurement 코드 업데이트 {#section_1798D9D0F05C47E29816AC4EEB9A0913}

Analytics를 사용하는 경우 지역 데이터 수집(RDC)에 있는지 확인합니다. 데이터 수집 도메인이 [!DNL omtrdc.net]이거나 CNAME이 [!DNL omtrdc.net]으로 매핑된 경우 RDC를 사용해야 합니다. 자세한 내용은 [RDC로 전환](https://docs.adobe.com/content/help/ko-KR/analytics/technotes/rdc/regional-data-collection.html)을 참조하십시오. 자사 쿠키를 사용하는 경우 데이터 수집 CNAME 및 도메인 간 추적에 대해 알려면 [CNAME 및 Experience Cloud ID 서비스](https://docs.adobe.com/content/help/ko-KR/id-service/using/reference/analytics-reference/cname.html)를 참조하십시오.

방문자 API를 비롯한 JavaScript 라이브러리를 업데이트하여 Analytics 구현을 현대화하는 것이 좋습니다. Dynamic Tag Management에서 [!DNL Adobe Analytics] 도구를 추가하고 구성 방법으로 *`Automatic`*&#x200B;을 지정하는 간편한 방법입니다.

[!UICONTROL Dynamic Tag Management]에서 **`<Web Property Name>`** > **[!UICONTROL 개요]** > **[!UICONTROL 도구 추가]** > **[!UICONTROL Adobe Analytics]**&#x200B;를 클릭합니다. 배포에 대해서는 Dynamic Tag Management에서 [Adobe Analytics 설정](https://docs.adobe.com/content/help/ko-KR/dtm/using/tools/analytics-dtm.html)을 참조하십시오.

## Adobe Target 구현 업데이트 {#section_C2F4493C7A36406DAE2266B429A4BD24}

* 라이브러리 검색이 자동으로 수행되도록 [Experience Platform Launch](https://docs.adobe.com/content/help/ko-KR/launch/using/extensions-ref/adobe-extension/targetv2-extension/adobe-target-extension-v2.html)에서 [!UICONTROL Adobe Target 확장]을 추가하는 것이 좋습니다. [!UICONTROL Experience Platform Launch]를 사용하여 Adobe Target(및 기타 솔루션)용으로 [Experience Cloud ID 서비스 확장](https://docs.adobe.com/content/help/ko-KR/launch/using/extensions-ref/adobe-extension/id-service-extension/overview.html)을 설정할 수도 있습니다. Adobe Target에서 핵심 서비스를 사용하려면 [!UICONTROL Experience Cloud ID 서비스] 업데이트가 **필요합니다**. ([!UICONTROL Dynamic Tag Management]를 사용하는 경우 [Adobe Target 도구](https://docs.adobe.com/content/help/ko-KR/dtm/using/tools/target.html)를 추가하십시오. [!UICONTROL Dynamic Tag Management]를 사용하여 Adobe Target용으로 Experience Cloud ID 서비스를 배포할 수도 있습니다.)
* [!UICONTROL Experience Platform Launch]나 [!UICONTROL Dynamic Tag Management]를 사용하지 않는 경우 수동으로 [mbox 라이브러리를 업데이트하십시오](https://docs.adobe.com/content/help/ko-KR/target/using/implement-target/client-side/mbox-implement/target-download-config-mbox.html).
* [!DNL Adobe Target]에 대한 보고 소스로 Adobe Analytics를 사용하기 위한 액세스 권한을 요청하십시오. [!DNL Target] 및 [!DNL Analytics] 데이터가 처리 중에 동일한 서버 호출에 결합되므로 방문자가 두 솔루션 간에 연결됩니다. [Analytics for Target 구현](https://docs.adobe.com/content/help/ko-KR/target/using/integrate/a4t/a4t.html)을 참조하십시오.

   >[!IMPORTANT]
   >
   >모든 Analytics 고객에게 고객 속성과 같은 핵심 서비스가 공급됩니다. Analytics 사용자가 아닌 경우 고객 지원 센터에 문의하여 제공받을 수 있도록 요청하십시오.

## 구현 확인 {#section_E641782A0F4F44AF8C9C91216BE330D5}

다음 프로세스에 따라 사이트에서 Experience Cloud ID 서비스가 올바르게 구현되도록 합니다.

1. Experience Cloud ID 서비스에 대한 요청을 볼 수 있게 사이트에 대한 쿠키를 지웁니다. 이 요청은 첫 번째 방문에서 수행된 후 매주 방문자마다 거의 한 번씩 수행됩니다.
1. 패킷 분석기 또는 웹 브라우저 디버거의 네트워크 패널을 사용하여 [!DNL dpm.demdex.net]으로 진행되는 요청을 찾습니다.
1. 이 응답에는 `d_mid` 및 값이 포함됩니다(예: `_setMarketingCloudFields({"d_mid":"4235...`).
1. Analytics 요청에 `mid` 매개 변수(Marketing Cloud ID)가 포함되어 있는지 확인합니다. 유예 기간(활성화된 경우) 동안 `aid` 매개 변수(Analytics 방문자 ID)도 표시되어야 합니다.

Experience Cloud ID가 포함된 예상 응답은 다음과 같습니다.

![](assets/mac_id_response.png)

Experience Cloud ID(mid)가 포함된 Analytics 이미지 요청(`mid` 또는 _방문자 ID_&#x200B;라고도 함):

![](assets/mid.png)

mbox 요청의 Experience Cloud ID:

![](assets/mbox_request.png)

### 유예 기간이란 무엇입니까?

Experience Cloud ID 서비스를 배포하면 새 방문자는 더 이상 데이터 수집 서버에서 Analytics Experience Cloud ID를 받지 않습니다. 사이트의 섹션이 Experience Cloud ID 서비스를 아직 구현하지 않은 경우 방문자가 이러한 섹션으로 이동하면 Experience Cloud ID는 인식되지 않으며 방문자에게 이전 Analytics 방문자 ID가 지정됩니다. 이로 인해 중복 방문 및 잘못된 특성을 포함한 잠재적 문제가 발생할 수 있습니다.

예를 들어 사이트의 지원 섹션에 별도의 CMS에서 관리되는 경우 이 섹션에 대해 다른 Analytics JavaScript 파일을 보유할 수 있습니다. 지원 사이트에 ID 서비스를 배포하기 전에 기본 사이트에 Experience Cloud ID를 배포하는 경우 새 방문자가 지원 섹션을 방문하면 이전 Analytics ID를 받게 되며 두 사이트 섹션에 걸쳐 진행되는 방문이 다른 방문으로 보고됩니다.

여러 JavaScript 파일 또는 다른 기술(예: Flash)을 사용하는 사이트에 Experience Cloud ID 서비스를 배포하면 사이트의 모든 부분에서 동시에 해당 Experience Cloud ID 서비스를 사용하도록 설정해야 하므로 조정 문제가 발생할 수 있습니다. 유예 기간을 구성하면 새 방문자가 ID 서비스에서 Analytics 방문자 ID를 계속 받게 되므로 방문자는 방문자 ID 서비스를 사용하도록 업그레이드되지 않은 사이트의 섹션에서 일관되게 식별될 수 있습니다.

## 사용자 및 제품 관리 {#section_B6E95F4E0E12483CB9DA99CBC0C5A4AF}

Admin Console을 실행 중이면 사용자 및 제품 프로필을 관리할 수 있는 [Admin Console](https://adminconsole.adobe.com/)로 이동합니다.

![](assets/menu-administration-shell.png)

[Experience Cloud 사용자 및 제품 관리](../admin-getting-started/admin-getting-started.md#topic_3FCB4099640647E3B2411ADBFCE81909)를 참조하십시오.

### 고객 속성

[!UICONTROL 고객 속성] 그룹에 추가된 사용자의 경우 Experience Cloud 인터페이스 왼쪽에 [!UICONTROL 고객 속성] 메뉴 항목이 표시됩니다.

## 속성 및 대상 데이터 공유 시작 {#section_960C06093623462E8EA247B3E97274A1}

다음 기능을 활용할 수 있습니다.

### [!UICONTROL 사용자] > [!UICONTROL 고객 속성]

CRM(고객 관계 관리) 데이터베이스에서 엔터프라이즈 고객 데이터를 캡처하는 경우, 이 데이터를 Experience Cloud의 고객 속성 데이터 소스에 업로드할 수 있습니다. 업로드했으면 [!DNL Adobe Analytics] 및 [!DNL Adobe Target]의 데이터를 활용합니다.

[고객 속성](../attributes/attributes.md#concept_ACFEE7C8B8E94875BA0825CDF4913AF1)을 참조하십시오

### [!UICONTROL 사용자] > [!UICONTROL 대상 라이브러리]

Experience Cloud [!UICONTROL 대상]은 대상을 만들고, 기존 대상을 결합하여 복합 대상을 만들고, 모든 공유 대상을 볼 수 있는 인터페이스입니다.

[대상](../audience-library/audience-library.md#topic_679810123CAA4E0CA4FA3417FB0100C7)을 참조하십시오

## 데이터 저장 및 개인 정보 공개

Adobe [!DNL Experience Cloud] 내의 실시간 대상 프로파일링 및 기타 핵심 서비스를 활용하는 경우, 이러한 서비스의 사용이 데이터가 상주하는 데이터 센터(및 국가)에 영향을 줄 수 있습니다. 특히, Adobe [!DNL Experience Cloud]의 핵심 서비스는 Adobe Audience Manager를 활용하므로, [!UICONTROL 사용자] 서비스 내에서 사용된 데이터는 미국의 Audience Manager 서버 내에 상주해야 합니다.

[!UICONTROL 사용자] 서비스를 통해 사용할 수 있는 핵심 서비스를 활용할 때 다른 Adobe 제품에서 대상 관리로 전송되는 데이터 유형은 다음과 같습니다.

* [!DNL Analytics] 키/값 쌍(props, eVars, list vars 등). 기본적으로 로그 줄에는 IP의 마지막 8진수를 포함하는 IP 주소가 포함됩니다(IP 주소가 Adobe [!DNL Analytics] 내의 IP 난독화 설정에 따라 수정되지 않았다고 가정).
* 방문자가 Audience Manager에서 설정된 규칙에 따라 자격을 평가하는 트레이트 및 세그먼트
* (선택 사항) 하나 이상의 ID. ID 서비스 구현에 따라, CRM ID 또는 해시된 이메일 주소와 같은 하나 이상의 ID를 전송할 수도 있습니다. 이 데이터가 Adobe [!DNL Analytics]로 전송되면 Adobe 고객 관리로 전달됩니다. 개인 데이터는 Adobe [!DNL Analytics]에 제공하지 않는 것이 좋습니다. 개인 데이터의 경우 Adobe로 전송하기 전에 단방향 해시를 사용해서 데이터를 가리는 것이 좋습니다.
* 백엔드 세그먼트 공유 기능을 통해 [!DNL Analytics]에서 시작된 세그먼트
* demdex.net 쿠키는 타사 쿠키가 차단되지 않은 경우에 설정됩니다. `AMCV_###@AdobeOrg` 자사 쿠키는 항상 Experience Cloud ID 서비스를 사용하여 설정됩니다.

이러한 모든 데이터 요소는 로그 파일 형식에서 Adobe Audience Manager로 전달됩니다. Audience Manager는 미국 내에서 이 데이터를 처리하고 저장합니다. Audience Manager는 미국 외부에서 이 데이터를 저장하고 처리하기 위한 옵션을 제공하지 않습니다.

### 쿠키 및 옵트아웃

실시간 대상 프로파일링을 사용할 때 [!DNL Analytics] 및 [!DNL Target]에 사용되는 쿠키 외에, Audience Manager 쿠키가 활용됩니다.

적절한 옵트아웃 기능을 제공하려는 경우 사이트 방문자가 기존 옵트아웃 프로세스에 Audience Manager 옵트아웃을 추가해야 합니다.

지침이 필요하면 [Adobe Experience Cloud - Adobe 옵트 아웃 구현](https://docs.adobe.com/content/help/ko-KR/analytics/implementation/javascript-implementation/data-collection/opt-out.html)을 참조하십시오.

도메인 간 추적을 사용하려면 [데이터 수집 CNAME 및 도메인 간 추적](https://docs.adobe.com/content/help/ko-KR/id-service/using/reference/analytics-reference/cname.html)을 참조하십시오.
