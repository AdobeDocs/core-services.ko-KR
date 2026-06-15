---
description: ID 서비스가 CX 엔터프라이즈 애플리케이션 간에 어떻게 저장되고 사용되는지 알아봅니다.
solution: Experience Cloud,Analytics,Target
title: Experience Cloud 쿠키
uuid: a4788c1c-0402-4fc8-b894-cd24fa794f4f
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: bd9bea58-9987-40d6-84e0-da185388bbbb
TQID: https://experienceleague.adobe.com/2i8AyRTW37TGYTpcLBh-ZMTyET0NvpRweTnUuk8Nnis
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
  - id: e43347a8-f2c5-4aa4-8623-6f13875d7e3a
  - id: e55547f1-a1ff-40c6-8978-026e40ab7fa4
feature_v2:
  - id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
subfeature_v2:
  - id: b75843fa-0a67-4a44-a6b1-cc627b0481dc
  - id: fef08361-6ac5-460c-93fe-d063e40b6a49
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 50012e2564e88e1a6e16578e3331136c7df0cb21
workflow-type: tm+mt
source-wordcount: 370
ht-degree: 77%

---

# CX 엔터프라이즈 쿠키

Adobe CX Enterprise는 쿠키를 사용하여 CX 엔터프라이즈 애플리케이션에서 사용되는 방문자 ID를 저장합니다. 이러한 쿠키는 특히 [experience.adobe.com](https://experience.adobe.com)에서 Adobe CX 엔터프라이즈 응용 프로그램에 액세스하는 데 적용됩니다.

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
   <td colname="col1"> <p>정보가 저장됨 </p> </td> 
   <td colname="col2"> <p> CX Enterprise ID(ECID) 또는 MID의 사본을 포함합니다. MID는 이 구문, s_ecid=MCMID|&lt;ECID&gt;를 따르는 키-값 쌍에 저장됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> 만료 </p> </td> 
   <td colname="col2"> <p>2년, 대부분의 최신 브라우저는 13개월로 잘립니다.</p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> 사용 </p> </td> 
   <td colname="col2"> <p>이 쿠키는 클라이언트가 AMCV 쿠키를 설정한 후에 고객의 도메인에 의해 설정됩니다. 이 쿠키의 목적은 자사 상태의 지속적인 ID 추적을 허용하는 것이며 AMCV 쿠키가 만료된 경우 참조 ID로 사용됩니다. 자세한 내용은 AMCV 쿠키를 확인하십시오. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> 위치 </p> </td> 
   <td colname="col2"> <p>CNAME 고객에게만 해당됩니다. 서드파티 시나리오에 해당되지 않습니다. 쿠키는 CNAME 및 Analytics 이미지 요청에 사용된 동일한 도메인에 저장됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> 크기 </p> </td> 
   <td colname="col2"> <p>45바이트 </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> SameSite=Lax </p> </td> 
   <td colname="col2"> <p>이 설정을 사용하는 쿠키는 브라우저의 URL에 표시된 도메인이 쿠키의 도메인과 일치하는 경우에만 전송됩니다. 이 설정은 Chrome에서 쿠키의 새로운 기본값입니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

**쿠키 이름: AMCV_###@AdobeOrg**

[Experience Platform ID 서비스](https://experienceleague.adobe.com/docs/id-service/using/home.html?lang=ko) 는 JavaScript를 사용하여 현재 웹 사이트의 도메인에 있는 `AMCV_###@AdobeOrg` 쿠키에 고유한 방문자 ID를 저장합니다. 여기서 `###` 는 `AMCV_1FD6776A524453CC0A490D44%40AdobeOrg.`와 같은 임의의 문자열을 나타냅니다.

[쿠키 및 ID 서비스](https://experienceleague.adobe.com/docs/id-service/using/intro/cookies.html)도 참조하십시오.

<table id="table_1883C0836C1E4AF5A262FBF5000C1B11"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> <p>속성 </p> </th> 
   <th colname="col2" class="entry"> <p>설명 </p> </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>정보가 저장됨 </p> </td> 
   <td colname="col2"> <p> CX 엔터프라이즈 솔루션에서 사용하는 고유 방문자 ID. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> 만료 </p> </td> 
   <td colname="col2"> <p> 13개월 </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> 사용 </p> </td> 
   <td colname="col2"> <p> 이 쿠키는 고유한 방문자를 식별하는 데 사용됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> 위치 </p> </td> 
   <td colname="col2"> <p> 이 쿠키는 웹 사이트의 도메인에서 저장됩니다(이미지 요청의 도메인이 아님). </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> 크기 </p> </td> 
   <td colname="col2"> <p> 다양하며, 대부분의 고객은 이 쿠키의 길이가 약 200바이트 정도 될 것으로 예상할 수 있습니다. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>추가된 값이 없습니다. Chrome 기본값은 Lax입니다. </p> </td> 
   <td colname="col2"> <p> 이 설정을 사용하는 쿠키는 브라우저의 URL에 표시된 도메인이 쿠키의 도메인과 일치하는 경우에만 전송됩니다. 이 설정은 Chrome에서 쿠키의 새로운 기본값입니다. </p> </td> 
  </tr> 
 </tbody> 
</table>

