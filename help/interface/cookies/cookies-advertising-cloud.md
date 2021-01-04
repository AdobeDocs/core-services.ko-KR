---
description: 광고 참여 이벤트를 전환 이벤트에 매핑하고 해당 정보를 사용하여 광고 입찰을 최적화하는 Adobe Ad Cloud 쿠키에 대해 알아봅니다.
title: 'Advertising Cloud 쿠키 '
uuid: 2eec48a3-3e81-488e-8e30-5fd62885de0b
translation-type: tm+mt
source-git-commit: 3f26c1af19a0838913eec2b4135304f5f3fcf0b4
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 100%

---


# Advertising Cloud 쿠키{#advertising-cloud-cookies}

Advertising Cloud는 쿠키를 사용하여 광고 참여 이벤트를 전환 이벤트에 매핑하고 해당 정보를 사용하여 광고 입찰을 최적화합니다.

## 쿠키 이름: _lcc

<table id="table_821F8EBE91F244CBA72B0975B961B908"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> 특성 </th> 
   <th colname="col2" class="entry"> 설명 </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>정보가 저장됨 </p> </td> 
   <td colname="col2"> <p>검색 클릭 수의 ID 및 타임스탬프(yyyymmdd 형식)</p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>만료 </p> </td> 
   <td colname="col2"> <p>15분</p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>사용 </p> </td> 
   <td colname="col2"> <p>디스플레이 광고의 클릭 이벤트가 Adobe Analytics 히트에 적용되는지를 판별하는 데 사용되는 타사 쿠키 </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>위치 </p> </td> 
   <td colname="col2"> <p>everesttech.net </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>크기 </p> </td> 
   <td colname="col2"> <p>52바이트 </p> </td> 
  </tr> 
 </tbody> 
</table>

## 쿠키 이름: _tmae

<table id="table_28C2B62595E240D5A3C3E0BE147748C1"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> 특성 </th> 
   <th colname="col2" class="entry"> 설명 </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>정보가 저장됨 </p> </td> 
   <td colname="col2"> <p>Advertising Cloud DSP 추적을 사용한 광고 참여용 인코딩된 ID 및 타임스탬프 </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>만료 </p> </td> 
   <td colname="col2"> <p>1년 </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>사용 </p> </td> 
   <td colname="col2"> <p>"2016년 6월 30일에 마지막으로 본 광고 xyz123"과 같이 사용자의 참여를 광고로 저장하는 타사 쿠키 </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>위치 </p> </td> 
   <td colname="col2"> <p>everesttech.net </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>크기 </p> </td> 
   <td colname="col2"> <p>변수, 데이터가 인코딩되고 일반적으로 1KB보다 적음 </p> </td> 
  </tr> 
 </tbody> 
</table>

## 쿠키 이름: adcloud

<table id="table_D7CD238736BC4571883F92F47673F57C"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> 특성 </th> 
   <th colname="col2" class="entry"> 설명 </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>정보가 저장됨 </p> </td> 
   <td colname="col2"> <p>광고주의 웹 사이트에 대한 서퍼의 마지막 방문과 서퍼의 마지막 검색 클릭의 타임스탬프 및 사용자가 광고를 클릭할 때 생성된 ef_id</p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>만료 </p> </td> 
   <td colname="col2"> <p>2년 </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>사용 </p> </td> 
   <td colname="col2"> <p>서퍼 ID를 관련 대상 세그먼트 및 전환과 연관시키는 자사 쿠키 </p> <p> 마지막 방문에 대한 정보는 Adobe 서버에 대한 불필요한 요청을 방지하여 페이지 로드 횟수를 최적화하는 데 사용됩니다. </p> <p>마지막 검색 클릭에 대한 정보는 전환 이벤트가 클릭 또는 뷰스루의 결과(클릭 없는 노출 횟수에서의 전환 결과)라면 결정하는 데 도움이 됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>위치 </p> </td> 
   <td colname="col2"> <p>광고주의 최상위 수준 도메인(예: example.com) </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>크기 </p> </td> 
   <td colname="col2"> <p>변수이지만 일반적으로 50~150바이트 </p> </td> 
  </tr> 
 </tbody> 
</table>

## 쿠키 이름: ev_sync_*

(ev_sync_ax, ev_sync_bk, ev_sync_dd, ev_sync_fs, ev_sync_ix, ev_sync_nx, ev_sync_ox, ev_sync_pm, ev_sync_rc, ev_sync_tm, ev_sync_yh)

<table id="table_A05C02AB261946E0AABAD78259392D81"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> 특성 </th> 
   <th colname="col2" class="entry"> 설명 </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>정보가 저장됨 </p> </td> 
   <td colname="col2"> <p>yyyymmdd 형식으로 동기화가 수행되는 날짜 </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>만료 </p> </td> 
   <td colname="col2"> <p>yyyymmdd 형식으로 동기화가 수행되는 날짜 </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>사용 </p> </td> 
   <td colname="col2"> <p>Advertising Cloud 서퍼 ID를 파트너 광고 교환과 동기화하는 타사 광고 교환 관련 쿠키. 새 서퍼에 대해 작성되며, 기간이 만료되면 동기화 요청을 보냅니다. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>위치 </p> </td> 
   <td colname="col2"> <p>everesttech.net </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>크기 </p> </td> 
   <td colname="col2"> <p>8자 </p> </td> 
  </tr> 
 </tbody> 
</table>

## 쿠키 이름: everest_g_v2

<table id="table_04043292A43B41B69EAF17AF4E217C69"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> 특성 </th> 
   <th colname="col2" class="entry"> 설명 </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>정보가 저장됨 </p> </td> 
   <td colname="col2"> <p>브라우저 및 서퍼 ID </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>만료 </p> </td> 
   <td colname="col2"> <p>2년 </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>사용 </p> </td> 
   <td colname="col2"> <p>사용자가 처음에 클라이언트의 광고를 클릭한 후, 클라이언트의 웹 사이트에서 현재 및 이후 클릭 수를 다른 이벤트와 매핑하는 데 사용됩니다. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>위치 </p> </td> 
   <td colname="col2"> <p>everesttech.net </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>크기 </p> </td> 
   <td colname="col2"> <p>~27자 </p> </td> 
  </tr> 
 </tbody> 
</table>

## 쿠키 이름: everest_session_v2

<table id="table_1A3AE4CA71304ADB943CB1F64BE695F5"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> 특성 </th> 
   <th colname="col2" class="entry"> 설명 </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>정보가 저장됨 </p> </td> 
   <td colname="col2"> <p>세션 ID </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>만료 </p> </td> 
   <td colname="col2"> <p>브라우저를 종료하는 경우 </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>사용 </p> </td> 
   <td colname="col2"> <p>타사 브라우저 세션 쿠키, 하나의 쿠키가 모든 계정에 사용됨 </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>위치 </p> </td> 
   <td colname="col2"> <p>everesttech.net </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>크기 </p> </td> 
   <td colname="col2"> <p>~16자 </p> </td> 
  </tr> 
 </tbody> 
</table>

## 쿠키 이름: ev_tm

<table id="table_6C4D9DCFA4BF4FB2BD445E027550955F"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> 특성 </th> 
   <th colname="col2" class="entry"> 설명 </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>정보가 저장됨 </p> </td> 
   <td colname="col2"> <p>Advertising Cloud DSP(Demand Side Platform) ID </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>만료 </p> </td> 
   <td colname="col2"> <p>2년 </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>사용 </p> </td> 
   <td colname="col2"> <p>everest_g_v2 cookie 쿠키의 서퍼 ID에 해당하는 DSP ID를 저장하는 타사 쿠키 </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>위치 </p> </td> 
   <td colname="col2"> <p>everesttech.net </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>크기 </p> </td> 
   <td colname="col2"> <p>~20바이트 </p> </td> 
  </tr> 
 </tbody> 
</table>

## 쿠키 이름: id_adcloud

<table> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> 특성 </th> 
   <th colname="col2" class="entry"> 설명 </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>정보가 저장됨 </p> </td> 
   <td colname="col2"> <p>서퍼 ID </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>만료 </p> </td> 
   <td colname="col2"> <p>91일 </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>사용 </p> </td> 
   <td colname="col2"> <p>쿠키가 자사 도메인에 설정되었지만 아직 사용되지 않음 </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>위치 </p> </td> 
   <td colname="col2"> <p>광고주의 최상위 수준 도메인(예: example.com) </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>크기 </p> </td> 
   <td colname="col2"> <p>16바이트 </p> </td> 
  </tr> 
 </tbody> 
</table>
