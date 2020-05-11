---
description: 관리자는 Analytics Premium으로 업그레이드할 때 요구 사항 및 예상 내용과 Experience Cloud 관리자로서 도움말을 찾을 위치에 대해 알아볼 수 있습니다.
keywords: upgrading
seo-description: 관리자는 Analytics Premium으로 업그레이드할 때 요구 사항 및 예상 내용과 Experience Cloud 관리자로서 도움말을 찾을 위치에 대해 알아볼 수 있습니다.
seo-title: Analytics Premium 및 Experience Cloud로 업그레이드
solution: Experience Cloud
title: Analytics Premium 및 Experience Cloud로 업그레이드
topic: Premium
uuid: 450a601c-d199-4e90-b525-19bd9f9576d2
translation-type: tm+mt
source-git-commit: 0bc7032d0052ba03beac1140dfbfd630e1802bfd
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Analytics Premium 및 Experience Cloud로 업그레이드

관리자는 Analytics Premium으로 업그레이드할 때 요구 사항 및 예상 내용과 Experience Cloud 관리자로서 도움말을 찾을 위치에 대해 알아볼 수 있습니다.

## Analytics Premium {#section_7F50AD7906544F899B844BE31D3BB507}

Adobe Analytics Premium으로 업그레이드하면 데이터 웨어하우스, 애드혹 분석, 리포트 빌더 및 데이터 커넥터를 포함하여 Analytics Standard에서 사용할 수 있는 모든 기능 또는 제품을 제공합니다. (이러한 제품은 포인트 솔루션인 SiteCatalyst를 사용하여 고객에게 별도로 판매되었습니다.)

Analytics Premium은 다음과 같은 이점을 제공합니다.

* 250개의 전환 변수(eVar)에 액세스
* [모바일 앱 분석](https://docs.adobe.com/content/help/ko-KR/mobile-services/using/home.html)
* Data Workbench (시각적 데이터 쿼리, 규칙 기반 특성, 크로스 채널 분석)

>[!NOTE]
>
>업그레이드할 때는 마이그레이션이 필요하지 않지만 다음 사항을 고려해야 합니다.
>
>* eVar 76-250(SiteCatalyst) 및 100-250(표준)은 관리 도구에서 볼 수 있지만, 아직 활성화되지 않습니다.>
>* 기여도 분석은 Adobe에서 설정합니다. 위치(예외 항목 탐지 페이지에서 계속 사용 가능)는 변경되지 않지만 이제 모든 데이터 포인트 분석을 자동으로 시작합니다.>


## Analytics Premium Complete {#section_BFAD815EDF364845A52B340B2FD5B64C}

Analytics Premium Complete에서는 [Analytics Premium](../admin-getting-started/upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507)의 모든 기능과 다음 업그레이드를 이용할 수 있습니다.

| 제품 | 업그레이드 |
|--- |--- |
| Reports &amp; Analytics | <ul><li>[기여도 분석](https://docs.adobe.com/content/help/ko-KR/analytics/analyze/analysis-workspace/virtual-analyst/contribution-analysis/ca-tokens.html)</li><li>[고객 속성](../attributes/attributes.md#concept_ACFEE7C8B8E94875BA0825CDF4913AF1)(최대 200개)</li></ul> |
| Data Workbench | <ul><li>알고리즘 속성</li><li>사전 구성된 작업 영역</li></ul> |
| Analytics Platform | [라이브 스트림](https://helpx.adobe.com/analytics/kb/getting-started-with-livestream-api.html) (원시 데이터, 대시보드, 트리거) |

## Predictive Intelligence {#section_B407932C07A7476F83FB0275C3FB63DC}

예측 인텔리전스로 업그레이드하면 [Analytics Premium](../admin-getting-started/upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507) 과 다음을 사용할 수 있습니다.

| 제품 | 업그레이드 |
|---|---|
| Reports &amp; Analytics | [기여도 분석](https://docs.adobe.com/content/help/ko-KR/analytics/analyze/analysis-workspace/virtual-analyst/contribution-analysis/ca-tokens.html) |
| Data Workbench | 고객 자격 조건 및 예측 마케팅을 위한 사전 구축된 작업 영역 |
| Analytics Platform | 라이브 스트림(대시보드 및 트리거) |

## 고객 360 {#section_3B2AC245388248688067DC9A48957AFB}

고객 360으로 업그레이드하면 [Analytics Premium](../admin-getting-started/upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507) 과 다음을 제공합니다.

| 제품 | 업그레이드 |
|--- |--- |
| [고객 속성](../attributes/attributes.md) | 고객 속성(분석 및 세그먼트 공유) |
| Data Workbench | <ul><li>파생된 고객 속성</li><li>고객 확보를 위한 사전 구축된 작업 영역</li></ul> |
| Analytics Platform | [고객 속성](../attributes/attributes.md) |

## Advanced Attribution {#section_9E4986A8389946CCAA7D003268343296}

고급 기여도 분석은 데이터 워크벤치의 [Analytics Premium](../admin-getting-started/upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507)및 알고리즘 속성에 대한 액세스 권한을 제공합니다(25% 서버 호출 볼륨).

## 데이터 워크벤치 요구 사항 {#section_D959CA68D6DB42C38707F8E0CA3654CC}

지원되는 사용자는 `dwb@adobe.com`으로 이메일을 보내어 모든 클라이언트 라이센스를 Premium을 반영하도록 업데이트하라고 요청할 수 있습니다. 이렇게 하면 알고리즘 속성과 같은 기능이 활성화됩니다.

TechOps는 계약 약정을 검토하고 적절한 관리 인프라의 용량을 늘이거나 줄인 다음 계정 관리자나 컨설팅을 통해 모든 변경 사항을 배포합니다.

온-프레미스에서 실행되는 모든 소프트웨어는 비활성화되어야 합니다. 여기에는 Sensors가 포함되어 있으므로 Analytics 태그를 통해 적절한 추적을 해야 합니다.

## Experience Cloud - 사용자 및 제품 관리 {#section_6471C54454024301B2E0B687F79F6738}

[시작하기 - 핵심 서비스용 솔루션을 사용하도록 설정](../core-services/core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C)에 설명된 구현 현대화에 따를 경우 Analytics Standard 및 Premium 사용자는 Experience Cloud와 핵심 서비스를 이용할 수 있습니다. (해당 프로세스는 구현을 현대화하는 데 도움이 되며, Experience Cloud에서 관리자가 될 수 있도록 해줍니다.)

After you join the Experience Cloud, you can log in via the Experience Cloud at [!DNL experiencecloud.adobe.com] and begin using core services (including Customer Attributes, Audiences, and Mobile app analytics).

### 사용자 및 그룹 관리

사용자 관리는 [Adobe Admin Console](https://helpx.adobe.com/enterprise/help/aedash.html) (제품 링크)에서 수행됩니다.

Adobe 관리 콘솔에서 만든 그룹과 솔루션 그룹(예: Adobe Analytics) 간에 1:1 맵을 설정할 수 있습니다. 그 후에 매핑된 관리 콘솔 그룹에 추가된 새 사용자는 자동으로 만들어져 사용자의 Adobe ID에 연결된 Analytics 솔루션 계정을 갖게 됩니다. (기존 사용자는 Experience Cloud 로그인을 통해 솔루션에 액세스하려면 솔루션 계정 자격 증명을 수동으로 연결해야 합니다.)

>[!NOTE]
>
>여러 솔루션 그룹을 하나의 Admin Console 그룹에 매핑할 수 있습니다. 그러나 1:1 매핑이 권장됩니다. 미리 그룹을 매핑하면 CSV를 업로드하여 여러 사용자를 초대하고, 만들고, 권한을 부여하고, 추가할 수 있습니다.
