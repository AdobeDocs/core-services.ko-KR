---
description: 데스크톱 및 모바일 브라우저에서 모든 쿠키를 차단한 사용자를 삭제하십시오. 이 개인 정보 설정은 Analytics 데이터 수집을 거부하는 사용자를 제외합니다.
keywords: cookies;privacy
seo-description: 데스크톱 및 모바일 브라우저에서 모든 쿠키를 차단한 사용자를 삭제하십시오. 이 개인 정보 설정은 Analytics 데이터 수집을 거부하는 사용자를 제외합니다.
seo-title: 브라우저 쿠키에 대한 개인 정보 설정 활성화
solution: Marketing Cloud,Adobe Analytics,Adobe Target,Adobe Social
title: 브라우저 쿠키에 대한 개인 정보 설정 활성화
uuid: f6a56e8b-b021-49db-8eb4-6c14af0c7243
translation-type: tm+mt
source-git-commit: f7ec8bf6087a18be41c9efbf05f60e6cfd24e566

---


# 브라우저 쿠키에 대한 개인 정보 설정 활성화{#enable-privacy-settings-for-browser-cookies}

데스크톱 및 모바일 브라우저에서 모든 쿠키를 차단한 사용자를 제거할 수 있습니다. 이 기능은 데이터 수집을 거부하는 사용자를 제외하는 개인 정보 설정으로서, 사용자는 분석 처리를 중단하려는 사용자의 의도를 유지할 수 있습니다.

**브라우저 쿠키에 대한 개인 정보 설정을 활성화하려면**

1. Navigate to **[!UICONTROL Admin Tools]** > **[!UICONTROL Report Suites]**.
1. Click **[!UICONTROL Edit Settings]** > **[!UICONTROL General]** > **[!UICONTROL Privacy Settings]**.
1. **[!UICONTROL 개인 정보 설정]**&#x200B;을 활성화합니다(데스크톱 또는 모바일의 경우).

>[!IMPORTANT]
>
>많은 모바일 앱(예: Facebook 또는 Twitter의 앱 내 브라우저)은 표준 모바일 브라우저로 표시될 수 있지만 모든 쿠키를 허용하지 않습니다. 이 기능을 활성화하면 모바일 트래픽의 비율이 Analytics 보고서에서 제외될 수 있습니다.

**브라우저 개인 정보 설정 정보**

법률 및 규제 지침에서는 쿠키를 차단하는 사용자의 행동은 프로파일링을 거부하는 사용자의 행동과 동일하다고 명시했습니다. 이 기능을 활성화하면 사용자가 브라우저에서 모든 쿠키를 차단하도록 설정한 데스크톱 브라우저에서 수집된 데이터는 Analytics 보고서에서 제외됩니다. Adobe가 웹 브라우저를 인식하지 못하는 경우 데이터는 Analytics 보고서에 포함됩니다.

전 세계의 입법자는 (지침과 결제 모두) 쿠키 브라우저 설정이 프로파일링을 거부하는 사용자 선호도를 나타내는 것이라고 명시했습니다. 특히, 이러한 의원들은 타사 쿠키를 차단하는 브라우저 설정이 타사(교차 사이트) 추적의 옵트아웃 요청이라고 말했습니다. 모든 쿠키를 차단하는 것은 모든 추적을 위한 옵트아웃 요청입니다. 서버측 식별자(예: IP 주소 또는 사용자 에이전트)는 쿠키 브라우저 설정을 우회하는 바람직한 옵션일 수 있지만 일부 의원은 사용자 선택을 우회하는 것으로 봅니다.