---
title: Adobe Experience Platform Web SDK 쿠키
description: Web SDK가 구현에 적용되는 쿠키를 사용하는 방법에 대해 알아봅니다.
solution: Experience Cloud
feature: Cookies
topic: Administration
role: Admin
level: Experienced
source-git-commit: 66f78a04674a82335f5df20c4c15d983b6ebdc66
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# Adobe Experience Platform Web SDK 쿠키

Adobe Experience Platform Web SDK는 쿠키를 사용하여 구현과 관련된 값을 저장합니다.

| 이름 | 최대 나이 | 설명 |
|---|---|---|
| **kndct_orgid_identity** | 34128000(395일) | ECID 및 ECID와 관련된 기타 정보를 저장합니다. |
| **kndctr_orgid_consent_check** | 7200(2시간) | 동의 환경 설정 서버측을 검색하도록 서버에 알립니다. |
| **kndctr_orgid_consent** | 15552000(180일) | 웹 사이트에 대한 사용자의 동의 환경 설정을 저장합니다. |
| **kndctr_orgid_cluster** | 1800(30분) | 현재 사용자의 요청을 처리하는 Edge Network 영역을 저장합니다. Edge Network이 요청을 올바른 영역으로 라우팅할 수 있도록 URL 경로에 영역이 사용됩니다. 사용자가 다른 IP 주소 또는 다른 세션에 연결하는 경우 요청이 다시 가장 가까운 영역으로 라우팅됩니다. |
| **mbox** | 63072000(2년) | Target 마이그레이션 설정이 true로 설정된 경우에 표시됩니다. 타겟을 허용합니다. [mbox 쿠키](https://developer.adobe.com/target/implement/client-side/atjs/atjs-cookies/) 웹 SDK에서 설정합니다. |
| **mboxEdgeCluster** | 1800(30분) | Target 마이그레이션 설정이 true로 설정된 경우에 표시됩니다. 이를 통해 Web SDK는 올바른 에지 클러스터를 `at.js` 따라서 사용자가 사이트를 탐색할 때 Target 프로필이 동기화 상태를 유지할 수 있습니다. |
| **AMCV_###@AdobeOrg** | 34128000(395일) | 제공 시점 [`idMigrationEnabled`](https://experienceleague.adobe.com/en/docs/experience-platform/web-sdk/commands/configure/idmigrationenabled) 이(가) 활성화되었습니다. 사이트의 일부 부분이 여전히 을 사용하는 동안 웹 SDK로 전환하는 데 도움이 됩니다 `visitor.js`. |

Edge Network은 를 사용하여 모든 쿠키를 `secure` 및 `sameSite="none"` 속성. 현재 웹 사이트에 보안 섹션과 비보안 섹션이 모두 있는 경우 사용자 식별이 부정확할 수 있습니다. 사용자가 사이트의 보안 섹션에서 비보안 섹션으로 이동하면 Edge Network은 새 항목을 생성합니다 `ECID` (요청 포함)
