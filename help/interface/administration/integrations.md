---
description: Adobe Experience Cloud의 사용 가능한 애플리케이션 통합에 대해 알아봅니다.
solution: Experience Cloud
title: Experience Cloud 통합
uuid: a9893c6b-bccc-4fb5-b724-724644c7def5
feature: Admin Console
topic: Administration
role: Admin
level: Experienced
exl-id: 7f8fa610-32f0-4b18-8054-3ba05436a10e
source-git-commit: a4e0461791cd676365857c2dd4ef28c0e40c3430
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 74%

---

# Experience Cloud 통합 개요

이 페이지에서는 Experience Cloud 응용 프로그램 통합을 시작하는 몇 가지 방법에 대해 설명합니다. 자세한 내용은 Experience League에서 [통합 비디오 튜토리얼](https://experienceleague.adobe.com/docs/experience-platform/tags/home.html) 라이브러리를 검색하십시오.

## 플랫폼 서비스용 Experience Cloud 애플리케이션 활성화 {#section_A3D024994DA3492F8435CFCC4EF035C2}

다음 방법을 설명합니다.

* Experience Cloud에서 회사를 프로비저닝합니다.
* 관리자가 될 수 있도록 설정.
* [Experience Cloud ID 서비스 구현](https://experienceleague.adobe.com/docs/id-service/using/home.html).
* [!UICONTROL Platform 데이터 수집]을 통해 [!DNL Analytics] 및 [!DNL Target] 구현을 현대화하십시오.
* [[!DNL Customer Attributes]](../services/customer-attributes/attributes.md) 및 [[!DNL Audience Library]](../services/audiences/overview.md)과(와) 같은 Experience Cloud 서비스를 시작합니다.

솔루션 또는 서비스:

* [[!DNL Experience Platform Data Collection]](https://experienceleague.adobe.com/docs/experience-platform.html)
* [[!DNL Analytics]](https://experienceleague.adobe.com/docs/analytics.html?lang=ko-KR)
* [[!DNL Target]](https://experienceleague.adobe.com/docs/target.html)
* [Experience Cloud ID 서비스](https://experienceleague.adobe.com/docs/id-service/using/home.html)

## Experience Cloud ID 서비스 {#section_6ECCCFA2D84D4D4F88C879C799CA9D78}

ID 서비스는 Experience Cloud의 모든 애플리케이션에서 방문자를 식별하는 범용 영구 ID를 제공합니다. 이 ID는 Analytics, Audience Manager, Adobe Target, 비디오 하트비트 및 기타 Experience Cloud 애플리케이션이나 제품과 같은 서비스에 대한 ID 생성 코드를 대체할 수 있습니다.

[Experience Cloud ID 서비스](https://experienceleague.adobe.com/docs/id-service/using/home.html)를 참조하십시오

**해당 애플리케이션 또는 서비스**

* [Adobe Analytics](https://experienceleague.adobe.com/docs/id-service/using/implementation/setup-analytics.html)
* [Adobe Target](https://experienceleague.adobe.com/docs/id-service/using/implementation/setup-target.html)

## Audiences {#section_5F60D7B0833348B9A1D74663AADCB42C}

도움말: [Audiences](/help/interface/services/audiences/overview.md)

Experience Cloud [!UICONTROL 대상 라이브러리]에서 대상을 만들고 관리합니다. 다음과 같은 다양한 소스에서 대상을 만들거나 파생할 수 있습니다.

* [!DNL Experience Cloud]에서 대상을 새로 만드는 경우.
* [!DNL Analytics] 세그먼트를 [!DNL Experience Cloud]에 게시하는 경우.
* From [!DNL Audience Manager].

**해당 솔루션 또는 서비스**

* [Adobe Target의 활동](https://experienceleague.adobe.com/docs/target/using/activities/activities.html)
* Audience Manager의 [세분화](https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/audience-analytics-workflow/aam-analytics-segments.html)
* [Advertising Cloud](https://enterprise.efrontier.com/CMDashboard/?ticket=JrciD7q2bF1y2mDWFHmEyibbOnNwb2JBRF7z6tKAOIWkBimlPxCUaZyJnPLqsfdqsf3fpxWoxGasvatKA8S6-h4tlDvxQcm8Gc10dSF9q_E%3D&amp;ticket=JrciD7q2bF1y2mDWFHmEyibmxtHqnZFSOMml-n993zOBc-ovZGNZkX5vgePWqKNMoMmPSqf9PkzFeYF4UN6GqSXDVNDvwgnvv9KT8PvVxk8%3D)(로그인 필요)

## 고객 속성 {#section_6A9EA6847F654F129381869E5016626C}

도움말: [고객 속성](/help/interface/services/customer-attributes/attributes.md)

CRM(고객 관계 관리) 데이터베이스에서 엔터프라이즈 고객 데이터를 캡처하는 경우, 이 데이터를 Experience Cloud의 고객 속성 데이터 소스에 업로드할 수 있습니다. 업로드한 후에는 [!DNL Adobe Analytics] 및 [!DNL Adobe Target]의 데이터를 사용합니다.

**해당 솔루션 또는 서비스**

* Adobe Analytics: 고객 속성 보고서
* Adobe Target: 고객 속성에 대한 Adobe Target의 [구독](/help/interface/services/customer-attributes/subscription.md) 구성

## Experience Cloud Assets {#section_92BC5DFDB0E0499CB0DD34B85E06F79A}

도움말: [Creative Cloud와 Experience Cloud 폴더 공유](/help/interface/services/assets/creative-cloud.md)

Experience Cloud와 Creative Cloud 간에 폴더 및 에셋을 공유합니다. 공유 에셋에 공동 작업을 수행하고, 주석을 달고, Adobe Target과 같은 Experience Cloud 애플리케이션에서 사용합니다.

**해당 애플리케이션 또는 서비스**

* Adobe Experience Cloud
* Adobe Creative Cloud
* Adobe Target

## Analytics - Analytics의 AEM Assets 보고 {#section_0A16AE14F128470AA02EFC6457BDCE75}

도움말: [Analytics의 AEM Assets 보고](https://experienceleague.adobe.com/docs/analytics/integration/aem-assets-reporting.html)

Analytics에서 AEM 에셋 인사이트에서 제공된 에셋에 대한 노출 횟수 및 클릭 수를 수집할 수 있습니다.

**해당 애플리케이션 또는 서비스**

* [!DNL Analytics]
* [!DNL Experience Manager]

## Audience Manager 통합 {#section_8FEFE1746E26416EB7E73095BBAD5345}

[Audience Manager](https://experienceleague.adobe.com/docs/audience-manager/user-guide/implementation-integration-guides/implementation-and-integration.html)

Experience Cloud 애플리케이션 또는 Audience Manager의 기타 외부 시스템에 있는 데이터로 작업합니다.

**해당 애플리케이션 또는 서비스**

* [Analytics 서버측 전달](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/server-side-forwarding/ssf.html?lang=ko-KR)
* [Audience Manager 세그먼트를 Analytics에 보내기](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/destinations/experience-cloud-destinations/create-analytics-destination.html)
* [Adobe Target 데이터 통합](https://experienceleague.adobe.com/docs/audience-manager/user-guide/implementation-integration-guides/integration-other-applications/aam-target-integration.html)

## Adobe Target {#section_739716AB6022424CBC38724CDED10701}

도움말: [Adobe Target과 Experience Cloud 통합](/help/interface/services/audiences/overview.md)

Adobe Target을 Adobe Analytics 및 기타 Experience Cloud 애플리케이션과 통합하여 두 애플리케이션에서 동일한 데이터, Audiences, 속성 및 지표를 사용할 수 있도록 합니다.

**해당 애플리케이션 또는 서비스**

* 고객 속성: 고객 속성에 대한 Adobe Target의 [구독](/help/interface/services/customer-attributes/subscription.md) 구성
* Experience Cloud Audiences: [Experience Cloud 대상 라이브러리](/help/interface/services/audiences/overview.md)
* Analytics: [Adobe Target용 보고 소스 Adobe Analytics](https://experienceleague.adobe.com/docs/target/using/integrate/a4t/a4t.html)
* Audience Manager: [Adobe Audience Manager와 Adobe Target 데이터 통합](https://experienceleague.adobe.com/docs/audience-manager/user-guide/implementation-integration-guides/integration-other-solutions/aam-target-integration.html)
* Campaign: [Adobe Target과 Campaign 통합](https://experienceleague.adobe.com/docs/target/using/integrate/campaign-and-target.html)

## Experience Manager 통합 {#section_32FB010EF8B4429FBC63C8DC2A9BE98F}

* 비디오 자습서: [Experience Manager 통합](https://experienceleague.adobe.com/docs/integrations-learn/experience-cloud/integrations-between-applications/overview.html)

* 제품 설명서: [Experience Manager 설명서](https://experienceleague.adobe.com/docs/experience-manager-cloud-service.html)

## Experience Manager - Assets {#section_CB865F8EFE4C4147BF8E2E4B66B5A318}

도움말: [Experience Cloud 및 Creative Cloud로 AEM Assets 통합 구성](https://experienceleague.adobe.com/docs/)

AEM(Adobe Experience Manager) 에셋 내의 에셋을 Adobe Creative Cloud와 동기화하거나 그 반대로 동기화합니다. 에셋을 Experience Cloud와 동기화하거나 그 반대로 동기화할 수 있습니다. Experience Cloud를 통해 이러한 동기화를 설정할 수 있습니다.

**해당 애플리케이션 또는 서비스**

* AEM
* Creative Cloud
* [Experience Cloud](https://experienceleague.adobe.com/docs/)

## [!DNL Adobe Advertising] {#section_9B1935F8BBC147C89C6DB68A35CB1BAB}

* 도움말(로그인 필요): [Adobe Experience Cloud 솔루션 및 서비스와의 통합](https://enterprise.efrontier.com/CMDashboard?ticket=JrciD7q2bF1y2mDWFHmEyhyMKZp71ZLeaANvF-RcNMF7oNuZNABh76cKJLNlJJeJ1hQ5vAW1AO1t1DW8tZWM3lYZ8TSh96YAQISUdtHCCgA%3D&amp;ticket=JrciD7q2bF1y2mDWFHmEyibbOnNwb2JBRF7z6tKAOIWkBimlPxCUaZyJnPLqsfdqsf3fpxWoxGasvatKA8S6-h4tlDvxQcm8Gc10dSF9q_E%3D)

* Experience League의 [Adobe Advertising 설명서](https://experienceleague.adobe.com/docs/advertising.html)

**해당 애플리케이션 또는 서비스**

**Analytics:** 사이트 참여 및 전환 데이터를 매일 [!DNL Adobe Advertising]에 전송할 수 있습니다. 해당 데이터를 광고 최적화 및 보고에 사용할 수 있습니다. 또한 [!DNL Advertising]에서 매일 Analytics에 검색 엔진 및 소셜 네트워크 트래픽 데이터를 전송할 수 있으며, 해당 데이터를 Reports &amp; Analytics, Report Builder 및 AdHoc Analysis 기능의 보고서에 사용할 수 있습니다.

**태그:** 검색, 소셜 및 디스플레이 광고 랜딩 페이지에 대해 [Experience Platform 태그를 사용하여 Advertising 픽셀 기반 전환 추적 태그](https://experienceleague.adobe.com/docs/experience-platform/tags/home.html) 및 서드파티 추적 태그를 만들 수 있습니다. (또한 [!DNL Advertising] 태그를 직접 [!DNL Advertising] 내에서 만들 수 있습니다.)

**Experience Cloud Audiences:** (디스플레이 관리 부서가 있는 광고주) [Adobe Experience Cloud Audiences](../services/audiences/overview.md) 를 디스플레이 광고 대상으로 사용할 수 있습니다. Experience Cloud에서 만든 대상과 Experience Cloud에 게시한 Analytics의 대상을 자동으로 사용할 수 있습니다. [!DNL Adobe Advertising] 계정이 이를 허용하도록 구성된 경우 Audience Manager의 대상을 사용할 수도 있습니다.

Adobe Experience Cloud, 프로필 및 Audiences 액세스 관련 정보와 [!DNL Adobe Advertising] 및 Adobe Experience Cloud Audiences 사이의 초기 설정의 자세한 정보를 알아보려면 계정 관리자에게 문의하십시오. **참고:** Adobe Target도 사용하는 경우 Adobe Experience Cloud에 게시한 모든 대상을 Adobe Target의 활동에도 사용할 수 있습니다.

**Experience Cloud 자산:** (디스플레이 관리 부서가 있는 광고주) 새 디스플레이 베타 보기를 사용하여 Adobe Experience Cloud 자산을 디스플레이 광고를 위한 크리에이티브 기능으로 사용할 수 있습니다. Adobe Experience Cloud 에셋에 액세스하려면 Adobe Experience Cloud을 통해 [Adobe Advertising에 로그인](https://enterprise.efrontier.com/CMDashboard)해야 합니다. Adobe Experience Cloud 액세스 관련 정보를 자세히 알아보려면 계정 관리자에게 문의하십시오.

**Experience Cloud 알림:** 각 페이지 상단의 알림 링크에서 검색 Beta 경고 템플릿에서 생성된 모든 경고를 볼 수 있습니다. Experience Cloud 시스템 업데이트, 게시물, 멘션, 공유된 에셋 받기도 가능합니다. 알림에 액세스하려면 [Adobe Experience Cloud을 통해 Adobe Advertising에 로그인](https://enterprise.efrontier.com/CMDashboard)해야 합니다. Adobe Experience Cloud 액세스 관련 정보를 자세히 알아보려면 계정 관리자에게 문의하십시오.
