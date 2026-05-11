---
description: Analytics 및 Target용  [!DNL Customer Attributes] 에서 구독을 구성하고 데이터 소스를 활성화하는 방법에 대해 알아봅니다.
solution: Experience Cloud
title: ' [!DNL Customer Attributes]에서 구독을 구성하는 방법'
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: cfa2aa5c-337f-401e-80eb-cbe36cb1d41e
TQID: 'https://experienceleague.adobe.com/SVDhQ4Y2-CIJ7pVhapEqhu1gRkYSrPjmSI8-NejBddI'
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
feature_v2:
  - id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
subfeature_v2: id:id:
role_v2: id:
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: f01d85af42b8f2c27dbada8f73546bc6fe4bf710
workflow-type: tm+mt
source-wordcount: 408
ht-degree: 47%

---

# 고객 속성 가입 구성

[!DNL Customer Attributes] 구독을 통해 CX Enterprise와 애플리케이션([!DNL Analytics] 및 [!DNL Target]) 간에 고객 특성 데이터 흐름을 사용할 수 있습니다.

예를 들어 Adobe Analytics 가입을 구성하면 속성 데이터를 보고서에서 사용할 수 있습니다. [!DNL Adobe Target]을(를) 사용하는 경우 타깃팅 및 세그멘테이션을 위해 고객 특성을 업로드할 수 있습니다.

**구독을 구성하고 데이터 원본을 활성화하려면**

1. 편집할 데이터 원본을 [!DNL Customer Attributes]에서 찾습니다.

   [!DNL CX Enterprise]에서 **[!UICONTROL Apps]** ![메뉴](assets/menu-icon.png) > **[!DNL Customer Attributes]**&#x200B;을(를) 클릭합니다.

1. [!UICONTROL Edit Customer Attribute Source]에서 **[!UICONTROL File Upload]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Configure Subscriptions]**&#x200B;을(를) 클릭합니다.

   ![CX Enterprise에서 구독 구성](assets/configure-subscriptions.png)

1. 고객 특성 원본을 활성화하려면 **[!UICONTROL Active]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

1. [!DNL Analytics] 또는 [!DNL Target]에 대한 구독을 구성하려면 **[!UICONTROL Configure]**&#x200B;을(를) 클릭합니다.

   다음 예제에서는 [!DNL Target] 구독을 보여 줍니다.

   ![단계 결과](assets/subscription-target.png)

   | 요소 | 설명 |
   | --- | --- |
   | 솔루션 | **Adobe Analytics**<br>[!DNL Analytics]을(를) 선택하고 특성 데이터를 받을 보고서 세트와 포함할 특성을 지정합니다.<br>**Adobe Target**<br>&#x200B;타기팅 및 세분화를 위해 고객 속성을 업로드할 수 있습니다. 이 기능은 특성 데이터를 기반으로 테스트를 타깃팅하거나 Analytics의 세분화에 데이터를 사용할 수 있도록 하려는 경우 유용합니다.<br>방문자를 위해 업로드된 고객 특성 데이터는 로그인 시 사용할 수 있습니다(**[!DNL Target]** > **대상**.<br>여러 데이터 소스가 지원됩니다. 웹 사이트에서 고객 ID를 설정하는 경우 별칭 중 하나 이상이 [!DNL Target]에 등록되어 있는지 확인하십시오. |
   | 보고서 세트(Adobe Analytics) | Analytics의 보고서 세트입니다.<br>단일 특성 소스 내에서 총 10개를 초과하는 보고서 세트를 Analytics 구독에 추가할 수 없습니다. 포함할 보고서 세트를 선택할 때는 다음 제안을 고려하십시오.<ul><li>인증된 공통 고객 세트를 포함하는 보고서 세트를 선택합니다. 한 보고서 세트의 인증된 고객이 다른 보고서 세트의 인증된 고객과 겹치지 않으면 이러한 보고서 세트를 다른 속성 소스로 분리하십시오.</li><li>가능한 경우 속성 소스에 포함된 보고서 세트가 비슷한 트래픽 볼륨을 발생해야 합니다.</li></ul><br>인증된 공통 고객 세트가 있는 보고서 세트가 10개보다 많은 경우 추가 고객 속성 소스를 구성하고 각각이 최대 10개의 보고서 세트를 포함하도록 할 수 있습니다. |
   | 포함할 속성(Analytics 및 [!DNL Target]) | 애플리케이션으로 보낼 속성입니다. <br>구독을 구성하고 속성을 선택할 때 보유하고 있는 애플리케이션에 따라 다음과 같은 제한이 _보고서 세트마다_ 적용됩니다.<ul><li>Foundation: 0개</li><li>Select: 3개</li><li>Prime: 15개</li><li>Ultimate: 200개</li><li>Standard: 총 3개</li><li>Premium: 보고서 세트당 200개</li><li>[!DNL Target] 표준: 5개</li><li>[!DNL Target] Premium: 200개</li></ul><br>**참고:** Analytics Premium으로 업그레이드할 때 추가 속성은 24시간 후에 사용할 수 있습니다. 이 시간 중에 속성 구독 최대값 오류가 표시될 수 있습니다. |

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.
