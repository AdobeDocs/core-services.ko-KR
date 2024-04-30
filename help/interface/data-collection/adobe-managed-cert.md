---
description: Adobe Experience Cloud 자사 쿠키에 사용할 보안 인증서를 설정하는 방법을 알아봅니다.
solution: Experience Cloud,Analytics
title: Adobe 관리 인증서 프로그램
index: y
snippet: y
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: e15abde5-8027-4aed-a0c1-8a6fc248db5e
source-git-commit: 028b11dfbcfc0c5c9f6fd1c69350574f81f2846b
workflow-type: tm+mt
source-wordcount: '929'
ht-degree: 9%

---

# Adobe 관리 인증서 프로그램

Adobe 관리 인증서 프로그램은 CNAME 구현에 필요한 자사 인증서를 설정하는 권장 프로세스입니다. 프로그램이 구성되면 완전히 자동화됩니다. 만료된 인증서로 인해 데이터 수집에 영향을 주지 않도록 적시에 인증서를 갱신합니다. 프로그램은 처음 100개의 CNAME에 대해 무료입니다.

현재 자체 인증서를 관리하는 경우 자사 쿠키 사용을 위해 인증서를 구매, 유지 관리 및 Adobe에게 제공할 책임이 있습니다. Adobe 고객 지원 센터에 문의하여 Adobe 관리 인증서 프로그램으로의 마이그레이션에 대해 논의할 수 있습니다.

## 구현

자사 데이터 수집을 위한 새 인증서를 구현하려면 다음 단계를 따르십시오.

1. 다운로드 및 작성 [자사 도메인 요청 양식](cookies/assets/First_Party_Domain_Request_Form.xlsx)

1. Adobe 고객 지원 센터에서 Adobe 관리 인증서 프로그램에 자사 데이터 수집을 설정하도록 요청하는 티켓을 엽니다.

1. 티켓을 받으면 Adobe 담당자가 CNAME 레코드를 제공합니다. Adobe가 귀하를 대신하여 인증서를 구입할 수 있으려면 먼저 회사의 DNS 서버에서 이러한 레코드를 구성해야 합니다. 예: 호스트 이름 `data.example.com` 포인트 대상 `hiodsibxvip01.data.adobedc.net`.

1. CNAME 레코드가 조직 서버에 있으면 Adobe은 DigiCert와 협력하여 Adobe 데이터 수집 서버에 인증서를 구입하고 설치합니다.

## 호스트 이름 전달의 유효성 검사 {#validate}

Adobe이 인증서를 설치했으면 다음 방법 중 하나를 사용하여 인증서가 작동하는지 확인할 수 있습니다.

+++**브라우저 유효성 검사**

모든 브라우저를 사용하여 인증서가 올바르게 설치되었는지 확인할 수 있습니다. CNAME 입력 `_check` 주소 표시줄에 대한 경로로 사용됩니다. 예:

`data.example.com/_check`

모든 것이 작동하면 브라우저가 다음을 표시합니다. `SUCCESS`. 인증서가 올바르게 설치되지 않으면 보안 경고가 표시됩니다.

+++

+++**명령줄(`curl`)**

대부분의 최신 운영 체제는 이미 [`curl`](https://curl.se) 설치됨.

명령줄에 다음을 입력합니다.

```sh
curl data.example.com/_check
```

모든 것이 올바르게 작동하면 콘솔은 를 반환합니다. `SUCCESS`.

>[!TIP]
>
>다음을 사용할 수 있습니다. `-k` 문제 해결에 도움이 되는 보안 경고를 비활성화하는 플래그입니다.

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
Aliases: smetrics.example.com
```

+++

## 구현 코드 업데이트 {#update}

인증서가 올바르게 작동하는지 확인한 후에는 이러한 값을 사용하도록 Adobe 구현을 업데이트할 수 있습니다.

* Adobe Analytics AppMeasurement 구현의 경우 [`trackingServer`](https://experienceleague.adobe.com/en/docs/analytics/implementation/vars/config-vars/trackingserver) 구성 변수를 채우는 방법에 따라 페이지를 순서대로 표시합니다. 기존 구현이 있는 경우 [방문자 마이그레이션](https://experienceleague.adobe.com/en/docs/analytics/technotes/visitor-migration) 기존 방문자가 새 방문자로 계산되지 않도록 하는 방법에 대한 추가 단계입니다.
* Web SDK 구현의 경우 [`edgeDomain`](https://experienceleague.adobe.com/en/docs/experience-platform/web-sdk/commands/configure/edgedomain) 다음 내에 있는 속성 [`configure`](https://experienceleague.adobe.com/en/docs/experience-platform/web-sdk/commands/configure/overview) 명령입니다.

## 유지 관리 및 갱신

자사 인증서가 만료되기 30일 전에 Adobe이 CNAME이 여전히 유효하고 사용 중인지 확인합니다. 이 경우 Adobe은 사용자가 서비스를 계속 사용할 것으로 가정하고 사용자를 대신하여 인증서를 자동으로 갱신합니다.

>[!IMPORTANT]
>
>조직의 CNAME 레코드가 제거되거나 더 이상 제공된 Adobe 보안 호스트 이름으로 매핑되지 않는 경우 Adobe이 인증서를 갱신할 수 없습니다. Adobe 시스템의 항목은 더 이상의 통신 없이 제거되도록 표시됩니다.

## 자주 묻는 질문

+++이 프로세스는 안전합니까?

예. Adobe 관리 인증서 프로그램은 인증서를 Adobe에게 제공하는 조직보다 안전합니다. Adobe 및 발급 인증 기관 외부에서 인증서나 개인 키를 변경하지 않습니다.

+++

+++Adobe은 어떻게 도메인의 인증서를 구입할 수 있습니까?

Adobe 소유 호스트 이름에 지정된 호스트 이름을 지정한 경우에만 인증서를 구입할 수 있습니다. 기본적으로 이 호스트 이름을 Adobe에 위임하고 Adobe이 사용자를 대신하여 인증서를 구매할 수 있도록 합니다.

+++

+++인증서가 해지되도록 요청할 수 있습니까?

예. 도메인의 소유는 인증서를 해지하도록 요청할 수 있습니다. 이 프로세스를 시작하려면 Adobe 고객 지원 센터에 문의하십시오.

+++

+++어떤 암호화 유형을 사용합니까?

Adobe이 DigiCert와 협력하여 SHA-2 인증서를 발행합니다.

+++

+++이 프로그램에 추가 비용이 발생합니까?

아니요. Adobe은 모든 Adobe Experience Cloud 고객에게 추가 비용 없이 이 서비스를 제공합니다.

+++

+++Adobe은 어떤 암호 보안 수준을 제공합니까?

Adobe는 자사 데이터 수집에서의 보안에 대한 다양한 고객 요구 사항에 부합하는 두 가지의 암호 보안 수준을 제공합니다. 이러한 수준은 Adobe 서버와의 HTTPS 연결에 지원되는 암호화 알고리즘을 결정합니다. Adobe은 최신 보안 사례를 기반으로 지원되는 알고리즘 세트를 정기적으로 검토하고 업데이트합니다. 암호 보안 설정을 변경하려면 고객 지원 센터에 문의하십시오.

* **표준** 는 TLS 1.2 이상 및 128비트 이상의 암호화가 필요합니다. 안전한 암호화를 유지하면서 가장 광범위한 장치 호환성을 제공하도록 설계되었습니다.
* **높음** 암호 보안 수준에는 TLS 1.2 이상이 필요하며 더 약한 암호에 대한 지원을 제거합니다. 가장 강력한 암호화를 원하며 구형 장치에 대한 지원에 관심이 없는 고객을 위해 설계되었습니다.

다음 클라이언트는 암호 보안이 로 설정된 상태에서 연결할 수 없는 것으로 알려져 있습니다 **높음**:

* Windows 8.1 이하(2018년에 마지막으로 업데이트됨)
* Windows Phone 8.1 이하(2016년에 마지막으로 업데이트됨)
* OS X 10.10 이하(2017년에 마지막으로 업데이트됨)
* iOS 8.4 이하(2015년에 마지막으로 업데이트됨)

+++

+++지원되는 HTTPS 인증서 유형은 무엇입니까?

Adobe은 다양한 고객 요구 사항을 충족하기 위해 RSA 및 ECC 인증서 유형을 모두 지원합니다. RSA 인증서는 클라이언트에 대해 더 광범위하게 지원되지만 ECC 인증서는 서버 측과 클라이언트 측에서 처리 시간이 줄어듭니다. Adobe 관리 인증서의 경우 RSA와 ECC가 모두 제공됩니다. 고객 관리 인증서의 경우 RSA가 필요하며 ECC를 사용하는 것이 좋습니다. 최신 클라이언트는 RSA와 ECC를 모두 지원합니다. 다음 클라이언트는 일반적으로 RSA 인증서만 지원합니다.

* Windows Vista 이하(2012년에 마지막으로 업데이트됨)
* Windows Phone 8.0 이하(2014년에 마지막으로 업데이트됨)
* OS X 10.8 이하(2013년에 마지막으로 업데이트됨)
* iOS 5.1 이하(2012년에 마지막으로 업데이트됨)
* Android 4.3 이하(2013년에 마지막으로 업데이트됨)

+++
