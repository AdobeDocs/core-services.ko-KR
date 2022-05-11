---
description: Adobe Experience Cloud를 사용하는 관리자를 위한 브라우저 지원에 대해 알아보고, 일반적인 질문에 대한 답변을 얻을 수 있습니다.
keywords: 핵심 서비스, Experience Cloud, Experience Platform, Analytics, Target, 사용자 관리
solution: Experience Cloud
title: 'Experience Cloud FAQ '
index: true
feature: Admin Console
topic: Administration
role: Admin
level: Experienced
exl-id: 062576da-328e-4b46-9e71-5a25733d607a
source-git-commit: 8cb55c6fb6f0acfb8787b0125f7c4a25bcb71e28
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 100%

---

# Experience Cloud FAQ

Experience Cloud를 사용하는 관리자를 위한 브라우저 지원, 일반적인 질문과 답변을 살펴볼 수 있습니다.

## Experience Cloud에서 지원되는 브라우저는 무엇입니까?

* Microsoft® Edge (현재 및 이전의 두 버전)
* Google Chrome (현재 및 이전 두 버전)
* Mozilla Firefox (현재 및 이전 두 버전)
* Safari (현재 및 이전 두 버전)
* Opera (현재 및 이전 두 버전)

## 애플리케이션이 핵심 서비스에 대해 활성화되어 있는지 어떻게 알 수 있습니까?

핵심 서비스에 대한 구현이 제공되지 않은 경우, 다음 방법에 대해 설명하는 [핵심 서비스에 대한 애플리케이션 활성화](core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C)를 참조하십시오.

1. [Experience Cloud에 참여 및 관리자 되기](core-services.md#section_2423F0BD3DF642658103310EE5EA6154)
1. [Experience Platform Launch를 사용하여 Experience Cloud ID 서비스 구현](https://experienceleague.adobe.com/docs/experience-platform/tags/get-started/quick-start.html?lang=ko-KR)
1. [보고서 세트를 Experience Cloud 조직에 매핑](core-services.md#concept_apg_zq2_rw)
1. [(Analytics 전용) Analytics AppMeasurement 코드 현대화](core-services.md#section_1798D9D0F05C47E29816AC4EEB9A0913)
1. [(Adobe Target만 해당) Adobe Target 구현 현대화](core-services.md#section_C2F4493C7A36406DAE2266B429A4BD24)
1. [구현 확인](core-services.md#section_E641782A0F4F44AF8C9C91216BE330D5)
1. [사용자 및 제품 관리](core-services.md#section_B6E95F4E0E12483CB9DA99CBC0C5A4AF)
1. [핵심 서비스 사용 시작](core-services.md#section_960C06093623462E8EA247B3E97274A1)

추가적인 도움이 필요하면 [Adobe 지원 센터](https://experienceleague.adobe.com/?support-solution=General#support)에 문의하십시오.

## Adobe에서 우리 회사에 Experience Cloud 액세스를 위한 비용을 청구합니까?

아니요. Experience Cloud는 추가 비용 없이 포함됩니다. 그렇지만 특정 핵심 서비스에는 추가 비용이 있을 수 있습니다.

## 우리 회사에서 Experience Cloud 인터페이스를 통해 로그인해야 하는 이유는 무엇입니까?

Experience Cloud 인터페이스에서 제공하는 기능은 귀하의 비즈니스에 새로운 가치를 가져옵니다. 또한 향후 애플리케이션에 액세스하기 위한 표준 경로로 사용되며 결과적으로는 다른 개별 애플리케이션 로그인 흐름을 대체하게 됩니다. Experience Cloud를 통해 로그인하면 나중에 원활하게 전환할 수 있습니다.

## 우리 회사 마이그레이션에 대한 우려를 해결하려면 어떻게 해야 합니까?

[Adobe 지원 센터](https://experienceleague.adobe.com/?support-solution=General#support)에 문의하십시오.

## [!DNL Adobe Support]는 어떤 방식으로 내 Adobe 클라우드 환경에 액세스하여 문제를 해결합니까?

[!DNL Adobe Support]는 사용자의 명시적 인증을 요구하는 Adobe 브랜디드 이메일(아래 예)을 수신하는 가장 요청을 제출할 수 있습니다. 액세스 권한은 제한된 시간 동안 부여됩니다. 권한이 부여된 후 언제든지 해당 액세스 권한을 해지할 수 있습니다. Adobe는 Adobe 담당자가 수행한 모든 작업을 기록합니다.

![Adobe 지원 사례](assets/support-email.png)

## _프로비저닝이란_ 무엇입니까?

Experience Cloud의 프로비저닝은 다음을 의미합니다.

* 사용자는 [!DNL Experience Cloud]에 로그인하고 애플리케이션을 연결할 수 있습니다.
* 또한 Experience Cloud를 통해 사용자와 같은 기능을 사용할 수 있습니다.
* 애플리케이션별 로그인 프로세스의 사용을 중단할 준비를 갖출 수 있습니다.
* 애플리케이션에 대한 액세스 제어 권한은 그대로 유지할 수 있습니다.

## 사용자 및 제품 프로필을 관리하려면 어떻게 해야 합니까?

* 도움이 필요하면 [Admin Console 사용 안내서](https://helpx.adobe.com/kr/enterprise/admin-guide.html) 를 참조하십시오.

* 사용자 자격 및 제품 관리는 [Adobe Admin Console](https://adminconsole.adobe.com/enterprise)(제품 링크)에서 수행됩니다.

* **중요:** Analytics 관리자는 [Admin Console의 Analytics 사용자 관리](https://experienceleague.adobe.com/docs/analytics/admin/user-product-management/migrate-users/c-migration-tool.html?lang=ko-KR)에서 사용자 ID를 Analytics 관리 도구에서 Admin Console로 마이그레이션하는 작업에 대해 참조하십시오.

## Experience Cloud에 로그인할 수 없으면 어떻게 해야 합니까?

Admin Console 관리자는 사용자에게 액세스 권한을 부여할 수 있습니다. 사용자에게 로그인 지침이 포함된 이메일이 전송됩니다.

[Adobe 지원 센터에 문의](https://experienceleague.adobe.com/?support-solution=General#support) 하여 회사가 완전히 프로비저닝되었는지 확인해야 할 수 있습니다.

## 사용자가 계정 링크를 관리하려면 어디로 이동해야 합니까?

일부 사용자는 애플리케이션(Analytics) 계정을 Adobe ID 또는 Enterprise ID에 연결해야 할 수 있습니다.

[Adobe ID에 애플리케이션 계정 연결](organizations.md#task_FD389E78640848919E247AC5E95B8369)을 참조하십시오.

## 사용자 계정 프로필 및 조직을 관리하려면 어떻게 해야 합니까?

[사용자 계정 관리](organizations.md#topic_C31CB834F109465A82ED57FF0563B3F1)를 참조하십시오.

## 조직이란?

[](organizations.md) 조직은 관리자가 그룹과 사용자를 구성하고, Experience Cloud에서 SSO(Single Sign-On)를 제어할 수 있도록 하는 항목입니다. 조직은 모든 Experience Cloud 제품 및 애플리케이션을 포괄하는 로그인 회사와 같은 기능을 합니다. 대부분의 경우 조직은 회사 이름입니다. 그렇지만 한 회사에 여러 조직이 있을 수 있습니다.

## 내 IMS 조직 ID는 어디서 볼 수 있습니까?

자세한 내용은 [조직 ID 조회](organizations.md)를 참조하십시오.

## 사용자 중 한 명이 회사를 퇴사할 경우 어떻게 해야 합니까?

애플리케이션 자체에서 액세스 권한이 제거됩니다. 따라서 Experience Cloud에서 또는 직접 로그인을 통해 제품에 액세스할 수 없습니다. Experience Cloud 수준에서도 제거해야 합니다.

## Adobe ID란?

[ID 유형](https://helpx.adobe.com/kr/enterprise/using/identity.html)을 참조하십시오.

## 사용자의 애플리케이션 계정을 연결할 수 있습니까?

아니요. 사용자는 자체 애플리케이션을 사용자 이름 및 암호에 연결해야 합니다.

## 우리 회사에 Social이 없는데 내게 보이는 이유는 무엇입니까?

Adobe Social은 Analytics와 함께 판매할 수 있는 제품입니다. 따라서 Analytics가 있으면 이 애플리케이션이 보이지만 구입하지 않으면 액세스할 수 없습니다.
