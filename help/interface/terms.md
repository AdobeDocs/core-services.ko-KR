---
description: Adobe Experience Cloud의 용어와 Experience Cloud 및 Creative Cloud 용어의 차이점에 대해 알아봅니다.
solution: Experience Cloud
title: 용어
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 3799f806-2794-43ab-9e70-06ee693871e7
source-git-commit: eb2ad8a8255915be47b6002a78cc810b522170d2
workflow-type: tm+mt
source-wordcount: '1445'
ht-degree: 100%

---

# 용어

Experience Cloud 사용자를 위한 용어 참조 및 Creative Cloud에서 그러한 용어를 사용하는 방법을 설명합니다(해당하는 경우).

| 용어 | Creative Cloud | Experience Cloud |
|--- |----- |---- |
| 에셋 | Creative Cloud에서 에셋은 일반적으로 이미지 파일입니다.<br>에셋은 Photoshop 파일의 레이어, PowerPoint 파일의 슬라이드, PDF의 페이지, ZIP에 들어 있는 파일일 수 있습니다. | Experience Cloud에서 에셋은 디지털 문서, 이미지, 비디오 또는 오디오 파일로, 다양한 렌디션과 하위 에셋을 가질 수 있습니다. 해당 예는 다음과 같습니다.<ul><li>파일</li><li>문서</li><li>이미지</li><li>비디오</li><li>오디오 클립</li><li>프레젠테이션</li><li>이미지 템플릿</li><li>비디오 템플릿</li></ul> |
| 속성 |  | 사람들이 [세그먼트](https://experienceleague.adobe.com/docs/analytics/components/segmentation/seg-home.html?lang=ko-KR)에 대한 자격이 되는 경우 공통으로 가지는 사항. (Audience Manager의 [트레이트](https://experienceleague.adobe.com/docs/audience-manager/user-guide/aam-glossary.html?lang=ko-KR)와 비슷합니다.) |
| Audiences | Creative Cloud에서 대상은 비디오를 보는 사람이 될 수 있습니다. | Experience Cloud에서 대상이란 사용자가 캠페인 활동에서 타기팅할 수 있는 사람의 컬렉션을 의미합니다.<br>대상의 멤버십은 방문자의 컨텍스트에 따라 작동하는 규칙 세트 또는 고정된 목록을 기반으로 결정할 수 있습니다. Facebook 그룹의 이메일 가입자 또는 멤버 목록을 예로 들 수 있습니다.<br> [Experience Cloud Audiences](audience-library.md)에서 대상을 만들고 관리하는 것은 Experience Cloud에 공유하는 기능을 추가하여 세그먼트를 만들고 사용하는 것과 비슷합니다.<br>**Adobe Target**<br> Adobe Target에서 대상은 이전에 세그먼트라고 불렀습니다.<br>**Adobe Analytics**<br> Analytics에서 대상은 웹 사이트 방문자로 생각할 수 있습니다. 대상 세그먼트를 만들고 대상을 Experience Cloud에 게시할 수 있습니다. |
| 캠페인 | Creative Cloud에서, 캠페인은 Creative Cloud 이미지 에셋을 사용하는 마케팅 캠페인으로 생각할 수 있습니다. | Experience Cloud에서 캠페인은 대상에 표시되는 콘텐츠 내용을 결정합니다. 콘텐츠가 표시되는 위치와 시기도 결정합니다. 캠페인에는 특정 목표가 있으며, 지표로 목표를 추적합니다.<br>캠페인을 실행하기 위해서는 캠페인의 규칙 세트와 방문자의 컨텍스트가 일치해야 하고, 위치 채널의 기술적 제한에 따른 콘텐츠 배달이 필요합니다.<br>Adobe Target에서 캠페인과 활동이라는 용어는 동의어입니다. |
| 채널 | Creative Cloud에서 채널은 서로 다른 유형의 정보를 저장하는 회색 음영 이미지일 수 있습니다. 정보 채널과 색상 채널이 있습니다. | Experience Cloud에서, 채널은 위치 속성이나 캠페인에 있는 활동입니다.<br>Analytics에서 마케팅 채널은 이메일 캠페인 방식 등 일반적으로 방문자가 사이트에 도착하는 방식에 대한 통찰력을 제공하는 데 사용됩니다.<br>해당 예는 다음과 같습니다.<ul><li>이메일</li><li>디스플레이 광고</li><li>소셜 네트워크</li><li>유료 검색</li><li>자연어 검색</li><li>참조 도메인</li></ul> |
| 컨텍스트 | 일반적으로 수행되는 선택 또는 작업에 따라 사용할 수 있는 메뉴 또는 정보를 나타냅니다. | 컨텍스트는 디지털 속성에 대한 방문자의 현재 상호 작용에 대한 세부 사항을 설명합니다. 컨텍스트의 예에는 마우스 위치, 양식 필드의 상태, 장바구니의 값 또는 사용하고 있는 디바이스가 포함됩니다.<br>[Dynamic tag management](https://experienceleague.adobe.com/docs/experience-platform/tags/home.html?lang=ko-KR)는 현재 시장에서 가장 강력한 컨텍스트 탐지 및 서비스 활성화 기능을 제공하며 프로필 및 대상 서비스의 컨텍스트 구성 요소를 제공합니다. |
| 소비자 ID | 특별한 용도는 없습니다. | Experience Platform Co-op 그래프 멤버가 개인을 인식하는 데 사용하는 ID. 이 번호는 브랜드에 의해 지정되며 종종 CRM 시스템에 유지됩니다. **참고:** 이 ID를 _setCustomerIDs_(소비자 ID를 Experience Cloud로 보내는 [Experience Cloud ID 서비스](https://experienceleague.adobe.com/docs/id-service/using/intro/about-id-service.html?lang=ko-KR) 기능 호출)와 혼동하지 마십시오. |
| 콘텐츠 | Creative Cloud에서 콘텐츠는 페이지의 텍스트 및 이미지를 나타냅니다. 이 용어는 Creative와 Experience Cloud 간에 유사하게 사용됩니다. | Experience Cloud에서 콘텐츠는 구체적 목표를 지원하기 위해 캠페인의 일부로 사용할 수 있는 마케팅 콘텐츠를 참조하며,<br>특정 위치에 사용되고 에셋으로 구성될 수 있습니다. 콘텐츠는 제품 정보처럼 구조화하거나, 모바일 애플리케이션의 화면 또는 웹 페이지처럼 구조화하지 않을 수 있습니다.<br>해당 예는 다음과 같습니다.<ul><li>웹 페이지</li><li>배너</li><li>상태 업데이트</li><li>주석</li><li>텍스트 광고</li><li>제품 정보</li><li>제품 평가</li><li>양식 데이터</li><li>검색 색인의 문서</li><li>소셜 게시물</li><li>기사</li><li>발행물</li></ul> |
| 대시보드 | 특별한 용도는 없습니다. | 하나의 보기에서 여러 주요 지표를 나타내는 데이터 시각화 컬렉션입니다. |
| 데이터 사용 적용 | 특별한 용도는 없습니다. | 데이터 사용 시 Adobe 기업 개인정보 보호정책, 계약 고려 사항 및 일반 개인정보 보호 원칙을 준수할 수 있도록 데이터 사용 메타데이터를 사용하기 위해 시스템(애플리케이션, 앱, 서비스, SDK, API 등)을 통해 제정되고 정의된 정책, 시스템 디자인, 관행 및 절차. |
| 디바이스 | 특별한 용도는 없습니다. | 애플리케이션이 실행되는 태블릿, 휴대폰 또는 데스크탑 등의 하드웨어 디바이스. |
| Device Co-op | 특별한 용도는 없습니다. | 디바이스 간에 개인을 더 잘 식별하고 더 의미 있고 일관된 환경을 제공하기 위해 소비자가 사용하는 디바이스에 대한 데이터를 공유하는 데 동의한 브랜드 그룹. |
| [!UICONTROL Experience Cloud ID 서비스] (ECID) | 특별한 용도는 없습니다. | 사이트 방문자에게 지정된 고유한 영구 ID. Experience Platform ID 서비스에서 사용할 수 있는 특정 엔티티입니다. [자세히...](https://experienceleague.adobe.com/docs/id-service/using/home.html?lang=ko-KR) |
| [!UICONTROL Experience Platform ID 서비스] | 특별한 용도는 없습니다. | ID를 연결하는 서비스입니다. 사람 기반의 경험 관리를 위한 디바이스 연결 서비스입니다. |
| 연결 | 특별한 용도는 없습니다. 연결은 하이퍼링크 탐색 및 글꼴, 속성, 레이어 등의 항목 연결을 나타냅니다. | Experience Cloud에서 연결은 일반적으로 서로 다른 애플리케이션 계정을 인터페이스에 연결하는 것을 말합니다.<br> [조직 및 계정 연결](organizations.md)을 참조하십시오.<br>또한 다른 사용자에게 전송된 Analytics 보고서에 대한 표준 URL을 연결이라고도 합니다. |
| 위치 | Creative Cloud에서 위치는 파일 위치 또는 열린 이미지나 문서의 위치를 나타냅니다. | Experience Cloud에서 위치는 대상이 콘텐츠를 보고 상호 작용할 수 있는 장소입니다. 위치와 콘텐츠 간의 연관성이 다소 정적이거나 캠페인 규칙에 따라 동적으로 관리할 수 있습니다. 위치는 콘텐츠를 배달할 수 있는 방법 및 지표를 수집할 수 있는 방법을 결정하는 특정 채널에 항상 속합니다.<br>해당 예는 다음과 같습니다.<ul><li>사이트</li><li>속성(소셜)</li><li>인벤토리 표시</li><li>랜딩 페이지</li><li>모바일 애플리케이션</li><li>슬롯(비디오)</li></ul> |
| 지표 | Creative Cloud에서 사용되지 않습니다. | 주요 개념 및 목표에 대한 숫자들을 집계합니다. Analytics에서 지표는 보기 수, 선택 횟수, 다시 로드 횟수, 평균 체류 시간, 판매량, 주문 수, 매출액 등과 같은 방문자 활동에 대한 수량 정보입니다. |
| 조직 | Creative Cloud에서 사용되지 않습니다. | 조직은 관리자가 사용자와 제품을 구성하고 Experience Cloud에서 SSO(Single Sign-On)를 제어할 수 있도록 해 주는 Experience Cloud 엔티티입니다. 대부분의 경우, 조직은 청구 회사입니다. |
| 포트폴리오 | 여러 파일 또는 에셋의 어셈블리입니다. | 캠페인 컨테이너. |
| 제품 프로필 | [제품 및 프로필 관리](https://helpx.adobe.com/kr/enterprise/using/manage-products.html)를 참조하십시오. | 사용자가 제품 또는 서비스에 대한 이용 자격을 충족하려면 사용자가 제품 프로필의 일부여야 합니다. 제품 관리자는 사용자가 구입한 플랜과 연결하여 제품 프로필에 라이선스를 지정합니다.<br>사용자는 여러 제품 프로필에 속할 수 있으며 각각 사용자에게 서로 다른 라이선스가 부여됩니다. 사용자의 최종 자격 요건은 해당 사용자에게 각 제품 프로필로 제공된 모든 라이선스의 통합입니다. |
| 예약 | Adobe Story의 장면 시퀀스 또는 ColdFusion의 예약된 작업일 수 있습니다. | Experience Cloud에서 예약은 캠페인, 채널 및 활동 활성화의 시작 날짜(연, 월, 일) 및 종료 날짜입니다. 활동 예약에는 분 단위까지의 세부기간이 있습니다. 예약을 변경하면 카드가 만들어집니다.<br>해당 예는 다음과 같습니다.<ul><li>캠페인 예약</li><li>채널 예약</li><li>활동 예약</li></ul> |
| 세그먼트 | N/A | 대상을 평가하는 규칙 세트의 출력입니다. Analytics에서 원할 경우 [세그먼트](https://experienceleague.adobe.com/docs/analytics/components/segmentation/seg-home.html?lang=en) 를 사용하여 Experience Cloud에 전달할 수 있는 대상을 정의할 수 있습니다. <br>Audience Manager에서 세그먼트는 방문자의 멤버십 자격 또는 해당 세그먼트에 포함할 수 있는 자격을 부여하는 [트레이트](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/traits/traits-overview.html?lang=ko-KR) 및 모든 기준의 컬렉션입니다. 또한 이러한 공통적인 속성을 공유하는 사람들의 컬렉션이기도 합니다. |
| 공유 | Creative Cloud에서는 플랫폼 간에 외부적으로 파일을 공유할 수 있습니다(소셜, 커뮤니티, 이메일 등). | Experience Cloud에서 인터페이스 내의 보드 안에서 에셋을 카드로만 공유할 수 있습니다. 사이트에 로그인한 사람은 공유를 사용할 수 있습니다. |
| 솔루션 | 특별한 용도는 없습니다. | Experience Cloud에서 애플리케이션은 Adobe Analytics, Adobe Social, Adobe Target 등과 같은 제품으로 알려져 있습니다. |
| 트레이트 | 해당 없음 | 키-값 쌍(예:color=blue)입니다. Audience Manager에서 [트레이트](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/traits/traits-overview.html?lang=en)는 세그먼트를 만드는 데 사용됩니다. |

{style=&quot;table-layout:auto&quot;}
