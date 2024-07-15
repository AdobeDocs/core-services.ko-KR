---
description: Experience Cloud 중앙 인터페이스 구성 요소에 대해 알아봅니다. 이 도움말에는 Admin Console에서의 사용자 및 제품 관리, Experience Cloud 서비스를 위한 애플리케이션 활성화, 대상자 라이브러리, 고객 속성, Experience Cloud Assets 등에 대한 도움말이 포함되어 있습니다.
title: Experience Cloud 인터페이스 도움말 및 설명서
uuid: aec6f689-e617-4876-ae6c-e961cfcb991a
feature: Central Interface Components
topic: Administration
role: Admin
level: Experienced
exl-id: aedad5cb-3282-4a97-8e7e-6d65f7b75ba9
source-git-commit: a4e0461791cd676365857c2dd4ef28c0e40c3430
workflow-type: tm+mt
source-wordcount: '717'
ht-degree: 100%

---

# Experience Cloud 중앙 인터페이스 개요

[Experience Cloud](https://experience.adobe.com)는 Adobe의 디지털 마케팅 애플리케이션, 제품 및 서비스 통합 제품군입니다. 직관적인 인터페이스에서 클라우드 애플리케이션, 제품 기능 및 서비스에 빠르게 액세스할 수 있습니다.

![Experience Cloud](assets/landing.png)

Experience Cloud 헤더에서 다음 작업을 수행할 수 있습니다.

* 애플리케이션 및 서비스에 액세스하기
* 도움말 메뉴에서 제품 설명서, 튜토리얼 및 커뮤니티 게시물 검색 Experience League에서 결과 보기
* 검색 필드에서 글로벌 검색을 사용하여 전역으로 비즈니스 오브젝트 검색 (Experience Platform 사용자만 해당)
* 계정 환경 설정 관리 (경고, 알림 및 구독)

## Experience Cloud에 로그인 {#signin}

로그인한 다음 올바른 [조직](administration/organizations.md)에 속해 있는지 확인하십시오.

1. [Adobe Experience Cloud](https://experience.adobe.com)를 탐색하십시오.
1. Adobe 이메일 주소를 입력한 다음 **[!UICONTROL 계속]**&#x200B;을 선택합니다.
1. 계정을 선택합니다.
1. 암호를 입력합니다.
1. 올바른 조직에 속해 있는지 확인합니다.

   ![올바른 조직에 속해 있는지 확인합니다](assets/organizations-menu.png)

   **조직 확인**

   올바른 [조직](administration/organizations.md)에 로그인했는지 확인하려면 프로필 아바타를 클릭하여 조직 이름을 확인합니다. 둘 이상의 조직에 대한 액세스 권한을 보유하고 있다면 다른 조직을 확인하고 헤더 표시줄에서 바로 해당 조직으로 전환할 수도 있습니다.

   조직이 Federated ID를 사용하는 경우 Experience Cloud를 통해 이메일 주소 및 암호를 입력할 필요 없이 조직의 SSO(Single Sign-On)로 로그인할 수 있습니다. 이 작업을 수행하려면 `#/sso:@domain`을 Experience Cloud URL(`https://experience.adobe.com`)에 추가하십시오.

   예를 들어 조직에 Federated ID와 도메인 `adobecustomer.com`가 있는 경우 URL 링크를 `https://experience.adobe.com/#/sso:@adobecustomer.com`로 설정합니다. 애플리케이션 경로가 첨부된 이 URL을 책갈피로 지정하여 바로 특정 애플리케이션으로 이동할 수도 있습니다. (예: Adobe Analytics의 경우 `https://experience.adobe.com/#/sso:@adobecustomer.com/analytics`.)

## Experience Cloud 애플리케이션 액세스 {#navigation}

Experience Cloud에 로그인하면 통합 헤더에서 모든 애플리케이션, 서비스 및 조직에 빠르게 액세스할 수 있습니다.

조직의 Experience Cloud 애플리케이션 및 서비스에 액세스하려면 애플리케이션 선택기 ![메뉴](assets/menu-icon.png)로 이동하십시오.

![Experience Cloud 애플리케이션 액세스](assets/platform-core-services.png)

## 도움말 및 지원 요청 {#support}

헤더의 도움말 아이콘(![자산](assets/help-icon.png))을 사용하여 [Experience League](https://experienceleague.adobe.com/#home)의 도움말 콘텐츠(설명서, 튜토리얼 및 교육 과정)와 개별 애플리케이션의 추가 리소스가 포함된 학습 및 도움말을 이용하십시오. 오픈엔드 피드백을 제출하고 우선 순위가 지정된 지원 티켓을 만들 수도 있습니다.

![도움말 및 지원 요청](assets/search-menu.png)

[!UICONTROL 도움말] 메뉴로 또한 다음에 액세스할 수 있습니다.

* **[!UICONTROL 지원]:** 지원 티켓을 만들거나 Twitter를 사용하여 [!UICONTROL 지원 센터]에 문의합니다.
* **[!UICONTROL 피드백]:** Experience Cloud 경험에 관한 의견을 공유할 수 있습니다. 귀하의 피드백은 Adobe의 제품 및 서비스를 개선하는 데 사용됩니다.
* **[!UICONTROL 상태]:** `https://status.adobe.com/experience_cloud`로 이동하여 제품 작동 상태 및 [!UICONTROL 구독 관리]를 확인합니다.
* **[!UICONTROL 개발자 연결]:** `adobe.io`로 이동하여 개발자 설명서를 찾습니다.

## 사용자 프로필 및 계정 환경 설정 {#preferences}

Experience Cloud 환경 설정에는 알림, 구독 및 경고가 포함됩니다. 계정 환경 설정 메뉴에서 다음을 할 수 있습니다.

* 어두운 테마 지정 (일부 애플리케이션에서는 이 테마를 지원하지 않음)
* [조직](administration/organizations.md) 검색
* 로그아웃
* 계정 환경 설정, 알림 및 구독 구성

환경 설정을 관리하려면 계정 메뉴 **[!UICONTROL 환경 설정]**&#x200B;에서 ![환경 설정](assets/preferences-icon-sm.png)을 선택합니다.

![사용자 프로필 및 계정 환경 설정](assets/preferences-page.png)

[!UICONTROL Experience Cloud 환경 설정]에서 다음 기능을 구성할 수 있습니다.

| 기능 | 설명 |
|--- |--- |
| 기본 [조직](administration/organizations.md) | Experience Cloud를 시작할 때 보려는 조직을 선택합니다. |
| [!UICONTROL 제품 데이터 수집] | 귀하가 Adobe 제품을 사용하는 방식에 대한 데이터를 Adobe에서 수집하는 데 사용되는 기술을 선택하십시오. |
| [!UICONTROL 맞춤형 학습 권장 사항 및 프로모션] | Adobe 제품에 대한 개인화된 지원을 받을 위치를 선택하십시오. 해당 지원은 이메일, 제품 내 알림 및 Experience League 커뮤니티를 통해 제공됩니다. [자세히 보기.](features/personalized-learning.md) |
| [!UICONTROL 구독] | 구독하기 원하는 제품 및 범주를 선택하십시오. [!UICONTROL 알림] 팝업 및 이메일 알림. |
| [!UICONTROL 우선 순위] | 높은 우선 순위로 고려하고 싶은 범주를 선택하십시오. 이러한 범주는 높음 태그로 표시되며 경고처럼 게재되도록 구성할 수 있습니다. |
| [!UICONTROL 경고] | 브라우저에 경고를 표시할 알림을 선택하십시오. 경고는 창의 오른쪽 상단에 몇 초 동안 표시됩니다. |
| 이메일 | 이메일 알림을 수신할 빈도를 지정합니다. (발송하지 않음, 실시간, 매일 또는 매주) |

{style="table-layout:auto"}

## 알림 및 공지 {#notifications}

제품 릴리스, 유지 관리 알림, 공유 항목 및 승인 요청을 포함하여 관련성 있고 실행 가능한 업데이트에 대한 알림을 받으려면 **[!UICONTROL 알림]**&#x200B;을 선택합니다.

![알림 및 공지](assets/notifications-menu-small.png)
