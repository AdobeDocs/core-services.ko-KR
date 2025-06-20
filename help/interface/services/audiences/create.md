---
description: 속성 규칙을 사용하여 Adobe Experience Cloud에서 대상자를 만들고 복합 대상자를 정의하는 방법을 알아봅니다.
solution: Experience Cloud
title: 대상자 만들기
uuid: 7e622539-296e-4ff3-93b0-ec1c08b35429
feature: Audience Library
topic: Administration
role: Admin
level: Experienced
exl-id: b65a12f5-fa89-400a-b279-13c381cd6c22
source-git-commit: 361175f290d73f1637673420700874a2415e3fca
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 92%

---

# 대상자 만들기

속성 규칙을 사용하여 Experience Cloud에서 대상자를 만들고 복합 대상자를 정의하는 방법을 알아봅니다.

이 문서는 다음 방법을 이해하는 데 도움이 됩니다.

* 대상자 만들기
* 규칙 만들기
* 규칙을 사용하여 복합 대상자 정의

다음 그래픽에는 복합 대상자의 두 가지 규칙이 나와 있습니다.

![복합 대상자의 2가지 규칙](assets/audience_sharing.png)

각 원은 대상자 멤버십을 정의하는 규칙을 나타냅니다. 두 대상자 규칙 모두에서 멤버 자격을 얻은 방문자는 겹쳐지면서 정의된 복합 대상자가 됩니다.

>[!NOTE]
>
>대상자는 지정된 기간 동안의 데이터 수집이 완료된 후에 완전히 정의됩니다.

다음 예에서는 복합 대상자에 대한 규칙을 만드는 방법을 보여 줍니다. 이 대상자는 다음으로 구성됩니다.

* 페이지 데이터 또는 원시 분석 데이터에서 파생된 홈/가든 섹션
* [!DNL Experience Cloud]에 [게시된](overview.md) [!DNL Adobe Analytics] 세그먼트에서 파생된 Chrome 및 Safari 사용자.

  ![복합 대상자에 대한 규칙 만들기](assets/audience_create.png)

**대상자를 만들려면**

1. [!DNL Experience Cloud]에서 [!DNL Experience Platform]의 **[!UICONTROL 사용자]** > **[!UICONTROL 대상자 라이브러리]를 클릭합니다.**
1. [!UICONTROL 대상] 페이지에서 **[!UICONTROL 새로 만들기]**&#x200B;를 클릭합니다. ![추가](assets/add_icon_small.png)

   ![단계 결과](assets/audience_create_new.png)

1. [!UICONTROL 새 대상자 만들기] 페이지에서 제목 및 설명을 지정합니다.
1. [!UICONTROL 규칙]에서 다음과 같은 속성 소스를 선택합니다.

   * **[!UICONTROL Real-Time Analytics 데이터:]** (또는 Raw 데이터) 이것은 Real-Time Analytics 이미지 요청에서 파생된 속성 데이터이며 eVar 및 이벤트와 같은 데이터를 포함합니다. 이 속성 소스를 사용할 때 보고서 세트를 선택하고 포함할 차원 또는 이벤트를 정의해야 합니다. 이 보고서 세트 선택 옵션은 보고서 세트에 사용되는 변수 구조를 제공합니다.

   >[!NOTE]
   >
   >캐싱으로 인해, Analytics에서 삭제된 보고서 세트는 삭제가 Experience Cloud에 표시되는 데 12시간이 필요합니다.

   * [!DNL Experience Cloud] 원본에서 파생된 **[!UICONTROL Experience Cloud:]** 특성 데이터입니다. 예를 들어 [!DNL Analytics]에서 만든 대상자 세그먼트의 데이터이거나 [!DNL Audience Manager]의 데이터일 수 있습니다.

1. 대상자 규칙을 정의한 다음 **[!UICONTROL 저장]을 클릭합니다.**

>[!NOTE]
>
>이러한 규칙을 작성할 때 구현 변수를 이해해야 합니다.

[!UICONTROL 규칙]에서 *`Home & Garden`* 속성 선택 사항을 정의합니다.

* **[!UICONTROL 속성 소스:]** Raw Analytics 데이터
* **[!UICONTROL 보고서 세트:]** 보고서 세트 31
* 차원 = **[!UICONTROL Store (Merch) (v6)]** > **[!UICONTROL Equals]** > **[!UICONTROL Home &amp; Garden]**

![대상자 라이브러리의 속성 선택 사항](assets/home_garden.png)

*Chrome 및 Safari 방문자*&#x200B;는 Analytics에서 공유되는 대상자 세그먼트입니다.

* **[!UICONTROL 속성 소스:]** Experience Cloud
* **[!UICONTROL 차원:]** Chrome/Safari 방문자

![Chrome/Safari 방문자](assets/chrome_safari.png)

비교를 위해 *OR* 규칙을 추가하여 뜰/가구와 같은 사이트 섹션의 모든 방문자를 볼 수 있습니다.

![또는 대상자에 대한 규칙](assets/audiences_rule_patio.png)

결과 규칙은 홈/가든을 방문한 Chrome/Safari 사용자로 구성되는 정의된 대상자입니다. 뜰/가구 세그먼트는 사이트 섹션을 방문하는 모든 방문자에 대한 추가적인 인사이트를 제공합니다.

![Experience Cloud에서 정의된 대상자](assets/defined_audience.png)

* **이전 예상:** (점선 원) [!DNL Analytics] 데이터를 기반으로 만들어진 규칙을 나타냅니다.
* **실제 대상:** (실선 원)30일 동안의 Audience Manager 데이터를 포함하여 만들어진 모든 규칙입니다. Audience Manager 데이터가 30일이 되면 선은 실선이 되고 실제 수치를 나타냅니다.

지정된 기간 동안 데이터 수집이 완료되면 원이 합쳐지면서 정의된 대상자를 표시합니다.

대상자가 저장되면 다른 애플리케이션에 사용할 수 있습니다. 예를 들어 공유 대상자를 Adobe Target 활동에 포함할 수 있습니다.
