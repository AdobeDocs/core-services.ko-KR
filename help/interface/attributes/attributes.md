---
description: 고객 속성을 Experience Cloud에 업로드하는 방법에 대한 개요 및 사전 요구 사항.
keywords: core services;Customer Attributes
seo-description: 고객 속성을 Experience Cloud에 업로드하는 방법에 대한 개요 및 사전 요구 사항.
seo-title: 고객 속성
solution: Experience Cloud
title: 고객 속성
uuid: 1621402d-990f-46f9-981a-473280559069
translation-type: tm+mt
source-git-commit: 75d3d045964aa42f7ac6b32b25cfd77aa7f663a9
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 19%

---


# 사용자 특성

> **[!DNL Experience Platform]** 사람 **[!UICONTROL >]** 고객 속성 **[!UICONTROL 으로이동합니다.]**

CRM(고객 관계 관리) 데이터베이스에서 엔터프라이즈 고객 데이터를 캡처하는 경우, 이 데이터를 Experience Cloud의 고객 속성 데이터 소스에 업로드할 수 있습니다. 업로드했으면 [!DNL Adobe Analytics] 및 [!DNL Adobe Target]의 데이터를 활용합니다.

![](assets/custom_reports.png)

## 고객 속성을 업로드하기 위한 사전 요구 사항 {#section_BD38693AFBF34926BA28E964963B4EA0}

* **솔루션 활성화:** [경험 플랫폼 서비스에 대한 솔루션을 활성화합니다](../core-services/core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C).

* **그룹 멤버십:** 고객 속성 데이터를 업로드하려면 사용자가 [고객 속성 그룹의 구성원이어야 합니다](../admin-getting-started/admin-getting-started.md#task_3295A85536BF48899A1AB40D207E77E9). 또한 Adobe Analytics 그룹 또는 Adobe Target 그룹에 속해야 합니다.

   To know whether your company has access to Customer Attributes, your [!DNL Experience Cloud] administrator should log into the [Experience Cloud](https://experience.adobe.com). 관리 > **[!UICONTROL 관리]** **[!UICONTROL 콘솔]** > **[!UICONTROL 제품으로]**&#x200B;이동합니다. If *Customer Attributes* displays as one of the [!UICONTROL Product Profiles], you are ready to begin.

   Users that are added to the Customer Attributes will see the [!UICONTROL Customer Attributes] menu item on the left side of the Experience Cloud interface.

* **고객 속성에** Adobe Target [!DNL at.js] (모든 버전) 또는 [!DNL mbox.js] 버전 58 이상이 필요합니다.

   at.js 또는 [Mbox.js 구현](https://docs.adobe.com/content/help/en/target/using/implement-target/client-side/deploy-at-js/how-to-deployatjs.html) 배포 [방법을 참조하십시오](https://docs.adobe.com/content/help/ko-KR/target/using/implement-target/client-side/mbox-implement/mbox-download.html).

## What is enterprise customer data? {#section_6F34C29F11414842AA57D2B1248FA3C6}

엔터프라이즈 데이터는 다른 시스템에 있습니다. 그것은 복잡할 수 있고 다른 사람들에게 다른 것을 의미할 수 있습니다. 이 데이터에는 멤버십, 충성도 수준, 연령, 성별, 소유 제품, 관심사 및 라이프타임 값과 같은 정보가 포함될 수 있습니다.

다음 이미지는 멤버 ID, 권한 있는 제품, 가장 최근에 실행한 제품 등을 포함한 제품의 가입자 데이터를 보여주는 데이터 파일의 예입니다.

![](assets/01_crs_usecase.png)

After you create the data file, you can upload it to the customer attribute source that you create in **[!UICONTROL Experience Cloud]** > **[!UICONTROL Customer Attributes]**.

이 워크플로우에 대한 자세한 내용은 [고객 속성 데이터 업로드](../attributes/t-crs-usecase.md#task_BCC327B2A0EF4A1BBB2934013AB92B78)를 참조하십시오.

## 솔루션 사용 사례 {#section_4E77650F6CEE4C4ABCD0B3221A5AE5D9}

데이터가 Experience Cloud에 저장된 후 사용자 지정하여 보고, 세그멘테이션, 활동 및 캠페인을 위한 솔루션에 공유할 수 있습니다.

예:

| 솔루션 | 장점 및 사용 사례 |
|--- |--- |
| Adobe Analytics | 마케터와 분석가는 다음을 이해할 수 있습니다.<ul><li>골드 수준 고객에게 가장 효과적인 온라인 캠페인</li><li>Gold 수준 고객이 검색하는 제품과 Platinum 수준 고객이 검색하는 제품</li><li>사이트 재디자인이 이전 고객의 전환율에 긍정적인 영향을 미치는지 여부</li><li>낮은 라이프타임 값을 갖는 고객이 내 사이트에서 검색하는 제품은 무엇입니까?</li></ul> |
| Adobe Target | 속성 데이터를 통해 Adobe Target 사용자는 다음을 수행할 수 있습니다.<ul><li>충성도 클럽 회원에게 특별 할인 및 할인 혜택을 제공합니다.</li><li>고급 고객에게 더 비싼 제품을 추천합니다.</li><li>이미 이메일을 받은 고객의 경우 이메일 등록용으로 예약된 공간에 업셀링 오퍼를 표시합니다</li></ul> |
