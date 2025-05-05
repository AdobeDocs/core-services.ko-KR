---
description: Experience Cloud에  [!DNL Customer Attributes] 을(를) 업로드하기 위한 데이터 파일 요구 사항 및 여러 데이터 소스에 대해 알아봅니다.
solution: Experience Cloud
title: 데이터 파일 및 데이터 소스
uuid: 9dd0e364-889b-45db-b190-85c0930a101e
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: e2dfe10d-7003-4afa-a5e6-57703d74efd4
source-git-commit: c39672f0d8a0fd353b275b2ecd095ada1e2bf744
workflow-type: tm+mt
source-wordcount: '1178'
ht-degree: 90%

---

# [!DNL Customer Attributes]의 데이터 파일 및 데이터 원본 정보

[!DNL Customer Attributes]을(를) Experience Cloud에 업로드하기 위한 데이터 파일 요구 사항 및 여러 데이터 소스입니다.

엔터프라이즈에서 CRM 또는 비슷한 데이터에 액세스해야 합니다. Experience Cloud에 업로드하는 데이터는 `.csv` 파일이어야 합니다. FTP 또는 sFTP를 통해 업로드하는 경우 `.fin` 파일도 업로드합니다.

[!DNL Customer Attributes]은(는) 하루에 몇 개의 파일을 처리하도록 디자인되었습니다. 작은 파일이 대량으로 있어 처리가 지연되는 문제를 방지하기 위해 동일한 조직의 이전 일괄 처리 후 30분 이내에 전송된 파일은 우선 순위가 낮은 큐로 라우팅됩니다.

## 허용되는 파일 형식 및 이름 지정 요구 사항 {#section_6F64FA02ACCC4215B0862CB6A1821FBF}

<table id="table_C27955F6B52A45B28BEEAAF14FFC86D8"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> 파일 유형 </th> 
   <th colname="col2" class="entry"> 설명 </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <span class="filepath"> .csv </span> </p> </td> 
   <td colname="col2"> <p>쉼표로 구분된 값 파일(예: Excel에서 만든 파일)입니다. 이 파일은 고객 속성 데이터를 포함합니다. </p> <p> <b>이름 지정 요구 사항:</b> 파일 이름 확장명에 공백이 들어 있지 않은지 확인하십시오. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="filepath"> .fin </span> </p> </td> 
   <td colname="col2"> <p>(필수) <span class="filepath">.fin</span> 파일은 데이터 업로드를 끝냈음을 시스템에 알려 줍니다. <span class="filepath">.fin</span> 파일의 이름은 <span class="filepath">.csv</span> 파일의 이름과 일치해야 합니다. </p> <p>Adobe에서는 <span class="filepath">.fin</span> 확장명의 빈 텍스트 파일을 만들 것을 권장합니다. 빈 파일을 만들면 공간 및 업로드 시간이 단축됩니다. </p> <p> <p>참고: 업로드 후에는 <span class="filepath">.fin</span> 파일 이름을 다시 바꿀 수 없습니다. <span class="filepath">.fin</span> 파일은 따로 업로드해야 하며 이전에 업로드한 파일을 이름 변경 후 사용할 수 없습니다. </p> </p> <p>고객 속성 FTP에서 <span class="filepath">.fin</span> 파일을 업로드하면 시스템이 데이터를 빠르게(1분 이내) 검색합니다. 이 경우 데이터를 덜 자주(시간당 약 한 번) 선택하는 다른 Adobe FTP 기반 시스템과 다릅니다. </p> <p>드래그 앤 드롭 업로드 방법을 사용할 때는 <span class="filepath">.fin</span> 파일이 필요하지 않습니다. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="filepath"> .gz</span> 또는 <span class="filepath">.zip </span> </p> </td> 
   <td colname="col2"> <p> <span class="filepath"> .gz</span>(gzip) 또는 <span class="filepath">.zip</span> - 압축된 파일용. <span class="filepath">.zip</span> 파일은 보관 위치에 둘 이상의 파일로 포함될 수 있습니다. </p> <p> <b>이름 지정 요구 사항:</b> <span class="filepath">.zip</span> 또는 <span class="filepath">.gz</span>의 이름은 <span class="filepath">.csv</span>의 이름과 일치해야 합니다 . 예를 들어 <span class="filepath">.csv</span> 파일이 <span class="filepath">crm_small.csv</span>이면 <span class="filepath">.zip</span> 파일은 <span class="filepath">crm_small.csv.zip</span>이어야 합니다 . </p> <p>.fin 파일은 .csv와 일치해야 합니다. </p> </td> 
  </tr> 
 </tbody> 
</table>

## 속성 데이터 파일에 대한 요구 사항 {#section_169FBF5B7BBA47CE825B7A330CF3FE98}

**CSV 예**

CSV 파일은 다음 형식을 따라야 합니다.

![속성 데이터 파일에 대한 요구 사항](assets/cvs.png)

텍스트 편집기에 표시되는 동일한 파일:

![속성 데이터 파일에 대한 요구 사항](assets/csv_txt.png)

**지침**

<table id="table_A9849CC9AA784763921DE057F0F61515"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> 항목 </th> 
   <th colname="col2" class="entry"> 설명 </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>드래그 앤 드롭 </p> </td> 
   <td colname="col2"> <p>드래그 앤 드롭 파일은 100MB보다 작아야 합니다. </p> <p>드래그 앤 드롭 업로드 방법을 사용할 때는 <span class="filepath">.fin</span> 파일이 필요하지 않습니다. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>고객 ID 열 </p> </td> 
   <td colname="col2"> <p> 첫 번째 열은 고유한 고객 ID여야 합니다. 사용된 ID는 Experience Cloud ID 서비스에 전달되는 ID에 해당해야 합니다. </p> <p>Analytics의 경우 prop 또는 eVar에 저장되는 ID입니다. </p> <p>Target의 경우 setCustomerID 값입니다. </p> <p> 이 고객 ID는 CRM가 데이터베이스의 각 사용자에 대해 사용하는 고유한 식별자입니다. 나머지 열은 CRM에서 가져오는 속성입니다. 업로드할 속성의 수를 선택합니다. </p> <p>열 제목에는 읽을 수 있는 친근한 이름이 권장되지만 필수는 아닙니다. 업로드 후에 스키마의 유효성을 검사할 때 업로드한 행 및 열에 친근한 이름을 매핑할 수 있습니다. </p> <p> <b>고객 ID에 대하여</b> </p> <p>일반적으로 기업에서는 CRM 시스템의 고객 ID를 사용합니다. 이 ID는 사용자가 로그인할 때 <span class="codeph">setCustomerID</span> 호출을 사용하여 설정됩니다. 이 ID는 Experience Cloud에 업로드되는 CRM 파일의 키로도 사용됩니다. <a href="t-crs-usecase.md" format="dita" scope="local">별칭 ID</a>는 Audience Manager에서 별칭 데이터가 저장되는 데이터 저장소용의 친근한 이름입니다. 이 시스템에서는 별칭을 데이터 저장소(setCustomerID를 통해)로 보냅니다. CRM 파일은 이 데이터 저장소의 데이터에 적용됩니다. </p> <p><span class="codeph">setCustomerIDs</span> 정보에 대해서는 <a href="https://experienceleague.adobe.com/docs/id-service/using/reference/authenticated-state.html?lang=ko" format="https" scope="external">고객 ID 및 인증 상태</a>를 참조하십시오 . </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>후속 머리글 및 열 </p> </td> 
   <td colname="col2"> <p>후속 머리글은 각 속성의 이름을 나타내야 합니다. </p> <p> 이러한 열에는 CRM에서 가져오는 고객 속성이 포함되어야 합니다. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>속성 제한 </p> </td> 
   <td colname="col2"> <p>수백 개의 <span class="filepath"> .csv </span> 열을 Experience Cloud의 고객 특성 서비스에 업로드할 수 있습니다. 그렇지만 구독을 구성하고 속성을 선택할 때 보유하고 있는 애플리케이션에 따라 다음과 같은 제한이 적용됩니다. </p> <p> 
     <ul id="ul_2BB85067918D4BB3B59394F3E3E37A6D"> 
      <li id="li_93703988B9934384B4B94A839D028380"> <b>Analytics Standard</b>: 총 3개 </li> 
      <li id="li_D1E5E7BD24C54591B14D15DE97447835"> <b>Analytics Premium</b>: 보고서 세트당 200개 </li> 
      <li id="li_8C891FE3D1EF49FA9F81E2E32CD0B9CA"> <b>Adobe Target Standard:</b> 5개 </li> 
      <li id="li_2B66D43023F34EA685CE2C38A9250CEA"> <b>Adobe Target Premium:</b> 200개 </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>행 제한 </p> </td> 
   <td colname="col2"> <p>행 수에는 알려진 제한이 없습니다. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>열 제한 </p> </td> 
   <td colname="col2"> <p>실질적으로 열 수는 약 200개로 제한됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>문자 제한 </p> </td> 
   <td colname="col2"> <p>Analytics 구독을 생성할 때 업로드된 파일의 필드 길이는 255자로 잘립니다. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>FTP 지침 및 크기 제한 </p> </td> 
   <td colname="col2"> <p> 
     <ul id="ul_E157EE6F98914EADA0C103D1D1E705D3"> 
      <li id="li_84FBD455DD164A28AC16F4A5AB19E4B3">FTP의 최대 파일 크기 제한은 업로드당 4GB입니다. </li> 
      <li>최소 파일 크기 제한은 업로드당 10mb입니다. </li>
      <li>30분마다 1개 파일을 업로드할 수 있습니다. </li>
      <li id="li_B69A20C51D824727AA99C1F6F78537A4"> FTP 사이트의 루트 폴더에 <span class="filepath">.csv</span>(및 <span class="filepath">.fin</span>) 파일을 추가해야 합니다. </li> 
     </ul> </p> <p> <p>중요: FTP 계정에 대해 허용되는 총 공간은 40GB입니다. 처리된 파일을 삭제하는 것은 사용자의 책임입니다. </p> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>파일 요구 사항 </p> </td> 
   <td colname="col2"> <p> 각 속성 소스에는 동일한 수의 쉼표로 구분된 필드가 포함되어야 합니다. </p> <p> 줄 바꿈, 큰따옴표 또는 쉼표를 포함하는 필드는 따옴표로 묶어야 합니다. </p> <p> 필드의 큰따옴표 문자는 백슬래시(\)를 사용해서 이스케이프해야 합니다. </p> <p> 빈 열은 <span class="term"> null </span>로 저장됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>여러 파일 </p> </td> 
   <td colname="col2"> <p>고객 속성 데이터를 업로드할 때, 빠르게 연속해서 업로드할 파일이 여러 개 있으며 특히 파일이 큰 경우 다음 파일을 업로드하기 전에 이전 파일이 처리되었는지 확인하십시오. 이전 파일이 [!UICONTROL 고객 속성] FTP 계정 내에서 처리된 폴더 또는 실패한 폴더로 이동된 시기를 확인하여 이를 모니터링할 수 있습니다. </p> <p> 큰 파일을 작은 파일로 분할하여 빠르게 연속하여 제출하는 경우, 다음 파일을 제출하기 전에 각 파일이 완전히 처리되도록 하지 않는 한, 실제 처리 속도가 느려질 수 있습니다. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>문자 인코딩 </p> </td> 
   <td colname="col2"> <p>일본의 경우 UTF-8이 필수입니다. </p> </td> 
  </tr> 
   <tr> 
   <td colname="col1"> <p>이전 데이터 </p> </td> 
   <td colname="col2"> <p> 고객 속성은 [!DNL Analytics]의 기본 방문자 프로필에 연결되어 있습니다. 따라서 [!UICONTROL 고객 속성]은 [!DNL Analytics]의 해당 방문자 프로필 전체 수명 동안의 방문자와 연관되어 있습니다. 이 프로필에는 고객이 처음으로 로그인하기 전에 발생한 동작이 포함됩니다. </p> <p> Data Warehouse 채우기 방법을 사용하는 경우, 데이터는 Analytics ID(AID)를 기반으로 하는 post_visid_high/low에 연결되어 있습니다. Experience Cloud ID 서비스를 사용하는 경우 데이터는 Experience Cloud ID(MID)를 기반으로 하는 post_visid_high/low에 연결되어 있습니다. </p> <p> Data Warehouse 채우기 방법은 2022년 10월부터 더 이상 사용할 수 없습니다. </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>데이터 피드 </p> </td> 
   <td colname="col2"> <p>데이터 피드에서는 고객 속성을 사용할 수 없습니다. </p> </td> 
  </tr> 
 </tbody> 
</table>

## 여러 데이터 소스 사용 {#section_76DEB6001C614F4DB8BCC3E5D05088CB}

고객 속성 소스를 만들거나, 수정하거나, 삭제할 때, ID가 새 데이터 소스와의 동기화를 시작하기 전에 약 한 시간 정도의 지연이 있습니다.

각 고객 속성 소스에 대한 별칭 ID는 고유해야 합니다. 동일한 ID를 사용하는 데이터 소스가 여러 개 있는 경우, 다음과 같이 설정할 수 있습니다.

**Dynamic Tag Management의 VisitorAPI.js 또는 Experience Cloud ID 도구에서 다음을 수행합니다.**

다음과 같이 적절한 데이터 소스에 해당하는 두 개의 고객 ID를 설정합니다.

```
Visitor.setCustomerIDs({ 
     "ds_id1":"123456", 
     "ds_id2":"123456" 
});
```

(자세한 내용은 [고객 ID 및 인증 상태](https://experienceleague.adobe.com/docs/id-service/using/reference/authenticated-state.html?lang=ko)를 참조하십시오.)

**[!UICONTROL Experience Cloud]** > **[!UICONTROL 사용자]** > **[!UICONTROL 고객 속성]**&#x200B;에서 다음을 수행합니다.

위의 고객 ID에 해당하는 고유한 별칭 ID를 사용하여 두 개의 고객 속성 소스를 만듭니다. 이 방법을 사용하면 동일한 참조 ID를 여러 고객 속성 소스로 보낼 수 있습니다.
