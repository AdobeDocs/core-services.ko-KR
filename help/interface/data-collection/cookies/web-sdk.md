---
title: Adobe Experience Platform 웹 SDK 쿠키
description: 웹 SDK에서 구현에 적용되는 쿠키를 사용하는 방법을 알아봅니다.
solution: Experience Cloud
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: 14f06dc9-255e-4a6c-adec-471107cf202e
TQID: 'https://experienceleague.adobe.com/jysQ5m7o0cI3ECKz2RWZB4Kt3own7XAPm04pr4yLh-k'
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
    internal-label: CX Enterprise
feature_v2:
  - id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
    internal-label: Administration
subfeature_v2:
  - id: b75843fa-0a67-4a44-a6b1-cc627b0481dc
    internal-label: Support
  - id: fef08361-6ac5-460c-93fe-d063e40b6a49
    internal-label: Getting started
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 7b12d5debfccd62ab7b416e9a6fe278d251a4ca5
workflow-type: tm+mt
source-wordcount: '984'
ht-degree: 0%
---
# Adobe Experience Platform Web SDK 쿠키

Adobe Experience Platform Web SDK은 쿠키를 사용하여 구현에 따른 값을 저장합니다.

| 이름 | 최대 나이 | 크기 | 설명 |
| --- | --- | --- | --- |
| **`AMCV_###@AdobeOrg`** | 웹 SDK에서 작성한 경우 33696000(390일) | 웹 SDK(`MCMID\|<ECID>`)에서 쓰는 경우 44바이트, `VisitorAPI.js`에서 쓰는 경우 더 큼 | 기본값인 [`idMigrationEnabled`](https://experienceleague.adobe.com/ko/docs/experience-platform/collection/js/commands/configure/idmigrationenabled)이(가) 활성화된 경우 표시됩니다. 사이트의 일부 부분이 여전히 `VisitorAPI.js`을(를) 사용하는 동안 웹 SDK으로 전환하는 데 도움이 됩니다. 웹 SDK은 이 쿠키를 읽고 기존 ECID를 재사용합니다. Edge Network이 ECID를 반환하면 웹 SDK은 쿠키가 없거나 다른 ECID를 포함하는 경우 이 쿠키에 씁니다. |
| **`com.adobe.alloy.getTld`** | 없음(세션 쿠키, 즉시 삭제) | 22바이트 | 웹 SDK에서 현재 사이트의 최상위 도메인을 확인하기 위해 내부적으로 사용하는 임시 도우미 쿠키입니다. 웹 SDK은 라이브러리가 로드될 때, `configure` 명령이 실행되기 전과 동의를 평가하기 전에 이 쿠키를 쓰고 삭제하므로 쿠키 스캐너가 동의 전에 설정된 대로 이 쿠키를 보고할 수 있습니다. 쿠키에는 자체 이름만 포함되어 있으며 동작 또는 프로필 데이터를 저장하지 않습니다. |
| **`demdex`** | 15552000(180일) | 다양함 | `demdex.net` 도메인의 타사 쿠키. [`thirdPartyCookiesEnabled`](https://experienceleague.adobe.com/ko/docs/experience-platform/collection/js/commands/configure/thirdpartycookiesenabled)이(가) 활성화되어 있고(기본값) 브라우저에서 기본적으로 Chrome 또는 Edge과 같은 서드파티 쿠키를 허용하는 경우 표시됩니다. 이 경우 웹 SDK은 이 쿠키를 설정하는 `adobedc.demdex.net`에 ID 요청을 보냅니다. Audience Manager은 이 쿠키를 사용하여 고유 ID를 할당하고 ID 동기화, 세그먼테이션, 모델링 및 보고를 지원합니다. [Audience Manager 쿠키](audience-manager.md)의 `demdex`을(를) 참조하십시오. |
| **`kndctr_<orgId>_identity`** | 34128000(395일) | 100-120바이트(변수) | 해당 장치에 대한 ECID 및 기타 관련 정보를 저장합니다. |
| **`kndctr_<orgId>_cluster`** | 1800(30분) | 3-5바이트 | 현재 사용자의 요청을 제공하는 Edge Network 영역(위치 힌트)을 저장합니다. Edge Network이 요청을 올바른 영역으로 라우팅할 수 있도록 이 영역은 URL 경로에 사용됩니다. 사용자가 쿠키 라이프타임 내에 다른 IP 주소와 연결하는 경우 요청이 다시 가장 가까운 영역으로 라우팅됩니다. |
| **`kndctr_<orgId>_consent`** | 15552000(180일) | 10-11바이트 | 방문자의 동의 환경 설정을 저장합니다. 동의 환경 설정 자체를 저장하기 때문에 동의와 관계없이 항상 설정하십시오. |
| **`kndctr_<orgId>_consent_check`** | 7200(2시간) | | TTL이 만료된 후 Edge Network에 서버측에서 동의를 다시 확인하라는 신호를 보내는 세션 범위 도우미입니다. 캐시된 동의에 TTL을 적용합니다. |
| **`kndctr_<orgId>_personalization`** | 34128000(395일) | | Adobe Target이 콘텐츠를 개인화하는 데 사용하는 세션 정보를 저장합니다. |
| **`kndctr_<orgId>_advertising`** | 쿠키가 업데이트될 때마다 31622400(366일) 갱신됩니다 | 80바이트~1KB(변수) | Adobe Advertising 구성 요소(베타)가 웹 SDK 빌드에 포함되고 방문자의 동의가 `in`인 경우 표시됩니다. 웹 SDK은 페이지 URL에 Adobe Advertising 클릭 매개 변수(`s_kwcid` 또는 `ef_id`)가 포함되어 있거나 [Adobe Advertising DSP](https://experienceleague.adobe.com/ko/docs/experience-platform/tags/extensions/client/web-sdk/configure/advertising) 광고주가 구성된 경우 이 쿠키를 기록합니다. 검색 클릭 데이터(`_les_lsc`), 해시된 IP 주소, LiveRampRampID 봉투(RampID JavaScript 경로가 구성된 경우) 및 중복 전환을 스로틀하는 데 사용되는 전환 타임스탬프를 포함할 수 있는 URL로 인코딩된 JSON을 저장합니다. 기본적으로 타사 쿠키를 허용하는 브라우저에서 Adobe Advertising 서퍼 ID를 저장하고 클릭 데이터(`ev_lcc`)를 표시합니다. 이 쿠키는 현재 호스트 이름에서만 설정됩니다. 구성 요소는 `pixel.everesttech.net`, `www.everestjs.net`(ID5 파트너 ID가 구성된 경우) 및 RampID `ats.js` 경로에서도 리소스를 로드합니다. 이러한 리소스는 이 페이지에 나열되지 않은 자체 쿠키를 설정할 수 있습니다. |
| **`kndctr_<orgId>_bc_session_id`** | 없음(세션 쿠키) | | Brand Concierge 구성 요소(베타)를 사용할 때 표시됩니다. Brand Concierge 채팅 세션 ID를 저장합니다. 웹 SDK은 [`stickyConversationSession`](https://experienceleague.adobe.com/ko/docs/experience-platform/collection/js/commands/configure/conversation)을(를) 사용하도록 설정한 경우에만 이 쿠키를 읽으므로 채팅 세션이 페이지 로드 중에 지속됩니다. |
| **`mbox`** | 63072000(2년) | | [`targetMigrationEnabled`](https://experienceleague.adobe.com/ko/docs/experience-platform/collection/js/commands/configure/targetmigrationenabled)이(가) 활성화된 경우 표시됩니다. 웹 SDK에서 Target [mbox 쿠키](https://developer.adobe.com/target/implement/client-side/atjs/atjs-cookies/)를 설정할 수 있습니다. |
| **`mboxEdgeCluster`** | 1800(30분) | | [`targetMigrationEnabled`](https://experienceleague.adobe.com/ko/docs/experience-platform/collection/js/commands/configure/targetmigrationenabled)이(가) 활성화된 경우 표시됩니다. 웹 SDK에서 올바른 에지 클러스터를 `at.js`에 전달하면 사용자가 사이트를 탐색할 때 Target 프로필이 동기화 상태를 유지할 수 있습니다. `kndctr_<orgId>_cluster` 쿠키가 없으면 웹 SDK도 이 쿠키를 읽어 요청을 일치하는 Edge Network 영역으로 라우팅합니다. |
| **`s_ecid`** | 63115200(2년) | ~45바이트 | `s_ecid=MCMID\|<ECID>` 형식의 CX Enterprise ID(ECID/MID) 복사본을 포함합니다. 주로 CNAME(자사) 시나리오에서 ECID의 자사 백업 역할을 합니다. [`idMigrationEnabled`](https://experienceleague.adobe.com/ko/docs/experience-platform/collection/js/commands/configure/idmigrationenabled)을(를) 사용하도록 설정하면 웹 SDK이 이 쿠키를 읽어 기존 ECID를 다시 사용합니다. |
| **Audience Manager 쿠키 대상**(이름은 다름) | 대상이 다른 라이프타임을 지정하지 않는 한 10일 864000 | 다양함 | Edge Network이 방문자에 대해 Audience Manager [쿠키 대상](https://experienceleague.adobe.com/ko/docs/audience-manager/user-guide/features/destinations/custom-destinations/create-cookie-destination)을 반환하는 경우 표시됩니다. 웹 SDK은 대상에 정의된 쿠키 이름, 값 및 도메인을 사용하여 자사 쿠키를 기록합니다. 값은 URL로 인코딩되며 Audience Manager Data Integration Library(DIL)와 일치합니다. |

Edge Network은 `secure` 및 `sameSite="none"` 특성을 사용하여 모든 쿠키를 설정합니다. 현재 웹 사이트에 보안 섹션과 비보안 섹션이 모두 있는 경우 사용자 식별이 부정확할 수 있습니다. 사용자가 사이트의 보안 섹션에서 비보안 섹션으로 이동하면 Edge Network은 요청을 통해 새 `ECID`을(를) 생성합니다.

웹 SDK이 Edge Network의 방향이 아니라 자체적으로 만드는 쿠키는 다른 특성을 사용합니다. `AMCV_###@AdobeOrg` 쿠키 및 Audience Manager 쿠키 대상에는 HTTPS 페이지에서만 `secure` 및 `sameSite="none"` 특성이 포함됩니다. `com.adobe.alloy.getTld` 및 `kndctr_<orgId>_advertising` 쿠키는 브라우저의 기본 특성을 사용합니다.
