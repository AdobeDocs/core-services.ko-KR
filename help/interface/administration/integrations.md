---
description: Adobe CX Enterprise에서 사용 가능한 애플리케이션 통합 찾기
solution: Experience Cloud
title: Experience Cloud 통합
uuid: a9893c6b-bccc-4fb5-b724-724644c7def5
feature: Admin Console
topic: Administration
role: Admin
level: Experienced
exl-id: 7f8fa610-32f0-4b18-8054-3ba05436a10e
TQID: https://experienceleague.adobe.com/6Sh6sOZ--ct2sz5sMR-qRwZmvoC51zQkV9LqVRXmi-o
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
feature_v2:
  - id: dab36b01-8bfa-48f3-8392-626455a058e6
  - id: fc7979f3-56c3-43ca-9784-f1ea3dc69c4b
  - id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
subfeature_v2:
  - id: b75843fa-0a67-4a44-a6b1-cc627b0481dc
  - id: d27b1945-f442-4607-91bd-537a0b16e687
  - id: ecb4a972-6786-444c-a014-abc528b9407a
  - id: fef08361-6ac5-460c-93fe-d063e40b6a49
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1
  - id: d3cdead0-685a-4489-9250-4bb709942f66
  - id: df401a2a-327d-468c-a5e4-b7b7ccd071a0
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 7bfc22e90d727d1743c2b6b7bc645033d5d38f1b
workflow-type: tm+mt
source-wordcount: 1113
ht-degree: 31%

---

# CX 엔터프라이즈 통합

이 페이지에서는 CX 엔터프라이즈 애플리케이션 통합을 시작하는 몇 가지 방법에 대해 설명합니다. 자세한 내용은 Experience League에서 [통합 비디오 튜토리얼](https://experienceleague.adobe.com/docs/experience-platform/tags/home.html?lang=ko) 라이브러리를 검색하십시오.

## 플랫폼 서비스용 CX 엔터프라이즈 애플리케이션 활성화

다음 방법을 설명합니다.

* CX Enterprise에서 회사 프로비저닝.
* 관리자가 될 수 있도록 설정.
* [방문자 ID 서비스 구현](https://experienceleague.adobe.com/docs/id-service/using/home.html?lang=ko).
* [!UICONTROL Platform 데이터 수집]을 통해 [!DNL Analytics] 및 [!DNL Target] 구현을 현대화하십시오.
* [고객 특성](../services/customer-attributes/attributes.md) 및 [대상 라이브러리](../services/audiences/overview.md)와 같은 CX 엔터프라이즈 서비스를 사용하십시오.

솔루션 또는 서비스:

* [[!DNL Experience Platform Data Collection]](https://experienceleague.adobe.com/docs/experience-platform.html?lang=ko)
* [[!DNL Analytics]](https://experienceleague.adobe.com/docs/analytics.html?lang=ko)
* [[!DNL Target]](https://experienceleague.adobe.com/docs/target.html?lang=ko)
* [방문자 ID 서비스](https://experienceleague.adobe.com/docs/id-service/using/home.html?lang=ko)

## 방문자 ID 서비스

방문자 ID 서비스는 CX Enterprise의 모든 애플리케이션에서 방문자를 식별하는 범용 영구 ID를 제공합니다. Analytics, Audience Manager, Adobe Target, 비디오 하트비트 및 기타 CX 엔터프라이즈 애플리케이션 및 제품과 같은 서비스에 대한 ID 생성 코드를 대체할 수 있습니다.

[방문자 ID 서비스](https://experienceleague.adobe.com/docs/id-service/using/home.html?lang=ko) 보기

**해당 애플리케이션 또는 서비스**

* [Adobe Analytics](https://experienceleague.adobe.com/ko/docs/analytics/implementation/id/overview)
* [Adobe Target](https://experienceleague.adobe.com/ko/docs/id-service/using/implementation/setup-target)

## 대상자

도움말: [Audiences](/help/interface/services/audiences/overview.md)

CX Enterprise [!UICONTROL 대상 라이브러리]에서 대상을 만들고 관리합니다. 다음과 같은 다양한 소스에서 대상자를 만들거나 파생할 수 있습니다.

* [!DNL CX Enterprise]에서 만든 새 항목.
* [!DNL Analytics]개 세그먼트가 [!DNL CX Enterprise]에 게시되었습니다.
* From [!DNL Audience Manager].

**해당 솔루션 또는 서비스**

* [Adobe Target의 활동](https://experienceleague.adobe.com/docs/target/using/activities/activities.html?lang=ko)
* Audience Manager의 [세분화](https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/audience-analytics-workflow/aam-analytics-segments.html?lang=ko)
* [Advertising Cloud](https://enterprise.efrontier.com/CMDashboard/?ticket=JrciD7q2bF1y2mDWFHmEyibbOnNwb2JBRF7z6tKAOIWkBimlPxCUaZyJnPLqsfdqsf3fpxWoxGasvatKA8S6-h4tlDvxQcm8Gc10dSF9q_E%3D&ticket=JrciD7q2bF1y2mDWFHmEyibmxtHqnZFSOMml-n993zOBc-ovZGNZkX5vgePWqKNMoMmPSqf9PkzFeYF4UN6GqSXDVNDvwgnvv9KT8PvVxk8%3D)&#x200B;(로그인 필요)

## 고객 속성

도움말: [고객 속성](/help/interface/services/customer-attributes/attributes.md)

CRM(고객 관계 관리) 데이터베이스에서 엔터프라이즈 고객 데이터를 캡처하는 경우, 이 데이터를 CX Enterprise의 고객 속성 데이터 소스에 업로드할 수 있습니다. 업로드한 후에는 [!DNL Adobe Analytics] 및 [!DNL Adobe Target]의 데이터를 사용합니다.

**해당 솔루션 또는 서비스**

* Adobe Analytics: 고객 속성 보고서
* Adobe Target: 고객 특성을 사용하도록 Adobe Target의 [구독](/help/interface/services/customer-attributes/subscription.md)을 구성하십시오.

## CX Enterprise 에셋

도움말: [Creative Cloud과 CX 엔터프라이즈 폴더 공유](/help/interface/services/assets/share.md)

CX Enterprise와 Creative Cloud 간에 폴더 및 에셋을 공유합니다. 공유 에셋에 공동 작업을 수행하고, 주석을 달고, Adobe Target과 같은 CX 엔터프라이즈 애플리케이션에서 사용합니다.

**해당 애플리케이션 또는 서비스**

* Adobe CX 엔터프라이즈
* Adobe Creative Cloud
* Adobe Target

## Analytics - Analytics의 AEM Assets 보고

도움말: [Analytics의 AEM Assets 보고](https://experienceleague.adobe.com/docs/analytics/integration/aem-assets-reporting.html?lang=ko)

Analytics에서 AEM 에셋 인사이트에서 제공된 에셋에 대한 노출 횟수 및 클릭 수를 수집할 수 있습니다.

**해당 애플리케이션 또는 서비스**

* [!DNL Analytics]
* [!DNL Experience Manager]

## Audience Manager 통합

[Audience Manager](https://experienceleague.adobe.com/docs/audience-manager/user-guide/implementation-integration-guides/implementation-and-integration.html?lang=ko)

CX 엔터프라이즈 애플리케이션이나 Audience Manager의 기타 외부 시스템의 데이터로 작업합니다.

**해당 애플리케이션 또는 서비스**

* [Analytics 서버측 전달](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/server-side-forwarding/ssf.html?lang=ko-KR)
* [Analytics에 Audience Manager 세그먼트 보내기](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/destinations/experience-cloud-destinations/create-analytics-destination.html?lang=ko)
* [Adobe Target 데이터 통합](https://experienceleague.adobe.com/docs/audience-manager/user-guide/implementation-integration-guides/integration-other-applications/aam-target-integration.html?lang=ko)

## Adobe Target

도움말: [Adobe Target과 CX Enterprise 통합](/help/interface/services/audiences/overview.md)

Adobe Target을 Adobe Analytics 및 기타 CX 엔터프라이즈 애플리케이션과 통합하여 두 애플리케이션에서 동일한 데이터, 대상, 속성 및 지표를 사용할 수 있도록 합니다.

**해당 애플리케이션 또는 서비스**

* 고객 속성: 고객 속성에 대한 Adobe Target의 [구독](/help/interface/services/customer-attributes/subscription.md) 구성
* CX 엔터프라이즈 대상: [CX 엔터프라이즈 대상 라이브러리](/help/interface/services/audiences/overview.md)
* Analytics: [Adobe Target용 보고 소스 Adobe Analytics](https://experienceleague.adobe.com/docs/target/using/integrate/a4t/a4t.html?lang=ko)
* Audience Manager: [Adobe Audience Manager와 Adobe Target 데이터 통합](https://experienceleague.adobe.com/docs/audience-manager/user-guide/implementation-integration-guides/integration-other-solutions/aam-target-integration.html?lang=ko)
* Campaign: [Adobe Target과 Campaign 통합](https://experienceleague.adobe.com/docs/target/using/integrate/campaign-and-target.html?lang=ko)

## Experience Manager 통합

* 비디오 자습서: [Experience Manager 통합](https://experienceleague.adobe.com/docs/integrations-learn/experience-cloud/integrations-between-applications/overview.html?lang=ko)

* 제품 설명서: [Experience Manager 설명서](https://experienceleague.adobe.com/docs/experience-manager-cloud-service.html?lang=ko)

## Experience Manager - Assets

도움말: [CX Enterprise 및 Creative Cloud과 AEM Assets 통합 구성](https://experienceleague.adobe.com/docs/?lang=ko)

AEM(Adobe Experience Manager) 에셋 내의 에셋을 Adobe Creative Cloud와 동기화하거나 그 반대로 동기화합니다. 자산을 CX Enterprise 와 동기화하거나 그 반대로 동기화할 수 있습니다. CX Enterprise 를 통해 이 동기화를 설정할 수 있습니다.

**해당 애플리케이션 또는 서비스**

* AEM
* Creative Cloud
* [CX Enterprise](https://experienceleague.adobe.com/docs/?lang=ko)

## [!DNL Adobe Advertising]

* 도움말(로그인 필요): [Adobe CX 엔터프라이즈 솔루션 및 서비스와 통합](https://enterprise.efrontier.com/CMDashboard?ticket=JrciD7q2bF1y2mDWFHmEyhyMKZp71ZLeaANvF-RcNMF7oNuZNABh76cKJLNlJJeJ1hQ5vAW1AO1t1DW8tZWM3lYZ8TSh96YAQISUdtHCCgA%3D&ticket=JrciD7q2bF1y2mDWFHmEyibbOnNwb2JBRF7z6tKAOIWkBimlPxCUaZyJnPLqsfdqsf3fpxWoxGasvatKA8S6-h4tlDvxQcm8Gc10dSF9q_E%3D)

* Experience League의 [Adobe Advertising 설명서](https://experienceleague.adobe.com/docs/advertising.html?lang=ko)

**해당 애플리케이션 또는 서비스**

**Analytics:** 사이트 참여 및 전환 데이터를 매일 [!DNL Adobe Advertising]에 전송할 수 있습니다. 해당 데이터를 광고 최적화 및 보고에 사용할 수 있습니다. 또한 [!DNL Advertising]에서 매일 Analytics에 검색 엔진 및 소셜 네트워크 트래픽 데이터를 전송할 수 있으며, 해당 데이터를 Reports &amp; Analytics, Report Builder 및 AdHoc Analysis 기능의 보고서에 사용할 수 있습니다.

**태그:** 검색, 소셜 및 디스플레이 광고 랜딩 페이지에 대해 [Experience Platform 태그를 사용하여 Advertising 픽셀 기반 전환 추적 태그](https://experienceleague.adobe.com/docs/experience-platform/tags/home.html?lang=ko) 및 서드파티 추적 태그를 만들 수 있습니다. (또한 [!DNL Advertising] 태그를 직접 [!DNL Advertising] 내에서 만들 수 있습니다.)

**CX 엔터프라이즈 대상:**(디스플레이 관리 부서가 있는 광고주) [Adobe CX 엔터프라이즈 대상](../services/audiences/overview.md)을 디스플레이 광고 대상으로 사용할 수 있습니다. CX Enterprise에서 만든 대상과 CX Enterprise에 게시한 Analytics의 대상을 자동으로 사용할 수 있습니다. [!DNL Adobe Advertising] 계정이 이를 허용하도록 구성된 경우 Audience Manager의 대상을 사용할 수도 있습니다.

Adobe CX 엔터프라이즈, 프로필 및 대상에 대한 액세스와 [!DNL Adobe Advertising] 및 Adobe CX 엔터프라이즈 대상 간의 초기 설정에 대한 자세한 내용은 계정 관리자에게 문의하십시오. **참고:** Adobe Target도 사용하는 경우 Adobe CX Enterprise에 게시한 모든 대상을 Adobe Target의 활동에도 사용할 수 있습니다.

**CX 엔터프라이즈 Assets:**(디스플레이 관리 부서가 있는 광고주) 새 디스플레이 Beta 보기를 사용하여 Adobe CX 엔터프라이즈 자산을 디스플레이 광고를 위한 크리에이티브 기능으로 사용할 수 있습니다. Adobe CX Enterprise 에셋에 액세스하려면 [Adobe CX Enterprise를 통해 Adobe Advertising에 로그인](https://enterprise.efrontier.com/CMDashboard)해야 합니다. Adobe CX Enterprise 액세스에 대한 자세한 내용은 계정 관리자에게 문의하십시오.

**CX 엔터프라이즈 알림:** 각 페이지 상단의 알림 링크에서 검색 Beta 경고 템플릿에서 생성된 모든 경고를 볼 수 있습니다. 또한 CX 엔터프라이즈 시스템 업데이트, 게시물, 언급 및 공유된 에셋을 가져올 수 있습니다. 알림에 액세스하려면 [Adobe CX Enterprise를 통해 Adobe Advertising에 로그인](https://enterprise.efrontier.com/CMDashboard)해야 합니다. Adobe CX Enterprise 액세스에 대한 자세한 내용은 계정 관리자에게 문의하십시오.

