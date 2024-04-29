---
description: 광고 참여 이벤트를 전환 이벤트에 매핑하고 해당 정보를 사용하여 광고 입찰을 최적화하는 Adobe Advertising 쿠키에 대해 알아봅니다.
title: Adobe Advertising 쿠키
uuid: 2eec48a3-3e81-488e-8e30-5fd62885de0b
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: 6818edea-31b1-49fc-bca2-32828c7ca78d
source-git-commit: c39672f0d8a0fd353b275b2ecd095ada1e2bf744
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 11%

---

# Adobe Advertising 쿠키

Adobe Advertising(이전의 Adobe Advertising Cloud)는 쿠키를 사용하여 광고 참여 이벤트를 전환 이벤트에 매핑하고 해당 정보를 사용하여 광고 입찰을 최적화합니다.

>[!NOTE]
>
>를 사용하는 베타 Adobe Advertising Javascript 태그 [Adobe Experience Cloud ID(ECID) 서비스](https://experienceleague.adobe.com/docs/id-service/using/intro/overview.html?lang=ko-KR) 자사 생성 [Experience Cloud](experience-cloud.md) `s_ecid` Adobe Advertising 쿠키가 아닌 쿠키.

| 쿠키 이름 | 만료 | 크기 | 위치 | 설명 |
| --- | --- | --- | --- | --- |
| **`_lcc`** | 15분 | 52바이트 | `everesttech.net` | 디스플레이 클릭 수의 ID 및 타임스탬프를 저장합니다. 디스플레이 광고의 클릭 이벤트가 Adobe Analytics 히트에 적용되는지 여부를 결정합니다. |
| **`_tmae`** | 1년 | 1 KB | `everesttech.net` | DSP 추적을 사용하여 광고 참여에 대한 인코딩된 ID 및 타임스탬프를 저장합니다. 마지막으로 본 광고와 같은 광고를 통한 사용자 참여 포함 |
| **`adcloud`** | 1년 | 50-150바이트 | 자사 | 방문자가 웹 사이트에 마지막으로 방문한 시점과 방문자가 마지막으로 검색한 클릭의 타임스탬프. 또한 다음을 저장합니다. `ef_id` 방문자가 광고를 클릭할 때 만들어진 것입니다. 방문자 ID를 관련 대상 세그먼트 및 전환과 연결합니다. 불필요한 Adobe 요청을 방지하여 페이지 로드 시간을 최적화하는 데 도움이 됩니다. |
| **`ev_sync_*`** |  | 8바이트 | `everesttech.net` | 동기화가 수행되는 날짜 `yyymmdd` 포맷. Adobe Advertising 방문자 ID를 파트너 광고 교환과 동기화합니다. 새 방문자에 대해 만들어지며 만료되면 동기화 요청을 보냅니다. 쿠키 포함 `ev_sync_ax`, `ev_sync_bk`, `ev_sync_dd`, `ev_sync_fs`, `ev_sync_ix`, `ev_sync_nx`, `ev_sync_ox`, `ev_sync_pm`, `ev_sync_rc`, `ev_sync_tm`, 및 `ev_sync_yh`. |
| **`everest_g_v2`** | 1년 | ~27바이트 | `everesttech.net` | 브라우저 및 방문자 ID를 저장합니다. 사용자가 처음에 광고를 클릭한 후 만들어집니다. 현재 및 후속 클릭을 웹 사이트의 다른 이벤트와 매핑하는 데 사용됩니다. |
| **`everest_session_v2`** | Session | ~16바이트 | `everesttech.net` | 현재 세션 ID를 저장합니다. |
| **`ev_tm`** | 2년 | ~20바이트 | `everesttech.net` | DSP(Adobe Advertising Demand Side Platform) ID를 저장합니다. 의 방문자 ID에 해당합니다. `everest_g_v2` 쿠키. |
| **`id_adcloud`** | 91일 | 16바이트 | 자사 | 방문자 ID를 저장합니다. |

{style="table-layout:auto"}
