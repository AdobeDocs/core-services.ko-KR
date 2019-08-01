---
description: 대상 마케팅 활동을 위해 Analytics 대상 세그먼트를 Experience Cloud 및 Adobe Target에 게시합니다.
keywords: 핵심 서비스
seo-description: 대상 마케팅 활동을 위해 Analytics 대상 세그먼트를 Experience Cloud 및 Adobe Target에 게시합니다.
seo-title: Analytics 대상 세그먼트 게시
solution: Experience Cloud
title: Analytics 대상 세그먼트 게시
uuid: 4201dc22-4b79-457c-a614-949bba087617
translation-type: tm+mt
source-git-commit: b74e0a08b43dfa8e5b35c5a650d159a58485883c

---


# Analytics 대상 세그먼트 게시

대상 마케팅 활동을 위해 Analytics 대상 세그먼트를 Experience Cloud 및 Adobe Target에 게시합니다.

1. Analytics에서 [세그먼트 만듭니다](https://marketing.adobe.com/resources/help/en_US/analytics/segment/seg_build.html).
1. On the Segment Builder, enable the **[!UICONTROL Publish this segment to the Experience Cloud]** option.

   ![](assets/ec_audience_example.png)

   | 요소 | 설명 |
   |--- |---|
   | 이 세그먼트를 Experience Cloud에 게시 (&lt; 보고서 세트 이름 &gt; 용) | 이 세그먼트를 Experience Cloud에 게시합니다. Adobe Target, Audience Manager, Advertising Cloud, Campaign 및 고객 분석의 마케팅 및 세그멘테이션 활동에 고객을 사용할 수 있습니다.<br>세그먼트를 게시하려면 제목 및 설명 필드가 필요합니다.<br>이 옵션이 활성화되면 제목 및 대상 세그먼트 정의가 공유되지만 실제 데이터는 공유되지 않습니다. 해당 대상이 Target의 활동과 연결되면 Analytics에서는 해당 Experience Cloud 및 Target 대상의 자격을 규정하는 방문자용 ID를 전송하기 시작합니다. 이때 대상 이름 및 해당 데이터가 Experience Cloud 대상 페이지에 표시되기 시작합니다.<br>Analytics에서 Experience Cloud로 공유하는 대상은 2천만 명의 대상 구성원을 초과할 수 없습니다.<br>캐싱으로 인해, Analytics에서 삭제된 보고서 세트는 삭제가 Experience Cloud에 표시되는 데 12시간이 필요합니다.<br>Experience Cloud에 게시된 세그먼트를 삭제하려면 먼저 게시 취소해야 합니다. To unpublish a segment, just **unclick** the checkbox that you used to publish it. You **cannot** unpublish a segment that is currently in use by any of the following Adobe solutions: [!DNL Analytics] (in [!DNL Audience Analytics]), [!DNL Campaign], [!DNL Advertising Cloud] (for [!DNL Core Service] &amp; [!DNL Audience Manager] customers) and all other external partners (for [!DNL Audience Manager] customers). You **can** unpublish a segment that is in use by [!DNL Target].<br>방문자가 Analytics에서 공유한 대상 자격을 얻으면 24~48시간이 지연된 후에 Target, Advertising Cloud 및 Campaign에서 정보를 실행할 수 있습니다.<br>**데이터 개인 정보**<br>대상은 방문자의 인증 상태에 따라 필터링되지 않습니다. 방문자가 인증되지 않음 및 인증됨 상태의 사이트를 검색할 수 있는 경우 방문자가 인증되지 않음 상태일 때 발생하는 작업 때문에 여전히 방문자가 대상에 포함될 수 있습니다. 대상을 공유할 때 파생되는 전반적인 개인 정보 문제를 이해하려면 [Analytics 개인 정보 개요](https://marketing.adobe.com/resources/help/en_US/reference/?f=c_Privacy_Overview)를 검토하십시오. |
   | 대상을 만들기 위한 창 선택 | 이것은 고정된 시간 창이 아니라 **롤링** 시간 창입니다. |

1. **[!UICONTROL 저장을 클릭합니다]**.
1. [!DNL Adobe Target]에 액세스하여 [!UICONTROL 대상]을 클릭합니다.
1. [!UICONTROL 대상] 페이지에서 Experience Cloud에서 가져온 대상을 찾습니다.

   이러한 대상은 활동에서 사용할 수 있습니다.
