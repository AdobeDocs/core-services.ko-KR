---
title: 데이터 수집 도메인 선택
description: Adobe으로 데이터를 전송하는 데 사용할 수 있는 도메인과 조직의 테넌트 ID를 찾는 방법에 대해 알아봅니다.
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
  - id: d3cdead0-685a-4489-9250-4bb709942f66
    internal-label: Data collection
source-git-commit: e1185eeafc809b036b10955880536db7a576ca0b
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 3%
---
# 데이터 수집 도메인 선택

데이터 수집 도메인은 구현이 데이터를 보내는 호스트 이름입니다. Adobe 데이터 수집을 사용하는 모든 Adobe CX Enterprise 제품(예: Adobe Analytics, Customer Journey Analytics, Adobe Experience Platform, Adobe Target 및 Adobe Journey Optimizer)은 이 도메인을 사용합니다.

## 데이터 수집 도메인 옵션

| 옵션 | 구현 도메인 | 지역 잠금 [RDC](rdc.md) | 인증서 유지 관리 |
| --- | --- | --- | --- |
| [타사 도메인](#third-party) | `example.data.adobedc.net` | 지원되지 않음 | 없음 |
| [Adobe 관리 인증서](adobe-managed-cert.md)가 있는 자사 도메인 | `data.example.com` | 지원됨 | 없음(Adobe에서 자동으로 인증서 갱신) |
| [고객 관리 인증서](customer-managed-cert.md)가 있는 자사 도메인 | `data.example.com` | 지원됨 | 조직에서 인증서를 갱신하여 Adobe에 제공합니다. |
| 서드파티 원본이 있는 [CDN(콘텐츠 전송 네트워크)](cdn.md#third-party-origin) | `data.example.com` | 지원되지 않음 | 없음 |
| 자사 원본이 있는 [CDN](cdn.md#first-party-origin) | `data.example.com` | 지원됨 | 조직에서 인증서를 갱신하여 Adobe에 제공합니다. |

## 타사 데이터 수집 도메인 {#third-party}

자사 도메인을 사용하지 않는 경우 데이터를 `data.adobedc.net`의 하위 도메인으로 보냅니다. Adobe에서는 조직의 [테넌트 ID](#tenant-id)을(를) 하위 도메인으로 사용하는 것이 좋습니다. 예: `example.data.adobedc.net`. 이 도메인은 [CDN을 통해 데이터 수집을 라우팅](cdn.md)할 때도 권장되는 원본입니다.

* 타사 도메인은 항상 기본 [RDC 유형](rdc.md#third-party-data-collection)을(를) 사용합니다.
* `example.data.adobedc.net`보다 더 아래의 하위 도메인은 사용하지 마십시오. 예를 들어 `custom.example.data.adobedc.net`은(는) 올바른 데이터 수집 도메인이 아닙니다.
* 이전 구현에서는 `sc.omtrdc.net` 또는 `2o7.net`과(와) 같은 도메인을 사용할 수 있습니다. 이러한 도메인은 여전히 유효하지만 가능한 경우 `data.adobedc.net`을(를) 사용하는 것이 좋습니다.

### 테넌트 ID 찾기 {#tenant-id}

1. Adobe ID 자격 증명을 사용하여 [Adobe CX Enterprise](https://experience.adobe.com)에 로그인합니다.
1. CX Enterprise 인터페이스의 모든 곳에서 `[Cmd]` + `[I]`(macOS) 또는 `[Ctrl]` + `[I]`(Windows)을 누릅니다.
1. **[!UICONTROL 사용자 데이터 디버거]**&#x200B;가 나타납니다. **[!UICONTROL 할당된 조직]** 탭을 선택합니다.
1. 원하는 IMS 조직을 확장합니다.
1. **[!UICONTROL 테넌트]** 필드를 찾습니다. 이 값은 임차인 ID입니다.

테넌트 ID가 `@AdobeOrg`에서 끝나는 IMS 조직 ID와 다릅니다. 각 IMS 조직에는 하나의 테넌트 ID가 있습니다. 회사에서 여러 IMS 조직을 사용하는 경우 각 조직에는 자체 테넌트 ID가 있습니다.

## 구현 업데이트 {#update-implementation}

데이터 수집 도메인을 변경하면 Adobe에 데이터를 전송하는 모든 구현을 업데이트합니다.

* **웹 SDK 태그 확장**: 확장을 구성할 때 [[!UICONTROL Edge 도메인]](https://experienceleague.adobe.com/ko/docs/experience-platform/tags/extensions/client/web-sdk/configure/general) 필드를 업데이트합니다.
* **웹 SDK(alloy)**: `configure` 명령 내에서 [`edgeDomain`](https://experienceleague.adobe.com/ko/docs/experience-platform/collection/js/commands/configure/edgedomain) 속성을 업데이트합니다.
* **Adobe Analytics 확장**: 확장을 구성할 때 [[!UICONTROL SSL 추적 서버]](https://experienceleague.adobe.com/ko/docs/experience-platform/tags/extensions/client/analytics/overview) 필드를 업데이트합니다. [방문자 ID 서비스 태그 확장](https://experienceleague.adobe.com/ko/docs/experience-platform/tags/extensions/client/id-service/overview)도 설치되어 있는지 확인하십시오. 자세한 내용은 [Analytics 태그 확장을 사용한 방문자 식별](https://experienceleague.adobe.com/ko/docs/analytics/implementation/id/analytics-extension)을 참조하십시오.
* **AppMeasurement**: [`trackingServerSecure`](https://experienceleague.adobe.com/ko/docs/analytics/implementation/vars/config-vars/trackingserversecure) 구성 변수를 업데이트합니다. `VisitorAPI.js`을(를) 사용하여 [방문자 ID 서비스](https://experienceleague.adobe.com/ko/docs/id-service/using/home)도 구현했는지 확인하십시오. 자세한 내용은 [AppMeasurement을 사용한 방문자 식별](https://experienceleague.adobe.com/ko/docs/analytics/implementation/id/appmeasurement)을 참조하십시오.
* **다른 구현**: 모바일 앱 또는 서버측 구현과 같이 Adobe에 데이터를 보내는 다른 구현에서 데이터 수집 도메인을 업데이트합니다.

구현에서 방문자 ID 서비스 또는 웹 SDK을 사용하지 않는 경우 데이터 수집 도메인을 변경하면 방문자 쿠키의 도메인이 변경되고 재방문자는 새 방문자로 카운트될 수 있습니다.

사이트에서 여러 구현 방법을 사용하지만 이러한 방법을 동시에 모두 업데이트할 수 없는 경우에는 유예 기간 구성을 고려해 보십시오. 방문자가 사이트에서 새 방문자로 계산되지 않도록 하는 방법에 대한 추가 단계는 [방문자 ID 서비스 마이그레이션 고려 사항](https://experienceleague.adobe.com/ko/docs/analytics/implementation/id/migration)을 참조하십시오.
