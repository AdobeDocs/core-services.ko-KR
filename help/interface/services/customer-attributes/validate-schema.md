---
description: Adobe CX Enterprise에서  [!DNL Customer Attributes] 스키마의 유효성을 검사하는 방법을 알아봅니다.
solution: Experience Cloud
title: ' [!DNL Customer Attributes] 스키마의 유효성을 검사하는 방법'
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 776d1fd3-c733-4970-a76b-4c3c0119ee77
TQID: https://experienceleague.adobe.com/J-AaDn4HtD1bS-VCPn2XiPLVBbTnYyl5o1NpJ9HFj1g
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
feature_v2:
  - id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
subfeature_v2:
  - id: b75843fa-0a67-4a44-a6b1-cc627b0481dc
  - id: fef08361-6ac5-460c-93fe-d063e40b6a49
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 50012e2564e88e1a6e16578e3331136c7df0cb21
workflow-type: tm+mt
source-wordcount: 345
ht-degree: 39%

---

# 스키마 유효성 검사

유효성 검사 프로세스를 사용하여 표시 이름 및 설명을 업로드된 속성(문자열, 정수, 숫자 등)에 매핑할 수 있습니다.

스키마는 이러한 설정에 따라 만들어집니다. 이 스키마는 앞으로 이 데이터 소스로 업로드되는 모든 데이터의 유효성을 검사하는 데 사용됩니다. 이 매핑 프로세스가 원본 데이터를 변경하지는 않습니다.

>[!NOTE]
>
>유효성 검사 후 스키마를 업데이트하면 고객 속성이 삭제됩니다. [스키마 업데이트(속성 삭제)](t-crs-usecase.md)를 참조하십시오.

**스키마의 유효성을 검사하려면**

1. [!DNL Customer Attributes]에서 편집할 특성 원본을 클릭합니다.

1. **[!UICONTROL 고객 특성 편집 Source]**&#x200B;에서 **[!UICONTROL 파일 업로드]**&#x200B;를 클릭합니다.

1. [!UICONTROL 파일 업로드 및 스키마 유효성 검사] 페이지에서 **[!UICONTROL 작업]** > **[!UICONTROL 스키마 보기/편집]**&#x200B;을 클릭합니다

   ![스키마 편집](assets/actions.png)

   [!UICONTROL 스키마 편집] 페이지에서 각 스키마 행은 업로드된 CSV 파일의 열을 나타냅니다.

   ![CX Enterprise의 스키마 편집 페이지](assets/schema-edit.png)

**작업**

* **[!UICONTROL 데이터 추가:]** 새 특성 데이터를 이 데이터 원본에 업로드합니다.

* **[!UICONTROL 스키마 보기/편집:]** 다음 단계에 설명된 대로 표시 이름을 특성 데이터에 매핑합니다.

* **[!UICONTROL FTP 설정:]** FTP 계정을 만들어 [FTP를 통해 데이터를 업로드](t-upload-attributes-ftp.md)(선택 사항).

* **[!UICONTROL ID 조회:]** `.csv`의 CID(고객 ID)를 입력하여 해당 ID에 대한 CX Enterprise 정보를 조회합니다. 이 기능은 방문자에 대한 속성 데이터가 표시되지 않는 문제를 해결하는 데 유용합니다.

   * **[!UICONTROL ECID(CX Enterprise ID):]** 최신 CX Enterprise ID 서비스를 사용하는 경우에 표시됩니다. MCID 서비스를 사용하고 있지만 ID가 표시되지 않는 경우 CX Enterprise에서 해당 CID에 대한 별칭을 수신하지 못한 것입니다. 방문자가 로그인되어 있지 않거나 해당 ID가 구현되지 않은 것입니다.

   * **[!UICONTROL CID(고객 ID):]** 이 CID와 연결된 특성입니다. prop 또는 eVar을 사용하여 CID(AVID)를 업로드하며 속성은 표시되지만 AVID는 표시되지 않는 경우 방문자가 사이트에 로그인되어 있지 않은 것입니다.

   * **[!UICONTROL AVID(Analytics 방문자 ID):]**&#x200B;은(는) prop 또는 eVar을 사용하여 CID를 업로드하는 경우에 표시됩니다. 이러한 ID가 CX Enterprise로 전달되는 경우 입력한 CID와 연결된 모든 방문자 ID가 여기에 표시됩니다.
