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
source-git-commit: eb2ad8a8255915be47b6002a78cc810b522170d2
workflow-type: tm+mt
source-wordcount: '1421'
ht-degree: 99%

---

# Experience Cloud 통합 개요

Adobe Experience Cloud는 강력한 기능 세트를 갖춘 일반 데이터 플랫폼을 기반으로 구축한 최고의 통합 애플리케이션 및 서비스 세트입니다.

## 플랫폼 서비스용 Experience Cloud 애플리케이션 활성화 {#section_A3D024994DA3492F8435CFCC4EF035C2}

도움말: [플랫폼 서비스용 애플리케이션 활성화](core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C)

다음 방법을 설명합니다.

* Experience Cloud에서 회사 프로비저닝.
* 관리자가 될 수 있도록 설정.
* [Experience Cloud ID 서비스 구현](https://experienceleague.adobe.com/docs/id-service/using/home.html?lang=ko-KR).
* Platform 데이터 수집으로 [!DNL Analytics] 및 [!DNL Target] 구현을 현대화하십시오.
* 핵심 서비스 사용 시작.

솔루션 또는 서비스:

* Activation - Experience Platform 데이터 수집(이전의 Launch)
* Analytics
* Target
* [Experience Cloud ID 서비스](https://experienceleague.adobe.com/docs/id-service/using/home.html?lang=en)

## Experience Cloud ID 서비스 {#section_6ECCCFA2D84D4D4F88C879C799CA9D78}

ID 서비스는 Experience Cloud의 모든 애플리케이션에서 방문자를 식별하는 범용 영구 ID를 제공합니다. 이 ID는 Analytics, Audience Manager, Adobe Target, 비디오 하트비트 및 기타 Experience Cloud 애플리케이션이나 제품과 같은 서비스에 대한 ID 생성 코드를 대체할 수 있습니다.

[Experience Cloud ID 서비스](https://experienceleague.adobe.com/docs/id-service/using/home.html?lang=en)를 참조하십시오

**해당 애플리케이션 또는 서비스**

* [Adobe Analytics](https://experienceleague.adobe.com/docs/id-service/using/implementation/setup-analytics.html?lang=ko-KR)
* [Adobe Target](https://experienceleague.adobe.com/docs/id-service/using/implementation/setup-target.html?lang=ko-KR)

## Audiences {#section_5F60D7B0833348B9A1D74663AADCB42C}

도움말: [Audiences](audience-library.md#topic_679810123CAA4E0CA4FA3417FB0100C7)

Experience Cloud 대상 라이브러리에서 Audiences를 만들고 관리합니다. 다음과 같은 다양한 소스에서 대상을 만들거나 파생할 수 있습니다.

* [!DNL Experience Cloud]에서 대상을 새로 만드는 경우.
* [!DNL Analytics] 세그먼트를 [!DNL Experience Cloud]에 게시하는 경우.
* From [!DNL Audience Manager].

**해당 솔루션 또는 서비스**

* [Adobe Target의 활동](https://experienceleague.adobe.com/docs/target/using/activities/activities.html?lang=ko-KR)
* Audience Manager의 [세분화](https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/audience-analytics-workflow/aam-analytics-segments.html?lang=ko-KR)
* [Advertising Cloud](https://enterprise.efrontier.com/CMDashboard/?ticket=JrciD7q2bF1y2mDWFHmEyibbOnNwb2JBRF7z6tKAOIWkBimlPxCUaZyJnPLqsfdqsf3fpxWoxGasvatKA8S6-h4tlDvxQcm8Gc10dSF9q_E%3D&amp;ticket=JrciD7q2bF1y2mDWFHmEyibmxtHqnZFSOMml-n993zOBc-ovZGNZkX5vgePWqKNMoMmPSqf9PkzFeYF4UN6GqSXDVNDvwgnvv9KT8PvVxk8%3D) (로그인 필요)

## 고객 속성 {#section_6A9EA6847F654F129381869E5016626C}

도움말: [고객 속성](attributes.md#concept_ACFEE7C8B8E94875BA0825CDF4913AF1)

CRM(고객 관계 관리) 데이터베이스에서 엔터프라이즈 고객 데이터를 캡처하는 경우, 이 데이터를 Experience Cloud의 고객 속성 데이터 소스에 업로드할 수 있습니다. 업로드한 후에는 [!DNL Adobe Analytics] 및 [!DNL Adobe Target]의 데이터를 사용합니다.

**해당 솔루션 또는 서비스**

* Adobe Analytics: 고객 속성 보고서
* Adobe Target: 고객 속성에 대한 Adobe Target의 [구독](subscription.md) 구성

## Experience Cloud Assets {#section_92BC5DFDB0E0499CB0DD34B85E06F79A}

도움말: [Creative Cloud와 Experience Cloud 폴더 공유](creative-cloud.md)

Experience Cloud와 Creative Cloud 간에 폴더 및 에셋을 공유합니다. 공유 에셋에 공동 작업을 수행하고, 주석을 달고, [!DNL Social] 및 [!DNL Target]과 같은 Experience Cloud 애플리케이션에서 사용합니다.

**해당 애플리케이션 또는 서비스**

* [!DNL Experience Cloud]
* [!DNL Creative Cloud]
* [!DNL Target]
* [!DNL Social]

## Analytics - Analytics의 AEM Assets 보고 {#section_0A16AE14F128470AA02EFC6457BDCE75}

도움말: [Analytics의 AEM Assets 보고](https://experienceleague.adobe.com/docs/analytics/integration/aem-assets-reporting.html?lang=ko-KR)

Analytics에서 AEM 에셋 인사이트에서 제공된 에셋에 대한 노출 횟수 및 클릭 수를 수집할 수 있습니다.

**해당 애플리케이션 또는 서비스**

* [!DNL Analytics]
* [!DNL Experience Manager]

## Audience Manager 통합 {#section_8FEFE1746E26416EB7E73095BBAD5345}

[Audience Manager](https://experienceleague.adobe.com/docs/audience-manager/user-guide/implementation-integration-guides/implementation-and-integration.html?lang=ko-KR)

Experience Cloud 애플리케이션 또는 Audience Manager의 기타 외부 시스템에 있는 데이터로 작업합니다.

**해당 애플리케이션 또는 서비스**

* [Analytics 서버측 전달](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/server-side-forwarding/ssf.html?lang=ko-KR)
* [Audience Manager 세그먼트를 Analytics에 보내기](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/destinations/experience-cloud-destinations/create-analytics-destination.html?lang=ko-KR)
* [Adobe Target 데이터 통합](https://experienceleague.adobe.com/docs/audience-manager/user-guide/implementation-integration-guides/integration-other-applications/aam-target-integration.html?lang=ko-KR)

## 활성화 {#section_A23510A2D57842F6BAD043650C06DE42}

도움말: [시작하기](https://experienceleague.adobe.com/docs/experience-platform/tags/get-started/quick-start.html?lang=ko-KR)

Experience Cloud 활성화 애플리케이션을 사용하여 Experience Cloud 애플리케이션을 설정 및 디버깅합니다.

1. [Experience Platform Launch](https://experienceleague.adobe.com/docs/experience-platform/tags/home.html?lang=ko-KR) 를 사용하여 페이지에 Experience Cloud 애플리케이션을 활성화하는 코드를 삽입합니다.
1. [Adobe Cloud Platform Auditor](https://experienceleague.adobe.com/docs/auditor/using/overview.html?lang=ko-KR) 를 사용하여 구현을 테스트합니다.

Adobe Experience Cloud Debugger 확장 프로그램을 사용하여 감사에서 발견한 문제를 디버깅하거나 구현에 대한 다른 정보를 조사합니다.

**해당 애플리케이션 또는 서비스**

* [Analytics](https://experienceleague.adobe.com/docs/analytics/analyze/analysis-workspace/home.html?lang=ko-KR)
* [Audience Manager](https://experienceleague.adobe.com/docs/experience-platform/tags/extensions/adobe/audience-manager/overview.html?lang=ko-KR)
* [Advertising Cloud](https://experienceleague.adobe.com/docs/experience-platform/tags/home.html?lang=en)
* [Adobe Target](https://experienceleague.adobe.com/docs/experience-platform/tags/home.html?lang=en)
* [MAC ID 서비스](https://experienceleague.adobe.com/docs/experience-platform/tags/home.html?lang=en)
* [Nielsen 추적](https://experienceleague.adobe.com/docs/experience-platform/tags/home.html?lang=en)

## Adobe Target {#section_739716AB6022424CBC38724CDED10701}

도움말: [Adobe Target과 Experience Cloud 통합](audience-library.md)

Adobe Target을 Adobe Analytics 및 기타 Experience Cloud 애플리케이션과 통합하여 두 애플리케이션에서 동일한 데이터, Audiences, 속성 및 지표를 사용할 수 있도록 합니다.

**해당 애플리케이션 또는 서비스**

* 고객 속성: 고객 속성에 대한 Adobe Target의 [구독](subscription.md) 구성
* Experience Cloud Audiences: [Experience Cloud 대상 라이브러리](audience-library.md)
* Analytics: [Adobe Target용 보고 소스 Adobe Analytics](https://experienceleague.adobe.com/docs/target/using/integrate/a4t/a4t.html?lang=ko-KR)
* Dynamic Tag Management: [DTM을 사용하여 Adobe Target을 구현하는 모범 사례](https://experienceleague.adobe.com/docs/experience-platform/tags/home.html?lang=en)
* Audience Manager: [Adobe Audience Manager와 Adobe Target 데이터 통합](https://experienceleague.adobe.com/docs/audience-manager/user-guide/implementation-integration-guides/integration-other-solutions/aam-target-integration.html?lang=ko-KR)
* Campaign: [Adobe Target과 Campaign 통합](https://experienceleague.adobe.com/docs/target/using/integrate/campaign-and-target.html?lang=ko-KR)

## Experience Manager 통합 {#section_32FB010EF8B4429FBC63C8DC2A9BE98F}

도움말: [Experience Manager 설명서](https://experienceleague.adobe.com/docs/experience-manager-cloud-service.html?lang=ko-KR)

기타 애플리케이션 및 서드파티 서비스와 AEM을 통합합니다.

**해당 애플리케이션 또는 서비스**

* [Analytics](https://experienceleague.adobe.com/docs/)
* [Analytics with External Providers](https://experienceleague.adobe.com/docs/)
* [Experience Cloud](https://experienceleague.adobe.com/docs/)
* [Creative Cloud](https://experienceleague.adobe.com/docs/)
* [Audience Manager](https://experienceleague.adobe.com/docs/)
* [Campaign](https://experienceleague.adobe.com/docs/)
* [Scene7](https://experienceleague.adobe.com/docs/)
* [Adobe Target](https://experienceleague.adobe.com/docs/)
* [서드파티 서비스](https://experienceleague.adobe.com/docs/) (data connectors)
* [확장](https://experienceleague.adobe.com/docs/)

## Experience Manager - Assets {#section_CB865F8EFE4C4147BF8E2E4B66B5A318}

도움말: [Experience Cloud 및 Creative Cloud로 AEM Assets 통합 구성](https://experienceleague.adobe.com/docs/)

AEM(Adobe Experience Manager) 에셋 내의 에셋을 Adobe Creative Cloud와 동기화하거나 그 반대로 동기화합니다. 에셋을 Experience Cloud와 동기화하거나 그 반대로 동기화할 수 있습니다. Experience Cloud를 통해 이러한 동기화를 설정할 수 있습니다.

**해당 애플리케이션 또는 서비스**

* AEM
* Creative Cloud
* [Experience Cloud](https://experienceleague.adobe.com/docs/)

## [!DNL Adobe Advertising] {#section_9B1935F8BBC147C89C6DB68A35CB1BAB}

도움말(로그인 필요): [Adobe Experience Cloud 솔루션 및 서비스와의 통합](https://enterprise.efrontier.com/CMDashboard?ticket=JrciD7q2bF1y2mDWFHmEyhyMKZp71ZLeaANvF-RcNMF7oNuZNABh76cKJLNlJJeJ1hQ5vAW1AO1t1DW8tZWM3lYZ8TSh96YAQISUdtHCCgA%3D&amp;ticket=JrciD7q2bF1y2mDWFHmEyibbOnNwb2JBRF7z6tKAOIWkBimlPxCUaZyJnPLqsfdqsf3fpxWoxGasvatKA8S6-h4tlDvxQcm8Gc10dSF9q_E%3D)

**해당 애플리케이션 또는 서비스**

**Analytics:** 사이트 참여 및 전환 데이터를 매일 [!DNL Adobe Advertising]에 전송할 수 있습니다. 해당 데이터를 광고 최적화 및 보고에 사용할 수 있습니다. 또한 [!DNL Advertising]에서 매일 Analytics에 검색 엔진 및 소셜 네트워크 트래픽 데이터를 전송할 수 있으며, 해당 데이터를 Reports &amp; Analytics, Report Builder 및 AdHoc Analysis 기능의 보고서에 사용할 수 있습니다.

**Dynamic Tag Manager:** Dynamic Tag Manager를 사용하여 검색, 소셜 및 디스플레이 광고 랜딩 페이지에 대한 서드파티 추적 태그 및 [광고 픽셀 기반 전환 추적 태그를 만들 수 있습니다.](https://experienceleague.adobe.com/docs/experience-platform/tags/home.html?lang=en) (또한 [!DNL Advertising] 태그를 직접 [!DNL Advertising] 내에서 만들 수 있습니다.)

**Experience Cloud Audiences:** (디스플레이 관리 부서가 있는 광고주) [Adobe Experience Cloud Audiences](audience-library.md) 를 디스플레이 광고 대상으로 사용할 수 있습니다. Experience Cloud에서 만든 대상과 Adobe Experience Cloud에 게시한 Analytics의 대상을 자동으로 사용할 수 있습니다. [!DNL Adobe Advertising] 계정이 이를 허용하도록 구성된 경우 Audience Manager의 대상을 사용할 수도 있습니다. Adobe Experience Cloud, 프로필 및 Audiences 액세스 관련 정보와 [!DNL Adobe Advertising] 및 Adobe Experience Cloud Audiences 사이의 초기 설정의 자세한 정보를 알아보려면 계정 관리자에게 문의하십시오. **참고:** Adobe Target도 사용하는 경우 Adobe Experience Cloud에 게시한 모든 Audiences를 Adobe Target의 활동에도 사용할 수 있습니다.

**Experience Cloud Assets:** (디스플레이 관리 부서가 있는 광고주) 새 디스플레이 Beta 보기를 사용하여 Adobe Experience Cloud Assets를 디스플레이 광고를 위한 크리에이티브 기능으로 사용할 수 있습니다. Adobe Experience Cloud 에셋에 액세스하려면 [Adobe Experience Cloud를 통해 Adobe Advertising에 로그인해야 합니다.](https://enterprise-test.efrontier.com/CMDashboard?ticket=JrciD7q2bF1y2mDWFHmEyoBomG0VowpcEgK5zzKFq3mDArroL6xIS3XkmJFZMeeXlj0uIZz-IEcOn3nVHmy9bwdSxEcDv6FMvTkjwz5rpIs%3D&amp;ticket=JrciD7q2bF1y2mDWFHmEykzc2nFNvATOY54xOo03rW0GSLGdEpu5MvttCo6msEyImNVq7_lmlTup-LwCdnPIHA7mJrhugFMnbqTmSB-dfmw%3D) Adobe Experience Cloud 액세스 관련 정보를 자세히 알아보려면 계정 관리자에게 문의하십시오.

**Experience Cloud 알림:** 각 페이지 상단의 알림 링크에서 검색 Beta 경고 템플릿에서 생성된 모든 경고를 볼 수 있습니다. Experience Cloud 시스템 업데이트, 게시물, 멘션, 공유된 에셋 받기도 가능합니다. 알림에 액세스하려면 [Adobe Experience Cloud를 통해 Adobe Advertising에 로그인](https://enterprise-test.efrontier.com/CMDashboard?ticket=JrciD7q2bF1y2mDWFHmEyoBomG0VowpcEgK5zzKFq3mDArroL6xIS3XkmJFZMeeXlj0uIZz-IEcOn3nVHmy9bwdSxEcDv6FMvTkjwz5rpIs%3D&amp;ticket=JrciD7q2bF1y2mDWFHmEykzc2nFNvATOY54xOo03rW0GSLGdEpu5MvttCo6msEyImNVq7_lmlTup-LwCdnPIHA7mJrhugFMnbqTmSB-dfmw%3D)해야 합니다. Adobe Experience Cloud 액세스 관련 정보를 자세히 알아보려면 계정 관리자에게 문의하십시오.
