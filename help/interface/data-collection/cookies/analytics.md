---
description: Adobe Experience Cloud의 Adobe Analytics 쿠키에 대해 알아봅니다.
solution: Analytics
title: Adobe Analytics 쿠키
uuid: e2d3d61d-2708-48b2-a7e6-2331f2aed8e0
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: bc8ce894-f98c-4475-8a07-d74ae76f7451
source-git-commit: d3a559ca2f7963256d48a25cd51099edb5e3fe76
workflow-type: tm+mt
source-wordcount: '535'
ht-degree: 11%

---

# Adobe Analytics 쿠키

Adobe Analytics는 쿠키를 사용하여 서로 다른 브라우저의 요청을 구분하고 애플리케이션이 나중에 사용할 수 있도록 유용한 정보를 저장합니다. 또한 검색 정보를 고객 레코드와 연결하는 데 사용할 수도 있습니다.

Analytics는 쿠키를 사용하여 새로운 방문자를 익명으로 정의하고 클릭스트림 데이터를 분석하며 특정 캠페인에 대한 응답 또는 판매 주기 기간과 같은 웹 사이트의 활동 내역을 추적합니다.

| 쿠키 이름 | 만료 | 크기 | 위치 | 설명 |
| --- | --- | --- | --- | --- |
| **`s_ecid`** | 13개월 | 45바이트 | 자사 | Experience Cloud ID(ECID) 또는 MID를 저장합니다. HTTP 응답으로 설정됩니다. MID는 `s_ecid=MCMID` 형식으로 저장됩니다. 클라이언트가 AMCV 쿠키를 설정한 후에 를 설정합니다. 영구적 자사 ID 추적을 허용하며 AMCV 쿠키가 만료되는 경우 참조 ID로 사용됩니다. `SameSite`이(가) &quot;Lax&quot;로 설정되어 있습니다. 웹 SDK을 사용하여 Adobe Analytics을 구현하는 경우 쿠키 만료는 2년으로 설정되지만 대부분의 최신 브라우저에서는 만료가 13개월로 잘립니다. |
| **`s_cc`** | Session | 4바이트 | 자사 | 쿠키가 활성화되었는지 여부를 확인합니다. JavaScript에서 설정합니다. |
| **`s_sq`** | Session | 100-200바이트 | 자사 | Activity Map에서 사용됩니다. 여기에는 방문자가 클릭한 이전 링크에 대한 정보가 포함되어 있습니다. JavaScript에서 설정합니다. |
| **`s_vi`** | 2년 | 44바이트 | 자사 또는 `*.omtrdc.net`(타사) | 고유 방문자 ID 및 타임스탬프를 저장합니다. HTTP 응답으로 설정됩니다. 각 방문자 ID는 Adobe 서버의 방문자 프로필과 연결됩니다. 방문자 프로필은 모든 방문자 ID 쿠키 만료와 관계없이 비활성 기간 1년 후 삭제됩니다. `Secure`이(가) &quot;없음&quot;이고 연결이 HTTPS인 경우 `SameSite` 플래그가 설정됩니다. `SameSite`은(는) 기본적으로 자사 쿠키에 대해 &quot;Lax&quot;입니다. `SameSite` 또는 `omtrdc.net`에서와 같이 서드파티 쿠키를 사용할 때 `2o7.net`은(는) &quot;없음&quot;입니다. 단일 CNAME을 사용하여 여러 도메인 또는 속성을 추적할 때 `SameSite`을(를) &quot;없음&quot;으로 설정합니다. |
| **`s_fid`** | 2년 | 33바이트 | 자사 | 대체 고유 방문자 ID 및 타임스탬프를 저장합니다. 타사 쿠키 제한 사항으로 인해 표준 `s_vi` 쿠키를 설정할 수 없는 경우 JavaScript에서 설정합니다. 자사 쿠키 구현에 사용되지 않습니다. |
| **`s_ac`** | 즉각적인 상태가 됨 | 1바이트 | 자사 | AppMeasurement 쿠키를 설정할 올바른 도메인을 확인하는 데 도움이 됩니다. 정적 값 `"1"`을(를) 포함합니다. 이 쿠키가 설정되면 즉시 삭제됩니다. |

## 플러그인에 의해 설정된 쿠키

일부 구현에서는 Analytics에 추가 기능을 제공하는 코드 조각인 플러그인을 사용합니다. 이러한 플러그인은 위에 나열되지 않은 쿠키를 설정할 수 있습니다. 사용 가능한 플러그인 목록과 플러그인이 설정하는 쿠키는 [Analytics 플러그인 개요](https://experienceleague.adobe.com/en/docs/analytics/implementation/vars/plugins/impl-plugins)를 참조하십시오.

## Analytics 쿠키 삭제 결과

방문자가 Analytics 쿠키를 삭제하는 경우 다음을 고려하십시오.

* **방문자 ID가 손실됨:** 쿠키가 삭제되면 Adobe Analytics에서 재방문자를 인식할 수 없습니다. 다음에 사용자가 사이트를 방문할 때 새 방문자로 계산됩니다. [크로스 디바이스 분석](https://experienceleague.adobe.com/en/docs/analytics/components/cda/overview)을 통해 이러한 영향을 완화할 수 있습니다.
* **세션 연속성이 끊어졌습니다.** 모든 세션 기반 또는 다중 방문 분석(예: 속성 또는 전환 추적)이 중단됩니다. 쿠키 삭제 후 발생하는 이벤트 및 전환은 동일한 사용자가 이전 활동에 연결할 수 없습니다.
* **Personalization 및 세그먼테이션이 영향을 받습니다.** 이전 데이터가 현재 방문과 더 이상 연결되지 않으므로 방문자 기록 또는 동작을 기반으로 한 세그먼트 또는 개인화된 경험이 재설정됩니다.
* **도메인 간 추적이 중단됨:** 서드파티 쿠키의 경우 이를 삭제하면 Adobe Analytics에서 사용자가 소유한 여러 도메인 간에 사용자 활동을 연결할 수 없습니다.
