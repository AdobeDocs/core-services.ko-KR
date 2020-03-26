---
description: Adobe Experience Cloud는 쿠키를 사용하여 Experience Cloud 솔루션에서 사용되는 방문자 ID를 저장합니다.
keywords: cookies;privacy
seo-description: Adobe Experience Cloud는 쿠키를 사용하여 Experience Cloud 솔루션에서 사용되는 방문자 ID를 저장합니다.
seo-title: Experience Cloud 쿠키
solution: Marketing Cloud,Analytics,Adobe Target,Adobe Social
title: Experience Cloud 쿠키
uuid: a4788c1c-0402-4fc8-b894-cd24fa794f4f
translation-type: tm+mt
source-git-commit: f7ec8bf6087a18be41c9efbf05f60e6cfd24e566

---


# Experience Cloud 쿠키{#experience-cloud-cookies}

Adobe Experience Cloud는 쿠키를 사용하여 Experience Cloud 솔루션에서 사용되는 방문자 ID를 저장합니다.

**쿠키 이름: s_ecid**

<table id="table_FF4C70D3D4CC425BA65162D5A9504F7D"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> <p>속성 </p> </th> 
   <th colname="col2" class="entry"> <p>설명 </p> </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>저장된 정보 </p> </td> 
   <td colname="col2"> <p> Experience Cloud ID(ECID) 또는 MID의 사본을 포함합니다. MID는 이 구문, s_ecid=MCMID|&lt;ECID&gt;를 따르는 키-값 쌍에 저장됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> 만료 </p> </td> 
   <td colname="col2"> <p>2년 </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> 사용 </p> </td> 
   <td colname="col2"> <p>이 쿠키는 클라이언트가 AMCV 쿠키를 설정한 후에 고객의 도메인에 의해 설정됩니다. 이 쿠키의 목적은 퍼스트 파티 상태에서 영구 ID 추적을 허용하기 위한 것이며, AMCV 쿠키가 만료된 경우 참조 ID로 사용됩니다. 자세한 내용은 AMCV 쿠키를 확인하십시오. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> 위치 </p> </td> 
   <td colname="col2"> <p>CNAME 고객에게만 해당됩니다. 타사 시나리오에 해당되지 않습니다. 쿠키는 CNAME 및 Analytics 이미지 요청에 사용된 동일한 도메인에 저장됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> 크기 </p> </td> 
   <td colname="col2"> <p>45바이트 </p> </td> 
  </tr> 
 </tbody> 
</table>

**쿠키 이름: AMCV_###@AdobeOrg**

The [Experience Platform ID Service](https://docs.adobe.com/content/help/en/id-service/using/home.html) uses JavaScript to store a unique visitor ID in an `AMCV_###@AdobeOrg` cookie on the domain of the current website, where `###` represents a random string of characters, such as `AMCV_1FD6776A524453CC0A490D44%40AdobeOrg.`

See also, [Cookies and the ID Service](https://docs.adobe.com/content/help/en/id-service/using/intro/cookies.html).

<table id="table_1883C0836C1E4AF5A262FBF5000C1B11"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> <p>속성 </p> </th> 
   <th colname="col2" class="entry"> <p>설명 </p> </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>저장된 정보 </p> </td> 
   <td colname="col2"> <p> Experience Cloud 솔루션에 사용되는 고유 방문자 ID. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> 만료 </p> </td> 
   <td colname="col2"> <p> 2년 </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> 사용 </p> </td> 
   <td colname="col2"> <p> 이 쿠키는 고유 방문자를 식별하는 데 사용됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> 위치 </p> </td> 
   <td colname="col2"> <p> 이 쿠키는 이미지 요청의 도메인이 아닌 웹 사이트의 도메인에 저장됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> 크기 </p> </td> 
   <td colname="col2"> <p> 다양하지만 대부분의 고객은 이 쿠키의 길이가 약 200바이트라고 예상할 수 있습니다. </p> </td> 
  </tr> 
 </tbody> 
</table>
