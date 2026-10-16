---
description: Adobe CX Enterprise 자사 쿠키에 사용할 보안 인증서를 설정하는 방법을 알아봅니다.
solution: Experience Cloud,Analytics
title: Adobe 관리 인증서 프로그램
index: true
snippet: 'y'
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: e15abde5-8027-4aed-a0c1-8a6fc248db5e
autotag-review: '2026-09-09T20:12:24.943Z'
TQID: 'https://experienceleague.adobe.com/8CSBLQaw3KOByyxxCYr1By4gyAQsDIhiofOdAzn38dg'
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
    internal-label: CX Enterprise
  - id: e55547f1-a1ff-40c6-8978-026e40ab7fa4
    internal-label: Analytics
feature_v2:
  - id: b3f03848-ae12-48b2-8aab-cad18567eb32
    internal-label: Metrics
  - id: e9dbdbc5-3e52-40f0-a7bc-e18542967b7a
    internal-label: Implementations
  - id: fd307ce7-56f5-4ee3-af68-a7833ff6e85e
    internal-label: API
  - id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
    internal-label: Administration
subfeature_v2:
  - id: b75843fa-0a67-4a44-a6b1-cc627b0481dc
    internal-label: Support
  - id: c8add8f2-4250-4fd9-9cde-9707036c567d
    internal-label: Methods
  - id: d2311670-43bd-4c2e-bc98-1da2aaba9cef
    internal-label: Appmeasurement implementation
  - id: e992d880-33bc-4949-a648-aa7d410276cd
    internal-label: Validation
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
    internal-label: Measurement
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
  - id: d3cdead0-685a-4489-9250-4bb709942f66
    internal-label: Data collection
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 18fd590d6f0fd1800e3d5c62851453aa91d9db5f
workflow-type: tm+mt
source-wordcount: '1055'
ht-degree: 2%
---
# Adobe 관리 인증서 프로그램

Adobe 관리 인증서 프로그램은 CNAME 구현에 필요한 자사 인증서를 설정하는 권장 프로세스입니다. 프로그램이 구성되면 완전히 자동화됩니다. 만료된 인증서로 인해 데이터 수집에 영향을 주지 않도록 적시에 인증서를 갱신합니다. 프로그램은 처음 100개의 CNAME에 대해 무료입니다.

Adobe 관리 인증서 프로그램은 CDN(콘텐츠 전달 네트워크)을 통한 데이터 수집 라우팅을 지원하지 않습니다. CDN을 사용하는 경우 [CDN을 통해 데이터 수집 라우팅](cdn.md)을 참조하십시오. 자체 인증서를 관리해야 하는 조직은 [고객 관리 인증서](customer-managed-cert.md)를 대신 사용할 수 있습니다. 현재 자체 인증서를 관리하고 Adobe 관리 인증서 프로그램으로 이동하려는 경우 Adobe 고객 지원 센터에 문의하십시오.

## 구현

자사 데이터 수집을 위한 새 인증서를 구현하려면 다음 단계를 수행합니다.

1. [자사 도메인 요청 양식](cookies/assets/First_Party_Domain_Request_Form.xlsx)을 다운로드하여 작성
1. Adobe 고객 지원 센터에서 Adobe 관리 인증서 프로그램에 대한 자사 데이터 수집을 설정하도록 요청하는 티켓을 엽니다. 조직에 데이터 상주 또는 준수 요구 사항이 있는 경우 요청에 원하는 [RDC 유형](rdc.md)을(를) 지정하십시오.
1. 티켓을 받으면 Adobe 담당자가 CNAME 레코드를 제공합니다. Adobe에서 귀하를 대신하여 인증서를 구입할 수 있으려면 먼저 회사의 DNS 서버에서 이 레코드를 구성해야 합니다. 예를 들어 호스트 이름 `data.example.com`은(는) `hiodsibxvip01.data.adobedc.net`을(를) 가리킵니다. 조직에서 DNS CAA(인증 기관 인증) 레코드를 사용하는 경우 CAA 레코드에서 DigiCert가 인증서를 발급할 수 있도록 허용하는지 확인하십시오. [유지 관리 및 갱신](#renewals)을 참조하세요.
1. CNAME 레코드가 조직 서버에 있으면 Adobe은 DigiCert와 협력하여 Adobe 데이터 수집 서버에서 인증서를 구입하고 설치합니다.
1. 자사 용도로 Adobe CNAME에서 호스팅할 때 `robots.txt` 파일을 업데이트해야 하는 경우 고객 지원 센터에 문의하십시오. 이러한 요청은 Google이 하위 도메인에서 크롤링을 차단하도록 `robots.txt` 파일을 업데이트하려는 경우에 적용됩니다.

## 호스트 이름 전달의 유효성 검사

Adobe이 인증서를 설치했으면 다음 방법 중 하나를 사용하여 인증서가 작동하는지 확인할 수 있습니다.

+++**브라우저 유효성 검사**

모든 브라우저를 사용하여 인증서가 올바르게 설치되었는지 확인할 수 있습니다. 주소 표시줄의 경로로 `_check`을(를) 사용하여 CNAME을 입력하십시오. 예:

`data.example.com/_check`

모든 기능이 작동하면 브라우저에 `SUCCESS`이(가) 표시됩니다. 인증서가 올바르게 설치되지 않으면 보안 경고가 표시됩니다.

+++

+++**명령줄(`curl`)**

대부분의 최신 운영 체제에는 이미 [`curl`](https://curl.se)이(가) 설치되어 있습니다.

명령줄에 다음을 입력합니다.

```sh
curl data.example.com/_check
```

모든 것이 올바르게 작동하면 콘솔은 `SUCCESS`을(를) 반환합니다.

>[!TIP]
>
>`-k` 플래그를 사용하여 문제 해결에 도움이 되는 보안 경고를 비활성화할 수 있습니다.

+++

+++**명령줄(`nslookup`)**

명령줄에 다음을 입력합니다.

```sh
nslookup data.example.com
```

모든 것이 올바르게 작동하면 Adobe의 데이터 수집 서버가 반환됩니다.

```text
Server: hiodsibxvip01.corp.adobe.com
Address: 10.50.112.247

Name: example.com.ssl.d1.sc.omtrdc.net
Addresses: 63.140.37.126
    63.140.37.206
    63.140.36.51
    63.140.36.145
Aliases: data.example.com
```

+++

## 구현 코드 업데이트

새 CNAME 호스트 이름을 사용하려면 인증서가 올바르게 작동하는지 확인한 후 Adobe 구현을 업데이트합니다. [구현 업데이트](collection-domain.md#update-implementation)를 참조하세요.

## 유지 관리 및 갱신 {#renewals}

Adobe이 인증서를 자동으로 갱신합니다. 인증서가 만료되기 30일 전에 Adobe은 CNAME이 아직 유효하고 사용 중인지 확인한 다음 사용자를 대신하여 인증서를 갱신합니다. 갱신을 계속 사용하려면 다음 DNS 변경 사항을 피하십시오.

* **CNAME 레코드 제거 또는 다시 지정**: CNAME 레코드가 제거되었거나 더 이상 Adobe 보안 호스트 이름을 가리키지 않으면 Adobe에서 인증서를 갱신할 수 없습니다. 이 조건에는 CNAME 레코드를 CDN(콘텐츠 전송 네트워크)으로 지정하는 것이 포함됩니다. CDN을 사용하려면 DNS 레코드를 변경하기 전에 [기존 자사 구현을 CDN으로 이동](cdn.md#migrate)을 참조하십시오.
* **DigiCert를 인증하지 않는 CAA 레코드를 추가**: 인증 기관은 호스트 이름 및 상위 도메인에서 CAA(인증 기관 인증) 레코드를 확인합니다. CAA 레코드를 사용하는 경우 `digicert.com`을(를) 승인된 발급자로 포함하십시오. 예: `example.com. IN CAA 0 issue "digicert.com"`.
* **DigiCert 발급을 특정 계정으로 제한**: DigiCert의 도메인 잠금 기능은 `example.com. IN CAA 0 issue "digicert.com; account=<token>"`과(와) 같은 CAA 레코드에 `account=` 매개 변수를 추가합니다. 이 매개 변수는 `digicert.com`이(가) 승인된 경우에도 조직의 DigiCert 계정에 대한 발급을 제한하므로 Adobe에서 인증서를 얻을 수 없습니다. 조직에 DigiCert 도메인 잠금이 필요한 경우 대신 [고객 관리 인증서](customer-managed-cert.md)를 사용하십시오. 도메인 등록자에 설정된 도메인 잠금(전송 잠금)은 관련이 없으며 Adobe 관리 인증서에 영향을 주지 않습니다.

>[!IMPORTANT]
>
>CNAME 레코드가 더 이상 Adobe 보안 호스트 이름을 가리키지 않으면 Adobe 시스템의 항목이 더 이상 통신하지 않고 제거되도록 표시됩니다.

## 자주 묻는 질문

+++이 프로세스는 안전합니까?

예. Adobe 관리 인증서 프로그램은 [고객 관리 인증서](customer-managed-cert.md)보다 안전합니다. 인증서나 개인 키가 Adobe 및 발급 인증 기관 외부로 전송되지 않습니다.

+++

+++Adobe은 어떻게 도메인의 인증서를 구입할 수 있습니까?

Adobe 소유 호스트 이름에 지정된 호스트 이름을 지정한 경우에만 인증서를 구입할 수 있습니다. 이 호스트 이름을 Adobe에 위임하고 Adobe이 사용자를 대신하여 인증서를 구매할 수 있도록 합니다.

+++

+++인증서가 해지되도록 요청할 수 있습니까?

예. 도메인의 소유는 인증서를 해지하도록 요청할 수 있습니다. 이 프로세스를 시작하려면 Adobe 고객 지원 센터에 문의하십시오.

+++

+++어떤 암호화 유형을 사용합니까?

Adobe은 DigiCert와 협력하여 SHA-2 인증서를 발행합니다.

+++

+++이 프로그램은 추가 비용이 발생합니까?

Adobe은 처음 100개의 CNAME에 대해 추가 비용 없이 모든 Adobe CX Enterprise 고객에게 이 프로그램을 제공합니다.

+++

+++Adobe은 어떤 암호 보안 수준을 제공합니까?

Adobe은 자사 데이터 수집에서의 보안에 대한 다양한 고객 요구 사항을 충족하기 위해 두 가지 암호 보안 수준을 제공합니다. 이러한 수준은 Adobe 서버와의 HTTPS 연결에 지원되는 암호화 알고리즘을 결정합니다. Adobe은 최신 보안 사례를 기반으로 지원되는 알고리즘 세트를 정기적으로 검토하고 업데이트합니다. 암호 보안 설정을 변경하려면 고객 지원 센터에 문의하십시오.

* **표준**&#x200B;에는 TLS 1.2 이상 및 128비트 이상의 암호화가 필요합니다. 안전한 암호화를 유지하면서 가장 광범위한 장치 호환성을 제공하도록 설계되었습니다.
* **높음**&#x200B;은(는) TLS 1.2 이상이 필요하며 더 약한 암호에 대한 지원을 제거합니다. 가장 강력한 암호화를 원하는 고객을 위해 설계되었습니다. 암호 보안이 **높음**(으)로 설정되어 있으면 2015년 이전에 릴리스된 클라이언트는 일반적으로 연결할 수 없습니다.

+++

+++지원되는 HTTPS 인증서 유형은 무엇입니까?

Adobe은 RSA 및 ECC 인증서를 모두 지원하며 최신 클라이언트는 두 가지 인증서 유형을 모두 지원합니다. ECC 인증서는 서버와 클라이언트 모두에서 처리 시간이 단축됩니다. Adobe 관리 인증서의 경우 Adobe에서 RSA 인증서와 ECC 인증서를 모두 제공합니다. [고객 관리 인증서](customer-managed-cert.md)의 경우 RSA가 필요하며 ECC가 권장됩니다.

+++

