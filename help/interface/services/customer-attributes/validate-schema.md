---
description: Adobe Experience Cloud에서  [!DNL Customer Attributes] 스키마의 유효성을 검사하는 방법을 알아봅니다.
solution: Experience Cloud
title: ' [!DNL Customer Attributes] 스키마의 유효성을 검사하는 방법'
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 776d1fd3-c733-4970-a76b-4c3c0119ee77
source-git-commit: 21120abb5ab0fcc8d556012851548f39f3875038
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 49%

---

# 스키마 유효성 검사

유효성 검사 프로세스를 사용하여 표시 이름 및 설명을 업로드된 속성(문자열, 정수, 숫자 등)에 매핑할 수 있습니다.

스키마는 이러한 설정에 따라 만들어집니다. 이 스키마는 앞으로 이 데이터 소스로 업로드되는 모든 데이터의 유효성을 검사하는 데 사용됩니다. 이 매핑 프로세스가 원본 데이터를 변경하지는 않습니다.

>[!NOTE]
>
>유효성 검사 후 스키마를 업데이트하면 고객 특성이 삭제됩니다. [스키마 업데이트(속성 삭제)](t-crs-usecase.md)를 참조하십시오.

**스키마의 유효성을 검사하려면**

1. [!DNL Customer Attributes]에서 편집할 특성 원본을 클릭합니다.

1. **[!UICONTROL 고객 특성 편집 Source]**&#x200B;에서 **[!UICONTROL 파일 업로드]**&#x200B;를 클릭합니다.

1. [!UICONTROL 파일 업로드 및 스키마 유효성 검사] 페이지에서 **[!UICONTROL 작업]** > **[!UICONTROL 스키마 보기/편집]**&#x200B;을 클릭합니다

   ![스키마 편집](assets/view_edit_schema.png)

   [!UICONTROL 스키마 편집] 페이지에서 각 스키마 행은 업로드된 CSV 파일의 열을 나타냅니다.

   ![Experience Cloud에서 스키마 페이지 편집](assets/edit-schema.png)

**작업**

* **[!UICONTROL 데이터 추가:]** 새 속성 데이터를 이 데이터 소스에 업로드합니다.

* **[!UICONTROL 스키마 보기/편집:]** 다음 단계에 설명된 대로 표시 이름을 속성 데이터에 매핑합니다.

* **[!UICONTROL FTP 설정:]** FTP 계정을 만들어 [FTP를 통해 데이터를 업로드](t-upload-attributes-ftp.md)(선택 사항).

* **[!UICONTROL ID 조회:]** `.csv`의 CID(고객 ID)를 입력하여 해당 ID에 대한 Experience Cloud 정보를 조회합니다. 이 기능은 방문자에 대한 속성 데이터가 표시되지 않는 문제를 해결하는 데 유용합니다.

   * **[!UICONTROL ECID(Experience Cloud ID):]** 최신 Experience Cloud ID 서비스를 사용하는 경우에 표시됩니다. MCID 서비스를 사용하고 있지만 ID가 표시되지 않는 경우 Experience Cloud에서 해당 CID에 대한 별칭을 수신하지 못한 것입니다. 방문자가 로그인되어 있지 않거나 해당 ID가 구현되지 않은 것입니다.

   * **[!UICONTROL CID(고객 ID):]** 이 CID와 연결된 특성입니다. prop 또는 eVar을 사용하여 CID(AVID)를 업로드하며 속성은 표시되지만 AVID는 표시되지 않는 경우 방문자가 사이트에 로그인되어 있지 않은 것입니다.

   * **[!UICONTROL AVID(Analytics visitor ID):]** prop 또는 eVar을 사용하여 CID를 업로드하는 경우에 표시됩니다. 이러한 ID가 Experience Cloud에 전달되는 경우 입력한 CID와 연결된 모든 방문자 ID가 여기에 표시됩니다.
