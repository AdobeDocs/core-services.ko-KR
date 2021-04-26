---
description: Adobe Target에서 어떻게 쿠키를 사용하여 어떤 온라인 컨텐츠 및 오퍼가 방문자와 밀접한 관련이 있는지 테스트하는 기능을 웹 사이트 운영자에게 제공하는지 알아봅니다.
keywords: cookies;privacy
solution: Experience Cloud,Analytics,Target,Social
title: 'Adobe Target 쿠키 '
uuid: 44f7e32e-8d99-4682-8b54-8364d001b403
feature: 쿠키
topic: 관리
role: Administrator
level: Experienced
exl-id: c4399cc0-8333-47b8-b830-2ba7359f464a
translation-type: tm+mt
source-git-commit: dcb6fa5d8458995cba66bc2f89c954aa6bcd5923
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 55%

---

# Adobe Target 쿠키{#target-cookies}

Adobe Target은 쿠키를 사용하여 웹 사이트 운영자가 어떤 온라인 컨텐츠 및 오퍼가 방문자와 관련이 있는지 테스트할 수 있도록 합니다.

필요한 경우 쿠키 지속 시간을 제외하고 이러한 설정을 변경할 수 있습니다. 쿠키 설정을 변경하는 경우 계정 담당자에게 문의하십시오.

>[!NOTE]
>
>Adobe Target 사용자는 사용자 지정 타사 쿠키를 생성할 수도 있습니다.

| 설정 | 정보 |
| --- | --- |
| 쿠키 이름 | mbox. |
| 쿠키 도메인 | mbox를 제공하는 도메인의 두 번째 및 최상위 수준입니다. 회사 도메인에서 제공되기 때문에 쿠키는 자사 쿠키입니다. 예: `mycompany.com`. |
| 서버 도메인 | `clientcode.tt.omtrdc.net`[!DNL Adobe Target]( 계정에 대해 클라이언트 코드 사용) |
| 쿠키 지속 시간 | 쿠키는 마지막 로그인부터 2년 동안 방문자 브라우저에 유지됩니다. 쿠키 지속 시간은 변경할 수 없습니다. |



>[!NOTE]
>
>도메인 이름에 `mycompany.co.uk`와 같은 국가 코드가 포함되어 있는 경우 클라이언트 서비스와 작업하여 이 코드를 지원하도록 [!DNL at.js]를 구성하십시오.

쿠키는 방문자가 Adobe Target 캠페인을 경험하는 방식을 관리하기 위해 많은 값을 유지합니다.

| 값 | 정의 |
| --- | --- |
| session ID | 지정된 사용자 세션의 고유 식별자입니다. 기본적으로 세션이 30분 동안 비활성화된 후 만료됩니다. sessionId를 직접 생성하는 경우(예: 서버측 구현의 경우) 다음을 확인하십시오.<ul><li>세션 ID는 공백, 물음표( ? ) 또는 슬래시( / ).</li><li>* 세션 ID 길이는 1자에서 128자 사이여야 합니다.</li><li>특정 세션의 경우 값이 여러 요청에서 동일해야 합니다</li><li>지정된 방문자에 대한 병렬 세션(별개의 sessionIds)은 특정 시점에 있어서는 안 됩니다.</li></ul>Edge Cluster의 특정 노드에 대한 라우팅은 세션 ID를 사용하여 수행됩니다.<ul><li>세션은 서버측에서 30분 동안 활성 상태입니다. 따라서 `tntId/thirdPartyId`에서 마지막으로 요청한 요청 후 30분 이내에 특정 `tntId/thirdPartyId`에 다른 세션 ID를 사용하면 안 됩니다. 그렇지 않으면 프로필 변경 내용이 일관되지 않고 예측할 수 없을 수 있습니다.</li><li>동일한 세션 ID를 여러 `tntIds/thirdPartyIds`에 사용하면 `tntId/thirdPartyIDs`에 의해 식별된 프로파일에 예측할 수 없는 변경 사항이 발생할 수 있습니다.</li></ul> |
| pc ID | 방문자 브라우저의 반영구 ID입니다. 쿠키가 수동으로 삭제될 때까지 지속됩니다. |
| check | 방문자가 쿠키를 지원하는지 여부를 확인하는 간단한 테스트 값입니다. 방문자가 페이지를 요청할 때마다 설정합니다. |
| disable | 방문자의 로드 시간이 at.js 파일에 구성된 시간 초과를 초과하는 경우 설정합니다. 기본적으로 1시간 동안 지속됩니다. |

