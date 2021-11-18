---
description: Analytics Premium으로 업그레이드할 때의 요구 사항과 예상되는 사항에 대해 알아봅니다.
keywords: Adobe Analytics Premium 업그레이드
solution: Experience Cloud
title: 'Analytics Premium 및 Experience Cloud로 업그레이드 '
topic: Administration
uuid: 450a601c-d199-4e90-b525-19bd9f9576d2
feature: Admin Console
role: Admin
level: Experienced
exl-id: 746d396d-9629-42db-8c55-07d2d24e4611
source-git-commit: ae14748aa7b0f0d803d48fe980a6743f53d996ab
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 86%

---

# Analytics Premium 및 Experience Cloud로 업그레이드

관리자는 Analytics Premium으로 업그레이드할 때 요구 사항 및 예상 내용과 Experience Cloud 관리자로서 도움말을 찾을 위치에 대해 알아볼 수 있습니다.

## Analytics Premium {#section_7F50AD7906544F899B844BE31D3BB507}

Adobe Analytics Premium으로 업그레이드하면 Data Warehouse, Ad Hoc Analysis, Report Builder 및 Data Connectors를 포함하여, Analytics Standard에서 사용할 수 있는 모든 기능을 사용할 수 있습니다.

Analytics Premium을 사용하면 다음 항목을 사용할 수 있습니다.

* 250개의 전환 변수(eVar)에 대한 액세스
* [모바일 앱 분석](https://experienceleague.adobe.com/docs/mobile-services/using/home.html?lang=ko-KR)
* Data Workbench (시각적 데이터 쿼리, 규칙 기반 속성, 크로스 채널 분석)

>[!NOTE]
>
>업그레이드할 때에는 마이그레이션이 필요하지 않지만, 다음과 같이 알아야 할 고려 사항이 몇 가지 있습니다.
>
>* eVars 76-250 및 100-250(표준)은 관리 도구에 표시되지만 활성화되어 있지는 않습니다.
>* 기여도 분석은 Adobe에 의해 켜져 있습니다. 위치는 변경되지 않으며 Anomaly Detection 페이지에서 계속 사용할 수 있으나, 모든 데이터 포인트 분석을 자동으로 시작합니다.


## Analytics Premium Complete {#section_BFAD815EDF364845A52B340B2FD5B64C}

Analytics Premium Complete에서는 [Analytics Premium](upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507)의 모든 기능과 다음의 업그레이드를 사용할 수 있습니다.

| 제품 | 업그레이드 |
|--- |--- |
| Reports &amp; Analytics | <ul><li>[기여도 분석](https://experienceleague.adobe.com/docs/analytics/analyze/analysis-workspace/virtual-analyst/contribution-analysis/ca-tokens.html?lang=ko-KR)</li><li>[고객 속성](attributes.md#concept_ACFEE7C8B8E94875BA0825CDF4913AF1)(최대 200개)</li></ul> |
| Data Workbench | <ul><li>알고리즘 기여도 분석</li><li>사전 빌드된 작업 공간</li></ul> |
| Analytics Platform | [라이브 스트림](https://github.com/AdobeDocs/analytics-1.4-apis/blob/master/docs/live-stream-api/index.md)(원시 데이터, 대시보드, 트리거) |

{style=&quot;table-layout:auto&quot;}

## Predictive Intelligence {#section_B407932C07A7476F83FB0275C3FB63DC}

Predictive Intelligence로 업그레이드하면 [Analytics Premium](upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507)과 다음 기능이 활성화됩니다.

| 제품 | 업그레이드 |
|---|---|
| Reports &amp; Analytics | [기여도 분석](https://experienceleague.adobe.com/docs/analytics/analyze/analysis-workspace/virtual-analyst/contribution-analysis/ca-tokens.html?lang=en) |
| Data Workbench | 대상 자격 조건 및 예측 마케팅을 위해 사전 빌드된 작업 공간. |
| Analytics Platform | 라이브 스트림(대시보드 및 트리거) |

{style=&quot;table-layout:auto&quot;}

## Customer 360 {#section_3B2AC245388248688067DC9A48957AFB}

Customer 360으로 업그레이드하면 [Analytics Premium](upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507)과 다음 기능이 제공됩니다.

| 제품 | 업그레이드 |
|--- |--- |
| [고객 속성](attributes.md) | 고객 속성(분석 및 세그먼트 공유) |
| Data Workbench | <ul><li>파생된 고객 속성</li><li>대상 검색을 위해 사전 빌드된 작업 공간</li></ul> |
| Analytics Platform | [고객 속성](attributes.md) |

{style=&quot;table-layout:auto&quot;}

## Advanced Attribution {#section_9E4986A8389946CCAA7D003268343296}

고급 기여도 분석에서는 [Analytics Premium](upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507)에 대한 액세스 권한과 Data Workbench에 있는 알고리즘 기여도 분석이 제공됩니다(25% 서버 호출 볼륨).

## Data Workbench 요구 사항 {#section_D959CA68D6DB42C38707F8E0CA3654CC}

지원되는 사용자는 `dwb@adobe.com`으로 이메일을 보내어 모든 클라이언트 라이선스를 Premium을 반영하도록 업데이트하라고 요청할 수 있습니다. 이 업데이트는 알고리즘 기여도와 같은 기능을 활성화합니다.

TechOps에서는 계약 약정을 검토하고 적절한 관리 인프라의 용량을 늘릴지 줄일지를 결정한 다음, 계정 관리자나 컨설팅을 통해 여러분과 조정하여 모든 변경 사항을 배포하게 됩니다.

온프레미스에서 실행되는 모든 소프트웨어는 비활성화해야 합니다. 이 소프트웨어에는 센서가 포함되어 있으므로 [!DNL Analytics] 태그를 통해 적절한 추적을 보장해야 합니다.

## Experience Cloud - 사용자 및 제품 관리 {#section_6471C54454024301B2E0B687F79F6738}

에 설명된 구현 현대화에 따를 경우 Analytics Standard 및 Premium 사용자는 Experience Cloud 및 핵심 서비스를 사용할 수 있습니다. [시작하기 - 핵심 서비스용 애플리케이션 활성화](core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C). (해당 프로세스는 구현을 현대화하는 데 도움이 되며, Experience Cloud에서 관리자가 될 수 있도록 해 줍니다.)

Experience Cloud에 참여하면 [!DNL experience.adobe.com]의 Experience Cloud를 통해 로그인하고 핵심 서비스(고객 속성, 대상 및 모바일 앱 분석 등)를 사용할 수 있습니다.

### 사용자 및 그룹 관리

사용자 관리는 [Adobe Admin Console](https://helpx.adobe.com/kr/enterprise/using/admin-console.html)(제품 링크)에서 수행됩니다.

Adobe Admin Console에서 만든 그룹과 솔루션 그룹(예: Adobe Analytics) 간에 1:1 매핑을 설정할 수 있습니다. 그런 다음 매핑된 Admin Console 그룹에 추가된 새 사용자에게는 자동으로 생성되고 사용자의 Adobe ID에 연결된 Analytics 애플리케이션 계정이 있습니다. (기존 사용자는 Experience Cloud 로그인을 통해 응용 프로그램에 액세스하려면 해당 응용 프로그램 계정 자격 증명을 수동으로 연결해야 합니다.)

>[!NOTE]
>
>여러 응용 프로그램 그룹을 하나의 Admin Console 그룹에 매핑할 수 있습니다. 하지만 1:1 매핑이 권장됩니다. 예정보다 빨리 그룹을 매핑하면 CSV를 업로드함으로써 사용자를 초대하고, 만들고, 권한을 부여하고, 여러 사용자를 추가할 수 있습니다.
