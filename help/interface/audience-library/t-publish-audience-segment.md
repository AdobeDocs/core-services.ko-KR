---
description: 대상 마케팅 활동을 위해 Analytics 대상 세그먼트를 Experience Cloud 및 Adobe Target에 게시합니다.
keywords: 핵심 서비스
seo-description: 대상 마케팅 활동을 위해 Analytics 대상 세그먼트를 Experience Cloud 및 Adobe Target에 게시합니다.
seo-title: Analytics 대상 세그먼트 게시
solution: Experience Cloud
title: Analytics 대상 세그먼트 게시
uuid: 4201 DC 22-4 B 79-457 C-A 614-949 BBA 087617
translation-type: tm+mt
source-git-commit: 85879d92104d8b6d739fb4d17dc8cfb7483a9343

---


# Analytics 대상 세그먼트 게시

대상 마케팅 활동을 위해 Analytics 대상 세그먼트를 Experience Cloud 및 Adobe Target에 게시합니다.

1. Analytics에서 [세그먼트 만듭니다](https://marketing.adobe.com/resources/help/en_US/analytics/segment/seg_build.html).
1. 세그먼트 빌더에서 Make this **[!UICONTROL Experience Cloud Audience]** 옵션을 활성화합니다.

   ![](assets/ec_audience_example.png)

   | 요소 | 설명 |
   |--- |---|
   | Experience Cloud 대상으로 지정(&lt;보고서 세트 이름&gt;용) | 이 세그먼트를 Experience Cloud에 게시합니다. Adobe Target의 마케팅 활동 및 Audience Manager의 세그멘테이션을 위해 대상을 사용할 수 있습니다.<br>세그먼트를 게시하려면 제목 및 설명 필드가 필요합니다.<br>이 옵션이 활성화되면 제목 및 대상 세그먼트 정의가 공유되지만 실제 데이터는 공유되지 않습니다. 해당 대상이 Target의 활동과 연결되면 Analytics에서는 해당 Experience Cloud 및 Target 대상의 자격을 규정하는 방문자용 ID를 전송하기 시작합니다. 이때 대상 이름 및 해당 데이터가 Experience Cloud 대상 페이지에 표시되기 시작합니다.<br>Analytics에서 Experience Cloud로 공유한 대상은 2,000만 명의 대상 구성원을 초과할 수 없습니다.<br>캐싱으로 인해, Analytics에서 삭제된 보고서 세트는 삭제가 Experience Cloud에 표시되기 12 시간이 되어야 합니다.<br>Analytics에서 게시된 세그먼트를 편집하거나 삭제할 수 있습니다. 세그먼트가 사용 중인 경우 세그먼트를 편집할 때 경고 메시지가 표시됩니다. 게시된 세그먼트가 Adobe Target에서 사용 중이면 삭제할 수 없습니다.<br>방문자가 Analytics에서 공유한 대상에 대한 자격을 갖추면 Target, Advertising Cloud 및 Campaign에서 해당 정보를 실행 가능한 24 - 48 시간이 지연됩니다.<br>**데이터 Privacyaudience**<br>는 방문자의 인증 상태에 따라 필터링되지 않습니다. 방문자가 인증되지 않음 및 인증됨 상태의 사이트를 검색할 수 있는 경우 방문자가 인증되지 않음 상태일 때 발생하는 작업 때문에 여전히 방문자가 대상에 포함될 수 있습니다. 대상을 공유할 때 파생되는 전반적인 개인 정보 문제를 이해하려면 [Analytics 개인 정보 개요](https://marketing.adobe.com/resources/help/en_US/reference/?f=c_Privacy_Overview)를 검토하십시오. |
   | 대상을 만들기 위한 창 선택 | 이것은 고정된 시간 창이 아니라 **롤링** 시간 창입니다. |

1. **[!UICONTROL 저장을 클릭합니다]**.
1. 액세스 [!DNL Adobe Target], [!UICONTROL 대상을 클릭합니다].
1. [!UICONTROL 대상] 페이지에서 Experience Cloud에서 소스 소스를 찾습니다.

   이러한 대상은 활동에서 사용할 수 있습니다.
