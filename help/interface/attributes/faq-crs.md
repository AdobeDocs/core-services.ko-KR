---
description: Analytics 및 Target의 고객 속성에 대한 FAQ 및 우수 사례입니다.
keywords: Customer Attributes
seo-description: Analytics 및 Target의 고객 속성에 대한 FAQ 및 우수 사례입니다.
seo-title: FAQ, 제한 사항 및 우수 사례
solution: Experience Cloud
title: FAQ, 제한 사항 및 우수 사례
uuid: e93eb531-23c7-4d75-92e8-75699f58546a
translation-type: tm+mt
source-git-commit: 0bc7032d0052ba03beac1140dfbfd630e1802bfd
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# FAQ, 제한 사항 및 우수 사례

Analytics 및 Target의 고객 속성에 대한 FAQ 및 우수 사례입니다.

## 모범 사례 및 제한 사항 {#section_7F5189B3DAA84EE6865B91D2026EE05A}

고객 속성 사용 시 [!UICONTROL 안내 및 제한 사항].

| 문제 | 설명 |
|--- |--- |
| [!UICONTROL 고객 속성] 구독 제한 | Analytics Premium으로 업그레이드하면 추가 속성을 사용할 수 있기 전에 24시간 지연이 발생합니다. 이 시간 중에 속성 가입 최대값 오류가 표시될 수 있습니다. |
| 동일한 장치에 여러 로그인 | 고객 속성을 사용하여 고객 프로파일을 데이터 소스에 업로드할 때 동일한 장치(즉, 동일한 Experience Cloud ID)를 공유하는 사용자가 권장됩니다. 이렇게 하면 장치에서 지속되는 ECID 서비스가 동일한 Experience Cloud ID 아래에 여러 사용자를 연결하여 예기치 않은 결과가 발생할 수 있습니다 [!DNL Target]. **참고:** Mobile의 경우 ECID는 모바일 앱이 설치된 후에 영구적이며, 앱을 다시 설치하여 새로운 ECID를 생성해야 합니다. 웹의 경우, 브라우저 쿠키가 지워진 후 새 ECID가 생성됩니다. |
| 일별 빈도 업로드 제한 | 고객 속성을 하루에 한 번만 업데이트하는 것이 좋습니다. 동일한 프로필 세트에 대해 다른 고객 프로필 데이터 파일을 업로드하려면 최소 24시간을 기다려야 합니다. |
| 사용자 지정 분석 ID(`s.visitorID`) | `s.visitorID`를 사용하여 고객 ID를 설정하는 것은 Analytics에서 사용자를 식별하는 방법입니다. 그러나 ID 서비스를 사용하여 Analytics 데이터를 내보내거나 가져오는 통합은 방문자가 식별될 때 작동하지 않습니다. 여기에는 공유 대상, Adobe Target(A4T)용 `s.visitorID.`<br>Analytics 및 고객 속성이 포함되지만 이에 국한되지 않습니다.<br>이러한 통합의 경우 사용자 지정 Analytics ID를 설정할 수 없습니다. |
| Analytics의 문자 길이 제한 | Analytics 구독을 만들 때 업로드된 파일의 필드 길이가 255로 잘립니다. |

## 고객 속성에 대한 FAQ {#section_E47866EEA83348E09FE43CEC5E44C461}

| 질문 | 답변 |
|--- |--- |
| 고객 속성에 대한 업로드 상태에 대한 알림을 받을 수 있습니까? | 예. [알림 관리](https://docs.adobe.com/content/help/en/core-services/interface/manage-users-and-products/organizations.html#concept_0105453AD71847B8BFCAF4A40915F157)를 참조하십시오. |
| 고객 속성을 시작하려면 어떻게 해야 합니까? | <ol><li>프로비전됩니다. Analytics 고객인 경우 Adobe에서 고객 속성에 대해 제공합니다. Adobe Target만 사용하고 Analytics가 없는 경우 고객 지원 센터에 연락하여 핵심 서비스에 대한 제공을 요청해야 합니다.</li> <li>CRM 팀과 대화합니다. Analytics 및 Experience Cloud 전체에서 사용할 수 있는 고객 데이터의 종류를 확인하십시오.</li><li>핵심 서비스 구현 구현을 현대화하는 [방법에 대한 단계는 핵심 서비스용](https://docs.adobe.com/content/help/ko-KR/core-services/interface/about-core-services/core-services.html) 솔루션 활성화를 참조하십시오. 자세한 내용은 고객 ID 동기화에 대한 섹션을 참조하십시오.</li></ol> **참고:** 핵심 서비스 구현에 대한 관리자의 FAQ는 [여기에서 확인할 수 있습니다](https://docs.adobe.com/content/help/en/core-services/interface/manage-users-and-products/faq.html#concept_13219B4E51784577B6FF78AAA203DE91). |
| 몇 개의 고객 속성을 사용할 수 있습니까? | You can upload hundreds of `.csv` columns to the customer attribute service. 그러나 구독을 구성하고 속성을 선택할 때 소유한 솔루션에 따라 보고서 세트당 다음 제한이 적용됩니다.  <ul><li>Foundation: 0개</li><li>Select: 3개</li><li>Prime: 15개</li><li>Ultimate: 200개</li><li>Standard: 총 3개</li><li>Premium: 200년</li><li>Adobe Target Standard: 5</li><li>Adobe Target Premium: 200년</li></ul> |
| Experience Cloud ID 서비스로 마이그레이션해야 합니까? | 마이그레이션은 사용하는 솔루션에 따라 다릅니다. <ul><li>Adobe Analytics:  적극 권장 </li><li>Adobe Target: 필수. </li></ul><br> ID 서비스를 사용하면 실시간 대상, Adobe Target 현대화, Analytics 통합 및 비디오 하트비트 추적 등 최신 Experience Cloud 기능을 사용할 수 있습니다. <br> 자세한 내용은 핵심 서비스용 솔루션 [활성화를 참조하십시오](https://docs.adobe.com/content/help/ko-KR/core-services/interface/about-core-services/core-services.html). <br>** 참고:** [Experience Cloud ID 서비스](https://docs.adobe.com/content/help/ko-KR/id-service/using/intro/overview.html) 는 이전에 _Analytics 방문자 ID 서비스로 알려진 최신 구현을 위한 것입니다._ |
| 고객 속성 기능은 Adobe Audience Manager와 어떤 관련이 있습니까? | Audience Manager는 데이터를 수신하여 대상을 식별할 수 있지만, 특성을 이전 행동 데이터와 연결하는 분석 기능을 수행하거나 Adobe Analytics에서 사용할 수 있는 보고, 분석 및 세그멘테이션 기능을 제공할 수 없습니다. [!UICONTROL 여러 솔루션에서 얻은 풍부한 데이터를 결합하여 Experience] Cloud에서 사용할 수 있는 단일 ID와 연결할 수 있습니다. <br>Adobe Target에서 고객 속성은 다른 규칙과 결합하여 대상을 만들 수 있는 개별 속성으로 표시됩니다. 사람 서비스에 공유된 [!UICONTROL 대상은] 수정할 수 없는 전체 대상입니다. |
| **(Analytics 전용)** 이 기능은 Analytics Premium에 제공된 기능과 어떻게 다릅니까? | 이전에는 고객 속성 데이터를 Analytics 데이터와 결합하려는 고객은 이 기능을 위해 데이터 워크벤치 도구에 많이 의존했습니다. 고객 속성은 고객 속성을 보고서 및 분석, 애드혹 분석 및 리포트 빌더에서 차원 및 지표로 제공하여 더 많은 사용자에게 이 기능을 노출합니다. Analytics Standard 고객은 고객 속성에 액세스할 수 있지만 제한된 기능을 사용할 수 있습니다. Analytics Premium 고객은 전체 기능을 사용할 수 있습니다. |
| **(Adobe Target만 해당)** Adobe Target에서 보지 못한 고객을 위해 데이터를 미리 로드하거나 업로드할 수 있습니까? | 예. 방문자가 Adobe Target에 처음으로 요청을 하면 시스템은 고객 속성에서 기존 정보에 대한 정보를 가져오고 해당 데이터를 사용하여 타깃팅합니다. **참고:**  이 데이터를 검색하는 데 방문자가 Adobe Target과의 첫 상호 작용에서 최대 20분이 소요될 수 있습니다. |
| **(Adobe Target만 해당)** 고객 속성 데이터를 공유 대상 데이터와 결합하여 수퍼 대상을 만들 수 있습니까? | 아니요. 공유 대상 데이터는 완료된 대상입니다. |
| **(Adobe Target에만 해당)** 고객 속성 기능은 Adobe Target의 벌크 프로필 API와 어떻게 비교합니까? | 벌크 프로필 API를 사용하면 개별 프로필 또는 일괄 API를 통해 Adobe Target 프로필을 직접 업데이트할 수 있습니다. 이 기능은 고객 속성과 유사하며 다음과 같은 주요 차이점이 있습니다.<ul><li>프로필 API는 REST API 호출이고 고객 속성은 FTP를 사용합니다.</li><li>Adobe Target의 프로필 API는 전체 Experience Cloud가 아닌 Adobe Target으로만 데이터를 보냅니다.</li><li>고객 속성은 이 외부 데이터를 만들고 관리하는 간단한 인터페이스를 제공합니다.</li></ul> |
| **(Adobe Target에만 해당)** 고객 속성에서 Adobe Target으로 데이터를 업로드하면 Adobe Target 방문자의 프로필 라이프타임이 연장됩니까? | 예. Adobe Target 도움말의 [방문자 프로필 라이프타임](https://docs.adobe.com/content/help/en/target/using/audiences/visitor-profiles/visitor-profile.html)을 참조하십시오. |
| **(Adobe Target만 해당)** 방문자가 고객 ID로 식별된 직후 고객 속성에 업로드된 데이터를 타깃팅할 수 있습니까? | 예. mbox 타사 ID가 포함된 Adobe Target에 대한 서버 호출에서 모든 고객 속성 데이터를 사용할 수 있습니다. |
| **(Adobe Target만 해당)** [ **[!UICONTROL 동기화 상태]** ] 열은 고객 속성 소스에 업로드된 파일에 대해 무엇을 나타냅니까? | 특정 속성 파일에서 상태 동기화 아이콘을 클릭하여 Adobe Target에 게시되고 동기화된 레코드 수를 볼 수 있습니다. `Sync %` 는 Adobe Target에서 동기화된 프로파일의 비율을 지정하는 실시간 지표입니다.<br> **참고:** 속성이 Adobe Target과 동기화되려면 최대 24시간이 걸릴 수 있습니다. |
| 고객 속성 소스에서 파일 업로드 지표가 나타내는 것은 무엇입니까? | 다음 지표의 도움을 받아 고객 속성에 업로드된 속성의 상태를 확인할 수 있습니다. <ul><li>레코드:  속성 파일에 있는 레코드 수입니다.</li><li>**새 레코드:** 속성 파일에 있는 새 레코드 수입니다.</li> <li>**업데이트된 레코드:** 파일에서 업데이트된 값이 있는 고객 속성에 이미 존재하는 레코드 수입니다.</li><li>**모든 데이터(레코드):** 고객 속성에 성공적으로 업로드된 총 레코드 수입니다.</li></ul> |
