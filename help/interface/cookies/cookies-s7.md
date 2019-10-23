---
description: Scene7은 쿠키를 사용하여 브라우저에 동적 미디어 제공 시 사용할 수 있는 유용한 정보를 저장합니다.
keywords: cookies;privacy
seo-description: Scene7은 쿠키를 사용하여 브라우저에 동적 미디어 제공 시 사용할 수 있는 유용한 정보를 저장합니다.
seo-title: Scene7 쿠키
solution: Marketing Cloud,Analytics,Target,Social
title: Scene7 쿠키
uuid: f9b9d13a-17e5-4139-8c84-6fe5d22c4196
translation-type: tm+mt
source-git-commit: 012283d79bda42f9dabb20b25903927b075f6d54

---


# Scene7 쿠키{#scene-cookies}

Scene7은 쿠키를 사용하여 브라우저에 동적 미디어 제공 시 사용할 수 있는 유용한 정보를 저장합니다.

Scene7은 이전의 일부 AS2 플래시 기반 뷰어에 대한 정보를 로컬에 저장합니다.

AS2 뷰어의 경우, 쿠키:

* 현재 페이지 및 이미지 보기, 현재 확대/축소 수준 등과 같은 사용자의 세션 상태를 추적합니다.
* 사용자의 이전 세션 이후 경과된 시간을 확인합니다. 뷰어는 이 정보를 사용하여 이전 세션을 계속 진행할지 또는 새 세션을 시작할지를 결정합니다. 이 정보는 Scene7 서버에도 전송되지만 사용되지는 않습니다.

AS2 Flash eCatalog 뷰어의 경우, 쿠키:

* 사용자가 생성한 컨텐츠(특히 전자 카탈로그 뷰어의 "스티커 메모" 기능에서 사용자가 입력한 컨텐츠)를 저장합니다. 이 컨텐츠는 사용자가 세션을 다시 시작할 때 복원됩니다.
* 사용자가 전자 카탈로그를 다른 사용자와 공유하기 위해 이메일을 시작하면 두 번째 AS2 뷰어 글머리 기호의 스티커 메모 컨텐츠가 서버에 복사되어 수신자에게 제공됩니다. 수신자가 뷰어 세션을 시작하면 스티커 메모 컨텐츠를 서버에서 검색하고 쿠키에 복사합니다. 이 기능은 거의 사용되지 않으므로 만료되지 않고 오래된 콘텐츠는 제거되지 않습니다. 현재 서버에 무기한으로 지속되고 있습니다.

최신 AS3 뷰어는 세션 지속성을 구현하지 않습니다.

**쿠키 이름: VatLogin.jsp**

| 특성 | 설명 |
|---|---|
| 저장되는 정보 | 세션 쿠키를 설정합니다. IPS ImageServer(IS, IR 및 SWFs/skins와 동영상 컨텍스트)에 삽입된 AuthFilter는 쿠키를 사용해 액세스를 승인합니다. 이 쿠키가 있는 경우, HTTP 요청이 통과하도록 허용합니다. 그렇지 않으면 권한이 없다는 메시지를 표시합니다. |
| 만료 | 이 쿠키는 세션 쿠키입니다. 현재 세션 만료는 Scene7 IPS [!DNL web.xml]에 45분으로 설정되어 있습니다. |

**쿠키 이름: s7js.flyout.InfoMessage.displayed`assetId`.state**

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
   <td colname="col2"> <p>&lt;assetId&gt;는 뷰어가 작동하고 있는 자산의 이름입니다. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> 만료 </td> 
   <td colname="col2"> 이 쿠키는 세션 쿠키로 브라우저를 닫으면 만료됩니다. </td> 
  </tr> 
 </tbody> 
</table>

**쿠키 이름: s7js.flyout.InfoMessage.displayed`assetId`_idx`id`.ant**

기존 DHTML 뷰어에서 상태 정보와 스티커 노트 데이터를 저장하기 위해 브라우저 쿠키를 사용합니다. 또한, 멀티스크린 DHTML 플라이아웃에서 메시지 표시기를 세션별로 만들도록 하기 위해 사용합니다.

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
   <td colname="col2"> <p> </p> <p> &lt;assetId&gt;는 뷰어가 작동하는 자산의 이름이며 &lt;id&gt;는 0을 기반으로 하는 스티커 노트 색인입니다. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> 만료 </td> 
   <td colname="col2"> 이 쿠키는 세션 쿠키로 브라우저를 닫으면 만료됩니다. </td> 
  </tr> 
 </tbody> 
</table>

