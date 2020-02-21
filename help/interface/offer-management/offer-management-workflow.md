---
description: 배치 및 오퍼 만들기, 오퍼 활동 삽입, 보고서 보기 등 오퍼 관리의 고급 워크플로우를 살펴봅니다.
seo-description: 배치 및 오퍼 만들기, 오퍼 활동 삽입, 보고서 보기 등 오퍼 관리의 고급 워크플로우를 살펴봅니다.
seo-title: 오퍼 관리 워크플로우
title: 오퍼 관리 워크플로우
uuid: c95ec474-88de-4e6e-92bf-f49f3a7b32c5
index: y
internal: n
snippet: y
translation-type: tm+mt
source-git-commit: 2f0c2eb70313c42da9e7ac1d75429ec768dea10d

---


# 오퍼 관리 워크플로우{#offer-management-workflow}

배치 및 오퍼 만들기, 오퍼 [!UICONTROL 활동 삽입], 보고서 보기 등 오퍼 관리의 고급 워크플로우를 살펴봅니다.

## 1단계 - 이메일 템플릿에서 개인화된 오퍼가 필요한 위치를 결정합니다. {#section_F184E589428B403EA8EB921BF230CF87}

개인화된 제안을 삽입할 이메일 캠페인을 식별합니다. 여기에서 이러한 오퍼를 삽입할 이메일 템플릿 내의 위치를 결정합니다. 예를 들어 고객의 업계나 성향에 따라 제품 오퍼를 수정하고, 동일한 기준을 기반으로 메시지를 변경하고, 고객의 지역에 따라 이미지를 변경할 수 있습니다.

![](assets/workflow1.png)

## 2단계 - 타깃팅할 Campaign의 속성을 결정하고 오퍼 관리와 공유합니다. {#section_1461F1FAC0B943E5BBDED6B3B00E9D5C}

오퍼 관리에서 오퍼를 만들 [!UICONTROL 때]특정 오퍼를 수신할 수 있는 프로파일을 제한하는 자격 규칙을 설정할 수 있습니다. 이러한 자격 조건 규칙은 Adobe Campaign에 존재하는 속성(또는 필드)을 기반으로 설정할 수 있습니다. 이 필드는 관리 수준 사용자가 오퍼 관리 자격 조건 규칙 빌더에 표시되기 전에 Campaign에서 공유해야  합니다.

이러한 속성 공유에 대한 자세한 내용은 캠페인에서 [오퍼 관리로 속성 공유를 참조하십시오](campaign.md#task_4DFA9A20D7B04E1F9AFF4774D67B6EBC).

## 3단계 - 오퍼 관리에 필요한 [!UICONTROL 배치를 입력합니다]{#section_71619756A86F4DB58B8200D8A1CE1B87}

배치는 올바른 오퍼 컨텐츠가 이메일 템플릿 내의 올바른 위치에 표시되도록 합니다. 오퍼에 컨텐츠를 추가할 때 해당 컨텐츠를 표시할 배치를 선택하라는 메시지가 표시됩니다.

동일한 배치를 가진 여러 위치를 가질 수 있습니다. 다음 예에서는 두 개의 서로 다른 크기 이미지에 대한 두 개의 배치와 템플릿의 위쪽과 아래쪽에 표시되는 텍스트에 대한 한 개의 배치가 있습니다.

필요한 배치를 결정하면 배치 탭에 추가할 수 [!UICONTROL 있습니다] .

![](assets/workflow2.png)

## 4단계 - 오퍼 만들기 {#section_C4F9732B0596425EB0BD5AE76E4BA6EF}

이메일 캠페인에 사용할 오퍼를 만듭니다. 제공할 최적의 오퍼를 결정하고 표시할 컨텐츠를 결정하기 위해 오퍼에 추가할 수 있는 데이터와 컨텐츠가 있습니다. 컨텐츠 표현을 만들 때 배치(Placement)에 정의된 배치 중 하나에 [연결합니다](placements.md). 오퍼를 만들고 제출하면 오퍼 활동에서 사용할 수 있습니다.

![](assets/workflow3.png)

## 5단계 - 이메일 캠페인을 만들고 오퍼 활동을 삽입합니다. {#section_6FD36404759B4C6E9FD3A65ACABB26C8}

오퍼를 만들었으므로 이메일 캠페인에서 사용할 수 있습니다. 컨텐츠 편집기에서 블록을 선택하고 오퍼 활동을 삽입할 수 있습니다. 오퍼 활동을 사용하면 오퍼 재고에서 오퍼 그룹을 선택할 수 있으며, 이 그룹에서 의사 결정 엔진에서 각 사용자에게 제공할 최상의 오퍼를 결정할 수 있습니다.

![](assets/workflow4.png)

## 6단계 - 이메일 캠페인 준비 및 보내기 {#section_EDD8EA4696664130A678D7C4483DA806}

이제 이메일 캠페인을 준비하면 [!UICONTROL 오퍼] 관리에서 현재 날짜, 프로필 속성 및 우선 순위를 기준으로 각 방문자에게 제공할 최상의 오퍼를 결정합니다. 또한 해당 위치의 배치에 사용할 수 있는 컨텐츠 표현이 있는지 여부를 결정합니다.

다음 예에서는 3개의 오퍼(A, B, C)가 포함된 오퍼 활동이 있는 이메일 캠페인을 설정했다고 가정합니다. 이메일의 위치 중 하나에서 제공할 오퍼를 결정할 수 있습니다. 준비 시 오퍼 [!UICONTROL 관리에서] 다음을 수행합니다.

1. 현재 날짜, 각 사용자의 프로필 데이터 및 우선 순위를 분석합니다.
1. 해당 정보를 오퍼의 데이터와 비교합니다.
1. 최적의 제안 결정

![](assets/workflow5.png)

## 7단계 - 보고서 보기 {#section_2104BAACAE154DE29B6EEB967C46F226}

제공된 오퍼와 오퍼 활동에서 오퍼가 수행되는 방식에 대한 보고서를 볼 수 있습니다. 이 보고서는 Adobe Campaign Standard 홈 페이지에서 보고서 탭을 선택하여 볼 수 있습니다.