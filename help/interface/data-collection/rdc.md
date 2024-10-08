---
title: 지역 데이터 수집
description: Experience Cloud의 지역 데이터 수집에 대해 알아봅니다.
exl-id: 295e9736-2a58-48a8-9968-5dfa33b70d95
source-git-commit: 2a80851c0a7d4ef7dbcc2565177b239f3e063164
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---

# 지역 데이터 수집

Adobe Experience Cloud은 RDC(지역 데이터 수집)를 사용하므로 방문자와 Adobe 간의 상호 작용이 가능한 한 방문자에게 가까운 위치에서 발생합니다. 에지 사이트에서 로컬로 수집된 데이터는 처리를 위해 핵심 사이트로 안전하게 전달됩니다. 처리된 데이터는 Adobe Experience Cloud 제품 및 서비스에 사용할 수 있습니다.

지역 데이터 수집 워크플로우는 다음과 같은 몇 가지 이점을 제공합니다.

* **성능**: RDC를 사용하면 방문자가 가장 가까운 에지 사이트에 연결됩니다. 이 최적화는 가장 빠른 응답 시간을 제공하여 더 정확한 추적과 더 빠른 로드 시간을 제공합니다.
* **중복성**: 에지 사이트와 핵심 사이트 간 통신이 중단되면 Adobe 인프라에서 데이터를 로컬로 저장한 다음 통신이 복원되면 핵심 사이트로 전달합니다. Adobe은 특정 위치가 중단되는 경우 트래픽을 다른 에지 사이트로 라우팅할 수도 있습니다.

현재 RDC에는 다음 위치(변경될 수 있음)가 포함되어 있습니다.

## 자사 데이터 수집

| RDC 유형 | 데이터 수집 센터 |
| --- | --- |
| 글로벌(기본값) | 오리건, 버지니아, 아일랜드, 파리, 뭄바이, 싱가포르, 도쿄, 시드니 |
| 글로벌 + 중국* | 베이징*, 오레곤, 버지니아, 아일랜드, 파리, 뭄바이, 싱가포르, 도쿄, 시드니 |
| 아메리카만 | 오리건, 버지니아 |
| 유럽만 해당 | 아일랜드, 파리 |
| 아시아 태평양만 | 뭄바이, 싱가포르, 도쿄, 시드니 |
| 중국만 해당* | 베이징 |

{style="table-layout:auto"}

_*중국 RDC에는 중국 성능 최적화 추가 기능 패키지가 필요하며 AppMeasurement 데이터 수집을 사용하는 Adobe Analytics에만 적용됩니다. 다른 Experience Cloud 서비스와 Web SDK 데이터 수집은 지원되지 않습니다. 중국 성능 최적화 추가 기능 패키지에 대한 자세한 내용은 Adobe 계정 팀에 문의하십시오._

## 타사 데이터 수집

타사 데이터 수집에는 웹 사이트 도메인과 일치하지 않는 쿠키 도메인이 포함됩니다. `adobedc.net`, `omtrdc.net` 및 `2o7.net`을(를) 예로 들 수 있습니다.

| RDC 유형 | 데이터 수집 센터 |
| --- | --- |
| 기본 | 오리건, 버지니아, 아일랜드, 파리, 뭄바이, 싱가포르, 도쿄, 시드니 |
| 기본값 + 중국* | 베이징*, 오레곤, 버지니아, 아일랜드, 파리, 뭄바이, 싱가포르, 도쿄, 시드니 |

{style="table-layout:auto"}
