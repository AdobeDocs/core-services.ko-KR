---
description: Analytics 및 Target의 고객 속성에 대한 FAQ 및 우수 사례입니다.
keywords: 고객 속성
seo-description: Analytics 및 Target의 고객 속성에 대한 FAQ 및 우수 사례입니다.
seo-title: FAQ, 제한 사항 및 우수 사례
solution: Experience Cloud
title: FAQ, 제한 사항 및 우수 사례
uuid: E 93 EB 531-23 C 7-4 D 75-92 E 8-75699 F 58546 A
translation-type: tm+mt
source-git-commit: 08c2caa1e0e5ca5c487294e9ce33600dde9c9a1e

---


# FAQ, 제한 사항 및 우수 사례

Analytics 및 Target의 고객 속성에 대한 FAQ 및 우수 사례입니다.


## 우수 사례 및 제한 사항 {#section_7F5189B3DAA84EE6865B91D2026EE05A}

고객 속성을 사용하는 경우 지침 및 제한 사항입니다.

| 문제 | 설명 |
|--- |--- |
| 고객 속성 등록 제한 사항 | Analytics Premium으로 업그레이드할 때 추가 특성은 24시간 후에 사용할 수 있습니다. 이 시간 중에 속성 가입 최대값 오류가 표시될 수 있습니다. |
| 사용자 정의 Analytics ID(s.visitorID) | Analytics에서 사용자를 식별하는 방법은  s. visitorid는 Analytics에서 사용자를 식별하는 방법입니다. 그러나 ID 서비스를 사용하여 Analytics 데이터를 내보내거나 가져오는 통합은 방문자가 s.visitorID를 사용하여 식별되는 경우 작동하지 않습니다.<br>여기에는 공유 대상, Analytics for Target(A4T) 및 고객 속성이 포함되지만, 이에 제한되지 않습니다.<br>이러한 통합의 경우 사용자 지정 Analytics ID를 설정할 수 없습니다. |
| Analytics의 문자 길이 제한 | Analytics 구독을 만들 때 업로드된 파일의 필드 길이는 255자로 잘립니다. |

## 고객 속성에 대한 FAQ {#section_E47866EEA83348E09FE43CEC5E44C461}

<table id="table_88631069013B408EBB0A810657662B36"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> 질문 </th> 
   <th colname="col2" class="entry"> 답변 </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>고객 속성과 관련된 업로드 상태에 대한 알림을 받을 수 있습니까? </p> </td> 
   <td colname="col2"> <p>예. <a href="../admin-getting-started/organizations.md#concept_0105453AD71847B8BFCAF4A40915F157" format="dita" scope="local">알림 관리</a>를 참조하십시오. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> 고객 속성 사용을 시작하려면 어떤 작업을 수행해야 합니까? </p> </td> 
   <td colname="col2"> 
    <ol id="ol_1FACEF0990B6486B8DE86245D17695A8"> 
     <li id="li_F0C1542853684F8591FDC1B441D31A56"> <p>제공을 받습니다. </p> <p><b>Analytics</b> 사용자인 경우 Adobe가 고객 속성을 제공합니다. <b>Target</b>만 사용하고 Analytics가 없는 경우 고객 지원 센터에 연락하여 핵심 서비스를 제공하도록 요청해야 합니다. </p> </li> 
     <li id="li_444FEDEE4B7244F79BA847662F5B17CB"> <p>CRM 팀과 대화합니다. Analytics 및 Experience Cloud 전체에서 사용하려는 고객 데이터 종류를 알아봅니다. </p> </li> 
     <li id="li_32D4AAF8C29748A78801A0E1BFB37AF5"> <p>핵심 서비스를 구현합니다. </p> <p>핵심 서비스에 대한 구현을 현대화하는 방법에 대한 단계에 대해서는 <a href="../core-services/core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C" format="dita" scope="local"> 시작하기 - 핵심 서비스에</a> 대한 솔루션 활성화를 참조하십시오. 자세한 내용은 고객 ID 동기화에 대한 섹션을 참조하십시오. </p> </li> 
    </ol> <p> <b>참고:</b> 핵심 서비스 구현에 대한 관리자의 FAQ는 <a href="../admin-getting-started/faq.md#concept_13219B4E51784577B6FF78AAA203DE91" format="dita" scope="local"> 여기</a>에서 확인하십시오. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> 제가 사용할 수 있는 고객 속성은 몇 개입니까? </p> </td> 
   <td colname="col2"> <p>수백 개의 <span class="filepath">.csv</span> 열을 고객 속성 서비스로 업로드할 수 있습니다. 그렇지만 구독을 구성하고 속성을 선택할 때 보유하고 있는 솔루션에 따라 다음과 같은 제한이 적용됩니다. </p> <p> 
     <ul id="ul_2BB85067918D4BB3B59394F3E3E37A6D"> 
      <li id="li_93703988B9934384B4B94A839D028380"> <b>Analytics Standard</b>: 3 합계 </li> 
      <li id="li_D1E5E7BD24C54591B14D15DE97447835"> <b>Analytics Premium</b>: 보고서 세트당 200개 </li> 
      <li id="li_8C891FE3D1EF49FA9F81E2E32CD0B9CA"> <b>Target Standard:</b> 5개 </li> 
      <li id="li_2B66D43023F34EA685CE2C38A9250CEA"> <b>Target Premium:</b> 200개 </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Experience Cloud ID 서비스로 마이그레이션해야 합니까? </p> </td> 
   <td colname="col2"> <p>마이그레이션은 사용하는 솔루션에 따라 다릅니다. </p> <p> 
     <ul id="ul_9C473434B5DA4C6299AAB209DEDFCDE7"> 
      <li id="li_8BC10EB2825F4ADF8CA61F71D4994A28"> <b>Adobe Analytics</b>: 강력히 권장됨 </li> 
      <li id="li_56F518E3F3DF4C93B6F7EF3B40ACC52F"> <b>Adobe Target:</b> 필수 </li> 
     </ul> </p> <p>ID 서비스를 사용하면 실시간 대상, Target 현대화, Analytics 통합 및 비디오 하트비트 추적을 비롯한 최신 Experience Cloud 기능을 사용할 수 있습니다. </p> <p>자세한 내용은 <a href="../core-services/core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C" format="dita" scope="local"> 핵심 서비스 - 솔루션 활성화 방법</a>. </p> <p> <b></b>참고: <span class="term"> Experience Cloud ID 서비스는</span> <span class="term"> 이전에 Analytics 방문자 ID 서비스로 알려진 기능의 현대화된</span>구현입니다. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>고객 속성 기능은 Adobe Audience Manager와 어떤 관련이 있습니까? </p> </td> 
   <td colname="col2"> <p>Audience Manager는 데이터를 수신하여 대상을 확인할 수 있지만 속성을 이전 행동 데이터와 결합하는 분석 기능을 수행하거나 Adobe Analytics에서 사용할 수 있는 보고, 분석 및 세그멘테이션 기능을 제공하지는 못합니다. 사용자 핵심 서비스는 여러 솔루션에서 가져온 다양한 데이터를 함께 결합하고 Experience Cloud에서 사용할 수 있게 단일 ID와 연결할 수 있도록 합니다. </p> <p> Adobe Target에서 고객 속성은 다른 규칙과 결합하여 대상을 구축할 수 있는 개별 속성으로 표시됩니다. 사용자 핵심 서비스에서 공유된 대상은 수정할 수 없는 전체 대상입니다. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>(Analytics 전용) </b>Analytics Premium에 제공된 기능과 비교할 때 이 기능은 어떤 차이가 있습니까? </p> </td> 
   <td colname="col2"> <p>이전에는 고객 속성 데이터를 Analytics 데이터에 결합하려는 고객이 이 기능을 사용하려면 Data Workbench 도구에 상당히 의존했습니다. 고객 속성은 고객 속성을 Reports &amp; Analytics, Ad Hoc Analysis 및 Report Builder에서 차원 및 지표로 제공하여 좀 더 다양한 대상에게 이 기능을 제공합니다. Analytics Standard 고객은 고객 속성에 액세스할 수 있지만 사용할 수 있는 기능은 제한됩니다. Analytics 프리미엄 고객은 전체 기능을 사용할 수 있습니다. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>(Target 전용)</b> Target에서 표시된 적이 없는 고객의 데이터를 미리 로드하거나 업로드할 수 있습니까? </p> </td> 
   <td colname="col2"> <p> 예. 방문자가 Target에 대해 첫 번째 요청을 수행하면 시스템은 고객 속성에서 고객에 대한 기존 정보를 가져온 다음 해당 데이터를 사용하여 타깃팅합니다. </p> <p> <p>참고: 이 데이터를 검색하는 데는 방문자가 Target과 처음 상호 작용한 시점부터 최대 20분이 걸릴 수 있습니다. </p> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>(Target 전용)</b> 고객 속성 데이터를 공유 대상 데이터와 결합하여 슈퍼 대상을 만들 수 있습니까? </p> </td> 
   <td colname="col2"> <p>아닙니다. 공유된 대상 데이터는 완전한 대상입니다. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>(Target 전용) </b>고객 속성 기능을 Target의 벌크 프로필 API와 어떻게 비교합니까? </p> </td> 
   <td colname="col2"> <p> <a href="https://marketing.adobe.com/developer/documentation/test-target/r-profile-update" format="https" scope="external">벌크 프로필 API</a>를 사용하면 개별 프로필에 대해 또는 대량으로 API를 통해 Target 프로필을 직접 업데이트할 수 있습니다. 이 기능은 고객 속성과 비슷하지만, 다음과 같은 주요 차이점이 있습니다. </p> 
    <ul id="ul_5AAA4A8497C04F50A8AAA9F776BB868E"> 
     <li id="li_B20AEA397F3B4C86A1140CDA61ABD575">프로필 API는 REST API 호출이며, 고객 속성은 FTP를 사용합니다. </li> 
     <li id="li_7FBE428EF5D34B6AA09B6368E8210344">Target의 프로필 API는 전체 Experience Cloud 대신 Target으로만 데이터를 보냅니다. </li> 
     <li id="li_CBB4D3FAF53944E0A066A4AD9F9C8760">고객 속성은 이러한 외부 데이터를 만들고 관리할 간단한 인터페이스를 제공합니다. </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>(Target 전용)</b> 고객 속성에서 Adobe Target으로 데이터를 업로드하면 Target 방문자의 프로필 라이프타임이 연장됩니까? </p> </td> 
   <td colname="col2"> <p>예. Adobe Target 도움말의 <a href="https://marketing.adobe.com/resources/help/en_US/target/ov/?f=c_visitor_profile_lifetime" format="https" scope="external">방문자 프로필 라이프타임</a>을 참조하십시오. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b> (Target 전용)</b> 방문자가 고객 ID로 식별되면 바로 고객 속성에 업로드된 데이터를 타깃팅할 수 있습니까? </p> </td> 
   <td colname="col2"> <p>예.  </p> <p>Target에 대한 서버 호출 시 여기에 mbox 타사 ID가 포함되면 모든 고객 속성 데이터를 사용할 수 있습니다. </p> </td> 
  </tr> 
 </tbody> 
</table>

