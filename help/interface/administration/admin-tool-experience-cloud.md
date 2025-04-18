---
title: 사용자 및 사용자 세부 정보 보기
description: Experience Cloud의 관리 도구에 대해 알아봅니다. 모든 Experience Cloud 사용자 및 정책의 정렬과 필터링 가능한 목록을 봅니다.
application: Experience Cloud
index: true
feature: Admin Console
topic: Administration
role: Admin
level: Experienced
exl-id: 127eecdd-3862-48ba-8cf6-a8082d2b7bae
source-git-commit: 163dc8ef83fb83a0e51879520bcb3ae697c95144
workflow-type: tm+mt
source-wordcount: '1258'
ht-degree: 82%

---

# [!UICONTROL 관리 도구]에서 Experience Cloud 사용자 및 정책 보기

관리자는 [!UICONTROL 관리 도구]에서 모든 Experience Cloud 사용자 및 정책을 세부 정보와 함께 정렬 및 필터링 가능한 목록으로 볼 수 있습니다. 사용자 세부 정보에는 사용자의 제품 액세스, 역할 및 마지막으로 액세스한 정보가 포함됩니다. 정책 세부 사항에는 정책의 (제품 프로필) 사용자, 그룹, 개발자, 통합 및 관리 목록과 정책에 대한 자세한 권한 및 리소스 정보가 포함됩니다.

1. `https://experience.adobe.com/.`에 로그인합니다.

   ![Admin Console에 액세스](../assets/admin-tool.png)

1. [!UICONTROL 빠른 액세스]에서 **[!UICONTROL 관리 도구]**&#x200B;를 클릭합니다.

   (또는 홈 페이지 URL에서 _home_ 을 _admin_&#x200B;으로 바꿀 수 있습니다.)

   [!UICONTROL 사용자] 페이지가 표시됩니다.

## 사용자 페이지

이 페이지에는 조직에서 Experience Cloud에 액세스할 수 있는 전체 사용자 목록이 표시됩니다. 여기에서는 애플리케이션 권한 및 마지막 로그인에 대한 정보가 제공됩니다. 사용자 목록을 검색, 정렬 및 필터링하여 요구에 맞게 표시할 수 있습니다.

![Admin Console 사용자 페이지](../assets/admin-tool-users.png)

| 요소 | 설명 |
|---|---|
| [!UICONTROL 이름] | 사용자의 이름과 성씨를 입력합니다. 이 열을 A에서 Z로 또는 Z에서 A로 정렬할 수 있습니다. 사용자에 대한 자세한 내용을 보려면 사용자 이름을 클릭하십시오. |
| [!UICONTROL 이메일] | 사용자와 연결된 이메일 주소입니다. 열은 A->Z, Z->A로 정렬할 수 있습니다. |
| [!UICONTROL ID 유형] | 사용자 계정의 ID 유형입니다. 특정 ID 유형이 표시되도록 필터를 적용할 수 있습니다. 자세한 내용은 [ID 유형 관리](https://helpx.adobe.com/kr/enterprise/using/identity.html) 를 참조하십시오. |
| [!UICONTROL 솔루션] | 사용자가 액세스할 수 있는 Experience Cloud 애플리케이션 요약입니다. 특정 애플리케이션 액세스 권한으로 사용자 목록의 범위를 좁히는 필터를 적용할 수 있습니다. |
| [!UICONTROL 마지막 로그인] | Experience Cloud에 최근 사용자가 로그인한 시간 및 날짜입니다. 이 열은 오름차순 또는 내림차순 날짜로 정렬할 수 있습니다. <br> **중요:** 2020년 1월 13일부터 사용자의 마지막 로그인 데이터는 365일 동안 유지됩니다. 이 정보는 Experience Cloud의 현재 로그인 활동을 표시하기 위한 것으로, 2020년 1월 13일 이전에 비활성 계정에 대해 조치를 취하기 위한 권장 사항은 아닙니다. |

## 사용자 목록 보기 사용자 지정

열을 검색, 정렬 또는 필터링하여 사용자 목록을 사용자 지정할 수 있습니다.

* 이름 또는 이메일로 사용자를 검색합니다. 입력한 텍스트 문자열과 일치하는 항목을 찾는 검색입니다.
* 오름차순 또는 내림차순 값으로 열을 정렬합니다. 이 정렬은 [!UICONTROL 이름,] [!UICONTROL 이메일] 및 [!UICONTROL 마지막 로그인] 열에 적용됩니다.
* 특정 기준을 가진 사용자 목록에 여러 필터를 적용하려면 **[!UICONTROL 필터링 기준]**&#x200B;을 클릭하세요. 여러 필터 카테고리가 적용될 때에는 검색에 이메일 도메인 `AND` ID 유형 `AND` 솔루션이 포함됩니다.

| 요소 | 설명 |
|---------|----------|
| [!UICONTROL 이메일 도메인] 필터 | 이메일 열에서 문자 문자열을 검색하여 결과를 하나 또는 여러 도메인으로 좁힐 수 있습니다. 각 검색어 뒤에 Enter 키를 눌러 여러 필터 추가하십시오. |
| [!UICONTROL ID 유형] 필터 | 사용 가능한 ID 유형 중에서 선택합니다. 여러 ID 유형을 필터로 사용할 수 있습니다. |
| [!UICONTROL 솔루션] 필터 | 사용 가능한 애플리케이션 중에서 선택합니다. 여러 애플리케이션 필터가 솔루션 1 `OR` 솔루션 2가 포함된 결과를 검색합니다. |

## 사용자 세부 사항 보기

[!UICONTROL 사용자] 페이지에서 사용자의 세부 사항을 보려면 사용자 이메일을 클릭하십시오.

![Admin Console의 사용자 세부 정보 보기](../assets/admin-tool-user-details.png)

각 사용자의 상세 보기에는 사용자의 애플리케이션 액세스, 관리자 및 제품 역할 및 마지막으로 액세스한 정보에 대한 중요한 세부 사항이 표시됩니다.

## 섹션에 대하여

이 섹션에는 다음과 같은 사용자 계정 요약이 표시됩니다.

* 사용자 아바타 및 시스템 관리 배지(해당되는 경우)
* 이름
* 이메일
* 사용자 이름(Federated ID 계정의 사용자 이름은 이메일 주소와 다를 수 있음)
* [ID 유형](https://helpx.adobe.com/kr/enterprise/using/identity.html)
* 국가
* 마지막 로그인

## 솔루션 요약

이 섹션에는 사용자가 액세스할 수 있는 Experience Cloud 애플리케이션 요약이 표시됩니다. 해당되는 경우 제품 관리 역할을 포함합니다.

## 자세한 제품 액세스 목록

이 섹션에는 사용자의 모든 제품 프로필 멤버십에 대한 전체 목록이 표시됩니다.

| 요소 | 설명 |
|---------|----------|
| [!UICONTROL 제품] | 제품 프로필과 연관된 제품의 이름입니다. |
| [!UICONTROL 인스턴스] | 제품 및 제품 프로필과 연관된 인스턴스(로그인 회사 또는 테넌트 등)의 이름입니다. |
| [!UICONTROL 제품 프로필] | 제품 프로필의 고유 이름입니다. |
| [!UICONTROL 지정 기준 그룹] | 사용자를 제품 프로필에 연결하는 사용자 그룹의 이름입니다. 빈 결과는 사용자가 그룹을 통해서가 아니라 제품 프로필에 직접 지정되었음을 나타냅니다. |
| [!UICONTROL 제품 역할] | 제품 프로필 내에서 사용자의 역할 지정합니다. 현재 이 정보는 Adobe Target 제품 프로필에만 적용됩니다. |

## 정책 페이지

이 페이지에는 조직의 전체 Experience Cloud 정책 목록이 표시됩니다. 제품, 인스턴스, 사용자 및 개발자에 대한 정보를 제공합니다. 정책 목록을 검색, 정렬 및 필터링하여 요구에 맞게 표시할 수 있습니다.

![Admin Console의 정책 페이지](../assets/admin-tool-policies.png)

| 요소 | 설명 |
|---|---|
| [!UICONTROL 제품 프로필] | 제품 프로필의 이름입니다. 열은 A->Z, Z->A로 정렬할 수 있습니다. 정책에 대한 자세한 정보를 보려면 제품 프로필의 이름을 선택하십시오. |
| [!UICONTROL 제품] | 제품 프로필과 연관된 제품입니다. 열은 A->Z, Z->A로 정렬할 수 있습니다. |
| [!UICONTROL 인스턴스] | 제품 프로필과 연계된 인스턴스(예: 테넌트 또는 로그인 회사)입니다. 고유 인스턴스 또는 테넌트가 없는 제품은 값에 &quot; - &quot;를 표시합니다. 열은 A->Z, Z->A로 정렬할 수 있습니다. |
| [!UICONTROL 사용자 수] | 직접 할당 및 그룹 할당을 포함하여 제품 프로필과 연결된 사용자의 고유 수입니다. 열은 가장 작은 항목에서 가장 큰 항목순으로 또는 가장 큰 항목에서 가장 작은 항목순으로 정렬할 수 있습니다. |
| [!UICONTROL 개발자 수] | 제품 프로필과 연관된 개발자 역할 수입니다. 열은 가장 작은 항목에서 가장 큰 항목순으로 또는 가장 큰 항목에서 가장 작은 항목순으로 정렬할 수 있습니다. |

## 정책 목록 보기 사용자 지정

열을 검색, 정렬 또는 필터링하여 정책 목록을 사용자 지정할 수 있습니다.

* 이름별로 제품 프로필을 검색합니다. 입력한 텍스트 문자열과 일치하는 항목을 찾는 검색입니다.
* 오름차순 또는 내림차순 값으로 열을 정렬합니다. 이 정렬은 [!UICONTROL 제품 프로필,] [!UICONTROL 제품,] [!UICONTROL 인스턴스,] [!UICONTROL 사용자 수,] 및 [!UICONTROL 개발자 수,] 열에 적용됩니다.
* 다양한 필터를 적용하여 제품 프로필을 특정 기준으로 나열하려면 **[!UICONTROL 필터 기준]** 아이콘을 클릭합니다. 여러 필터 카테고리가 적용되면 검색에 그룹 연관 `AND` 인스턴스 `AND` 솔루션이 포함됩니다.

| 요소 | 설명 |
|---------|----------|
| [!UICONTROL 인스턴스] 필터 | 인스턴스 열에서 문자 문자열을 검색하여 결과를 하나 또는 여러 인스턴스로 좁힐 수 있습니다. 각 검색어 뒤에 Enter 키를 눌러 여러 필터를 추가하십시오. |
| [!UICONTROL 솔루션] 필터 | 사용 가능한 애플리케이션 중에서 선택합니다. 여러 애플리케이션 필터가 솔루션 1 `OR` 솔루션 2가 포함된 결과를 검색합니다. |

## 정책 세부 사항 보기

[!UICONTROL 정책] 페이지에서 정책의 세부 사항을 보려면 제품 프로필 이름을 선택합니다.

![Admin Console의 정책 세부 정보 보기](../assets/admin-tool-policy-detail.png)

각 제품 프로필에 대한 세부 보기에는 제품 프로필의 주제(사용자, 그룹 등)에 대한 중요한 세부 정보가 표시됩니다. 제품 프로필에서 활성화한 권한 및 리소스도 표시합니다.

제품 프로필의 세부 사항을 CSV 파일로 내보낼 수 있습니다. [!UICONTROL CSV 내보내기] 옵션을 사용하면 두 개의 CSV 파일이 생성됩니다.

* 제목 세부 정보(사용자, 사용자 그룹, 개발자, 통합, 관리자)
* 권한 및 리소스 항목

## 요약 섹션

이 섹션에는 다음과 같은 제품 프로필 요약이 표시됩니다.

* 제품 프로필 이름
* 사용자 수
* 개발자 수
* 통합 수
* 관련 제품
* 인스턴스

## 자세한 제목 목록

이 섹션에는 제품 프로필에 할당된 모든 사용자, 사용자 그룹, 개발자, 통합 및 관리자의 전체 목록이 표시됩니다.

| 탭 | 설명 |
|---------|----------|
| [!UICONTROL 사용자] | 제품 프로필에 포함된 사용자 목록입니다. 사용자 그룹 연결이 [!UICONTROL 그룹별로 할당됨] 열에 나타납니다. |
| [!UICONTROL 사용자 그룹] | 제품 프로필과 연결된 사용자 그룹 목록입니다. |
| [!UICONTROL 개발자] | 제품 프로필과 연결된 개발자 목록입니다. |
| [!UICONTROL 통합] | 제품 프로필과 연결된 통합 목록입니다. |
| [!UICONTROL 관리자] | 제품 프로필과 연결된 관리자 목록입니다. |

## 자세한 권한 및 리소스 목록

이 섹션에는 제품 프로필에 사용할 수 있는 권한 및 리소스의 전체 목록이 표시됩니다. 제품 프로필에 포함된 권한 및 리소스는 &quot;✔&quot;으로 표시되었습니다. 권한 및 리소스 목록은 탭 및 열로 분류되어 쉽게 볼 수 있습니다. 탭과 열에는 현재 제품에 적용되는 섹션 목록이 표시됩니다.

## 관련 정보

* [!DNL Admin Console]의 [사용자 관리](https://helpx.adobe.com/kr/enterprise/using/users.html)