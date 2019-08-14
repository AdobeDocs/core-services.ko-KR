---
description: Survey는 쿠키를 사용하여 서로 다른 브라우저의 요청을 구분하고 고객 감정을 더 잘 이해하는 데 사용되는 유용한 정보를 저장합니다.
keywords: cookies;privacy
seo-description: Survey는 쿠키를 사용하여 서로 다른 브라우저의 요청을 구분하고 고객 감정을 더 잘 이해하는 데 사용되는 유용한 정보를 저장합니다.
seo-title: Survey 쿠키
solution: Marketing Cloud,Analytics,Target,Social
title: Survey 쿠키
uuid: e57d9b58-3c62-463a-ad52-e2a0de2e1ee1
index: y
internal: n
snippet: y
translation-type: tm+mt
source-git-commit: 426c1fecf16e1cf83cd28971e4de6fdb66b0e10d

---


# Survey 쿠키{#survey-cookies}

Survey는 쿠키를 사용하여 서로 다른 브라우저의 요청을 구분하고 고객 감정을 더 잘 이해하는 데 사용되는 유용한 정보를 저장합니다.

* [쿠키 이름: s_sv_sid](../cookies-overview/cookies-survey.md#section-03aa90aa7e36427b8cb12dc4a0f0291e)
* [쿠키 이름: s_sv_s1](../cookies-overview/cookies-survey.md#section-14ad50dfcd7342f9ac80283b1f0d3400)
* [쿠키 이름: s_sv_p1](../cookies-overview/cookies-survey.md#section-05d1c52c478541609f4a18a9c1eb032f)

## 쿠키 이름: s_sv_sid {#section-03aa90aa7e36427b8cb12dc4a0f0291e}

| 특성 | 설명 |
|---|---|
| 저장되는 정보 | 브라우저 내의 설문 조사를 렌더링하는 데 사용되는 JavaScript 파일을 제대로 캐싱할 수 있도록 고유한 숫자를 저장합니다. |
| 만료 | 이 쿠키는 세션 쿠키로 브라우저를 닫으면 만료됩니다. |

## 쿠키 이름: s_sv_s1 {#section-14ad50dfcd7342f9ac80283b1f0d3400}

<table id="table_6835D64C5D464A049F576621F2BE3FAD"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> 특성 </th> 
   <th colname="col2" class="entry"> 설명 </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> 저장되는 정보 </td> 
   <td colname="col2"> <p> 
     <ul id="ul_350369AFBEFF49938026D7D25D012A88"> 
      <li id="li_EA3D03382BFA474B802D1EE2054FABDB">설문 조사를 하도록 메시지가 표시되었을 때 방문자가 "나중에"를 클릭하여 연기한 설문 조사의 ID를 저장합니다. </li> 
      <li id="li_6111E8D568D64D7CBFB906046134025C"> 웹사이트의 다음 페이지에서 시작할 수 있는 설문 조사 ID를 저장합니다. </li> 
      <li id="li_A16519F487654435B50577DA08654E70">시작된 설문 조사 ID를 저장합니다. </li> 
      <li id="li_8322C91846AB4A65B277C435D61660BF">Survey 시스템이 실행되기 시작한 시간을 저장합니다(지연된 설문 조사용). </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> 만료 </td> 
   <td colname="col2"> 이 쿠키는 세션 쿠키로 브라우저를 닫으면 만료됩니다. </td> 
  </tr> 
 </tbody> 
</table>

## 쿠키 이름: s_sv_p1 {#section-05d1c52c478541609f4a18a9c1eb032f}

<table id="table_8F6CC83D32D54BEE99884318AD126C98"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> 특성 </th> 
   <th colname="col2" class="entry"> 설명 </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> 저장되는 정보 </td> 
   <td colname="col2"> <p> 
     <ul id="ul_A2717AD89DA540468963E9E7FBD382D5"> 
      <li id="li_21B0165911C74BA796111E9C93142B95">수행되었거나 거부된 설문 조사 ID를 저장합니다. </li> 
      <li id="li_DD966285CAE7438C9E43AFC4E91569F8">방문자가 샘플링 비율에 일치했는지 여부를 지정하는 정보를 저장합니다. </li> 
      <li id="li_27BD16FE78BC46C3846BFFE4DF65BCB3">사이트 종료 설문 조사를 시작할 때 사용되는 증가 수를 저장하여 방문자가 해당 사이트를 떠났는지 확인합니다. </li> 
      <li id="li_0C9FF8939615407BB9A0DB24C7C31CE6">방문자가 고객 지정 사용 유무 설정을 사용했으므로 설문 조사에서 제외해야 할지 여부를 나타내는 플래그를 저장합니다. </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> 만료 </td> 
   <td colname="col2"> 이 쿠키는 지속적입니다. </td> 
  </tr> 
 </tbody> 
</table>

<a id="section_488AFFB899004968A2479B2423E6EEB7"></a>

>[!NOTE]
>
>s_sv_s1 또는 s_sv_p1에 저장될 정보가 너무 큰 경우 필요에 따라 분산되어 추가 쿠키에 저장되며, s_sv_s2, s_sv_s3 등으로 또는 s_sv_p2, s_sv_p3 등으로 이름이 지정됩니다.

