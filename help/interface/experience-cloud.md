---
description: Experience Cloud 중앙 인터페이스 구성 요소에 대해 알아봅니다. 이 도움말에는 Admin Console에서의 사용자 및 제품 관리, Experience Cloud 서비스를 위한 애플리케이션 활성화, 대상자 라이브러리, 고객 속성, Experience Cloud Assets 등에 대한 도움말이 포함되어 있습니다.
title: Experience Cloud 인터페이스 도움말 및 설명서
uuid: aec6f689-e617-4876-ae6c-e961cfcb991a
feature: Central Interface Components
topic: Administration
role: Admin
level: Experienced
exl-id: aedad5cb-3282-4a97-8e7e-6d65f7b75ba9
source-git-commit: 8b32f5d688309c01acc5f0618d119f56d339a9e5
workflow-type: tm+mt
source-wordcount: '1229'
ht-degree: 99%

---

# Experience Cloud 중앙 인터페이스 구성 요소 안내서

[Experience Cloud](https://experience.adobe.com)는 Adobe의 디지털 마케팅 애플리케이션, 제품 및 서비스 통합 제품군입니다. 직관적인 인터페이스에서 클라우드 애플리케이션, 제품 기능 및 서비스에 빠르게 액세스할 수 있습니다.

![Experience Cloud](assets/landing.png)

Experience Cloud 헤더에서 다음 작업을 수행할 수 있습니다.

* 애플리케이션 및 서비스에 액세스하기
* 도움말 메뉴에서 제품 설명서, 튜토리얼 및 커뮤니티 게시물 검색 Experience League에서 결과 보기
* 검색 필드에서 글로벌 검색을 사용하여 전역으로 비즈니스 오브젝트 검색 (Experience Platform 사용자만 해당)
* 계정 환경 설정 관리 (경고, 알림 및 구독)

## Experience Cloud에 로그인 {#signin}

로그인한 다음 올바른 [조직](organizations.md)에 속해 있는지 확인하십시오.

1. [Adobe Experience Cloud](https://experience.adobe.com)를 탐색하십시오.
1. Adobe 이메일 주소를 입력한 다음 **[!UICONTROL 계속]**&#x200B;을 선택합니다.

   관리자는 [Experience Cloud 사용자 인증](admin-getting-started.md#migration)을 참조하여 ID 유형(Business ID)의 중요 업데이트에 대해 알아보십시오.

1. 계정을 선택합니다.
1. 암호를 입력합니다.
1. 올바른 조직에 속해 있는지 확인합니다.

   ![올바른 조직에 속해 있는지 확인합니다](assets/organizations-menu.png)

   **조직 확인**

   올바른 [조직](organizations.md)에 로그인했는지 확인하려면 프로필 아바타를 클릭하여 조직 이름을 확인합니다. 둘 이상의 조직에 대한 액세스 권한을 보유하고 있다면 다른 조직을 확인하고 헤더 표시줄에서 바로 해당 조직으로 전환할 수도 있습니다.

   조직이 Federated ID를 사용하는 경우 Experience Cloud를 통해 주소 및 암호를 입력할 필요 없이 조직의 SSO(Single Sign-On)로 로그인할 수 있습니다. 이 작업을 수행하려면 `#/sso:@domain`을 Experience Cloud URL(`https://experience.adobe.com`)에 추가하십시오.

   예를 들어 조직에 Federated ID와 도메인 `adobecustomer.com`가 있는 경우 URL 링크를 `https://experience.adobe.com/#/sso:@adobecustomer.com`로 설정합니다. 애플리케이션 경로가 첨부된 이 URL을 책갈피로 지정하여 바로 특정 애플리케이션으로 이동할 수도 있습니다. (예: Adobe Analytics의 경우 `https://experience.adobe.com/#/sso:@adobecustomer.com/analytics`.)

## Experience Cloud 애플리케이션 액세스 {#navigation}

Experience Cloud에 로그인하면 통합 헤더에서 모든 애플리케이션, 서비스 및 조직에 빠르게 액세스할 수 있습니다.

조직의 Experience Cloud 애플리케이션 및 서비스에 액세스하려면 애플리케이션 선택기 ![메뉴](assets/menu-icon.png)로 이동하십시오.

![Experience Cloud 애플리케이션 액세스](assets/platform-core-services.png)

## Experience Cloud의 브라우저 지원 {#browser}

최상의 성능을 위해 Experience Cloud는 최신 버전과 두 개의 이전 버전을 포함하여 가장 많이 사용되는 브라우저에 최적화되었습니다.

* Chrome
* Edge
* Firefox
* Opera
* Safari

브라우저가 목록에 없어도 지원될 수 있지만 목록에 있는 브라우저 중 하나를 선택하는 것이 좋습니다.

>[!NOTE]
>
>Experience Cloud 도메인에서 실행 중인 모든 애플리케이션이 전체 브라우저를 지원하는 것은 아닙니다. 확실치 않다면 특정 애플리케이션의 설명서를 참조하십시오.

## Experience Cloud의 언어 지원 {#languages}

Experience Cloud는 Adobe 사용자 계정 환경 설정에 설정되는 각 사용자의 기본 언어를 지원합니다. 현재 지원되는 언어는 다음과 같습니다.

* 중국어
* 영어
* 프랑스어
* 독일어
* 이탈리아어
* 일본어
* 한국어
* 포르투갈어
* 스페인어
* 대만어

모든 애플리케이션이 전 세계 언어를 지원하고 있지만 모든 애플리케이션이 위에서 언급된 모든 언어로 제공되지 않습니다. 기본 언어가 Experience Cloud 애플리케이션에서 지원되지 않는 경우 보조 언어를 기본값으로 설정할 수 있습니다. [Experience Cloud 사용자 환경 설정](https://experience.adobe.com/preferences)에서 수행할 수 있습니다.

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
* [조직](organizations.md) 검색
* 로그아웃
* 계정 환경 설정, 알림 및 구독 구성

환경 설정을 관리하려면 계정 메뉴 **[!UICONTROL 환경 설정]**&#x200B;에서 ![환경 설정](assets/preferences-icon-sm.png)을 선택합니다.

![사용자 프로필 및 계정 환경 설정](assets/preferences-page.png)

[!UICONTROL Experience Cloud 환경 설정]에서 다음 기능을 구성할 수 있습니다.

| 기능 | 설명 |
|--- |--- |
| 기본 [조직](organizations.md) | Experience Cloud를 시작할 때 보려는 조직을 선택합니다. |
| [!UICONTROL 제품 데이터 수집] | 귀하가 Adobe 제품을 사용하는 방식에 대한 데이터를 Adobe에서 수집하는 데 사용되는 기술을 선택하십시오. |
| [!UICONTROL 맞춤형 학습 권장 사항 및 프로모션] | Adobe 제품에 대한 개인화된 지원을 받을 위치를 선택하십시오. 해당 지원은 이메일, 제품 내 알림 및 Experience League 커뮤니티를 통해 제공됩니다. [자세히 보기.](personalized-learning-preferences.md) |
| [!UICONTROL 구독] | 구독하기 원하는 제품 및 범주를 선택하십시오. [!UICONTROL 알림] 팝업 및 이메일 알림. |
| [!UICONTROL 우선 순위] | 높은 우선 순위로 고려하고 싶은 범주를 선택하십시오. 이러한 범주는 높음 태그로 표시되며 경고처럼 게재되도록 구성할 수 있습니다. |
| [!UICONTROL 경고] | 브라우저에 경고를 표시할 알림을 선택하십시오. 경고는 창의 오른쪽 상단에 몇 초 동안 표시됩니다. |
| 이메일 | 이메일 알림을 수신할 빈도를 지정합니다. (발송하지 않음, 실시간, 매일 또는 매주) |

{style="table-layout:auto"}

## 알림 및 공지 {#notifications}

제품 릴리스, 유지 관리 알림, 공유 항목 및 승인 요청을 포함하여 관련성 있고 실행 가능한 업데이트에 대한 알림을 받으려면 **[!UICONTROL 알림]**&#x200B;을 선택합니다.

![알림 및 공지](assets/notifications-menu-small.png)

## Experience Cloud 도메인 {#domains}

Experience Cloud는 다음 호스트를 사용하여 애플리케이션을 제공하고 성능과 제품 경험을 개선합니다. Adobe에서 최적의 경험을 구축하려면 다음 도메인을 방화벽의 허용 목록에 추가하는 것이 좋습니다. 추가 도메인은 Adobe Analytics와 같은 특정 Experience Cloud 애플리케이션에서 사용할 수 있습니다. 자세한 내용은 해당 애플리케이션의 설명서를 참조하십시오.

| 기술 | 도메인 |
|--- |--- |
| Adobe Experience Cloud 도메인 | `adobe.com`, `adobe.net`, `adobe.io` |
| Adobe Identity Management Service (IMS) | `adobelogin.com` |
| Experience Cloud 글꼴 | `typekit.net` |
| Adobe 데이터 수집 (제품 지침 및 도움말용) | `adobedtm.com` |
| Gainsight (제품 지침 및 도움말용) | `esp.aptrinsic.com` |

## 관리 및 교차 애플리케이션 서비스에 대한 도움말 보기

이 안내서는 Admin Console의 Experience Cloud 사용자 및 제품 관리에 대한 도움말 액세스를 제공하며 플랫폼 서비스를 위한 애플리케이션을 활성화합니다. 또한 대상자 라이브러리, 고객 속성, Experience Cloud Assets 등의 도움말에 액세스할 수 있습니다.

* [[!UICONTROL 대상자 라이브러리]](audience-library.md)
* [[!UICONTROL 고객 속성]](attributes.md)
* [Experience Cloud [!UICONTROL Assets]](experience-cloud-assets.md)
* [Experience Cloud 쿠키](cookies-privacy.md)
* [사용자 및 제품 관리](admin-getting-started.md) (Admin Console)
* [핵심 서비스용 애플리케이션 활성화](core-services.md)
* [자주 묻는 질문](admin-getting-started.md)
* [조직 및 계정 연결](organizations.md)
* [통합](marketing-cloud-integrations.md)
* [Adobe Target과 Experience Cloud 통합](https://experienceleague.adobe.com/docs/target/using/integrate/a4t/a4t.html?lang=ko)
* [Experience Cloud 개인정보 보호 및 보안 개요](assets/Adobe-Marketing-Cloud-Privacy-and-Security-Overview.pdf)
* [DNS 프리페치](admin-getting-started.md#concept_6BC8C6856E3644F8956D7AD0A96383B7)

## 안내서

관련 Experience Cloud 안내서는 다음을 포함합니다.

* [Adobe Mobile](https://experienceleague.adobe.com/docs/mobile-services/using/home.html?lang=ko)
* [Experience Platform Co-op 그래프](https://experienceleague.adobe.com/docs/device-co-op/using/home.html?lang=ko)
* [Exchange](https://exchange.adobe.com/experiencecloud)
* [Experience Cloud ID 서비스](https://experienceleague.adobe.com/docs/id-service/using/home.html?lang=ko)
* [Experience Platform 태그](https://experienceleague.adobe.com/docs/tags.html?lang=ko-KR)
* [Experience Cloud Debugger](https://experienceleague.adobe.com/docs/debugger/using/experience-cloud-debugger.html?lang=ko)

## 튜토리얼

Adobe Experience League에서 제공하는 자체 도움말 튜토리얼과 빠른 사용 방법을 활용할 수 있습니다.

* [Experience League의 모든 튜토리얼](https://experienceleague.adobe.com/?lang=en#quick-how-tos)
* [Experience Platform 튜토리얼](https://experienceleague.adobe.com/docs/platform-learn/data-collection/overview.html?lang=ko)
* [Real-time Customer Data Platform](https://experienceleague.adobe.com/docs/platform-learn/tutorials/application-services/rtcdp/understanding-the-real-time-customer-data-platform.html?lang=ko)

## 릴리스 정보 및 관련 Experience Cloud 도움말

* [모든 Experience Cloud 애플리케이션에 대한 제품 설명서](https://experienceleague.adobe.com/docs/home.html?lang=ko) - Experience Cloud 학습 및 지원에서 탐색
* [릴리스 정보 및 제품 업데이트](https://experienceleague.adobe.com/docs/release-notes/experience-cloud/current.html?lang=ko) - Experience Cloud의 새로운 기능 및 구독을 통한 업데이트 받기
* [핵심 서비스 구현 튜토리얼](https://experienceleague.adobe.com/docs/platform-learn/data-collection/overview.html?lang=ko) - 핵심 서비스에 대한 비디오 및 튜토리얼 보기
* [Experience League의 전문가 지원](https://experienceleague.adobe.com/) - 전문가 및 커뮤니티의 안내형 학습
* [교육 및 훈련](https://helpx.adobe.com/kr/learning.html?promoid=KAUDK) - Adobe의 제품을 최대한 활용할 수 있도록 Adobe와 협력하기
* [고객 경험 블로그](https://blog.adobe.com/en/topics/digital-transformation) - Experience Cloud 블로그 보기
* [고객 지원](https://experienceleague.adobe.com/?support-solution=General#support) - Adobe 고객 지원 센터에 문의
