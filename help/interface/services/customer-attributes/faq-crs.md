---
description: Adobe Analytics 및 Adobe Target의 Adobe Experience Cloud [!DNL customer attributes] FAQ
solution: Experience Cloud
title: ' [!DNL customer attributes]에 대한 FAQ'
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 6031e544-822b-4843-b3d8-98a36a3c40e8
source-git-commit: 2f126877f6a5f090884ebe093f35e4f6d90b4df6
workflow-type: tm+mt
source-wordcount: '1033'
ht-degree: 81%

---

# [!DNL customer attributes]에 대한 FAQ

Adobe Analytics 및 Adobe Target의 [!DNL customer attributes] FAQ와 모범 사례

## 모범 사례 및 제한 사항 {#best_practices}

[!DNL customer attributes]를 사용할 때의 지침 및 제한 사항입니다.

| 문제 | 설명 |
|--- |--- |
| [!UICONTROL 고객 특성] 구독 제한 사항 | Analytics Premium으로 업그레이드할 때 더 많은 속성은 24시간 후에 사용할 수 있습니다. 이 시간 중에 [!UICONTROL 특성 구독 최대값] 오류가 표시될 수 있습니다. |
| 동일한 디바이스에 여러 로그인 | [!DNL customer attributes]를 사용하여 고객 프로필을 데이터 소스에 업로드할 때에는 디바이스(동일한 Experience Cloud ID)를 공유하는 사용자는 피하는 것이 좋습니다. Experience Cloud ID(ECID)는 디바이스에서 계속 유지됩니다. 디바이스를 공유하면 ECID가 여러 사용자를 동일한 ECID에 연결하여 예기치 않은 결과가 [!DNL Target]에 발생할 수 있습니다. **참고:** 모바일의 경우 ECID는 모바일 앱이 설치된 후에 영구적입니다. 새 ECID를 생성하려면 앱을 다시 설치해야 합니다. 웹의 경우, 브라우저 쿠키가 지워진 후 새 ECID가 생성됩니다. |
| 일일 업로드 빈도 제한 | [!DNL customer attributes]는 하루에 한 번만 업데이트하는 것이 좋습니다. 동일한 프로필 세트에 대해 다른 고객 프로필 데이터 파일을 업로드하려면 최소 24시간을 기다려야 합니다. |
| 사용자 정의 Analytics ID(`s.visitorID`) | `s.visitorID`을(를) 사용하여 고객 ID를 설정하는 것은 Adobe Analytics에서 사용자를 식별하는 방법입니다. 단, ID 서비스를 사용하여 [!DNL Analytics] 데이터를 내보내거나 가져오는 통합 기능은 방문자가 `s.visitorID.`<br>를 사용하여 식별될 때 작동하지 않습니다. 여기에는 공유 대상자, [!DNL Analytics] for Adobe Target(A4T) 및 [!DNL customer attributes]가 포함되지만 이에 국한되지 않습니다.<br>이러한 통합의 경우 사용자 정의 Analytics ID를 설정할 수 없습니다. |
| [!DNL Analytics]의 문자 길이 제한 | [!DNL Analytics] 구독을 생성할 때 업로드되는 파일의 필드 길이는 255자로 잘립니다. |

{style="table-layout:auto"}

## [!DNL customer attributes]에 대한 FAQ {#section_E47866EEA83348E09FE43CEC5E44C461}

| 질문 | 답변 |
|--- |--- |
| [!DNL customer attributes]와 관련된 업로드 상태에 대한 알림을 받을 수 있습니까? | 예. |
| [!DNL customer attributes] 사용을 시작하려면 어떤 작업을 수행해야 합니까? | <ol><li>프로비저닝을 받습니다. Adobe Analytics 고객인 경우 Adobe에서 [!DNL customer attributes]을(를) 프로비저닝하고 있습니다. Adobe Target만 사용하고 Analytics가 없는 경우 고객 지원 센터에 연락하여 핵심 서비스에 대한 프로비저닝을 요청합니다.</li> <li>CRM 팀과 대화합니다. Analytics 및 Experience Cloud 전체에서 사용하려는 고객 데이터 종류를 알아봅니다.</li><li>핵심 서비스 구현.</li></ol> |
| 사용할 수 있는 [!DNL customer attributes]는 몇 개입니까? | 수백 개의 `.csv` 열을 고객 속성 서비스에 업로드할 수 있습니다. 그렇지만 구독을 구성하고 속성을 선택할 때 보유하고 있는 애플리케이션에 따라 다음과 같은 제한이 (보고서 세트에 대해) 적용됩니다.  <ul><li>Foundation: 0개</li><li>Select: 3개</li><li>Prime: 15개</li><li>Ultimate: 200개</li><li>Standard: 총 3개</li><li>Premium: 200개</li><li>Adobe Target Standard: 5개</li><li>Adobe Target Premium: 200개</li></ul> |
| Experience Cloud ID 서비스로 마이그레이션해야 합니까? | 마이그레이션은 사용하는 애플리케이션에 따라 다릅니다. <ul><li>Adobe Analytics: 적극 권장 </li><li>Adobe Target: 필수. </li></ul><br>Experience Cloud ID 서비스를 사용하면 실시간 대상, Adobe Target 현대화, Analytics 통합 및 비디오 하트비트 추적을 비롯한 최신 Experience Cloud 기능을 사용할 수 있습니다. |
| 고객 속성 기능은 Adobe Audience Manager와 어떤 관련이 있습니까? | Audience Manager는 데이터를 수신하여 대상을 식별할 수 있지만 속성을 이전 행동 데이터와 연결하는 분석 기능을 수행할 수는 없습니다. 또한 Adobe Analytics에서 사용할 수 있는 보고, 분석 및 세분화 기능도 제공하지 않습니다. [!UICONTROL 고객 특성]을 사용하면 여러 응용 프로그램에서 가져온 다양한 데이터를 함께 연결하고 Experience Cloud에서 사용할 수 있도록 단일 ID와 연결할 수 있습니다. <br>Adobe Target에서 [!DNL customer attributes]는 다른 규칙과 결합하여 대상자를 구축할 수 있는 개별 속성으로 표시됩니다. [!UICONTROL People] 서비스에 공유된 대상자는 수정할 수 없는 전체 대상자입니다. |
| **(Adobe Analytics 전용)** Analytics premium에 제공된 기능과 비교할 때 이 기능은 어떤 차이가 있습니까? | 이전에는 고객 속성 데이터를 Analytics 데이터에 결합하려는 고객이 이 기능을 사용하려면 Data Workbench 도구에 상당히 의존했습니다. [!DNL customer attributes]은(는) [!DNL customer attributes]을(를) Report Builder에서 차원 및 지표로 제공하여 좀 더 다양한 대상자에게 이 기능을 제공합니다. Analytics Standard 고객은 [!DNL customer attributes]에 액세스할 수 있지만 사용할 수 있는 기능은 제한됩니다. Analytics 프리미엄 고객은 전체 기능을 사용할 수 있습니다. |
| **(Adobe Target만 해당)** Adobe Target에서 표시된 적이 없는 고객의 데이터를 미리 로드하거나 업로드할 수 있습니까? | 예. 방문자가 Adobe Target에 대해 첫 번째 요청을 수행하면 시스템은 [!DNL customer attributes]에서 고객에 대해 Adobe가 보유한 기존 정보를 가져온 다음 해당 데이터를 사용하여 타겟팅합니다. **참고:** 이 데이터를 검색하는 데는 방문자가 Adobe Target과 처음 상호 작용한 시점부터 최대 20분이 걸릴 수 있습니다. |
| **(Adobe Target만 해당)** 고객 속성 데이터를 공유 대상자 데이터와 결합하여 슈퍼 대상자를 만들 수 있습니까? | 아니요. 공유된 대상자 데이터는 완전한 대상자입니다. |
| **(Adobe Target만 해당)** [!DNL customer attributes] 기능을 Adobe Target의 벌크 프로필 API와 어떻게 비교합니까? | 벌크 프로필 API를 사용하면 개별 프로필에 대해 또는 대량으로 API를 통해 Adobe Target 프로필을 직접 업데이트할 수 있습니다. 이 기능은 [!DNL customer attributes]와 비슷하지만, 다음과 같은 주요 차이점이 있습니다.<ul><li>프로필 API는 REST API 호출이며, [!DNL customer attributes]는 FTP를 사용합니다.</li><li>Adobe Target의 프로필 API는 전체 Experience Cloud 대신 Adobe Target으로만 데이터를 보냅니다.</li><li>[!DNL customer attributes]는 이러한 외부 데이터를 만들고 관리할 간단한 인터페이스를 제공합니다.</li></ul> |
| **(Adobe Target만 해당)** [!DNL customer attributes]에서 Adobe Target으로 데이터를 업로드하면 Adobe Target 방문자의 프로필 라이프타임이 연장됩니까? | 예. Adobe Target 도움말의 [방문자 프로필 라이프타임](https://experienceleague.adobe.com/docs/target/using/audiences/visitor-profiles/visitor-profile.html?lang=ko) 을 참조하십시오. |
| **(Adobe Target만 해당)** 방문자가 고객 ID로 식별되면 바로 [!DNL customer attributes]에 업로드된 데이터를 타겟팅할 수 있습니까? | 예. Adobe Target에 대한 서버 호출 시 여기에 mbox 타사 ID가 포함되면 모든 고객 속성 데이터를 사용할 수 있습니다. |
| **(Adobe Target만 해당)** **[!UICONTROL 동기화 상태]** 열은 고객 속성 소스에 업로드된 파일에 대해 무엇을 나타냅니까? | 특정 속성 파일에 대한 동기화 상태 아이콘을 선택하여 Adobe Target에 의해 게시되고 동기화된 레코드 수를 볼 수 있습니다. `Sync %`는 Adobe Target에서 동기화된 프로필의 비율(%)을 지정하는 실시간 지표입니다.<br> **참고:** 속성이 Adobe Target과 동기화되려면 최대 24시간이 걸릴 수 있습니다. |
| [!DNL customer attributes] 소스에서 파일 업로드 지표가 나타내는 것은 무엇입니까? | 다음 지표의 도움을 받아 [!DNL customer attributes]에 업로드된 속성의 상태를 확인할 수 있습니다. <ul><li>레코드: 속성 파일에 있는 레코드 수입니다.</li><li>**새 레코드:** 속성 파일에 있는 새 레코드 수입니다.</li> <li>**업데이트된 레코드:** 파일에서 업데이트된 값이 있는 [!DNL customer attributes]에 존재하는 레코드 수입니다.</li><li>**모든 데이터(레코드):** [!DNL customer attributes]에 성공적으로 업로드된 총 레코드 수입니다.</li></ul> |

{style="table-layout:auto"}
