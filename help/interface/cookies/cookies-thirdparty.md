---
description: 서드파티 쿠키 지원이 브라우저 간에 점점 제한되고 있는 방법에 대해 알아봅니다.
keywords: cookies;privacy
solution: Experience Cloud,Analytics,Target
title: 타사 쿠키 지원이 고객에게 미치는 영향 | Adobe Experience Cloud
uuid: 27332e0d-6932-4a6e-b97b-0adeced0b050
translation-type: tm+mt
source-git-commit: 4bea0c29afa580dc63b21535ce5c275cd649c9a5
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 91%

---


# 타사 쿠키 지원 변경 방법이 고객에게 미치는 영향{#how-changes-to-third-party-cookie-support-impacts-customers}

타사 쿠키에 대한 지원이 브라우저 간에 점점 더 많이 제한됨에 따라 Adobe는 고객 요구 사항과 Adobe Experience Cloud 솔루션 전반에 걸친 소비자의 개인 정보 보호 권리 간에 신중하게 균형을 잡는 새로운 솔루션을 개발해왔습니다.

다음 목록은 타사 쿠키 지원이 Adobe Experience Cloud 솔루션의 현재 구현에 미치는 영향을 설명합니다.

## Adobe Analytics 및 Adobe Target

* [자사 구현](/help/interface/cookies/cookies-first-party.md)을 사용하는 고객은 크게 영향을 받지 않습니다.
* 자사 구현을 사용하지 않는 고객은 [Experience Platform ID 서비스](https://docs.adobe.com/content/help/ko-KR/id-service/using/implementation/implementation-guides.html)를 구현하여 자사 구현 없이 ID 쿠키를 자사 쿠키로 저장할 수 있습니다.

## Adobe Experience Manager

* Adobe Experience Manager는 전적으로 고객 도메인 내에서 운영되므로 타사 쿠키와는 최소한의 상호 작용만 있고 따라서 영향을 최소화할 수 있습니다.

## Adobe Social

* 고객이 최신 버전의 코드를 가지고 있는 한 Social은 영향을 받지 않습니다.

## Adobe Advertising Cloud

* 검색:

   * 검색이 Adobe Analytics 데이터를 기반으로 최적화된 경우 검색은 Adobe Analytics와 동일한 방식으로 영향을 받습니다.
   * 전환 데이터 수집은 영향을 받지 않아야 합니다.

* 표시:

   * 오늘 날 디스플레이 리마케팅은 전적으로 타사 쿠키 사용에 의존합니다.
   * 디스플레이는 또한 동기화를 위한 다양한 광고 네트워크 쿠키의 가용성에 크게 의존합니다.
   * 전체적인 영향은 알려지지 않았습니다. 그러나 디스플레이는 다른 서비스보다 영향을 더 많이 받습니다.
   * Adobe는 내부적으로 광고 파트너와 협력하여 광고 게재에 대한 영향을 최대한 평가하고 있습니다.

* Social:

   * Facebook 마켓플레이스 광고에는 아무런 영향이 없습니다.
   * FBX(Facebook Exchange)는 디스플레이 광고 게재와 동일한 영향을 받습니다.
