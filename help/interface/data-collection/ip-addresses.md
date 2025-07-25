---
title: Experience Cloud에서 사용하는 IP 주소
description: 조직의 방화벽이 Adobe에서 생성하는 IP 주소를 차단하는 경우 이 목록을 사용하여 방화벽 설정을 업데이트합니다.
exl-id: 1fca8d3b-ae8b-4095-96ef-d165f912b4c6
source-git-commit: a18b61cb32286680cb1ab2a296df33509fd95a00
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 11%

---

# Experience Cloud에서 사용하는 IP 주소

일부 방화벽 구성은 Adobe의 데이터 수집 서버 또는 데이터 액세스를 담당하는 서버에서 생성하는 IP 주소를 차단합니다. 이 범위 목록을 사용하여 액세스를 허용하고 조직 내에서 데이터를 보내도록 조직의 방화벽 설정을 변경할 수 있습니다. 이 페이지에는 Adobe에서 사용하는 인바운드 시스템(예: 데이터 수집)과 아웃바운드 시스템(예: Adobe Analytics의 데이터 피드)이 모두 포함되어 있습니다.

>[!IMPORTANT]
>
>Adobe은 이 문서를 최신 상태로 유지하기 위해 최선을 다하고 있지만 IP 범위 목록이 동일하게 유지된다고 보장할 수 없습니다. 비즈니스의 성장 및 확장과 같은 변화가 있을 수 있으며, 인터넷 레지스트리에서 Adobe의 IP 주소 공간을 변경해야 하거나, 인터넷 서비스 공급자가 제대로 작동하지 않을 수 있습니다.

아래에 나열된 IP 주소 블록 외에도 개별 Adobe Experience Cloud 제품에는 사용하는 자체 IP 주소가 있습니다.

* [Adobe Analytics](https://experienceleague.adobe.com/ko/docs/analytics/technotes/ip-addresses)
* [Customer Journey Analytics](https://experienceleague.adobe.com/ko/docs/analytics-platform/using/technotes/ip-addresses)
* [Marketo Engage](https://experienceleague.adobe.com/ko/docs/marketo/using/getting-started/initial-setup/configure-protocols-for-marketo#step-allowlist-marketo-ips)
* [Adobe Workfront](https://experienceleague.adobe.com/ko/docs/workfront/using/administration-and-setup/get-started-administration/configure-your-firewall)

## 모든 Adobe IP 주소 블록

다음 표에는 모든 Adobe 소유 IP 주소가 나와 있습니다. 이 표에는 전 세계 Adobe에서 운영하는 모든 Adobe 직원 사무실 및 데이터 센터가 포함되어 있습니다. 퍼블릭 클라우드에서 호스팅되는 서비스는 포함되지 않습니다.

| IP 블록(CIDR 표기법) |
| --- |
| `63.140.32.0/19` |
| `66.117.16.0/20` |
| `66.235.128.0/19` |
| `130.248.0.0/16` |
| `172.82.192.0/18` |
| `185.34.188.0/22` |
| `192.243.240.0/22` |

{style="table-layout:auto"}

## Adobe Experience Cloud 데이터 수집 및 FTP IP 주소 블록

조직에서 특정 IP 주소 범위를 허용하고자 할 경우 다음 표를 참조할 수 있습니다. 이러한 서비스에는 다음이 포함됩니다.

* 모든 Experience Cloud 제품에 대한 데이터 수집 서버
* 모든 Experience Cloud 제품용 FTP 서버

이 섹션의 모든 IP 범위는 위 표에 포함되어 있습니다.

| 위치 | IP 범위(CIDR 표기법) |
| --- | --- |
| 오스트레일리아 | `63.140.55.0/24` |
| 오스트레일리아 | `63.140.56.0/23` |
| 캘리포니아 | `63.140.32.0/23` |
| 캘리포니아 | `63.140.34.0/24` |
| 프랑스 | `63.140.62.0/23` |
| 인도 | `66.117.22.0/23` |
| 일본 | `130.248.169.0/23` |
| 일본 | `63.140.50.0/23` |
| 일본 | `66.117.31.0/24` |
| 런던 | `66.235.156.0/24` |
| 런던 | `185.34.188.0/22` |
| 런던 | `130.248.152.0/22` |
| 런던 | `130.248.244.0/23` |
| 오하이오 | `66.117.20.0/24` |
| 오레곤 | `66.235.132.0/22` |
| 오레곤 | `130.248.130.0/23` |
| 오레곤 | `130.248.150.0/24` |
| 오레곤 | `130.248.160.0/21` |
| 오레곤 | `192.243.242.0/24` |
| 싱가포르 | `130.248.170.0/23` |
| 싱가포르 | `130.248.240.0/24` |
| 싱가포르 | `63.140.44.0/22` |
| 싱가포르 | `63.140.48.0/23` |
| 싱가포르 | `66.117.30.0/24` |
| 싱가포르 | `172.82.240.8/29` |
| 싱가포르 | `172.82.240.88/29` |
| 버지니아 | `63.140.38.0/23` |
| 버지니아 | `63.140.54.0/24` |
| 버지니아 | `67.202.5.244` |

{style="table-layout:auto"}

Adobe Experience Cloud은 제한된 용량에서 IPv6도 지원합니다. 이러한 IP 블록은 위의 IPv4 블록들과 유사한 데이터 수집 목적을 제공하지만 FTP는 포함하지 않습니다.

| 위치 | Host |
| --- | --- |
| 오스트레일리아 | `2406:da1c:406:1a00::/56` |
| 오스트레일리아 | `2406:da1c:ce5:b400::/56` |
| 캘리포니아 | `2600:1f1c:366:d900::/56` |
| 프랑스 | `2a05:d012:706:d000::/56` |
| 인도 | `2406:da1a:f34:6a00::/56` |
| 아일랜드 | `2a05:d018:309:600::/56` |
| 일본 | `2406:da14:b07:ab00::/56` |
| 오하이오 | `2600:1f16:130f:7d00::/56` |
| 오레곤 | `2600:1f14:1eb:7d00::/56` |
| 오레곤 | `2600:1f14:9d3:2b00::/56` |
| 싱가포르 | `2406:da18:6e8:1e00::/56` |
| 버지니아 | `2600:1f18:1a20:e800::/56` |
| 버지니아 | `2600:1f18:4fd:6000::/56` |
| 버지니아 | `2600:1f18:b00:e100::/56` |
| 버지니아 | `2600:1f18:d1f:bd00::/56` |

>[!TIP]
>
>Adobe Analytics 내보내기 기능(Data Warehouse 및 데이터 피드 포함)에 대한 FTP 연결은 런던, 오레곤 및 싱가포르 위치에 있는 IPv4 주소에서만 시작됩니다.
