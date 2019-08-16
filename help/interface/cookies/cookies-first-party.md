---
description: Analytics는 쿠키를 사용하여 이미지 요청과 브라우저 세션 간에 지속되지 않는 변수 및 구성 요소에 대한 정보를 제공합니다.
keywords: cookies;privacy
seo-description: Analytics는 쿠키를 사용하여 이미지 요청과 브라우저 세션 간에 지속되지 않는 변수 및 구성 요소에 대한 정보를 제공합니다.
seo-title: 퍼스트 파티 쿠키
solution: Experience Cloud, 분석
title: 퍼스트 파티 쿠키
index: y
snippet: y
translation-type: tm+mt
source-git-commit: 2bdc4b7287ccacfc4d968278b2c3ffdaeddfc105

---


# 퍼스트 파티 쿠키 정보

Analytics는 쿠키를 사용하여 이미지 요청과 브라우저 세션 간에 지속되지 않는 변수 및 구성 요소에 대한 정보를 제공합니다. 이러한 무해 쿠키는 Adobe에서 호스트하는 도메인에서 생성되는 것으로, 타사 쿠키로 알려져 있습니다.

대부분의 브라우저와 안티스파이웨어 애플리케이션은 Analytics 데이터 수집에서 사용되는 쿠키를 포함하여 타사 쿠키를 거부하고 삭제하도록 설계되었습니다. 브라우저 및 프로그램에 의해 적용되는 추적 제한을 우회하기 위해 퍼스트 파티 쿠키를 구현할 수 있습니다.

퍼스트 파티 쿠키를 구현하는 데 두 가지 옵션을 사용할 수 있습니다.

* 경험 플랫폼 ID 서비스. ID 서비스는 JavaScript를 사용하여 퍼스트 파티 컨텍스트에서 쿠키를 설정할 수 있습니다.
* 회사 DNS 서버의 DNS 항목입니다.
* 사이트에 `https:` 프로토콜을 사용하여 보안 페이지가 있고 Experience Platform ID 서비스를 사용하지 않는 경우, 퍼스트 파티 쿠키를 구현하기 위해 Adobe에서 SSL 인증서를 얻을 수 있습니다.

SSL 인증서 발급 프로세스는 종종 혼란스럽고 시간이 걸릴 수 있습니다. 그 결과 Adobe는 업계 선도적인 인증 기관 (CA) 인 digicert 와의 파트너십을 구축했으며 이러한 인증서의 구매 및 관리를 자동화하는 통합 프로세스를 개발했습니다.

귀하의 허가가 있으면 Adobe는 CA와 협력하여 새로운 SHA -2 SSL 인증서를 발행, 배포 및 관리할 것입니다. Adobe는 이 인증서를 계속 관리하며 예상치 못한 만료, 해지 또는 보안 문제가 조직의 보안 수집을 위협하는 것은 아닙니다.

## Adobe 관리 인증서 프로그램

Adobe 관리 인증서 프로그램은 퍼스트 파티 쿠키를 위한 새 퍼스트 파티 SSL 인증서를 구현하는 권장 프로세스입니다.

Adobe 관리 인증서 프로그램에서는 추가 비용 없이 자사 쿠키를 위한 새 자사 SSL 인증서를 구현할 수 있습니다. 현재 자체 고객 관리 SSL 인증서를 보유하고 있는 경우 Adobe 관리 인증서 프로그램으로 마이그레이션하는 방법에 대해 Adobe 고객 지원 센터에 문의하십시오.

### 구현

퍼스트 파티 쿠키를 위한 새 퍼스트 파티 SSL 인증서를 구현하는 방법은 다음과 같습니다.

1. ![요청 양식을](assets/FPC_Request_Form.xlsx) 작성하고 Adobe Managed Program에서 퍼스트 파티 쿠키를 설정하도록 요청하는 고객 지원 센터를 통해 티켓을 엽니다. 문서 내에 각 필드가 예와 함께 설명되어 있습니다.

1. CNAME 레코드를 만듭니다 (아래 지침 참조). 티켓을 받으면 FPSSL 전문가가 CNAME 레코드 쌍을 제공해야 합니다. Adobe가 귀하를 대신하여 인증서를 구입할 수 있으려면 먼저 회사의 DNS 서버에서 이러한 기록을 구성해야 합니다. CNAME는 다음과 유사합니다.

* **보안 -** 예를 들어 호스트 이름은 `smetrics.example.com` 다음을 가리킵니다. `example.com.ssl.d1.omtrdc.net`.
* **비보안** - 예를 들어 호스트 이름은 `metrics.example.com` 다음을 가리킵니다. `example.com.d1.omtrdc.net`.

1. 이러한 CNAME 이 준비되면 Adobe는 digicert와 협력하여 Adobe 프로덕션 서버에 인증서를 구매 및 설치합니다. 기존 구현이 있는 경우 기존 방문자를 유지하기 위해 방문자 마이그레이션을 고려해야 합니다. 인증서가 Adobe의 프로덕션 환경에 라이브로 푸시된 후 추적 서버 변수를 새로운 호스트 이름으로 업데이트할 수 있습니다. 즉, 사이트가 안전하지 않은 경우 (HTTPS) 를 `s.trackingServer`업데이트합니다. 사이트가 보안 (https) 인 경우 `s.trackingServer` 및 `s.trackingServerSecure` 변수를 모두 업데이트합니다.

1. 호스트 이름 Ping (아래 참조).

1. 업데이트 구현 코드를 참조하십시오 (아래 참조).

### 유지 관리 및 갱신

SSL 인증서는 매년 만료됩니다. 즉, Adobe는 매년 각 구현에 대한 새 인증서를 구입해야 합니다. 조직 내의 지원되는 모든 사용자는 구현이 만료될 때마다 이메일 알림을 받게 됩니다. Adobe가 호스트 이름을 갱신하기 위해, 지원되는 한 사용자가 Adobe에서 이메일에 회신하고 데이터 수집을 위해 만료되는 호스트 이름을 계속 사용할 계획임을 나타내야 합니다. 이때 Adobe는 자동으로 새 인증서를 구입하여 설치합니다.

### FAQ

| 질문 | 답변 |
|---|---|
| **이 프로세스는 안전합니까?** | 예. Adobe Managed Program는 Adobe의 기존 방식보다 더 안전하며 Adobe와 인증 기관의 외부에서 인증서나 개인 키가 변경되지 않습니다. |
| **Adobe는 어떻게 도메인의 인증서를 구입할 수 있습니까?** | Adobe 소유 호스트 이름에 지정된 호스트 이름 (예: smetrics.example.com를 지정한 경우에만 인증서를 구입할 수 있습니다. 이것은 본질적으로 이 호스트 이름을 Adobe에 위임하며 Adobe가 사용자를 대신하여 인증서를 구매할 수 있도록 합니다. |
| **인증서가 폐지되도록 요청할 수 있습니까?** | 예, 도메인의 소유자로서, 인증서가 해지되었음을 요청할 수 있습니다. 이렇게 하려면 고객 지원 센터에 티켓을 열어야 합니다. |
| **이 인증서는 SHA -2 암호화를 사용합니까?** | 예. Adobe는 digicert와 협력하여 SHA -2 인증서를 발행합니다. |
| **이 경우 추가 비용이 발생합니까?** | 아니요. Adobe는 현재 모든 분석 고객에게 추가 비용 없이 이 서비스를 제공하고 있습니다. |

## CNAME 레코드 작성

조직의 네트워크 작업 팀은 새 CNAME 레코드를 만들어 DNS 서버를 구성해야 합니다. 각 호스트 이름은 Adobe의 데이터 수집 서버로 데이터를 전달합니다.

FPC 전문가는 구성된 호스트 이름과 가리키는 CNAME를 제공합니다. 예:

* **SSL 호스트**&#x200B;이름:`smetrics.mysite.com`
* **SSL CNAME**:`mysite.com.ssl.d1.sc.omtrdc.net`
* **SSL 이 아닌 호스트 이름**:`metrics.mysite.com`
* **비 SSL CNAME**:`mysite.com.d1.sc.omtrdc.net`

구현 코드가 변경되지 않는 한, 이 단계는 데이터 수집에 영향을 주지 않으며 구현 코드를 업데이트한 후 언제든지 수행할 수 있습니다.

>[!NOTE:] Experience Cloud 방문자 ID 서비스는 퍼스트 파티 쿠키를 활성화하기 위해 CNAME를 구성하는 대안을 제공합니다.

## 호스트 이름 Ping

호스트 이름을 ping 하여 올바른 전달을 보장합니다. 모든 호스트 이름은 데이터 손실을 방지하기 위해 ping에 응답해야 합니다.

CNAME 레코드가 제대로 구성되어 있고 Adobe에서 인증서 설치를 확인한 후 명령 프롬프트를 열고 호스트 이름을 ping 합니다. Using `mysite.com` as an example: `ping metrics.mysite.com`

모든 항목이 성공적으로 설정되었으면 다음과 유사한 내용이 반환됩니다.

```Pinging mysite.com.112.2o7.net [66.235.132.232] with 32 bytes of data:
Reply from 66.235.132.232: bytes=32 time=19ms TTL=246
Reply from 66.235.132.232: bytes=32 time=19ms TTL=246
Reply from 66.235.132.232: bytes=32 time=19ms TTL=246
Reply from 66.235.132.232: bytes=32 time=19ms TTL=246

Ping statistics for 66.235.132.232: Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds: Minimum = 19ms, Maximum = 19ms, Average = 19ms
```

CNAME 레코드가 올바르게 설정되지 않았거나 활성화되지 않으면 다음과 같이 반환됩니다.

`Ping request could not find the host. Please check the name and try again.`

>[!NOTE:] 사용 `https:// protocol`중인 경우 ping는 FPC 전문가가 지정한 업로드 날짜 후에만 응답합니다. 추가로 구현을 업데이트하기 전에 보안 호스트 이름 및 비보안 호스트 이름을 ping 하여 둘 다 올바르게 작동하는지 확인해야 합니다.

## 업데이트 구현 코드

자사 쿠키를 활용하도록 사이트에서 코드를 편집하려면 먼저 다음 전제 조건을 완료하십시오.

* Adobe 관리 인증서 프로그램의 구현 단계에 설명된 대로 SSL 인증서를 요청합니다.
* CNAME 레코드를 만듭니다.
* 호스트 이름 Ping.

호스트 이름이 응답하고 Adobe 데이터 수집 서버로 전달하는 것을 확인한 후에는 구현을 변경하여 자신의 데이터 수집 호스트 이름을 가리키도록 할 수 있습니다.

1. Open your core JavaScript file (`s_code.js/AppMeasurement.js`).
1.  코드 버전을 업데이트하려면 전체`s_code.js/AppMeasurement.js`   파일을 최신 버전으로 바꾸고 플러그인 또는 사용자 지정으로 바꿉니다. **또는**&#x200B;자사 쿠키와 관련된 코드만 업데이트하려면 s. trackingserver 및 s. trackingserversecure (SSL 사용 시) 를 찾아 새로운 데이터 수집 호스트 이름을 지정합니다. Using mysite.com as an example:`s.trackingServer = "metrics.mysite.com"` `s.trackingServerSecure = "smetrics.mysite.com"`

1. 업데이트된 코어 JavaScript 파일을 사이트에 업로드합니다.
1. 장기간 구현에서 퍼스트 파티 쿠키로 이동하거나 다른 자사 컬렉션 호스트 이름으로 변경하려는 경우 이전 도메인에서 새 도메인으로 방문자를 마이그레이션하는 것이 좋습니다.

Analytics 구현 안내서에서 [방문자 마이그레이션을](https://docs.adobe.com/help/en/analytics/implementation/javascript-implementation/visitor-migration.html) 참조하십시오.

JavaScript 파일을 업로드한 후 모든 것이 퍼스트 파티 쿠키 데이터 수집에 대해 구성됩니다. 데이터 수집이 정상적으로 진행될 수 있도록 다음 몇 시간 동안 분석 보고를 모니터링하는 것이 좋습니다. 그렇지 않은 경우, 위의 모든 단계가 완료되었는지 확인하고 조직의 지원 사용자 중 한 명이 고객 지원 센터에 문의하도록 하십시오.
