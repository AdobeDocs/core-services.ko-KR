---
description: 모든 Experience Cloud 사용자에 대한 목록을 정렬 가능하고 필터링 가능한 목록으로 보려면 Experience Cloud 관리 도구에 대해 알아보십시오.
keywords: core services
seo-description: 모든 Experience Cloud 사용자에 대한 목록을 정렬 가능하고 필터링 가능한 목록으로 보려면 Experience Cloud 관리 도구에 대해 알아보십시오.
seo-title: Experience Cloud 사용자 및 사용자 세부 사항 보기
solution: Experience Cloud
title: 'Experience Cloud 사용자 및 사용자 세부 사항 보기 '
index: true
translation-type: ht
source-git-commit: 43de353155c640b3ddc519147c94d7e9ffcafe4e
workflow-type: ht
source-wordcount: '693'
ht-degree: 100%

---


# 관리 도구에서 Experience Cloud 사용자 보기

관리자는 관리 도구에서 모든 Experience Cloud 사용자 목록과 세부 사항을 정렬 및 필터링 가능한 목록으로 볼 수 있습니다. 사용자 세부 정보에는 사용자의 제품 액세스, 역할 및 마지막으로 액세스한 정보가 포함됩니다. (**참고:** 사용자 및 제품 관리는 [Admin Console](admin-getting-started.md)에서 구성됩니다.)

1. `https://experience.adobe.com/.`에 로그인합니다.

   ![](assets/admin-tool.png)

1. Experience Cloud 홈에서 **[!UICONTROL 관리 도구]**&#x200B;를 클릭합니다.

   (또는 홈 페이지 URL에서 _home_&#x200B;을 _admin_&#x200B;으로 바꿀 수 있습니다.)

   [!UICONTROL 사용자] 페이지가 표시됩니다.

## 사용자 페이지

이 페이지에는 조직에서 Experience Cloud에 액세스할 수 있는 전체 사용자 목록이 표시됩니다. 여기에서는 솔루션 권한 및 마지막 로그인에 대한 정보가 제공됩니다. 사용자 목록을 검색, 정렬 및 필터링하여 요구에 맞게 표시할 수 있습니다.

![](assets/admin-tool-users.png)

| 요소 | 설명 |
|---|---|
| [!UICONTROL 이름] | 사용자의 이름과 성씨를 입력합니다. 이 열을 A에서 Z로 또는 Z에서 A로 정렬할 수 있습니다. 사용자에 대한 자세한 내용을 보려면 사용자 이름을 클릭하십시오. |
| [!UICONTROL 이메일] | 사용자와 연결된 이메일 주소입니다. 열은 A->Z, Z->A로 정렬할 수 있습니다. |
| [!UICONTROL ID 유형] | 사용자 계정의 ID 유형입니다. 특정 ID 유형이 표시되도록 필터를 적용할 수 있습니다. 자세한 내용은 [ID 유형 관리](https://helpx.adobe.com/kr/enterprise/using/identity.html)를 참조하십시오. |
| [!UICONTROL 솔루션] | 사용자가 액세스할 수 있는 Experience Cloud 솔루션 요약입니다. 특정 솔루션 액세스 권한으로 사용자 목록의 범위를 좁히는 필터를 적용할 수 있습니다. |
| [!UICONTROL 마지막 로그인] | Experience Cloud에 최근 사용자가 로그인한 시간 및 날짜입니다. 이 열은 오름차순 또는 내림차순 날짜로 정렬할 수 있습니다. <br> **중요:** 2020년 1월 13일부터 사용자의 마지막 로그인 데이터는 365일 동안 보관됩니다. 이 정보는 Experience Cloud의 최근 로그인 활동을 표시하기 위한 것으로서, 2020년 1월 13일 이전에 비활성 계정에 대해 조치를 취하기 위한 권장 사항은 아닙니다. |

## 사용자 목록 보기 사용자 지정

열을 검색, 정렬 또는 필터링하여 사용자 목록을 사용자 지정할 수 있습니다.

* 이름 또는 이메일로 사용자를 검색합니다. 입력한 텍스트 문자열과 일치하는 항목을 찾는 검색입니다.
* 오름차순 또는 내림차순 값으로 열을 정렬합니다. 이 방법은 [!UICONTROL 이름,] [!UICONTROL 이메일,] 및 [!UICONTROL 마지막 로그인] 열에 적용됩니다.
* 다양한 필터를 적용하여 사용자를 특정 기준으로 나열하려면 **[!UICONTROL 필터 기준]** 아이콘을 클릭합니다. 여러 필터 카테고리가 적용될 때에는 검색에 이메일 도메인 `AND` ID 유형 `AND` 솔루션이 포함됩니다.

| 요소 | 설명 |
|---------|----------|
| [!UICONTROL 이메일 도메인] 필터 | 이메일 열에서 문자 문자열을 검색하여 결과를 하나 또는 여러 도메인으로 좁힐 수 있습니다. 각 검색어 뒤에 Enter 키를 눌러 여러 필터 추가하십시오. |
| [!UICONTROL ID 유형] 필터 | 사용 가능한 ID 유형 중에서 선택합니다. 여러 ID 유형을 필터로 사용할 수 있습니다. |
| [!UICONTROL 솔루션] 필터 | 사용 가능한 솔루션 중에서 선택합니다. 여러 솔루션 필터가 솔루션 1 `OR` 솔루션 2가 포함된 결과를 검색합니다. |

## 사용자 세부 사항 보기

[!UICONTROL 사용자] 페이지에서 사용자의 세부 사항을 보려면 사용자 이메일을 클릭하십시오.

![](assets/admin-tool-user-details.png)

각 사용자의 상세 보기에는 사용자의 솔루션 액세스, 관리자 및 제품 역할 및 마지막으로 액세스한 정보에 대한 중요한 세부 사항이 표시됩니다.

## 섹션에 대하여

이 섹션에는 다음과 같은 사용자 계정 요약이 표시됩니다.

* 사용자 아바타 및 시스템 관리 배지(해당되는 경우)
* 이름
* 이메일
* 사용자 이름(Federated ID 계정의 사용자 이름이 이메일 주소와 다를 수 있음)
* [ID 유형](https://helpx.adobe.com/kr/enterprise/using/identity.html)
* 국가
* 마지막 로그인

## 솔루션 요약

이 섹션에는 사용자가 액세스할 수 있는 Experience Cloud 솔루션 요약이 표시됩니다. 해당되는 경우 제품 관리 역할을 포함합니다.

## 자세한 제품 액세스 목록

이 섹션에는 사용자의 모든 제품 프로필 멤버십에 대한 전체 목록이 표시됩니다.

| 요소 | 설명 |
|---------|----------|
| [!UICONTROL 제품] | 제품 프로필과 연관된 제품의 이름입니다. |
| [!UICONTROL 인스턴스] | 제품 및 제품 프로필과 연관된 인스턴스(로그인 회사 또는 테넌트 등)의 이름입니다. |
| [!UICONTROL 제품 프로필] | 제품 프로필의 고유 이름입니다. |
| [!UICONTROL 지정 기준 그룹] | 사용자를 제품 프로필에 연결하는 사용자 그룹의 이름입니다. 빈 결과는 사용자가 그룹을 통해서가 아니라 제품 프로필에 직접 지정되었음을 나타냅니다. |
| [!UICONTROL 제품 역할] | 제품 프로필 내에서 사용자의 역할 지정합니다. 현재 이 정보는 Adobe Target 제품 프로필에만 적용됩니다. |
