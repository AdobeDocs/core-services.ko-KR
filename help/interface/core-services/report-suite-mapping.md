---
description: 한 개 이상의 보고서 세트를 조직에 매핑하는 방법을 알아봅니다.
seo-description: 한 개 이상의 보고서 세트를 조직에 매핑하는 방법을 알아봅니다.
seo-title: 조직에 보고서 세트 매핑
title: 조직에 보고서 세트 매핑
uuid: b983d5a6-b3d0-4137-ac53-bc5681d3e58b
translation-type: tm+mt
source-git-commit: 08e8e5fea4e4e64a195ebe25ae3ef19e849cabc5

---


# 조직에 보고서 세트 매핑 {#topic_7C4740559EAC4E0FA5F8DEF886B580DA}

한 개 이상의 보고서 세트를 조직에 매핑하는 방법을 알아봅니다.

<!-- May 5 2020: This feature will likely be deprecated in Nov 2020. Any users with outstanding report suites that are not mapped will have 6 months to map their RS. -->

Experience Cloud 서비스(예: Experience Cloud ID 서비스 및 [!UICONTROL 사람])는 개별 보고서 세트 대신 조직과 연결됩니다. 이러한 서비스가 올바르게 작동하도록 하려면 각 Analytics 보고서 세트를 조직에 매핑해야 합니다. 매핑 프로세스:

* Experience Cloud 조직을 보고서 세트의 기본 조직으로 설정합니다.
* 보고서 세트에 액세스할 수 있는 사용자를 변경하지 않습니다(액세스 권한은 각 사용자에 대해 Adobe Analytics 로그인 계정으로 판별됨).

## 요구 사항

매핑할 보고서 세트에 대한 액세스 권한이 있는 로그인 회사의 Analytics 관리자여야 합니다. 또한 보고서 세트를 해당 조직에 매핑하려면 이 계정 [을 Experience Cloud 조직에](../admin-getting-started/organizations.md#topic_C31CB834F109465A82ED57FF0563B3F1) 연결해야 합니다.

지정된 보고서 세트에 액세스할 수 있는 해당 조직의 로그인 회사에 대한 Analytics 관리자 권한이 없는 경우 조직이 회색으로 표시됩니다.

## 조직에 보고서 세트 매핑 {#task_23993FE78DF6455FA8D7BE60686EA16C}

1. Click **[!UICONTROL Experience Cloud]** > **[!UICONTROL Administration]** > **[!UICONTROL Report Suite Mapping]**

1. 각 보고서 세트에 액세스할 수 있는 로그인 회사를 보려면 **[!UICONTROL 로그인 회사에 표시를 클릭합니다]**.

   이 보기는 매핑에 대한 올바른 결정을 내리는 데 도움을 주기 위한 것입니다.

1. 보고서 세트 옆에 있는 **[!UICONTROL 매핑된 조직]** 열에서 드롭다운을 클릭하고 매핑할 조직을 선택합니다.

   Experience Cloud 조직 선택에 대한 팁은 다음 섹션을 참조하십시오.

## 조직에 여러 보고서 세트 매핑 {#task_94955B0D8ABA4CB1A38746ECF8E32711}

1. Click **[!UICONTROL Experience Cloud]** > **[!UICONTROL Administration]** > **[!UICONTROL Report Suite Mapping]**.

1. 매핑할 보고서 세트를 선택합니다.

   ![](assets/rs-mapping-multiple.png)

1. 조직(이 예에서는 Outdoors Inc,)을 선택한 다음 **[!UICONTROL 선택을 클릭합니다]**.

   Experience Cloud 조직 선택에 대한 팁은 다음 섹션을 참조하십시오.

1. **[!UICONTROL 매핑 저장을 클릭합니다]**.

## Experience Cloud 조직 선택을 위한 팁 {#mapping-tips}

이 섹션에는 보고서 세트를 매핑해야 하는 Experience Cloud 조직을 선택하는 데 도움이 되는 팁이 포함되어 있습니다.

### 어떤 조직을 선택해야 합니까?

If the Experience Cloud ID Service is currently deployed on the report suite, ensure the organization you select in the Report Suite Mapping tool is the same organization specified in the [!DNL visitorAPI.js] file on your site. You can use the instructions in [Test and Verify the Experience Cloud ID Service](https://docs.adobe.com/content/help/en/id-service/using/implementation-guides/test-verify.html) to find the org ID that is being used by the Visitor ID service.

방문자 ID 서비스가 보고서 세트에 대한 데이터를 수집하는 사이트에 아직 배포되지 않은 경우, 나중에 Experience Cloud 방문자 ID 서비스를 배포하는 경우, 배포가 보고서 세트 매핑 도구에서 선택한 조직과 일치하는지 확인해야 합니다.

### 일부 조직이 회색으로 표시되는 이유는 무엇입니까?

이는 회색으로 표시된 보고서 세트에 매핑할 충분한 권한이 없음을 나타냅니다. 다음 예를 생각해 보십시오.

![](assets/rs-mapping.png)

이 다이어그램에서 파란색 키는 관리자 권한을 나타냅니다. 회색 선은 가시성을 나타냅니다.

이 사용자는 두 개의 Experience Cloud 조직에 액세스할 수 있습니다. 그는 다음과 같은 일을 했다.

* chapek Analytics [!UICONTROL 로그인 회사의] 관리자 계정을 자신의 [!UICONTROL Chapek] Corp Experience Cloud 조직 계정에 연결했습니다.
* Doohan Analytics 로그인 회사의 [!UICONTROL 관리자가] 아닌 계정을 자신의 [!UICONTROL Chapek] Corp Experience Cloud 조직 계정에 연결했습니다.
* 나이젤 분석 로그인 회사의 비관리 계정을 Nigel Inc Experience Cloud 조직 계정에 연결했습니다.

다음 포인트는 이 사용자가 이러한 보고서 세트에 대해 수행할 수 있으며 수행할 수 없는 매핑 작업을 나열합니다.

* [!UICONTROL 이 사용자는 연결된 Analytics 로그인 회사(] chapek [!UICONTROL )의 관리자이며] 이 계정이 이 조직에 연결되어 있으므로 Chapek-prod[!UICONTROL 보고서 세트를]Chapek Corp조직에 매핑할 수 있습니다.
* [!UICONTROL 이 사용자는 이 보고서] 세트가 표시되는 로그인 회사의 관리자가 아니므로 Nigel-prod 보고서 세트를 연결할 수 없습니다.
* [!UICONTROL 이 사용자는] Experience Cloud 조직에 연결된 로그인 회사( [!UICONTROL chapek] )의 관리자이므로 Doohan-prod[!UICONTROL 보고서 세트를 Chapek Corp에 매핑할 수 있습니다](Doohan Analytics 로그인 회사의 관리자가 아님). 이 사용자는 해당 매핑을 수행할 수 없지만 [!UICONTROL dohan-prod] 보고서 세트를 Nigel Inc Experience Cloud 조직에도 매핑할 수 있다는 점을 알아야 합니다. 이 경우 두 Experience Cloud 조직이 모두 목록에 표시되지만 Nigel Inc [!UICONTROL 가] 회색으로 표시됩니다. 매핑하기 전에 이 사용자는 온라인 로그인 회사의 관리자에게 문의하여 매핑에 가장 적합한 조직을 결정해야 합니다. 처음에 보고서 세트를 만든 조직과 다른 조직을 선택하는 경우 UI에 가능한 충돌 경고가 표시됩니다.

## FAQ {#section_099E485805994C929FF9C9F75219BEE1}

### 내 보고서 세트가 모두 표시되지 않는 이유는 무엇입니까?

보고서 세트 중 일부는 다른 로그인 회사 아래에 표시될 수 있습니다. 화면 상단의 드롭다운을 사용하여 현재 로그인 회사를 변경할 수 있습니다.

### 보고서 세트 중 하나에 대해 드롭다운에 나열된 일부 조직을 인식하지 못하는 경우 어떻게 됩니까?

The list shows you all the *possible* organizations your report suite could be mapped to, even you don’t have permission to map to all those report suites. 보고서 세트를 목록의 회색으로 표시된 보고서 세트 중 하나로 매핑해야 하는지 확실하지 않은 경우 조직의 Experience Cloud 관리자에게 문의하여 최선의 선택을 결정하십시오.

### &quot;로그인 회사에 표시&quot; 열에 보고서 세트에 대해 나열된 로그인 회사 중 일부를 인식하지 못하는 경우 어떻게 합니까?

이 보고서 세트가 다른 Experience Cloud 조직의 일부일 수 있는 다른 로그인 회사와 공유된 경우도 있습니다.

### 다른 조직에서 생성하는 보고서 세트에 대한 &quot;가능한 충돌&quot; 오류는 무엇입니까? 왜 그게 중요하죠?

보고서 세트 매핑에 대한 현명한 결정을 내리도록 도와주는 알림입니다. 조직이 이 보고서 세트에 더 적합할 수 있도록 하기 위해 원래 다른 조직 아래에 보고서 세트가 만들어졌다는 것을 알리고자 합니다.

### 보고서 세트가 매핑되는지 어떻게 알 수 있습니까?

매핑된 보고서 세트가 편집할 수 없는 형식으로 표시됩니다. 매핑을 변경해야 하는 경우 고객 지원 센터에 문의하십시오.

### Experience Cloud 조직의 조직 ID만 알고 있다면 어떻게 됩니까? 내 조직 ID의 이름을 찾으려면 어떻게 해야 합니까?

조직 및 계정 설정에서 [조직 이름을 찾을 수 있습니다](https://docs.adobe.com/content/help/ko-KR/core-services/interface/manage-users-and-products/organizations.html).

### &quot;Date Mapped&quot; 열에 날짜가 보입니다. 누가 그 지도를 만들었나요?

Analytics 인터페이스에서 보고서 세트 변경 로그를 참조하여 변경한 사용자 ID를 확인할 수 있습니다. &quot;IMS 조직에 연결된 패키지&quot; 이벤트를 찾습니다.
