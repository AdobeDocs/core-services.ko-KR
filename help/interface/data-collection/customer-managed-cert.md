---
title: 고객 관리 인증서
description: 자사 데이터 수집을 위해 고객 관리 인증서를 사용하는 시점과 이를 갱신하는 조직의 책임에 대해 알아봅니다.
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
    internal-label: CX Enterprise
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
  - id: d3cdead0-685a-4489-9250-4bb709942f66
    internal-label: Data collection
source-git-commit: 18fd590d6f0fd1800e3d5c62851453aa91d9db5f
workflow-type: tm+mt
source-wordcount: '694'
ht-degree: 1%
---
# 고객 관리 인증서

고객 관리 인증서를 사용하면 조직에서 자사 데이터 수집 호스트 이름에 대한 인증서를 가져와 Adobe에 제공합니다. Adobe은 해당 데이터 수집 서버에 인증서를 호스팅합니다. 조직은 현재 인증서가 만료되기 전에 인증서를 갱신하고 각각의 갱신된 인증서를 Adobe에 제공할 책임이 있습니다.

>[!TIP]
>
>Adobe은 대부분의 자사 구현에 대해 [Adobe 관리 인증서 프로그램](adobe-managed-cert.md)을 권장합니다. 보다 안전하며 인증서를 자동으로 갱신합니다. 조직에서 요구하는 경우에만 고객 관리 인증서를 사용하십시오.

## 고객 관리 인증서를 사용해야 하는 경우

* **자사 원본이 있는 CDN을 통해 데이터 수집을 라우팅합니다**: [Adobe 관리 인증서 프로그램](adobe-managed-cert.md)은(는) CDN 구현을 지원하지 않습니다. [자사 원본으로 CDN 구성](cdn.md#first-party-origin)을 참조하십시오.
* **보안 정책에서 인증서를 직접 제어해야 합니다**: 예를 들어 조직에서 Adobe 고객 지원 센터를 통해 취소를 요청하는 대신 자체 인증 기관을 통해 인증서를 취소할 수 있어야 합니다.
* **조직에 특정 인증 기관 또는 인증서 유형이 필요합니다**: Adobe 관리 인증서 프로그램은 DigiCert에서 발급한 인증서를 사용합니다.

## 인증서 메서드 비교

| | Adobe 관리 인증서 | 고객 관리 인증서 |
| --- | --- | --- |
| **인증서를 받는 사람** | Adobe, DigiCert 통과 | 원하는 상업 인증 기관을 통해 조직 |
| **갱신** | Adobe이 인증서를 자동으로 갱신합니다. | 조직에서 인증서를 갱신하여 각 만료 전에 Adobe에 제공합니다 |
| **인증서 유형** | Adobe은 RSA 및 ECC 인증서를 모두 제공합니다 | RSA 필요, ECC 사용 권장 |
| **CDN으로 지원** | 아니오 | 예, 자사 원본으로 |

## 고객 관리 인증서 설정

1. 고객 관리 인증서를 사용하여 자사 데이터 수집을 요청하려면 Adobe 고객 지원 센터에 문의하십시오. `data.example.com`과(와) 같은 자사 호스트 이름을 포함합니다. 조직에 데이터 상주 또는 준수 요구 사항이 있는 경우 요청에 원하는 [RDC 유형](rdc.md)을(를) 지정하십시오.
1. Adobe 고객 지원 센터는 호스트 이름에 CSR(인증서 서명 요청)을 제공합니다. Adobe은 개인 키를 생성하고 유지하므로 조직에서 개인 키를 처리하지 않습니다. Adobe은 RSA 인증서가 필요하며 ECC 인증서를 권장합니다. 각 인증서 유형에는 자체 CSR이 필요하므로 ECC 인증서를 원하는 경우 Adobe 고객 지원 센터에 ECC CSR을 요청하십시오.
1. 각 CSR을 원하는 상거래 인증 기관에 제출하여 서명된 인증서를 받습니다. 무료 인증서 서비스는 지원되지 않습니다. 고객 지원 센터의 지시에 따라 발급된 인증서를 Adobe에 제공합니다.
1. Adobe이 인증서를 설치하면 호스트 이름에 대한 트래픽을 Adobe으로 전달합니다.
   * **CDN 없이**: Adobe 고객 지원 센터에서 지시한 대로 조직의 DNS 레코드를 업데이트합니다.
   * **CDN으로**: CDN 원본을 자사 호스트 이름으로 설정합니다. [자사 원본으로 CDN 구성](cdn.md#first-party-origin)을 참조하십시오.
1. 구현이 이미 이 호스트 이름으로 데이터를 보내지 않는 경우 [구현을 업데이트](collection-domain.md#update-implementation)하십시오.

## 인증서 갱신 {#renewals}

조직은 현재 인증서가 만료되기 전에 인증서를 갱신하고 갱신된 인증서를 Adobe 고객 지원 센터에 제공합니다.

Adobe 서버의 인증서가 만료되면 브라우저 및 CDN이 호스트 이름에 대한 연결을 거부하고 이러한 요청의 데이터가 손실됩니다. CDN은 사용자에게 알리지 않고 이 데이터를 삭제할 수 있습니다.

최대 인증서 수명은 감소하고 있으며, 이로 인해 갱신이 더 자주 발생합니다. 자세한 내용은 CA/Browser Forum 서버 인증서 기본 요구 사항의 [6.3.2 인증서 작동 기간 및 키 쌍 사용 기간](https://cabforum.org/working-groups/server/baseline-requirements/requirements/#632-certificate-operational-periods-and-key-pair-usage-periods)을 참조하십시오. 데이터 수집의 간격을 방지하려면 다음 작업을 수행하십시오.

* Adobe에 제공하는 각 인증서의 만료 날짜를 추적합니다.
* 갱신을 위한 소유자를 지정하고 사원 변경을 통해 계속되도록 갱신 프로세스를 문서화합니다.

Adobe은 현재 셀프서비스 인증서 갱신 프로세스를 탐색하고 있습니다.

## 고객 관리 인증서 사용 중지

* **Adobe 관리 인증서 프로그램으로 이동하려면**: Adobe 고객 지원 센터에 문의하십시오. Adobe 관리 인증서 프로그램을 사용하려면 호스트 이름이 CDN이 아닌 Adobe을 직접 가리켜야 합니다.
* **자사 호스트 이름 사용을 중지하려면**: 호스트 이름을 사용하는 모든 구현을 업데이트한 다음 Adobe 고객 지원 센터에 문의하여 Adobe 서버에서 인증서를 제거하십시오.
* **타사 원본이 있는 CDN으로 이동하려면**: [기존 자사 구현을 CDN으로 이동](cdn.md#migrate)을 참조하십시오.
