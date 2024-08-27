---
description: Adobe Experience Cloud의 Audience Manager 쿠키에 대해 알아봅니다.
keywords: 쿠키
solution: Experience Cloud, Audience Manager
title: Audience Manager 쿠키
uuid: 8b384c38-b85a-4e93-b00e-41a9d3ae2b21
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: ab6de845-99ea-4cd8-b7cd-012fb641403f
source-git-commit: 2a80851c0a7d4ef7dbcc2565177b239f3e063164
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 99%

---

# Audience Manager 쿠키{#audience-manager-cookies}

Audience Manager는 몇 가지 간단한 쿠키를 사용하여 다양한 기능을 수행합니다. 이러한 기능에는 ID 할당, 데이터 호출 기록, 오류 추적 및 쿠키 설정 여부 테스트 등이 포함됩니다. 이 섹션에서는 Audience Manager에서 설정한 다양한 쿠키를 나열하고 설명합니다.

**demdex 쿠키**

<table id="table_1CCF7EA2BC9E421F8DEECA5F611E33F6"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> 속성 </th> 
   <th colname="col2" class="entry"> 설명 </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <b>용도</b> </p> </td> 
   <td colname="col2"> <p> <span class="keyword"> Audience Manager</span>는 이 쿠키를 설정하여 사이트 방문자에게 고유 ID를 할당합니다. <span class="wintitle"> demdex </span> 쿠키는 <span class="keyword"> Audience Manger </span>가 방문자 식별, ID 동기화, 세분화, 모델링, 보고 등과 같은 기본 기능을 수행하는 데 도움이 됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>콘텐츠</b> </p> </td> 
   <td colname="col2"> <p><span class="wintitle">demdex</span> 쿠키에는 아래 예와 같이 고유 사용자 ID(UUID)가 포함되어 있습니다. </p> <p> <span class="codeph"> 06151304227769720433039235178204449977 </span> </p> <p><a href="https://experienceleague.adobe.com/docs/audience-manager/user-guide/reference/ids-in-aam.html" format="https" scope="external">Audience Manager의 ID 색인</a>을 참조하십시오 . </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>기타 속성</b> </p> </td> 
   <td colname="col2"> <p> 
     <ul id="ul_11291DA87C5045E880034E06C863BCDA"> 
      <li id="li_40C30A06A12449A4A8748621223CA71B">라이프타임: <span class="wintitle"> demdex </span> 쿠키의 TTL(유지 기간)은 180일입니다. TTL은 각 사용자가 파트너 웹 사이트와 상호 작용할 때 180일로 재설정됩니다. 사용자가 TTL 간격 내에 해당 사이트를 다시 방문하지 않으면 쿠키가 만료됩니다. </li> 
      <li id="li_A589EDA2198249829207A183872EF1FF">옵트아웃: 사용자가 데이터 수집을 거부하는 경우 <span class="keyword">Audience Manager</span>는 <span class="codeph">Do Not Adobe Target</span> 문자열로 쿠키를 재설정합니다. 이 경우, 쿠키 TTL은 10년으로 설정됩니다. </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

**dextp 쿠키**

<table id="table_7343C9C9ADD24D3FA693ECC76E4A4045"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> 속성 </th> 
   <th colname="col2" class="entry"> 설명 </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <b>용도</b> </p> </td> 
   <td colname="col2"> <p> <span class="keyword"> Audience Manager</span>는 이 쿠키를 설정하여 마지막으로 데이터 동기화 호출을 수행한 시간을 기록합니다. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>콘텐츠</b> </p> </td> 
   <td colname="col2"> <p><span class="wintitle"> dextp </span> 쿠키에는 데이터 공급자 이름 또는 ID와,파이프로 구분된 문자열 형식의 UNIX UTC 타임스탬프가 들어 있습니다. 예에서 <i>기울임꼴</i>은 가변 자리 표시자를 나타냅니다. </p> <p> 
     <ul id="ul_80D0BC3FCF06470991E12712401D784A"> 
      <li id="li_03747A433CEB4756A26CD866E716B89D">이전 스타일: <span class="codeph"><span class="varname"> 데이터 공급자 이름 </span>-1490307822097| <span class="varname"> 데이터 공급자 이름 </span>-1490307822038 </span> </li> 
      <li id="li_79E7000E82DB4ADA9E9887B017343B2D">새 스타일: <span class="codeph">21-1-1490307821616|544-1-1490307821793|3-1-1490307821852|420-1-1490307822038| </span> </li> 
     </ul> </p> <p>아래의 dextp 데이터 구문 섹션을 참조하십시오. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>기타 속성</b> </p> </td> 
   <td colname="col2"> <p> 
     <ul id="ul_4922AC2CD55D4C888A6FBEB22F8B889B"> 
      <li id="li_91A68C44E53840379C2ACDED25468735">라이프타임: <span class="wintitle">dextp</span> 쿠키의 TTL(유지 기간)은 180일입니다. </li> 
      <li id="li_6B8C674EFAAC4DABA0A640CF29247F99">옵트아웃: 사용자가 데이터 수집을 거부하는 경우 <span class="keyword">Audience Manager</span>는 <span class="codeph">Do Not Adobe Target</span> 문자열로 쿠키를 재설정합니다. 이 경우, 쿠키 TTL은 10년으로 설정됩니다. </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

dextp 쿠키 데이터 구문:

다음 표는 `dextp` 쿠키의 요소들을 데이터 문자열의 위치별로 나열하고 정의합니다.

<table id="table_BE00604B97F24F5A94AA4F566063D785"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> 가변 위치 </th> 
   <th colname="col2" class="entry"> 설명 </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <b>첫 번째 또는 두 번째</b> </p> </td> 
   <td colname="col2"> <p>데이터 공급자 이름 또는 ID의 위치는, 쿠키가 새로운 스타일의 서식과 이전 스타일의 서식 중 어느 것을 사용하는지에 따라 다릅니다. </p> <p> <b>이전 스타일 서식:</b> </p> <p> 
     <ul id="ul_5BFBF40E3FE849CA859030F2D070FDF6"> 
      <li id="li_E8F4DC0CB15B472ABE9892B3A61D7F77">구문: <span class="codeph"> <span class="varname"> 데이터 공급자 이름 </span> - <span class="varname"> UNIX UTC 타임스탬프 </span> </span> </li> 
      <li id="li_7CD8B101156140F49EA97B18E9591402">예: <span class="codeph"> dataProvider1 - 1490307822038 </span> </li> 
     </ul> </p> <p>이전 스타일의 쿠키는 읽을 수 있는 이름으로 데이터 공급자를 식별합니다. </p> <p> <b>새 스타일 서식:</b> </p> <p> 
     <ul id="ul_AC6225CA781746148C125F21DFED1ED9"> 
      <li id="li_29C4B52E398B4EA28944980A15B05A57">구문: <span class="codeph"> <span class="varname"> 데이터 공급자 ID </span> - 1|2 - <span class="varname"> UNIX UTC 타임스탬프 </span> </span> </li> 
      <li id="li_3BF30CA5FED242DF96E0B54AFC64B06F">예: <span class="codeph"> 123345 - 1 - 1490307822038 </span> </li> 
     </ul> </p> <p>새 스타일 쿠키: </p> <p> 
     <ul id="ul_F05A91A455FA44C7A71186C0C9E31630"> 
      <li id="li_A8C9638173684359BABC4207845A4F48">읽을 수 있는 데이터 공급자 이름을 숫자 ID로 바꿉니다. </li> 
      <li id="li_28F1E2DB24904E53BE9718AD788CE61E">ID 1 또는 ID 2로 통화 유형을 식별합니다. ID 1은 ID 동기화 호출을 나타냅니다. ID 2는 더 이상 사용되지 않는 호출을 나타냅니다. ID 2의 dextp 쿠키는 많지 않거나 없어야 합니다. </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>마지막</b> </p> </td> 
   <td colname="col2"> <p>마지막 위치에는 UNIX UTC 타임스탬프가 포함됩니다. </p> </td> 
  </tr> 
 </tbody> 
</table>

**dst 쿠키**

<table id="table_83AE9B6350C6408BAECD9FCF33022B98"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> 속성 </th> 
   <th colname="col2" class="entry"> 설명 </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <b>용도</b> </p> </td> 
   <td colname="col2"> <p> <span class="keyword"> Audience Manager</span>가 데이터를 <a href="https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/destinations/destinations.html" format="https" scope="external">대상</a>에 전송하는 중 오류가 발생하면 이 쿠키를 설정합니다 . </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>콘텐츠</b> </p> </td> 
   <td colname="col2"> <p> <span class="wintitle">DST</span> 쿠기에는 파이프로 구분된 문자열 형식의 대상 ID 및 UNIX 타임스탬프 세트가 들어 있습니다. 예에서 <i>기울임꼴</i>은 가변 자리 표시자를 나타냅니다. </p> <p> 
     <ul id="ul_CE98076A02DA413486C1D341E9806889"> 
      <li id="li_850209D956644749B98C7A208C825C15">구문: <span class="codeph"> <span class="varname"> 대상 ID </span> - <span class="varname"> UNIX UTC 타임스탬프 </span> </span> </li> 
      <li id="li_4A22152C70844733982230EBF7B9EB78">예: <span class="codeph">067797-1490349684|1010788-1490349692|1067797-1490349692 </span> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>기타 속성</b> </p> </td> 
   <td colname="col2"> <p> 
     <ul id="ul_5D13DD701B484B51BF2808A69A919106"> 
      <li id="li_4E665114C63246FBA32A4E19984D2693">라이프타임: <span class="wintitle">dst</span> 쿠키의 ttl(유지 기간)은 180일입니다. </li> 
      <li id="li_A682B566704F43D2AB72487EFF212474">옵트아웃: 사용자가 데이터 수집을 거부하는 경우 <span class="keyword">Audience Manager</span>는 <span class="codeph">Do Not Adobe Target</span> 문자열로 쿠키를 재설정합니다. </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

**_dp 쿠키**

이 쿠키는 일시적입니다. [!DNL Audience Manager]는 `_dp` 쿠키를 설정하여 서드파티 컨텍스트에서 demdex.net 도메인의 다른 쿠키를 설정할 수 있는지 확인합니다. `_dp`이(가) 설정되면 값 1이 포함됩니다. [!DNL Audience Manager]는 이 값을 읽고 즉시 쿠키를 제거합니다. `_dp` 쿠키가 없으면 [!DNL Audience Manager]는 쿠키를 설정할 수 없다는 것을 알게 됩니다.
