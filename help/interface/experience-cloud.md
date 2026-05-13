---
description: CX Enterprise(이전 Experience Cloud)에 대해 알아봅니다. 로그인, 탐색, 검색, 환경 설정, 관리 및 대상 라이브러리, 고객 속성, Assets과 같은 공유 서비스를 다룹니다.
title: CX 엔터프라이즈 인터페이스 및 관리 가이드
uuid: aec6f689-e617-4876-ae6c-e961cfcb991a
feature: Central Interface Components
topic: Administration
role: Admin
level: Experienced
exl-id: aedad5cb-3282-4a97-8e7e-6d65f7b75ba9
TQID: https://experienceleague.adobe.com/7vFfu0DyoTnsrlrWVApm0LLW4jsC0LoXb55jJ3jdxeY
product_v2: id: e1971122-7081-4556-9222-8a31bd71800c
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 50012e2564e88e1a6e16578e3331136c7df0cb21
workflow-type: tm+mt
source-wordcount: 579
ht-degree: 43%

---

# Adobe CX 엔터프라이즈 인터페이스 및 관리 안내서

[Adobe CX Enterprise](https://experience.adobe.com)&#x200B;(Customer Experience Enterprise)는 Adobe의 디지털 마케팅 애플리케이션, 제품 및 서비스 통합 제품군입니다. 직관적인 인터페이스에서 클라우드 애플리케이션, 제품 기능 및 서비스에 빠르게 액세스할 수 있습니다.

<!-- ![CX Enterprise](assets/landing.png) -->

CX 엔터프라이즈 헤더에서 다음을 수행할 수 있습니다.

* 모든 CX 엔터프라이즈 애플리케이션 및 서비스 액세스
* 도움말 메뉴에서 제품 설명서, 튜토리얼 및 커뮤니티 게시물 검색 Experience League에서 결과 보기
* 검색 필드에서 글로벌 검색을 사용하여 전역으로 비즈니스 오브젝트 검색 (Experience Platform 사용자만 해당)
* 계정 [환경 설정](features/account-preferences.md) 관리 (경고, 알림 및 구독)

## CX Enterprise에 로그인

로그인한 다음 올바른 [조직](administration/organizations.md)에 속해 있는지 확인하십시오.

1. [Adobe CX Enterprise](https://experience.adobe.com)&#x200B;(으)로 이동합니다.
1. Adobe 이메일 주소를 입력한 다음 **[!UICONTROL Continue]**&#x200B;을(를) 클릭합니다.
1. 계정을 클릭합니다.
1. 암호를 입력합니다.
1. 올바른 조직에 속해 있는지 확인합니다.

   ![올바른 조직에 속해 있는지 확인합니다](assets/organizations-menu.png)

   **조직 확인**

   [조직](administration/organizations.md)은 인터페이스 헤더에 표시됩니다.

   조직이 Federated ID를 사용하는 경우 CX Enterprise를 사용하면 이메일 주소와 암호를 입력할 필요 없이 조직의 SSO(Single Sign-On)로 로그인할 수 있습니다. 이 작업을 수행하려면 CX 엔터프라이즈 URL(`https://experience.adobe.com`)에 `#/sso:@domain`을(를) 추가하십시오.

   예를 들어 조직에 Federated ID와 도메인 `example.com`가 있는 경우 URL 링크를 `https://experience.adobe.com/#/sso:@example.com`로 설정합니다. 애플리케이션 경로가 첨부된 이 URL을 책갈피로 지정하여 바로 특정 애플리케이션으로 이동할 수도 있습니다. (예: Adobe Analytics의 경우 `https://experience.adobe.com/#/sso:@example.com/analytics`.)

   **참고:** 조직의 관리자가 IP 주소별로 Adobe 제품에 대한 액세스를 제한할 수 있습니다. 이 경우 CX Enterprise에 로그인하거나 이 기능이 활성화된 조직으로 전환하면 오류가 발생할 수 있습니다. 자세한 내용은 [IP 주소로 제품 액세스 제한](https://helpx.adobe.com/enterprise/using/ip-based-access.html)을 참조하세요.


## CX 엔터프라이즈 애플리케이션 액세스

CX Enterprise에 로그인한 후 통합 헤더에서 모든 애플리케이션, 서비스 및 조직에 빠르게 액세스할 수 있습니다.

조직의 CX 엔터프라이즈 응용 프로그램 및 서비스에 액세스하려면 응용 프로그램 선택기 ![메뉴](assets/apps-icon.png)로 이동하십시오.

![CX 엔터프라이즈 애플리케이션에 액세스](assets/platform-core-services.png)

## 도움말 및 지원 요청

헤더의 **[!UICONTROL Help center]**(![asset](assets/help-icon.png))을 사용하여 [Experience League](https://experienceleague.adobe.com/#home)의 도움말 콘텐츠(설명서, 튜토리얼 및 교육 과정)와 개별 애플리케이션의 추가 리소스가 포함된 학습 및 도움말을 이용하십시오. 오픈엔드 피드백을 제출하고 우선순위가 지정된 지원 티켓을 만들 수도 있습니다.

![도움말 및 지원 요청](assets/search-menu.png)

[!UICONTROL Help] 메뉴를 통해 다음에 액세스할 수도 있습니다.

* **[!UICONTROL Support]:** 지원 티켓을 만들거나 Twitter를 사용하여 [!UICONTROL Support]에 문의하세요.
* **[!UICONTROL Feedback]:** CX 엔터프라이즈 환경에 대한 피드백을 공유합니다. 귀하의 피드백은 Adobe의 제품 및 서비스를 개선하는 데 사용됩니다.
* **[!UICONTROL Status]:** `https://status.adobe.com/experience_cloud`(으)로 이동하여 제품 작동 상태 및 [!UICONTROL Manage Subscriptions]을(를) 확인합니다.
* **[!UICONTROL Developer Connection]:** `adobe.io`(으)로 이동하여 개발자 설명서를 찾습니다.

## 사용자 프로필 관리

[!UICONTROL Profile] 메뉴에서 다음을 수행할 수 있습니다.

* 어두운 테마 지정 (일부 애플리케이션에서는 이 테마를 지원하지 않음)
* CX Enterprise [환경 설정](features/account-preferences.md) 관리
* [조직](administration/organizations.md) 선택 또는 검색
* [!UICONTROL Legal Notices] 보기
* 로그아웃
* 계정 환경 설정, 알림 및 구독 구성

## 제품 내 알림 및 공지 사항 보기

알림 및 공지 사항을 보려면 종 모양 아이콘을 클릭하십시오. 공지 사항에는 제품 릴리스, 유지 관리 알림, 공유 항목 및 승인 요청을 포함하여 관련성 있고 실행 가능한 업데이트에 대한 알림이 포함됩니다.

![알림 및 공지](assets/notifications-menu-small.png)

알림 및 경고를 관리하려면 [계정 환경 설정 및 알림](features/account-preferences.md)을 참조하십시오.

## 용어

Adobe은 마케팅 앱, Creative Cloud, Experience League 및 지원 사이트에서 유사한 이름을 사용합니다. 이러한 용어가 CX Enterprise와 다른 곳에서 어떻게 적용되는지 간략하게 비교하려면 [용어](more-resources/terms.md)를 참조하십시오.

