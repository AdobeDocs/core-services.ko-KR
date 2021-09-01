---
description: Adobe Experience Cloud에 로그인하고, 암호 및 알림을 관리하고, 기본 랜딩 페이지를 지정하는 방법을 알아봅니다.
keywords: 핵심 서비스, Experience Cloud 로그인
solution: Experience Cloud
title: '로그인 및 Experience Cloud 프로필 설정 관리 '
uuid: c1e13b99-0069-4fdb-8d72-ddcec3ed1121
feature: Admin Console
topic: Administration
role: Admin
level: Experienced
exl-id: 12addbb6-a29b-4d20-ac8f-77e0846150b5
source-git-commit: 1fb1abc7311573f976f7e6b6ae67f60ada10a3e7
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 90%

---

# 로그인 및 Experience Cloud 프로필 설정 관리

단일 솔루션에 로그인하지 않고 Experience Cloud에 로그인하면 사용자가 소유한 모든 솔루션 및 서비스에 SSO(Single Sign-On)를 사용할 수 있습니다. 이 도움말에서는 Experience Cloud에 로그인하고, 암호 및 알림을 관리하고, 기본 랜딩 페이지를 지정하는 방법에 대해 설명합니다.

>[!IMPORTANT]
>
>관리자는 [관리](admin-getting-started.md#topic_3FCB4099640647E3B2411ADBFCE81909)에서 사용자 및 제품 관리 업데이트에 대한 정보를 참고하십시오.

## Experience Cloud에 로그인(관리자) {#task_034FC955031347F3B02B686A09801A08}

로그인한 다음 올바른 [조직](organizations.md#topic_C31CB834F109465A82ED57FF0563B3F1)에 속해 있는지 확인하십시오.

1. Experience Cloud 메뉴( ![](assets/menu-icon.png))를 선택한 다음 **[!UICONTROL 관리]**&#x200B;를 선택합니다.

   **[!UICONTROL 관리]** 링크가 표시되지 않으면 표시된 [조직](organizations.md#topic_C31CB834F109465A82ED57FF0563B3F1)의 Experience Cloud 관리자가 아닌 것입니다. 관리자가 되는 것과 관련하여 지원이 필요한 경우 귀사의 고객 지원 또는 기존 Experience Cloud 관리자에게 문의하십시오.
1. **[!UICONTROL 관리]**&#x200B;를 선택합니다.

1. 다음 링크 중 하나를 선택하여 계속합니다.

| 요소 | 설명 |
|--- |--- |
| [Admin Console 기본 사항](experience-cloud.md) | Experience Cloud 솔루션 사용을 시작하기 위해 반드시 수행해야 하는 초기 절차에 대해 알아봅니다. |
| [ID 설정](https://helpx.adobe.com/kr/enterprise/using/set-up-identity.html) | 최종 사용자를 인증할 ID 시스템을 정의하고 설정합니다. |
| [사용자 관리](https://helpx.adobe.com/kr/enterprise/using/users.html) | Admin Console에 로그인 및 Experience Cloud 사용자 권한 및 제품 프로필 관리 방법에 대해 알아봅니다. |
| [Admin Console 실행](admin-getting-started.md) | Admin Console은 전체 조직에서 Adobe 사용자 및 제품 자격을 관리하는 중앙 위치입니다.<br>[직접 연결되는 링크](https://adminconsole.adobe.com)를 사용하여 Admin Console에 로그인할 수도 있습니다. |
| [Creative Cloud 사용자 관리](t-admin-add-cc-user.md) | Experience Cloud Assets을 통해 마케터는 Creative Cloud를 사용하여 디자이너 및 다른 크리에이티브 에셋과 폴더를 공유, 동기화 및 공동 작업할 수 있습니다. 여기서 조직과 공동 작업하도록 승인된 Creative Cloud 사용자를 관리할 수 있습니다. |
| [보고서 세트 매핑](core-services.md) | (Analytics 전용) Experience Cloud 핵심 서비스는 개별 보고서 세트 대신 조직과 연결됩니다. 이러한 서비스가 올바르게 작동하도록 하려면 각 Analytics 보고서 세트를 조직에 매핑해야 합니다. (이 작업은 [핵심 서비스용으로 Analytics를 활성화](core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C)하는 광범위한 워크플로의 일부입니다.) |
| [조직 ID](organizations.md) | *조직 ID*&#x200B;는 관리 페이지의 맨 아래에 있습니다. 이 ID는 프로비저닝된 Experience Cloud 회사와 연관된 ID입니다. 이 ID는 24자의 영숫자 문자열과 @AdobeOrg(포함 필수)로 구성됩니다. |

{style=&quot;table-layout:auto&quot;}

## Experience Cloud에 로그인(사용자) {#task_1BFE87E20DCB44078CAC82F3CD44B985}

Experience Cloud에 로그인하는 관리자 이외의 사용자를 위한 도움말입니다.


1. [조직](organizations.md)이 Experience Cloud에서 프로비저닝되었는지 관리자에게 확인합니다.


1. [Adobe Experience Cloud](https://experience.adobe.com) ([!DNL experience.adobe.com]) 로 이동합니다.
1. **[!UICONTROL Adobe ID으로 로그인]**&#x200B;을 선택합니다.

   Experience Cloud 관리자가 계정 유형(Adobe ID 또는 Enterprise ID)을 확인하는 데 도움을 줄 수 있습니다.

1. 랜딩 페이지에서 선택기 아이콘 ![](assets/menu-icon.png)을 선택하여 풀다운 메뉴에 액세스합니다.

   ![](assets/experience-cloud-core-services.png)

   이 메뉴에 표시되는 솔루션 및 서비스는 [관리자](admin-getting-started.md#topic_3FCB4099640647E3B2411ADBFCE81909)가 정의한 애플리케이션 권한에 따라 다릅니다.

## 기본 개인 계정 설정 구성 {#task_73CBCAE6C91749D19C95421E5AC311BA}

Experience Cloud에 로그인한 후 개인 세부 사항을 편집하고, 표시할 기본 [조직](admin-getting-started.md#concept_705C626560A54CA2A4215F1C870C42B2) 및 랜딩 페이지를 지정할 수 있습니다.

1. Experience Cloud에 로그인한 다음, 프로필 아이콘을 선택합니다.

   ![](assets/edit-profile.png)
1. **[!UICONTROL 프로필 편집]**&#x200B;을 선택합니다.

   ![](assets/default-organization.png)
1. 개인 정보를 계속 구성 및 편집한 후 **[!UICONTROL 변경 내용 저장]**&#x200B;을 선택합니다.

## 알림 활성화 {#concept_0105453AD71847B8BFCAF4A40915F157}

시스템 업데이트, 유지 관리 알림, 게시물, 언급 및 공유된 Assets에 대한 알림(이메일을 통해 또는 제품 내에서)을 받습니다. 고객 속성에 대한 업로드 상태를 포함하여 알림을 받으려는 제품 및 솔루션을 지정할 수도 있습니다.

알림으로 이동하려면 **[!UICONTROL 알림]** 아이콘 ![](assets/notifications-icon.png)을 선택한 다음 **[!UICONTROL 설정]** 아이콘 ![](assets/icon_edit_board.png)을 선택합니다.

본인에게 중요한 메시지 유형을 기반으로 하여 알림 표시를 정렬하고 알림을 검색할 수 있습니다. 다음 작업도 수행할 수 있습니다.

* 본인에게 중요한 메시지 유형별로 정렬합니다.
* 알림을 검색합니다.

![](assets/notifications-admin.png)

<!-- <p> <b>Analytics</b> </p> 
<ul id="ul_91BF597858124FA5BF338C36F6C5533F"> 
 <li id="li_FAD3E93CDE6242F58F14D55C8A6E23D7">Contribution analysis completed </li> 
 <li id="li_03D33D3228884CECA371B58656B2F3E7">Guided analysis shared </li> 
 <li id="li_DCF710F89317487B8DAA86CC05C694CA">Scheduled report failure </li> 
</ul> 
<p> <b>Adobe Target</b> </p> 
<p>Test started or stopped </p> 
<p> <b>Media Optimizer</b> </p> 
<p>Performance alerts </p> 
<p> <b>Dynamic Tag Manager</b> </p> 
<ul id="ul_9ACDA418933E40918744D9C32A57DD4B"> 
 <li id="li_4DD0FFD3D9F84A428703611EF767D4D0">New web property created </li> 
 <li id="li_C6B923012E9D40BA91F4CBF7D2D72986">New user added </li> 
 <li id="li_EB0B9D1CFDE24E6987935CCCBFC7892A">Approvals - publishing and approval status for new rules, data elements, and tools </li> 
 <li id="li_17B0B176FF85435FB7EDD4317BC18201">Property has been published </li> 
</ul> -->

## 프로필 및 암호 관리 {#task_7B89F4F38E5A4C4EB0FF842953856382}

Experience Cloud 프로필을 편집하고 기본 조직 및 랜딩 페이지 등을 지정할 수 있습니다.

1. Experience Cloud에 로그인.

1. Experience Cloud에서 프로필 사진을 선택합니다.

   ![](assets/edit-profile.png)
1. **[!UICONTROL 프로필 편집]**&#x200B;을 선택합니다.

   프로필 및 암호 페이지의 개인 세부 정보 아래의 필드 및 옵션을 작성합니다.

## 암호 복구 {#task_46541A2806164CB1A4AE8239604E4EB1}

1. 솔루션 로그인 페이지로 이동합니다.
1. **[!UICONTROL 암호를 잊으셨음]**&#x200B;을 선택합니다.

   솔루션 암호를 재설정하면 Experience Cloud에 대한 암호 연결 문제가 해결됩니다.

   Adobe Analytics 사용자의 경우 [https://sc2.omniture.com/password_recovery.html](https://sc2.omniture.com/password_recovery.html)로 이동합니다.

## 직접 연결되는 링크를 사용하여 솔루션 로그인 구성 {#concept_8BE493A08786469B88B210E13F78FF2F}

선택적으로, Experience Cloud 인터페이스에서 제공한 인증을 사용하여 솔루션의 특정 페이지에 로그인할 수 있습니다.

### URL 템플릿

`https://experience.adobe.com/#/@<tenantId>/<solutionname>?destURL=<fullURL>`

샘플 URL:

`https://experience.adobe.com/#/@aem62tenant/analytics?destURL=https%3A%2F%2Fsc.omniture.com%2Freports%2F11562.html`

>[!NOTE]
>
>URL을 `destURL` 매개 변수에 전달하기 전에 인코딩해야 합니다. ([URL Decoder / Encoder](https://meyerweb.com/eric/tools/dencoder/)와 같은 인코더 사이트를 이용할 수 있습니다.)

| 매개 변수 | 설명 | 예 | 필수/선택적 |
|--- |--- |--- |--- |
| `tenantId` | 사용자가 로그인해야 하는 테넌트의 이름입니다. | aem62tenant | 선택 사항입니다 |
| `destURL` | 사용자가 이동해야 하는 위치의 전체 URL입니다. | http://sc.omniture.com/login/?r=%2Fx%2F1_7xxzf&amp;tenantId=obuengsc&amp;company=OBU+Eng+SC | 선택 사항입니다 |
| `solutionname` | `destURL` 매개 변수의 소유자인 MAC 솔루션의 이름입니다. 사용자가 URL 소유자인 솔루션에 액세스할 수 있음을 확인하는 데 사용됩니다.  `solutionname`이 `destURL` 매개 변수와 동기화 상태임을 확인하는 것은 솔루션이 해야 하는 일입니다.  예를 들어, URL에 `solutionname`이 소셜로 포함되어 있고 제공된 `destURL`이 Analytics URL인 경우, 사용자가 Analytics에 액세스할 수 없는 경우에도 이 URL로 리디렉션됩니다. MAC은 `destURL`의 소유자가 솔루션 이름과 동기화 상태인지 여부를 확인하지 않습니다. | analytics | `destURL` 매개 변수가 사용되는 경우 필수입니다. |

{style=&quot;table-layout:auto&quot;}
