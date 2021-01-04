---
description: Adobe Target에서 어떻게 쿠키를 사용하여 어떤 온라인 컨텐츠 및 오퍼가 방문자와 밀접한 관련이 있는지 테스트하는 기능을 웹 사이트 운영자에게 제공하는지 알아봅니다.
keywords: cookies;privacy
solution: Experience Cloud,Analytics,Target,Social
title: 'Adobe Target 쿠키 사용 방법 '
uuid: 44f7e32e-8d99-4682-8b54-8364d001b403
translation-type: tm+mt
source-git-commit: 3f26c1af19a0838913eec2b4135304f5f3fcf0b4
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 97%

---


# Adobe Target 쿠키{#target-cookies}

Adobe Target은 쿠키를 사용하여 웹 사이트 운영자가 어떤 온라인 컨텐츠 및 오퍼가 방문자와 관련이 있는지 테스트할 수 있도록 합니다.

필요하면 이러한 설정을 쿠키 지속 시간은 제외하고 변경할 수 있습니다. 쿠키 설정을 변경하는 경우 계정 담당자에게 문의하십시오.

>[!NOTE]
>
>Adobe Target 사용자는 사용자 지정 타사 쿠키를 생성할 수도 있습니다.

<table id="table_54B402C6E19C4A70B1E27BC9DFF776EB"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> 설정 </th> 
   <th colname="col2" class="entry"> 정보 </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>쿠키 이름 </p> </td> 
   <td colname="col2"> <p>mbox. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>쿠키 도메인 </p> </td> 
   <td colname="col2"> <p>mbox를 제공하는 도메인의 두 번째 및 최상위 수준입니다. 회사 도메인에서 제공되기 때문에 쿠키는 자사 쿠키입니다. 예: <span class="filepath">mycompany.com</span>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>서버 도메인 </p> </td> 
   <td colname="col2"> <p> <span class="filepath">clientcode.tt.omtrdc.net</span>(Adobe Target 계정에 대해 클라이언트 코드 사용) </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>쿠키 지속 시간 </p> </td> 
   <td colname="col2"> <p>쿠키는 마지막 로그인부터 2년 동안 방문자 브라우저에 유지됩니다. 쿠키 지속 시간은 변경할 수 없습니다. </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>도메인 이름에 [!DNL mycompany.co.uk]와 같은 국가 코드가 포함되어 있는 경우 클라이언트 서비스와 작업하여 이 코드를 지원하도록 [!DNL mbox.js]를 구성하십시오.

쿠키는 방문자가 Adobe Target 캠페인을 경험하는 방식을 관리하기 위해 많은 값을 유지합니다.

<table id="table_5245F72A2D5A4322B40ABB10B7DFB338"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> 값 </th> 
   <th colname="col2" class="entry"> 정의 </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"> session ID</span> </p> </td> 
   <td colname="col2"> <p>사용자 세션의 고유 ID입니다. 기본적으로 30분 동안 지속됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"> pc ID</span> </p> </td> 
   <td colname="col2"> <p>방문자 브라우저의 반영구 ID입니다. 쿠키가 수동으로 삭제될 때까지 지속됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"> check</span> </p> </td> 
   <td colname="col2"> <p>방문자가 쿠키를 지원하는지 여부를 확인하는 간단한 테스트 값입니다. 방문자가 페이지를 요청할 때마다 설정합니다. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"> disable</span> </p> </td> 
   <td colname="col2"> <p>방문자의 로드 시간이 <span class="filepath">mbox.js</span> 파일에 구성된 시간을 초과하는 경우 설정됩니다. 기본적으로 1시간 동안 지속됩니다. </p> </td> 
  </tr> 
 </tbody> 
</table>

