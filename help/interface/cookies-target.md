---
description: Adobe Target에서 어떻게 쿠키를 사용하여 어떤 온라인 콘텐츠 및 오퍼가 방문자와 밀접한 관련이 있는지 테스트하는 기능을 웹 사이트 운영자에게 제공하는지 알아봅니다.
solution: Experience Cloud,Analytics,Target,Social
title: Adobe Target 쿠키
uuid: 44f7e32e-8d99-4682-8b54-8364d001b403
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: c4399cc0-8333-47b8-b830-2ba7359f464a
source-git-commit: eb2ad8a8255915be47b6002a78cc810b522170d2
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 92%

---

# Adobe Target 쿠키{#target-cookies}

Adobe Target은 쿠키를 사용하여 웹 사이트 운영자가 어떤 온라인 콘텐츠 및 오퍼가 방문자와 관련이 있는지 테스트할 수 있도록 합니다.

필요한 경우 쿠키의 지속 시간 이외의 다른 설정을 변경할 수 있습니다. 쿠키 설정을 변경하는 경우 계정 담당자에게 문의하십시오.

>[!NOTE]
>
>Adobe Target 사용자는 사용자 지정 서드파티 쿠키를 생성할 수도 있습니다.

| 설정 | 정보 |
| --- | --- |
| 쿠키 이름 | mbox. |
| 쿠키 도메인 | mbox를 제공하는 도메인의 두 번째 및 최상위 수준입니다. 회사 도메인에서 제공되기 때문에 쿠키는 자사 쿠키입니다. 예: `mycompany.com`. |
| 서버 도메인 | `clientcode.tt.omtrdc.net`, 클라이언트 코드를 [!DNL Adobe Target] 계정에 대해 사용. |
| 쿠키 지속 시간 | 쿠키는 마지막 로그인부터 2년 동안 방문자의 브라우저에 유지됩니다. 쿠키 지속 시간은 변경할 수 없습니다. |

{style=&quot;table-layout:auto&quot;}

>[!NOTE]
>
>도메인 이름에 `mycompany.co.uk`와 같은 국가 코드가 포함되어 있는 경우 클라이언트 서비스와 작업하여 이 코드를 지원하도록 `at.js` 를 구성하십시오.

쿠키는 방문자가 Adobe Target 캠페인을 경험하는 방식을 관리하기 위해 어느 정도의 값을 유지합니다.

| 값 | 정의 |
| --- | --- |
| 세션 ID | 사용자 세션의 고유 식별자. 30분 동안 활동이 없으면 기본적으로 세션이 만료됩니다. 세션 ID를 직접 생성하는 경우(예: 서버측 구현) 다음을 확인하십시오.<ul><li>세션 ID는 인쇄 가능한 모든 문자열이 될 수 있지만, 공백, 물음표( ? ), 슬래시( / )는 제외됩니다.</li><li>세션 ID는 1~128자 사이여야 합니다.</li><li>특정 세션의 경우 해당 값이 여러 요청에서 동일하게 유지되어야 합니다.</li><li>특정 시점에 정해진 한 방문자에 대해 병렬 세션(개별 세션 ID)이 있어서는 안 됩니다.</li></ul>에지 클러스터의 특정 노드에 대한 라우팅은 세션 ID를 사용하여 합니다.<ul><li>세션은 서버측에서 30분 동안 활성화됩니다. 따라서 특정 세션에 다른 세션 ID를 사용하면 안 됩니다 `tntId/thirdPartyId` 를 사용하여 마지막으로 수행한 요청의 30분 이내 `tntId/thirdPartyId`. 그렇지 않으면, 프로필 변경 사항이 일관되지 않고 예측할 수 없습니다.</li><li>방문자가 30분 동안 활동이 없으면 새 세션 ID를 사용해야 합니다.</li><li>여러 `tntIds/thirdPartyIds` 에 대해 같은 세션 ID를 사용하면 `tntId/thirdPartyIDs`에서 식별하는 프로필에 예측 불가능한 변경 사항을 초래할 수 있습니다.</li></ul>**참고**: 특정 세션 ID는 [동시 요청 수 제한](https://experienceleague.adobe.com/docs/target/using/troubleshoot/target-limits.html?lang=en#content-delivery) 을 참조하십시오. |
| pc ID | 방문자 브라우저의 반영구 ID입니다. 쿠키가 수동으로 삭제될 때까지 지속됩니다. |
| 확인 | 방문자가 쿠키를 지원하는지 여부를 확인하는 간단한 테스트 값입니다. 방문자가 페이지를 요청할 때마다 설정합니다. |
| 비활성화 | 방문자의 로드 시간이 at.js 파일에서 구성한 시간 제한을 초과할 경우 설정합니다. 기본적으로 이 타임아웃은 1시간 동안 지속됩니다. |

{style=&quot;table-layout:auto&quot;}
