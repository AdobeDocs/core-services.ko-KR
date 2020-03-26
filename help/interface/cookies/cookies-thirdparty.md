---
description: 타사 쿠키에 대한 지원이 브라우저 간에 점점 더 많이 제한됨에 따라 Adobe는 고객 요구 사항과 Adobe Experience Cloud 솔루션 전반에 걸친 소비자의 개인 정보 보호 권리 간에 신중하게 균형을 잡는 새로운 솔루션을 개발해왔습니다.
keywords: cookies;privacy
seo-description: 타사 쿠키에 대한 지원이 브라우저 간에 점점 더 많이 제한됨에 따라 Adobe는 고객 요구 사항과 Adobe Experience Cloud 솔루션 전반에 걸친 소비자의 개인 정보 보호 권리 간에 신중하게 균형을 잡는 새로운 솔루션을 개발해왔습니다.
seo-title: 타사 쿠키 지원 변경으로 인한 고객 영향
solution: Marketing Cloud,Analytics,Adobe Target,Adobe Social
title: 타사 쿠키 지원 변경으로 인한 고객 영향
uuid: 27332e0d-6932-4a6e-b97b-0adeced0b050
translation-type: tm+mt
source-git-commit: f7ec8bf6087a18be41c9efbf05f60e6cfd24e566

---


# How changes to third-party cookie support impact customers{#how-changes-to-third-party-cookie-support-impacts-customers}

타사 쿠키에 대한 지원이 브라우저 간에 점점 더 많이 제한됨에 따라 Adobe는 고객 요구 사항과 Adobe Experience Cloud 솔루션 전반에 걸친 소비자의 개인 정보 보호 권리 간에 신중하게 균형을 잡는 새로운 솔루션을 개발해왔습니다.

다음 목록은 타사 쿠키 지원이 Adobe Experience Cloud 솔루션의 현재 구현에 어떤 영향을 미치는지 보여줍니다.

## Adobe Analytics 및 Adobe Target

* [자사 구현](/help/interface/cookies/cookies-first-party.md)을 사용하는 고객은 크게 영향을 받지 않습니다.
* Customers that are not using first-party implementation can implement the [Experience Platform ID Service](https://docs.adobe.com/content/help/en/id-service/using/implementation-guides/implementation-guides.html) to store the ID cookie as a first-party cookie without a first-party implementation.

## Adobe Experience Manager

* Adobe Experience Manager는 전적으로 고객 도메인 내에서 운영되므로 타사 쿠키와는 최소한의 상호 작용만 있고 따라서 영향을 최소화할 수 있습니다.

## Adobe Social

* 고객이 최신 버전의 코드를 가지고 있는 한 Social은 영향을 받지 않습니다.

## Adobe Advertising Cloud

* 검색:

   * Adobe Analytics 데이터를 기반으로 검색을 최적화하면 Adobe Analytics와 같은 방식으로 검색에 영향을 줍니다.
   * 전환 데이터 수집은 영향을 받지 않습니다.

* 표시:

   * 오늘날 디스플레이 리마케팅은 전적으로 타사 쿠키 사용에 따라 달라집니다.
   * 또한 디스플레이는 동기화를 위한 다양한 광고 네트워크 쿠키의 가용성에 따라 크게 달라집니다.
   * 전체적인 영향은 알려지지 않았다. 그러나 첫 번째 시점에서는 디스플레이가 다른 서비스보다 더 영향을 받습니다.
   * Adobe는 광고 파트너와 내부적으로 협력하여 광고 게재에 미치는 영향을 전반적으로 평가하고 있습니다.

* Social:

   * Facebook 시장 광고에 영향을 주지 않습니다.
   * Facebook Exchange(FBX)는 디스플레이 광고 게재와 동일한 영향을 받습니다.
