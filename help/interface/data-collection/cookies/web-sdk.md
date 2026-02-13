---
title: Adobe Experience Platform 웹 SDK 쿠키
description: 웹 SDK에서 구현에 적용되는 쿠키를 사용하는 방법을 알아봅니다.
solution: Experience Cloud
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: 14f06dc9-255e-4a6c-adec-471107cf202e
TQID: https://experienceleague.adobe.com/jysQ5m7o0cI3ECKz2RWZB4Kt3own7XAPm04pr4yLh-k
product_v2: id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
feature_v2: id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
subfeature_v2: id: b75843fa-0a67-4a44-a6b1-cc627b0481dcid: fef08361-6ac5-460c-93fe-d063e40b6a49
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 0d253888322194189fea6d492ae19cf248357960
workflow-type: tm+mt
source-wordcount: 396
ht-degree: 0%

---

# Adobe Experience Platform Web SDK 쿠키

Adobe Experience Platform Web SDK은 쿠키를 사용하여 구현에 따른 값을 저장합니다.

| 이름 | 최대 나이 | 크기 | 설명 |
|---|---|---|---|
| **`AMCV_###@AdobeOrg`** | 34128000(395일) | 100-120바이트(변수) | [`idMigrationEnabled`](https://experienceleague.adobe.com/en/docs/experience-platform/collection/js/commands/configure/idmigrationenabled)이(가) 활성화된 경우 표시됩니다. 사이트의 일부 부분이 여전히 `visitor.js`을(를) 사용하는 동안 웹 SDK으로 전환하는 데 도움이 됩니다. 웹 SDK은 마이그레이션 중에 이 쿠키를 읽고 씁니다. |
| **`demdex`** | 15552000(180일) | 다양함 | Audience Manager ID 동기화가 활성화된 경우 표시됩니다. Audience Manager은 고유 ID를 할당하고 ID 동기화, 세그먼테이션, 모델링 및 보고를 지원하도록 이 쿠키를 설정합니다. `demdex`Audience Manager 쿠키[의 ](audience-manager.md)을(를) 참조하십시오. |
| **`kndctr_<orgId>_identity`** | 34128000(395일) | 100-120바이트(변수) | 해당 장치에 대한 ECID 및 기타 관련 정보를 저장합니다. |
| **`kndctr_<orgId>_cluster`** | 1800(30분) | 3-5바이트 | 현재 사용자의 요청을 제공하는 Edge Network 영역(위치 힌트)을 저장합니다. Edge Network이 요청을 올바른 영역으로 라우팅할 수 있도록 이 영역은 URL 경로에 사용됩니다. 사용자가 쿠키 라이프타임 내에 다른 IP 주소와 연결하는 경우 요청이 다시 가장 가까운 영역으로 라우팅됩니다. |
| **`kndctr_<orgId>_consent`** | 15552000(180일) | 10-11바이트 | 방문자의 동의 환경 설정을 저장합니다. 동의 환경 설정 자체를 저장하기 때문에 동의와 관계없이 항상 설정하십시오. |
| **`kndctr_<orgId>_consent_check`** | 7200(2시간) | | TTL이 만료된 후 Edge Network에 서버측에서 동의를 다시 확인하라는 신호를 보내는 세션 범위 도우미입니다. 캐시된 동의에 TTL을 적용합니다. |
| **`kndctr_<orgId>_personalization`** | 34128000(395일) | | Adobe Target이 콘텐츠를 개인화하는 데 사용하는 세션 정보를 저장합니다. |
| **`mbox`** | 63072000(2년) | | [`targetMigrationEnabled`](https://experienceleague.adobe.com/en/docs/experience-platform/collection/js/commands/configure/targetmigrationenabled)이(가) 활성화된 경우 표시됩니다. 웹 SDK에서 Target [mbox 쿠키](https://developer.adobe.com/target/implement/client-side/atjs/atjs-cookies/)를 설정할 수 있습니다. |
| **`mboxEdgeCluster`** | 1800(30분) | | [`targetMigrationEnabled`](https://experienceleague.adobe.com/en/docs/experience-platform/collection/js/commands/configure/targetmigrationenabled)이(가) 활성화된 경우 표시됩니다. 웹 SDK에서 올바른 에지 클러스터를 `at.js`에 전달하면 사용자가 사이트를 탐색할 때 Target 프로필이 동기화 상태를 유지할 수 있습니다. |
| **`s_ecid`** | 63115200(2년) | ~45바이트 | `s_ecid=MCMID\|<ECID>` 형식의 Experience Cloud ID(ECID/MID) 복사본을 포함합니다. 주로 CNAME(자사) 시나리오에서 ECID의 자사 백업 역할을 합니다. |

Edge Network은 `secure` 및 `sameSite="none"` 특성이 있는 모든 쿠키를 설정합니다. 현재 웹 사이트에 보안 섹션과 비보안 섹션이 모두 있는 경우 사용자 식별이 부정확할 수 있습니다. 사용자가 사이트의 보안 섹션에서 비보안 섹션으로 이동하면 Edge Network은 요청을 통해 새 `ECID`을(를) 생성합니다.
