---
description: Adobe Analytics에서 어떻게 쿠키를 사용하여 이미지 요청과 브라우저 세션 간에 지속되지 않는 변수 및 구성 요소에 대한 정보를 제공하는지 알아봅니다.
keywords: cookies;privacy
solution: Experience Cloud,Analytics
title: '"자사 쿠키 "'
index: y
snippet: y
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: e15abde5-8027-4aed-a0c1-8a6fc248db5e
source-git-commit: 8ec1639479777a67d351dff699815fde982a968e
workflow-type: tm+mt
source-wordcount: '1616'
ht-degree: 93%

---

# 자사 쿠키 정보

Analytics는 쿠키를 사용하여 이미지 요청과 브라우저 세션 간에 지속되지 않는 변수 및 구성 요소에 대한 정보를 제공합니다. 가능한 경우, Adobe는 자사 쿠키를 사용해 사이트에서 활동을 기록합니다. 소유한 다른 도메인과 같은 다른 사이트에서의 활동을 기록하려면 서드파티 쿠키가 필요합니다.

대부분의 브라우저 및 안티스파이웨어 애플리케이션은 서드파티 쿠키를 거부하고 삭제하도록 설계되었습니다. Adobe에서 쿠키는 서드파티 쿠키가 차단된 경우에만 설정될 수 있습니다. 특정 비헤이비어는 Experience Platform ID 서비스(ECID 서비스) 또는 Analytics 레거시 식별자(s_vi 쿠키)의 사용 여부에 따라 다릅니다.

* 수집 도메인과 사이트 도메인의 일치 여부와 관계없이 [Experience Platform ID 서비스(ECID 서비스)](https://experienceleague.adobe.com/docs/id-service/using/intro/overview.html?lang=en) 는 자사 쿠키를 자동으로 설정합니다. 서로 일치하지 않는 경우 ID 서비스는 JavaScript를 사용하여 사이트 도메인의 쿠키를 설정할 수 있습니다.
* [Analytics 레거시 식별자](https://experienceleague.adobe.com/docs/core-services/interface/administration/ec-cookies/cookies-analytics.html?lang=en) ( `s_vi` 쿠키)를 사용하는 경우, 이는 데이터 수집 서버를 구성한 방식에 따라 다릅니다. 데이터 수집 서버가 사이트의 도메인과 일치하면, 쿠키는 자사 쿠키로 설정됩니다. 데이터 수집 서버가 사이트의 도메인과 일치하지 않으면, 쿠키는 서드파티 쿠키로 설정됩니다. 이 경우, 서드파티 쿠키가 차단되면 Analytics는 표준 &#39;s_vi&#39; 쿠키 대신에 자사 [대체 ID(s_fid)](cookies-analytics.md) 를 설정합니다.

수집 서버가 사이트의 도메인과 일치하는지 확인하려면 CNAME 구현을 사용하여 CNAME 구현의 사용자 지정 도메인에서 Adobe의 데이터 수집 서버로 데이터를 전달할 수 있습니다. 여기에는 Adobe 호스트 도메인을 가리키도록 CNAME 별칭을 구성하기 위한 회사 DNS 설정의 변경도 관련되어 있습니다. 다양한 Adobe 제품이 CNAME 사용을 지원하며, 모든 경우에 CNAME는 특정 고객에 대해 신뢰할 수 있는 자사 엔드포인트를 만드는 데 사용되고, 해당 고객이 소유합니다. 여러 도메인을 제어하는 경우 도메인 간 사용자를 추적하기 위해 단일 CNAME 엔드포인트를 사용할 수 있지만, 사이트 도메인이 CNAME 도메인 쿠키와 일치하지 않으면 모두 서드파티로 설정됩니다.

>[!NOTE]
>
>수집 도메인이 사이트 도메인과 일치하는지에 관계없이 Apple의 ITP(Intelligent Tracking Prevention) 프로그램은 macOS의 Safari와 iOS 및 iPadOS의 모든 브라우저를 포함하는 ITP가 관리하는 브라우저에서 Adobe이 설정한 자사 쿠키를 단기간 동안 만듭니다. 2020년 11월 현재 CNAME를 통해 설정한 쿠키와 JavaScript를 통해 설정한 쿠키의 만료일이 동일합니다. 이 만료일은 변경될 수 있습니다.

데이터 수집에 CNAME를 설정하려는 경우와 사이트에 HTTPS 프로토콜을 사용하는 보안 페이지가 있는 경우, 자사 쿠키를 구현하기 위해 Adobe와 협력하여 SSL 인증서를 구할 수 있습니다.

SSL 인증서 발급 프로세스는 종종 혼란스럽고 시간이 걸릴 수 있습니다. 그 결과 Adobe는 업계 선도적인 인증 기관(CA)인 DigiCert와의 파트너십을 구축했으며 이러한 인증서의 구매 및 관리를 자동화하는 통합 프로세스를 개발했습니다.

귀하의 권한이 주어지면 Adobe는 CA와 협력하여 새로운 SHA-2 SSL 인증서를 발행, 배포 및 관리할 것입니다. Adobe는 예상치 못한 만료, 해지 또는 보안 문제가 조직의 보안 수집을 위협하지 않도록 이 인증서를 계속 관리합니다.

## Adobe 관리 인증서 프로그램

Adobe 관리 인증서 프로그램은 Adobe 수집 서버와 사이트 도메인이 서로 일치하도록 CNAME 구현에 필요한 자산 SSL 인증서를 설정하는 권장 프로세스입니다.

Adobe 관리 인증서 프로그램에서는 추가 비용 없이 새로운 자사 SSL 인증서를 구현할 수 있습니다(처음 100개 CNAME에 대해). 현재 자체 고객 관리 SSL 인증서를 보유하고 있는 경우 Adobe 관리 인증서 프로그램으로 마이그레이션하는 방법에 대해 Adobe 고객 지원 센터에 문의하십시오.

### 구현

자사 데이터 수집을 위한 새 자사 SSL 인증서를 구현하는 방법은 다음과 같습니다.

1. [자사 도메인 요청 양식](/help/interface/cookies/assets/First_Part_Domain_Request_Form.xlsx) 을 작성하고 Adobe 관리 프로그램에서 자사 데이터 수집을 설정하도록 요청하는 고객 지원 센터를 통해 티켓을 엽니다. 문서 내에 각 필드가 예와 함께 설명되어 있습니다.

2. CNAME 레코드를 만듭니다(아래 지침 참조).

   티켓을 수령하는 즉시 고객 지원 센터에서 CNAME 기록을 제공해야 합니다. Adobe가 귀하를 대신하여 인증서를 구입할 수 있으려면 먼저 회사의 DNS 서버에서 이러한 레코드를 구성해야 합니다. CNAME은 다음과 비슷합니다.

   **보안** - 예를 들어 호스트 이름 `smetrics.example.com` 은 `example.com.adobedc.net`을 가리킵니다.

>[!NOTE]
> 이전에는 Adobe이 고객에게 HTTPS용 CNAME과 HTTP용 CNAME 1개를 설정하도록 권장했습니다. 이 방법은 트래픽을 암호화하는 가장 좋은 방법이며 대부분의 브라우저에서 HTTP를 강력하게 비활성화하므로 더 이상 HTTP용 CNAME을 설정하지 않는 것이 좋습니다. HTTP에 대해 CNAME을 구성해야 하는 경우 Adobe 고객 지원 센터에 문의하십시오.

1. CNAME이 설치되면, Adobe는 DigiCert와 협력하여 Adobe 프로덕션 서버에 인증서를 구입하고 설치합니다.

   기존 구현이 있는 경우 기존 방문자를 유지하기 위해 방문자 마이그레이션을 고려해야 합니다. 인증서가 Adobe의 프로덕션 환경에 라이브로 푸시된 후 추적 서버 변수를 새로운 호스트 이름으로 업데이트할 수 있습니다. 즉, 사이트가 안전하지 않은 경우(HTTP) `s.trackingServer`를 업데이트하십시오. 사이트가 안전한 경우(HTTPS) `s.trackingServer` 및 `s.trackingServerSecure` 변수를 모두 업데이트합니다.

2. [호스트 이름 전달의 유효성을 검사합니다](#validate) (아래 참조).

3. [구현 코드를 업데이트합니다](#update) (아래 참조).

### 유지 관리 및 갱신

SSL 인증서는 매년 만료됩니다. 즉, Adobe는 매년 각 구현에 대한 새 인증서를 구입해야 합니다. 조직 내의 지원되는 모든 사용자는 구현 만료 시기가 다가올 때마다 이메일 알림을 받게 됩니다. Adobe가 호스트 이름을 갱신하기 위해, 지원되는 한 사용자는 Adobe에서 이메일에 회신하고 데이터 수집을 위해 만료되는 호스트 이름을 계속 사용할 계획임을 나타내야 합니다. 이때 Adobe는 자동으로 새 인증서를 구입하여 설치합니다.

### 자주 묻는 질문

| 질문 | 답변 |
|---|---|
| **이 프로세스는 안전합니까?** | 예. Adobe 관리 프로그램은 Adobe의 기존 방식보다 더 안전하며 Adobe 및 인증 기관의 외부에서 인증서나 개인 키가 변경되지 않습니다. |
| **Adobe는 어떻게 도메인의 인증서를 구입할 수 있습니까?** | Adobe 소유 호스트 이름에 지정된 호스트 이름(예: `telemetry.example.com`)을 지정한 경우에만 인증서를 구입할 수 있습니다. 이것은 본질적으로 이 호스트 이름을 Adobe에 위임하며 Adobe가 사용자를 대신하여 인증서를 구매할 수 있도록 합니다. |
| **인증서가 해지되도록 요청할 수 있습니까?** | 예. 도메인의 소유는 인증서를 해지하도록 요청할 수 있습니다. 이렇게 하려면 고객 지원 센터에서 티켓을 열면 됩니다. |
| **이 인증서는 SHA-2 암호화를 사용합니까?** | 예. Adobe는 DigiCert와 협력하여 SHA-2 인증서를 발행합니다. |
| **이 경우 추가 비용이 발생합니까?** | 아니요. Adobe는 현재 모든 Adobe Digital Experience 고객에게 추가 비용 없이 이 서비스를 제공하고 있습니다. |

{style=&quot;table-layout:auto&quot;}

## CNAME 레코드 만들기

조직의 네트워크 작업 팀은 새 CNAME 레코드를 만들어 DNS 서버를 구성해야 합니다. 각 호스트 이름은 Adobe의 데이터 수집 서버로 데이터를 전달합니다.

FPC 전문가가 구성된 호스트 이름과 지정할 CNAME을 제공합니다. 예:

* **SSL 호스트 이름**:`smetrics.mysite.com`
* **SSL CNAME**:`mysite.com.adobedc.net`

>[!NOTE]
> 여전히 비-보안 상태로 사용한다면 다음과 같이 표시됩니다.
> * **비SSL 호스트 이름**:`metrics.mysite.com`
> * **비 SSL CNAME**:`mysite.com.adobedc.net`


구현 코드를 변경하지 않는 한, 이 단계는 데이터 수집에 영향을 주지 않으며 구현 코드를 업데이트한 후 언제든지 완료할 수 있습니다.

## 호스트 이름 전달의 유효성 검사 {#validate}

유효성 검사에는 다음 방법을 사용할 수 있습니다.

### 브라우저를 사용하여 유효성 검사

CNAME이 설정되어 있고 인증서가 설치되어 있으면 브라우저를 사용하여 유효성을 검사할 수 있습니다.

`https://smetrics.adobe.com/_check`

>[!NOTE]
>
>인증서가 설치되어 있지 않으면 보안 경고가 표시됩니다.

### [!DNL curl]을 사용하여 유효성 검사

명령줄에서 [[!DNL curl]](https://curl.se/) 을 사용하는 것이 좋습니다. ([!DNL Windows] 사용자는 <https://curl.se/windows/>에서 [!DNL curl] 을 설치할 수 있습니다.)

CNAME이 있지만 인증서가 설치되어 있지 않다면
`curl -k https://smetrics.adobe.com/_check`
를 실행하십시오.
응답: `SUCCESS`

( `-k` 값은 보안 경고를 비활성화합니다.)

CNAME이 설정되어 있고 인증서가 설치되어 있다면
`curl https://smetrics.adobe.com/_check`
를 실행하십시오.
응답: `SUCCESS`

### [!DNL nslookup]을 사용하여 유효성 검사

유효성 검사에 `nslookup` 을 사용할 수 있습니다. 예를 들어 `smetrics.adobe.com`을 사용하는 경우 명령 프롬프트를 열고 `nslookup smetrics.adobe.com`을 입력하십시오.

모든 것이 성공적으로 설정되면 다음과 비슷한 결과가 표시됩니다.

```
nslookup smetrics.adobe.com
Server:             10.30.7.247
Address:     10.30.7.247#53

smetrics.adobe.com    canonical name = adobe.com.ssl.d1.sc.omtrdc.net.
Name:  adobe.com.ssl.d1.sc.omtrdc.net
Address: 54.218.180.161
Name:  adobe.com.ssl.d1.sc.omtrdc.net
Address: 52.39.8.230
Name:  adobe.com.ssl.d1.sc.omtrdc.net
Address: 54.187.216.46
```

## 구현 코드 업데이트 {#update}

자사 데이터 수집을 사용하도록 사이트에서 코드를 편집하려면 먼저 다음 전제 조건을 완료하십시오.

* [Adobe 관리 인증서 프로그램](#adobe-managed-certificate-program)의 *구현* 섹션에서 위에 설명된 절차를 수행하여 SSL 인증서를 요청합니다.
* CNAME 레코드를 만듭니다(위 참조).
* 호스트 이름의 유효성을 확인합니다(위 참조).

호스트 이름이 응답하고 데이터 수집 서버로 전달하는 것을 확인한 후에는 사용자의 구현을 변경하여 자신의 데이터 수집 호스트 이름을 가리키도록 할 수 있습니다.

1. 코어 JavaScript 파일(`s_code.js/AppMeasurement.js`)을 엽니다.
1. 코드 버전을 업데이트하려면 전체 `s_code.js/AppMeasurement.js` 파일을 최신 버전으로 바꾸고 플러그인 또는 사용자 지정으로 바꿉니다. **또는** 자사 데이터 수집과 관련된 코드만 업데이트하려면 s.trackingServer 및 s.trackingServerSecure(SSL 사용 시)를 찾아 새로운 데이터 수집 호스트 이름을 지정합니다. mysite.com 사용 예:`s.trackingServer = "metrics.mysite.com"` `s.trackingServerSecure = "smetrics.mysite.com"`

1. 업데이트된 코어 JavaScript 파일을 해당 사이트에 업로드합니다.

1. 장기간 구현에서 자사 데이터 수집으로 이동하거나 다른 자사 컬렉션 호스트 이름으로 변경하려는 경우, Adobe는 이전 도메인에서 새 도메인으로 방문자를 마이그레이션할 것을 권장합니다.

Analytics 구현 안내서의 [방문자 마이그레이션](https://experienceleague.adobe.com/docs/analytics/technotes/visitor-migration.html?lang=en) 을 참조하십시오.

JavaScript 파일을 업로드한 후에는 모든 것이 자사 쿠키 데이터 수집에 맞게 구성됩니다. Adobe는 데이터 수집이 정상적으로 진행될 수 있도록 다음 몇 시간 동안 Analytics 보고를 모니터링할 것을 권장합니다. 그렇지 않으면 위의 모든 단계가 완료되었음을 확인하고 조직에서 지원하는 사용자 중 한 명이 고객 지원 센터에 문의하도록 하십시오.
