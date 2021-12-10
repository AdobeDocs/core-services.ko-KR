---
description: 서드파티 쿠키 지원이 브라우저 전체에서 어떻게 점점 제한되고 있는지 알아봅니다.
keywords: cookies;privacy
solution: Experience Cloud,Analytics,Target
title: '서드파티 쿠키 지원 변경이 고객에게 영향을 미치는 방식 '
uuid: 27332e0d-6932-4a6e-b97b-0adeced0b050
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: 3d12a1b1-c952-4b42-815d-f64b31429cec
source-git-commit: ae14748aa7b0f0d803d48fe980a6743f53d996ab
workflow-type: ht
source-wordcount: '265'
ht-degree: 100%

---

# 서드파티 쿠키 지원 변경이 고객에게 영향을 미치는 방식{#how-changes-to-third-party-cookie-support-impacts-customers}

서드파티 쿠키에 대한 지원이 브라우저 전반에서 더욱 제한되었습니다. 따라서 Adobe는 고객 요구 사항과 Experience Cloud 애플리케이션 전반에 걸친 개인정보 보호에 대한 소비자의 권리 사이에서 신중하게 균형을 이루는 새로운 애플리케이션을 개발하고 있습니다.

다음 목록에서는 서드파티 쿠키 지원이 Experience Cloud 애플리케이션의 현재 구현에 미치는 영향을 간략하게 설명합니다.

## Adobe Analytics 및 Adobe Target

* 동일한 사이트 활동은 자사 쿠키에만 의존하기 때문에 Analytics 및 Target은 거의 영향을 받지 않습니다. 도메인 전반에 걸친 사용자 활동을 이해하려면 서드파티 쿠키가 필요합니다. 서드파티 쿠키가 차단된 브라우저의 경우에는 쿠키를 사용하는 교차 도메인 추적이 불가능합니다.

## Adobe Experience Manager

* Adobe Experience Manager는 전적으로 고객 도메인 내에서 운영되므로 서드파티 쿠키와는 최소한의 상호 작용만 있고 따라서 영향을 최소화할 수 있습니다.

## Adobe Social

* 고객이 최신 버전의 코드를 가지고 있는 한 Social은 영향을 받지 않습니다.

## Adobe Advertising Cloud

* 검색:

   * 검색이 Adobe Analytics 데이터를 기반으로 최적화된 경우 검색은 Adobe Analytics와 동일한 방식으로 영향을 받습니다.
   * 전환 데이터 수집은 영향을 받지 않아야 합니다.

* 표시:

   * 오늘 날 디스플레이 리마케팅은 전적으로 서드파티 쿠키 사용에 의존합니다.
   * 디스플레이는 또한 동기화를 위한 다양한 광고 네트워크 쿠키의 가용성에 크게 의존합니다.
   * 전체적인 영향은 알려지지 않았습니다. 그러나 디스플레이는 다른 서비스보다 영향을 더 많이 받습니다.
   * Adobe는 내부적으로, 그리고 Adobe의 광고 파트너와 협력하여 광고 게재에 미치는 영향의 전체 범위를 평가하고 있습니다.
