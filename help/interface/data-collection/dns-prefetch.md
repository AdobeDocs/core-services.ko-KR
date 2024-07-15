---
description: Experience Cloud의 다양한 애플리케이션과 서비스를 사용하여 페이지 로드 시간을 줄이는 데 도움이 되는 DNS 프리페치를 구현하는 방법을 알아봅니다.
solution: Experience Cloud
title: DNS 프리페치 사용
uuid: 4220e223-e00e-46b1-8bde-52248913bea1
topic: Administration
role: Admin
level: Experienced
exl-id: caf2ff76-2076-436d-a5a7-aff531464480
source-git-commit: 9ee4d9b0e670dec35cda530892c49e36bf7cc107
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 92%

---

# DNS 프리페치 사용

다양한 애플리케이션 및 서비스에서 페이지 로드 시간을 줄이는 데 도움이 되도록 DNS 프리페치를 구현합니다.

## DNS 프리페치 이해하기

브라우저에서는 DNS 프리페치를 사용하여 웹 페이지에 링크된 도메인 이름을 해당 IP 주소로 자동으로 확인합니다. 브라우저에서 웹 페이지를 로드하면 프리페치 프로세스가 시작됩니다. 예를 들어 페이지에 `www.adobe.com`에 대한 선택 가능 링크가 포함되어 있다고 가정하겠습니다. 브라우저에 이 페이지가 로드되면 [DNS 시스템](https://www.networksolutions.com/support/what-is-a-domain-name-server-dns-and-how-does-it-work/) 을 사용하여 링크된 도메인 이름을 검색하고 해당 숫자 IP 주소로 확인합니다. 사이트 방문자가 해당 링크 또는 버튼을 클릭하기 전에 도메인 이름이 이미 IP 주소로 확인되었으므로 DNS 프리페치는 페이지 성능을 향상시키는 데 도움이 됩니다. DNS 프리페치 프로세스는 사용자에게 투명합니다.

## DNS 프리페치 및 Adobe Experience Cloud 애플리케이션

DNS 프리페치는 페이지에 임베드된 정적 링크에서 자동으로 작동합니다. 즉, 다음과 같은 이유로 다른 [!UICONTROL Experience Cloud] 응용 프로그램 및 서비스에서는 자동 DNS 프리페치가 작동하지 않습니다.

* 각 Experience Cloud 애플리케이션 또는 서비스는 페이지가 로드될 때 동적으로 DNS 호출을 생성합니다.
* 이러한 호출을 수행하기 전에 브라우저에서 IP 주소로 도메인 이름을 확인할 수 없습니다.

하지만 Experience Cloud 애플리케이션으로 DNS 프리페치를 수동으로 구현할 수 있습니다. 아래 그림과 같이 HTML `<dns-prefetch>` 태그를 페이지 코드의 `<head>` 섹션에 추가하면 됩니다. 제대로 구현되면 DNS 프리페치가 페이지 로드 시간을 몇 밀리초 줄일 수 있습니다.

## DNS 프리페치 코드 샘플

다음 예는 서로 다른 [!DNL Experience Cloud] 애플리케이션 및 서비스에 DNS 프리페치를 호출하는 방법을 보여 줍니다. 일부 프리페치 호출에는 [!DNL Adobe] 조직 ID 또는 추적 서버 정보가 필요합니다. 이러한 예에서 *이탤릭체*&#x200B;로 된 코드는 변수 자리 표시자를 나타냅니다. 해당 코드를 자체 [!DNL Adobe] 파트너 ID, 고객 코드 또는 추적 서버 정보 등으로 교체합니다.

* **Analytics:** `<link rel="dns-prefetch" href="//data.example.com">`.

  비보안 및 보안 추적 서버를 사용하는 경우 각 DNS 이름에 대한 별도의 태그를 추가합니다.

* **Audience Manager:** `<link rel="dns-prefetch" href="//dpm.demdex.net">`

* **Experience Cloud ID 서비스:** `<link rel="dns-prefetch" href="//fast.examplepartnerid.demdex.net">`

* **Advertising Cloud:**

   * `<link rel="dns-prefetch" href="//pixel.everesttech.net">`
   * `<link rel="dns-prefetch" href="//cm.everesttech.net">`

* **[!DNL Target]:** `<link rel="dns-prefetch" href="//example.tt.omtrdc.net">`

>[!MORELIKETHIS]
>
>* Chromium에서 [DNS 프리페치](https://www.chromium.org/developers/design-documents/dns-prefetching)
