---
description: Adobe Experience Cloud의 솔루션 및 서비스에서 쿠키가 사용되는 방법을 알아봅니다.
title: Experience Cloud에서 쿠키를 사용하는 방법
uuid: 4255a13a-917b-4b5f-a7d4-4b2e7521d189
exl-id: 60f1a89e-d989-461b-a6a3-c1df022cd30b
source-git-commit: d6dc659104b3b24b60495cd97adb21ebb3962fc7
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 10%

---

# Experience Cloud에서 사용된 쿠키

Adobe Experience Cloud은 쿠키를 사용합니다. 쿠키는 웹 사이트가 나중에 사용하기 위해 브라우저에 전송하는 작은 데이터입니다. 쿠키는 사용자가 다시 방문하거나 페이지 사이를 이동할 때 웹 사이트가 기억하도록 도와줍니다. 쿠키는 방문 횟수를 추적하고 한 장치를 다른 장치와 구별하는 데 도움이 됩니다.

법률은 종종 누군가의 디바이스에서 쿠키를 저장하거나 사용하기 전에 권한을 얻도록 요구합니다. Adobe에서는 법률 팀에 문의하여 적용되는 규칙을 이해할 것을 권장합니다.

## 자사 쿠키 정보

Adobe Experience Cloud은 쿠키를 사용하여 페이지 보기 수 또는 브라우저 세션 간에 지속되지 않는 정보를 추적합니다. 가능한 경우, Adobe은 자사 쿠키(자체 웹 사이트에 연결됨)를 사용합니다. 소유한 여러 사이트 또는 도메인에서 활동을 추적하려면 서드파티 쿠키가 필요합니다.

일부 브라우저 및 안티스파이웨어 도구는 서드파티 쿠키를 차단합니다. Adobe에는 쿠키가 차단된 경우에도 쿠키가 계속 작동하는지 확인하는 방법이 있습니다. 이 방법이 작동하는 방식은 사용자가 Experience Platform ID 서비스(ECID) 또는 이전 Analytics 쿠키(예: `s_vi` 쿠키)를 사용하는지에 따라 다릅니다.

* [Experience Cloud Identity 서비스](https://experienceleague.adobe.com/ko/docs/id-service/using/intro/overview): ECID 서비스는 수집 도메인과 사이트 도메인의 일치 여부에 관계없이 항상 자사 쿠키를 설정합니다. JavaScript을 사용하여 사이트의 도메인에 쿠키를 배치합니다.

* [Analytics 레거시 식별자](analytics.md)(예: `s_vi` 쿠키): 쿠키가 퍼스트 파티 또는 서드파티인지 여부는 설정에 따라 다릅니다.

   * 데이터 수집 서버가 사이트의 도메인과 일치하면, 쿠키는 자사 쿠키입니다.
   * 일치하지 않으면 쿠키는 서드파티입니다. 서드파티 쿠키가 차단되면 Adobe은 일반적인 쿠키가 아닌 대체 쿠키(`s_fid`)를 설정합니다.

수집 서버가 사이트의 도메인과 일치하는지 확인하기 위해 **CNAME 설정**&#x200B;을 사용할 수 있습니다. 여기에는 Adobe 서버로 사용자 정의 도메인(소유)을 가리키도록 DNS 설정을 업데이트하는 작업이 포함됩니다. 이렇게 하면 추적 쿠키가 자사 쿠키로 표시됩니다. 하나의 CNAME이 여러 도메인에서 작동할 수 있지만 CNAME과 일치하지 않는 도메인은 여전히 서드파티 쿠키를 설정합니다.

>[!NOTE]
>
>Apple의 ITP(Intelligent Tracking Prevention)는 수집 도메인과 사이트 도메인이 일치하는 경우에도 Adobe의 자사 쿠키가 지속되는 기간을 제한합니다. ITP는 macOS의 Safari와 iOS 및 iPadOS의 모든 브라우저에 영향을 줍니다. 2020년 11월부터 CNAME을 사용하여 설정된 쿠키는 JavaScript으로 설정된 쿠키와 동일하게 만료됩니다. 이 시간 제한은 나중에 변경될 수 있습니다.

다음은 텍스트 간소화 버전입니다.

## 쿠키 및 개인정보 보호

Adobe은 개인 정보 보호 및 데이터 보안을 중요하게 생각합니다. 개인 정보 보호 조직, 규제 기관 및 AdChoices와 같은 프로그램과 함께 작동하여 사람들이 데이터 사용 방법을 제어할 수 있도록 합니다.

Adobe Experience Cloud의 대부분의 쿠키는 개인 정보를 저장하지 않습니다. 이 솔루션은 안전하고 귀사에서만 보고, 컨텐츠 및 광고에 사용됩니다. Adobe은 이 데이터를 다른 고객 또는 서드파티와 공유하지 않습니다. 단, 익명의 업계 전체 보고서(예: Digital Marketing Insight 보고서)는 예외입니다.

Adobe은 서로 다른 회사의 브라우저 데이터를 결합하지 않습니다. 개인정보 보호를 위해 일부 Adobe 도구는 각 웹 사이트에서 자체 쿠키 세트를 사용할 수 있도록 합니다. 또한 일부는 쿠키에 자체 도메인을 사용할 수 있도록 허용하므로, 자사 쿠키를 보다 안전하게 사용할 수 있습니다.

쿠키는 이전에 저장된 정보만 저장할 수 있습니다. 장치에서 코드를 실행하거나 다른 데이터를 읽을 수 없습니다. 또한 웹 브라우저에서는 쿠키를 설정한 웹 사이트에서만 읽을 수 있습니다. 예를 들어, Adobe.com만 설정된 쿠키를 읽을 수 있습니다.

다음 다이어그램은 표준 이미지 요청에 대한 쿠키 사용을 보여 줍니다.

![표준 이미지 요청에 대한 쿠키 사용](assets/CookiesProcessGraphic-01.png)

다음 다이어그램은 직접 이미지 요청에 대한 쿠키 사용을 보여 줍니다(JS 파일이 로드되지 않은 시나리오에서 사용됨).

![직접 이미지 요청에 대한 쿠키 사용](assets/CookiesProcessGraphic2.png)
