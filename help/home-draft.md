---
description: Experience Cloud 중앙 인터페이스 구성 요소에 대해 알아봅니다. Admin Console에서 사용자 및 제품 관리에 대한 도움을 받고 애플리케이션을 Experience Cloud 서비스로 사용할 수 있도록 하십시오. 대상자 라이브러리, 고객 속성, Experience Cloud Assets 등의 도움말에 액세스할 수 있습니다.
title: Experience Cloud 인터페이스 설명서
uuid: aec6f689-e617-4876-ae6c-e961cfcb991a
feature: Central Interface Components
topic: Administration
role: Admin
level: Experienced
exl-id: aedad5cb-3282-4a97-8e7e-6d65f7b75ba9
source-git-commit: 5df8104d3d148cc7bda823b27bf96429ddb6018d
workflow-type: tm+mt
source-wordcount: '790'
ht-degree: 80%

---

# Experience Cloud 중앙 인터페이스 개요

[Experience Cloud](https://experience.adobe.com)는 Adobe의 디지털 마케팅 애플리케이션, 제품 및 서비스 통합 제품군입니다. 직관적인 인터페이스에서 클라우드 애플리케이션, 제품 기능 및 서비스에 빠르게 액세스할 수 있습니다.

![Experience Cloud](assets/landing.png)

Experience Cloud 헤더에서 다음 작업을 수행할 수 있습니다.

* 모든 Experience Cloud 애플리케이션 및 서비스에 액세스
* 도움말 메뉴에서 제품 설명서, 튜토리얼 및 커뮤니티 게시물 검색 Experience League에서 결과 보기
* 검색 필드에서 글로벌 검색을 사용하여 전역으로 비즈니스 오브젝트 검색 (Experience Platform 사용자만 해당)
* 계정 [환경 설정](features/account-preferences.md)(경고, 알림 및 구독) 관리

## Experience Cloud에 로그인 {#signin}

로그인한 다음 올바른 [조직](administration/organizations.md)에 속해 있는지 확인하십시오.

1. [Adobe Experience Cloud](https://experience.adobe.com)를 탐색하십시오.
1. Adobe 이메일 주소를 입력한 다음 **[!UICONTROL 계속]**&#x200B;을 선택합니다.
1. 계정을 선택합니다.
1. 암호를 입력합니다.
1. 올바른 조직에 속해 있는지 확인합니다.

   ![올바른 조직에 속해 있는지 확인합니다](assets/organizations-menu.png)

   **조직 확인**

   [조직](administration/organizations.md)이 인터페이스 헤더에 표시됩니다.

   조직이 Federated ID를 사용하는 경우 Experience Cloud를 통해 이메일 주소 및 암호를 입력할 필요 없이 조직의 SSO(Single Sign-On)로 로그인할 수 있습니다. 이 작업을 수행하려면 `#/sso:@domain`을 Experience Cloud URL(`https://experience.adobe.com`)에 추가하십시오.

   예를 들어 조직에 Federated ID와 도메인 `adobecustomer.com`가 있는 경우 URL 링크를 `https://experience.adobe.com/#/sso:@adobecustomer.com`로 설정합니다. 애플리케이션 경로가 첨부된 이 URL을 책갈피로 지정하여 바로 특정 애플리케이션으로 이동할 수도 있습니다. (예: Adobe Analytics의 경우 `https://experience.adobe.com/#/sso:@adobecustomer.com/analytics`.)

## Experience Cloud 애플리케이션 액세스 {#navigation}

Experience Cloud에 로그인하면 통합 헤더에서 모든 애플리케이션, 서비스 및 조직에 빠르게 액세스할 수 있습니다.

조직의 Experience Cloud 애플리케이션 및 서비스에 액세스하려면 애플리케이션 선택기 ![메뉴](assets/menu-icon.png)로 이동하십시오.

![Experience Cloud 애플리케이션 액세스](assets/platform-core-services.png)

## 도움말 및 지원 요청 {#support}

헤더의 **[!UICONTROL 도움말 센터]**(![에셋](assets/help-icon.png))를 사용하여 [Experience League](https://experienceleague.adobe.com/#home)의 도움말 콘텐츠(설명서, 튜토리얼 및 교육 과정)와 개별 애플리케이션의 추가 리소스가 포함된 학습 및 도움말을 이용하십시오. 오픈엔드 피드백을 제출하고 우선 순위가 지정된 지원 티켓을 만들 수도 있습니다.

![도움말 및 지원 요청](assets/search-menu.png)

[!UICONTROL 도움말] 메뉴로 또한 다음에 액세스할 수 있습니다.

* **[!UICONTROL 지원]:** 지원 티켓을 만들거나 Twitter를 사용하여 [!UICONTROL 지원 센터]에 문의합니다.
* **[!UICONTROL 피드백]:** Experience Cloud 경험에 관한 의견을 공유할 수 있습니다. 귀하의 피드백은 Adobe의 제품 및 서비스를 개선하는 데 사용됩니다.
* **[!UICONTROL 상태]:** `https://status.adobe.com/experience_cloud`로 이동하여 제품 작동 상태 및 [!UICONTROL 구독 관리]를 확인합니다.
* **[!UICONTROL 개발자 연결]:** `adobe.io`로 이동하여 개발자 설명서를 찾습니다.

## 사용자 프로필 관리

[!UICONTROL 프로필] 메뉴에서 다음 작업을 수행할 수 있습니다.

* 어두운 테마 지정 (일부 애플리케이션에서는 이 테마를 지원하지 않음)
* Experience Cloud [환경 설정](features/account-preferences.md) 관리
* [조직](administration/organizations.md) 선택 또는 검색
* [!UICONTROL 법적 고지 사항] 보기
* 로그아웃
* 계정 환경 설정, 알림 및 구독 구성

## 제품 내 알림 및 공지 보기 {#notifications}

알림 및 공지를 보려면 벨 아이콘을 클릭합니다. 공지는 제품 릴리스, 유지 관리 알림, 공유 항목 및 승인 요청을 포함하여 관련성 있고 실행 가능한 업데이트일 수 있습니다.

![알림 및 공지](assets/notifications-menu-small.png)

알림 및 알림을 관리하려면 [계정 환경 설정 및 알림](features/account-preferences.md)을 참조하세요.


## 새로운 기능

Experience Cloud 중앙 인터페이스 구성 요소에 대한 최신 개선 사항에 대해 알아봅니다.

>[!BEGINTABS]

>[!TAB Experience Cloud과 Slack 통합]

[!DNL Slack] 채널로 Experience Cloud 알림을 보내도록 계정 환경 설정을 구성할 수 있습니다.

[!BADGE Beta]{type=Informative url="https://experienceleague.adobe.com/en/docs/core-services/interface/features/account-preferences#notifications" tooltip="Slack에 대해 알아보기"}


>[!TAB 새로운 Campaign Web 사용자 인터페이스]

새로운 Adobe Campaign 사용자 인터페이스를 경험하십시오. 더욱 현대적이고 직관적이며 동적입니다.

[![이미지](assets/do-not-localize/learn-more-button.svg)](start/campaign-ui.md#ac-web-ui)


>[!TAB 예정된 푸시 채널 변경 사항]

Android FCM(Firebase Cloud Messaging) 서비스에 대한 몇 가지 중요한 변경 사항은 2024년에 릴리스될 예정이며 Adobe Campaign 구현에 영향을 미칠 수 있습니다. 이 변경 사항을 지원하려면 Android 푸시 메시지에 대한 구독 서비스 구성을 업데이트해야 할 수 있습니다. 미리 확인하고 조치를 취할 수 있습니다.

[![이미지](assets/do-not-localize/learn-more-button.svg)](../technotes/upgrades/push-technote.md)



>[!ENDTABS]

## 기본 사항부터 시작

<table style="table-layout:fixed">
  <tr style="border: 0;">
    <td>
    <a href="start/whats-new.md"><img src="assets/do-not-localize/start-capabilities.png"></a>
    <div><strong>주요 기능</strong><br/>크로스 채널 캠페인 관리를 위한 Adobe Campaign v8의 주요 기능을 살펴보십시오.</div>
    </td>
    <td>
    <a href="start/connect.md"><img src="assets/do-not-localize/start-connect.jpeg"></a>
    <div><strong>Campaign v8에 연결</strong><br/>클라이언트 콘솔을 설치 및 구성하여 Adobe Campaign v8에 연결하고 캠페인 관리 여정을 시작하는 방법에 대해 알아보십시오.</div><br/>
    </td>
    <td>
    <a href="start/create-message.md"><img src="assets/do-not-localize/start-send.jpeg"></a>
    <div><strong>메시지 보내기</strong><br/>여러 채널(이메일, SMS, 푸시 알림 등)에서 메시지를 보내는 방법을 알아보십시오.
    </div></td>
    <td>
    <a href="audiences/create-profiles.md"><img src="assets/do-not-localize/start-profiles.png"></a>
    <div><strong>프로필 가져오기</strong><br/>Adobe Campaign v8 데이터베이스의 프로필 관리를 쉽게 살펴볼 수 있습니다. 수동으로 또는 가져오기를 통해 프로필을 추가하여 고객 데이터를 세분화하고 캠페인을 손쉽게 사용자 지정할 수 있습니다.</div>
    </td>
  </tr>
  <tr style="border: 0;">
    <td align="center"><a href="start/whats-new.md"><img src="assets/do-not-localize/learn-more-button.svg"></a></td>
    <td align="center"><a href="start/connect.md"><img src="assets/do-not-localize/learn-more-button.svg"></a></td>
    <td align="center"><a href="start/create-message.md"><img src="assets/do-not-localize/learn-more-button.svg"></a></td>
    <td align="center"><a href="audiences/create-profiles.md"><img src="assets/do-not-localize/learn-more-button.svg"></a></td>
    </tr>
</table>

## 설명서 살펴보기

<table style="table-layout:auto">
  <tr style="border: 0;">
    <td>
      <img src="assets/do-not-localize/icon-start.svg" width="35px">
    <br/>
      <strong>시작</strong><br/><a href="start/campaign-ui.md">사용자 인터페이스</a> - <a href="start/ac-components.md">구성 요소 및 프로세스</a> - <a href="start/v7-to-v8.md">Classic v7에서 v8로</a> - <a href="start/campaign-faq.md">FAQ</a>
    </td>
    <td>
      <img src="assets/do-not-localize/icon-experience.svg" width="35px">
    <br/>
      <strong>고객 경험</strong><br/><a href="../automation/workflow/about-workflows.md" target="_blank">워크플로로 자동화</a> - <a href="../automation/campaigns/set-up-campaigns.md" target="_blank">캠페인 오케스트레이션</a> - <a href="interaction/interaction.md">의사 결정 관리</a> - <a href="send/personalize.md">개인화</a>
    </td>
    <td>
      <img src="assets/do-not-localize/icon-send.svg" width="35px">
    <br/>
      <strong>메시지 보내기</strong><br/><a href="start/create-message.md">시작</a> - <a href="send/preview-and-proof.md">미리 보기 및 증명</a> - <a href="send/predictive.md">전송 시간 최적화</a> - <a href="reporting/gs-reporting.md">보고 및 분석</a>
    </td>
  </tr>
  <tr style="border: 0;">
    <td>
      <img src="assets/do-not-localize/icon_profile-audience.svg" width="35px">
    <br/>
      <strong>프로필 및 대상자</strong><br/><a href="audiences/create-profiles.md">프로필 추가</a> - <a href="audiences/create-audiences.md">대상자 만들기</a> - <a href="start/subscriptions.md">구독 관리</a> - <a href="start/privacy.md">개인 정보</a>
    </td>
    <td>
      <img src="assets/do-not-localize/icon-configure.svg" width="35px">
    <br/>
      <strong>아키텍처 및 구성</strong><br/><a href="architecture/architecture.md">아키텍처</a> - <a href="start/implement.md">Campaign v8 구현</a> - <a href="connect/integration.md">다른 솔루션과 연결</a> - <a href="start/gs-permissions.md">사용자 및 권한</a>
    </td>
    <td>
      <img src="assets/do-not-localize/icon-dev.svg" width="35px">
    <br/>
      <strong>개발자 리소스</strong><br/><a href="dev/datamodel.md">Campaign v8 데이터 모델</a> - <a href="dev/schemas.md">스키마</a> - <a href="dev/api.md">API</a>
    </td>
  </tr>
</table>

## 추가 리소스

[Adobe Campaign v8 제품 설명](https://helpx.adobe.com/kr/legal/product-descriptions/adobe-campaign-managed-cloud-services.html){target="_blank"} - [Adobe Campaign 웹 사용자 인터페이스 설명서](https://experienceleague.adobe.com/docs/campaign-web/v8/campaign-web-home.html?lang=ko-KR){target="_blank"} - [튜토리얼](https://experienceleague.adobe.com/docs/campaign-learn/tutorials/overview.html?lang=ko-KR){target="_blank"} - [[!DNL Adobe Campaign] 자동화 안내서](https://experienceleague.adobe.com/docs/campaign/automation/home.html?lang=ko){target="_blank"} - [Campaign v8용 컨트롤 패널](https://experienceleague.adobe.com/docs/control-panel/using/discover-control-panel/key-features.html?lang=ko){target="_blank"}

