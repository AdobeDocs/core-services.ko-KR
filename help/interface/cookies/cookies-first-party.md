---
description: Analytics는 쿠키를 사용하여 이미지 요청과 브라우저 세션 간에 지속되지 않는 변수 및 구성 요소에 대한 정보를 제공합니다.
keywords: cookies;privacy
seo-description: Analytics는 쿠키를 사용하여 이미지 요청과 브라우저 세션 간에 지속되지 않는 변수 및 구성 요소에 대한 정보를 제공합니다.
seo-title: 퍼스트 파티 쿠키
solution: Experience Cloud,Analytics
title: 퍼스트 파티 쿠키
index: y
snippet: y
translation-type: ht
source-git-commit: c8d38647750747212c2b825feff600419c1f3352
workflow-type: ht
source-wordcount: '1464'
ht-degree: 100%

---


# 자사 쿠키 정보

Analytics는 쿠키를 사용하여 이미지 요청과 브라우저 세션 간에 지속되지 않는 변수 및 구성 요소에 대한 정보를 제공합니다. 무해한 이러한 쿠키는 Adobe에서 호스트하는 도메인에서 생성되는 것으로서 타사 쿠키라고 합니다.

대부분의 브라우저 및 안티스파이웨어 애플리케이션은 Analytics 데이터 수집에서 사용되는 쿠키를 포함하여 타사 쿠키를 거부하고 삭제하도록 설계되었습니다. 방문자가 웹 사이트와 상호 작용하는 방법에 대한 추적을 지원하기 위해 자사 쿠키를 구현할 수 있습니다.

자사 쿠키를 구현하는 데 두 가지 옵션을 사용할 수 있습니다.

* Experience Platform ID 서비스. ID 서비스는 JavaScript를 사용하여 자사 컨텍스트에서 쿠키를 설정할 수 있습니다.
* CNAME 별칭을 Adobe 호스팅 도메인에 구성하기 위한 회사 DNS 서버의 DNS 항목입니다. 다양한 Adobe 제품이 CNAME 사용을 지원하며 모든 경우에 CNAME은 특정 고객에 대해 신뢰할 수 있는 자사 엔드포인트를 만드는 데 사용되며 해당 고객이 소유합니다. 해당 고객이 여러 도메인을 제어하는 경우 이 고객은 하나의 CNAME 엔드포인트를 사용하여 도메인에서 사용자를 추적할 수 있지만, 이렇게 하려면 CNAME 도메인의 외부에 있는 모든 도메인에 대한 타사 쿠키가 필요하므로 타사 쿠키가 차단되면 CNAME 엔드포인트가 작동하지 않으므로 권장되지 않습니다. Adobe CNAME은 서로 다른 고객이 소유한 도메인들에서 개인 또는 장치를 추적하는 데에는 사용되지 않습니다.

Adobe Experience Cloud ID 서비스에서 첫 번째 옵션을 사용할 때에도 Apple의 ITP는 자사 쿠키를 단명하게 하므로 두 번째 옵션과 함께 사용하는 것이 가장 좋습니다.

CNAME을 사용하는 두 번째 옵션의 경우 사이트에 HTTPS 프로토콜을 사용하는 보안 페이지가 있다면 자사 쿠키를 구현하기 위해 Adobe와 협력하여 SSL 인증서를 구할 수 있습니다. Adobe는 2020년 하반기에 HTTP 컬렉션에 대한 지원을 중단할 예정이므로 데이터 수집에 HTTPS만 사용할 것을 강력히 권장합니다.

SSL 인증서 발급 프로세스는 종종 혼란스럽고 시간이 걸릴 수 있습니다. 그 결과 Adobe는 업계 선도적인 인증 기관(CA)인 DigiCert와의 파트너십을 구축했으며 이러한 인증서의 구매 및 관리를 자동화하는 통합 프로세스를 개발했습니다.

귀하의 허가가 있으면 Adobe는 CA와 협력하여 새로운 SHA-2 SSL 인증서를 발행, 배포 및 관리할 것입니다. Adobe는 이 인증서를 계속 관리하며 예상치 못한 만료, 해지 또는 보안 문제가 조직의 보안 수집을 위협하지 않도록 합니다.

## Adobe 관리 인증서 프로그램

Adobe 관리 인증서 프로그램은 자사 쿠키를 위한 새 자사 SSL 인증서를 구현하는 권장 프로세스입니다.

Adobe 관리 인증서 프로그램에서는 추가 비용 없이 자사 쿠키를 위한 새로운 자사 SSL 인증서를 구현할 수 있습니다(처음 100개 CNAME에 대해). 현재 자체 고객 관리 SSL 인증서를 보유하고 있는 경우 Adobe 관리 인증서 프로그램으로 마이그레이션하는 방법에 대해 Adobe 고객 지원 센터에 문의하십시오.

### 구현

자사 쿠키를 위한 새 자사 SSL 인증서를 구현하는 방법은 다음과 같습니다.

1. [자타 쿠키 요청 양식](/help/interface/cookies/assets/FPC_Request_Form.xlsx)을 작성하고 Adobe 관리 프로그램에서 자사 쿠키를 설정하도록 요청하는 고객 지원 센터를 통해 티켓을 엽니다. 문서 내에 각 필드가 예와 함께 설명되어 있습니다.

1. CNAME 레코드를 만듭니다(아래 지침 참조).

   티켓을 받으면 고객 지원 담당자가 CNAME 레코드 쌍을 제공해야 합니다. Adobe가 귀하를 대신하여 인증서를 구입할 수 있으려면 먼저 회사의 DNS 서버에서 이러한 레코드를 구성해야 합니다. CNAMES는 다음과 유사합니다.

   **보안** - 예를 들어 호스트 이름 `smetrics.example.com`은 `example.com.ssl.d1.omtrdc.net`을 가리킵니다.

   **비보안** - 예를 들어 호스트 이름 `metrics.example.com`은 `example.com.d1.omtrdc.net`을 가리킵니다.

1. 이러한 CNAME이 준비되면 Adobe는 DigiCert와 협력하여 Adobe 프로덕션 서버에서 인증서를 구매 및 설치합니다.

   기존 구현이 있는 경우 기존 방문자를 유지하기 위해 방문자 마이그레이션을 고려해야 합니다. 인증서가 Adobe의 프로덕션 환경에 라이브로 푸시된 후 추적 서버 변수를 새로운 호스트 이름으로 업데이트할 수 있습니다. 즉, 사이트가 안전하지 않은 경우(HTTP) `s.trackingServer`를 업데이트하십시오. 사이트가 안전한 경우(HTTPS) `s.trackingServer` 및 `s.trackingServerSecure` 변수를 모두 업데이트합니다.

1. [호스트 이름 전달의 유효성을 확인합니다](#validate)(아래 참조).

1. [구현 코드를 업데이트합니다](#update)(아래 참조).

### 유지 관리 및 갱신

SSL 인증서는 매년 만료됩니다. 즉, Adobe는 매년 각 구현에 대한 새 인증서를 구입해야 합니다. 조직 내의 지원되는 모든 사용자는 구현 만료가 가까워올 때마다 이메일 알림을 받게 됩니다. Adobe가 호스트 이름을 갱신하기 위해, 지원되는 한 사용자는 Adobe에서 이메일에 회신하고 데이터 수집을 위해 만료되는 호스트 이름을 계속 사용할 계획임을 나타내야 합니다. 이때 Adobe는 자동으로 새 인증서를 구입하여 설치합니다.

### FAQ

| 질문 | 답변 |
|---|---|
| **이 프로세스는 안전합니까?** | 예, Adobe 관리 프로그램은 Adobe의 기존 방식보다 더 안전하며 Adobe와 인증 기관의 외부에서 인증서나 개인 키가 변경되지 않습니다. |
| **Adobe는 어떻게 도메인의 인증서를 구입할 수 있습니까?** | Adobe 소유 호스트 이름에 지정된 호스트 이름(예: `smetrics.example.com`)을 지정한 경우에만 인증서를 구입할 수 있습니다. 이것은 본질적으로 이 호스트 이름을 Adobe에 위임하며 Adobe가 사용자를 대신하여 인증서를 구매할 수 있도록 합니다. |
| **인증서가 해지되도록 요청할 수 있습니까?** | 예, 도메인의 소유는 인증서를 해지하도록 요청할 수 있습니다. 이렇게 하려면 고객 지원 센터에서 티켓을 열면 됩니다. |
| **이 인증서는 SHA-2 암호화를 사용합니까?** | 예, Adobe는 DigiCert와 협력하여 SHA-2 인증서를 발행합니다. |
| **이 경우 추가 비용이 발생합니까?** | 아니요, Adobe는 현재 모든 Adobe Digital Experience 고객에게 추가 비용 없이 이 서비스를 제공하고 있습니다. |

## CNAME 레코드 작성

조직의 네트워크 작업 팀은 새 CNAME 레코드를 만들어 DNS 서버를 구성해야 합니다. 각 호스트 이름은 Adobe의 데이터 수집 서버로 데이터를 전달합니다.

FPC 전문가는 구성된 호스트 이름과 가리키는 CNAME을 제공합니다. 예:

* **SSL 호스트 이름**:`smetrics.mysite.com`
* **SSL CNAME**:`mysite.com.ssl.sc.omtrdc.net`
* **비SSL 호스트 이름**:`metrics.mysite.com`
* **비 SSL CNAME**:`mysite.com.sc.omtrdc.net`

구현 코드를 변경하지 않는 한, 이 단계는 데이터 수집에 영향을 주지 않으며 구현 코드를 업데이트한 후 언제든지 완료할 수 있습니다.

>[!N참고:]
>
>Experience Cloud 방문자 ID 서비스에서는 자사 쿠키를 활성화하도록 CNAME을 구성하는 것에 대한 대안을 제공하지만, 최근의 Apple ITP 변경 사항으로 인해 Experience Cloud ID 서비스를 사용하는 경우에도 여전히 CNAME을 할당하는 것이 좋습니다.

## 호스트 이름 전달의 유효성 확인 {#validate}

유효성 확인에는 다음 방법을 사용할 수 있습니다.

### 브라우저를 사용하여 유효성 확인

CNAME이 설정되어 있고 인증서가 설치되어 있으면 브라우저를 사용하여 유효성을 확인할 수 있습니다.

`https://sstats.adobe.com/_check`

>[!N참고:]
>
>인증서가 설치되어 있지 않으면 보안 경고가 표시됩니다.

### [!DNL curl]을 사용하여 유효성 확인

명령줄에서 [!DNL [curl](https://curl.haxx.se/)]을 사용하는 것이 좋습니다. ([!DNL Windows] 사용자는 <https://curl.haxx.se/windows/>에서 [!DNL curl]을 설치할 수 있습니다.)

CNAME이 있지만 인증서가 설치되어 있지 않다면 `curl -k https://sstats.adobe.com/_check`를 실행하십시오.
응답: `SUCCESS`

(`-k` 값은 보안 경고를 비활성화합니다.)

CNAME이 설정되어 있고 인증서가 설치되어 있다면 `curl https://sstats.adobe.com/_check`를 실행하십시오.
응답: `SUCCESS`

### [!DNL nslookup]을 사용하여 유효성 확인

유효성 확인에 `nslookup`을 사용할 수 있습니다. 예를 들어 `sstats.adobe.com`을 사용하는 경우 명령 프롬프트를 열고 `nslookup sstats.adobe.com`을 입력하십시오.

모든 것이 성공적으로 설정되면 다음과 비슷한 결과가 표시됩니다.

```
nslookup sstats.adobe.com
Server:             10.30.7.247
Address:     10.30.7.247#53

sstats.adobe.com    canonical name = adobe.com.ssl.d1.sc.omtrdc.net.
Name:  adobe.com.ssl.d1.sc.omtrdc.net
Address: 54.218.180.161
Name:  adobe.com.ssl.d1.sc.omtrdc.net
Address: 52.39.8.230
Name:  adobe.com.ssl.d1.sc.omtrdc.net
Address: 54.187.216.46
```

## 구현 코드 업데이트 {#update}

자사 쿠키를 활용하도록 사이트에서 코드를 편집하려면 먼저 다음 전제 조건을 완료하십시오.

* [Adobe Managed Certificate 프로그램](#adobe-managed-certificate-program)의 *구현* 섹션에서 위에 설명된 절차를 수행하여 SSL 인증서를 요청합니다.
* CNAME 레코드를 만듭니다(위 사항 참조).
* 호스트 이름의 유효성을 확인합니다(위 참조).

호스트 이름이 응답하고 데이터 수집 서버로 전달하는 것을 확인했으면 사용자의 구현을 변경하여 자신의 데이터 수집 호스트 이름을 가리키도록 할 수 있습니다.

1. 코어 JavaScript 파일(`s_code.js/AppMeasurement.js`)을 엽니다.
1.  코드 버전을 업데이트하려면 전체`s_code.js/AppMeasurement.js` 파일을 최신 버전으로 바꾸고 플러그인 또는 사용자 지정으로 바꿉니다. **또는** 자사 쿠키와 관련된 코드만 업데이트하려면 s.trackingServer 및 s.trackingServerSecure(SSL 사용 시)를 찾아 새로운 데이터 수집 호스트 이름을 지정합니다. mysite.com 사용 예:`s.trackingServer = "metrics.mysite.com"` `s.trackingServerSecure = "smetrics.mysite.com"`

1. 업데이트된 코어 JavaScript 파일을 해당 사이트에 업로드합니다.

1. 장기간 구현에서 자사 쿠키로 이동하거나 다른 자사 컬렉션 호스트 이름으로 변경하려는 경우 이전 도메인에서 새 도메인으로 방문자를 마이그레이션하는 것이 좋습니다.

Analytics 구현 안내서의 [방문자 마이그레이션](https://docs.adobe.com/help/en/analytics/implementation/javascript-implementation/visitor-migration.html)을 참조하십시오.

JavaScript 파일을 업로드한 후에는 모든 것이 자사 쿠키 데이터 수집에 맞게 구성됩니다. 데이터 수집이 정상적으로 진행될 수 있도록 다음 몇 시간 동안 Analytics 보고를 모니터링하는 것이 좋습니다. 그렇지 않으면 위의 모든 단계가 완료되었음을 확인하고 조직에서 지원하는 사용자 중 한 명이 고객 지원 센터에 문의하도록 하십시오.
