---
description: 다양한 솔루션 및 서비스에서 페이지 로드 시간을 줄이는 데 도움이 되도록 DNS 프리페치를 구현합니다.
seo-description: 다양한 솔루션 및 서비스에서 페이지 로드 시간을 줄이는 데 도움이 되도록 DNS 프리페치를 구현합니다.
seo-title: 다양한 솔루션 및 서비스에서 DNS 프리페치 사용
solution: Experience Cloud
title: 다양한 솔루션 및 서비스에서 DNS 프리페치 사용
uuid: 4220e223-e00e-46b1-8bde-52248913bea1
translation-type: tm+mt
source-git-commit: f7ec8bf6087a18be41c9efbf05f60e6cfd24e566

---


# 다양한 솔루션 및 서비스에서 DNS 프리페치 사용

다양한 솔루션 및 서비스에서 페이지 로드 시간을 줄이는 데 도움이 되도록 DNS 프리페치를 구현합니다.

## DNS 프리페치 이해하기 {#section_772BF9CB7C4141DE9B0355146E2CD962}

브라우저는 DNS 프리페치를 사용하여 웹 페이지에 연결된 도메인 이름을 해당 IP 주소로 자동으로 확인합니다. 프리페치 프로세스는 브라우저가 웹 페이지를 로드할 때 시작됩니다. 예를 들어 페이지에 `www.adobe.com`에 대한 클릭 가능한 링크가 포함되어 있다고 가정하겠습니다. When a browser loads this page, it uses the [DNS system](https://www.networksolutions.com/support/what-is-a-domain-name-server-dns-and-how-does-it-work/) to look up the linked domain name and resolve it to a corresponding numeric IP address. 사이트 방문자가 해당 링크나 단추를 클릭하기 전에 도메인 이름이 IP 주소로 이미 확인되었기 때문에 DNS 프리페치는 페이지 성능을 향상시키는 데 도움이 됩니다. DNS 프리페치 프로세스는 사용자에게 투명하게 진행됩니다.

## DNS 프리페치 및 Adobe Experience Cloud 솔루션 {#section_202A07F9F79F4ABDA44B98BA1DDCD516}

DNS 프리페치는 페이지의 정적 포함 링크에서 자동으로 작동합니다. 또한 다음과 같은 이유로 인해 자동 DNS 프리페치가 다른 [!UICONTROL Experience] Cloud 솔루션 및 서비스에서 작동하지 않습니다.

* 각 Experience Cloud 솔루션 또는 서비스는 페이지가 로드될 때 동적으로 DNS 호출을 생성합니다.
* 이러한 호출이 수행되기 전에는 브라우저가 도메인 이름을 IP 주소로 확인할 수 없습니다.

그러나 Experience Cloud 솔루션을 사용하여 DNS 프리페치를 수동으로 구현할 수 있습니다. 아래 그림과 같이 HTML `<dns-prefetch>` 태그를 페이지 코드의 `<head>` 섹션에 추가하면 됩니다. 제대로 구현되면 DNS 프리페치가 페이지 로드 시간을 몇 밀리초 줄일 수 있습니다.

## DNS 프리페치 코드 샘플 {#section_E886F7B2861E48BA9EF3D8B3CE32B345}

다음 예는 서로 다른 [!DNL Experience Cloud] 솔루션 및 서비스에 DNS 프리페치를 호출하는 방법을 보여 줍니다. 일부 프리페치 호출에는 [!DNL Adobe] 조직 ID 또는 추적 서버 정보가 필요합니다. 이러한 예에서 *이탤릭체*&#x200B;로 된 코드는 변수 자리 표시자를 나타냅니다. 해당 코드를 자체 [!DNL Adobe] 파트너 ID, 고객 코드 또는 추적 서버 정보 등으로 교체합니다.

* **Analytics:** `<link rel="dns-prefetch" href="//insert tracking server name here">`.

   비보안 및 보안 추적 서버를 사용하는 경우 각 DNS 이름에 대한 별도의 태그를 추가합니다.

* **Audience Manager:** `<link rel="dns-prefetch" href="//dpm.demdex.net">`

* **Experience Cloud ID 서비스:** 여기에 파트너 ID `<link rel="dns-prefetch" href="//fast. *`삽입`*.demdex.net">`

* **Dynamic Tag Manager** (DTM): 필요하지 않습니다. DTM 링크는 페이지가 로드되는 즉시 사용 가능합니다.

* **Media Optimizer(Ad Cloud):**

   * `<link rel="dns-prefetch" href="//pixel.everesttech.net">`
   * `<link rel="dns-prefetch" href="//cm.everesttechnet">`


* **[!DNL Target]:**`<link rel="dns-prefetch" href="//insert customer code here.tt.omtrdc.net">`

>[!MORE_LIKE_THIS]
>
>* [DNS 프리페치](https://www.chromium.org/developers/design-documents/dns-prefetching)

