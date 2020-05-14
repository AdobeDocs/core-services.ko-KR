---
title: 일반 데이터 보호 규정에 대한 고객 속성 지원
description: 일반 데이터 보호 규정에 대한 고객 속성 지원
translation-type: tm+mt
source-git-commit: 4223f9260865756842ad43b99d2509908f4d6572
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---


# 일반 데이터 보호 규정에 대한 고객 속성 지원

이 페이지에서는 고객 속성이 일반 데이터 보호 규정(GDPR)을 지원하는 방법을 설명합니다.

>[!IMPORTANT]
>
>이 문서의 내용은 법률적 자문을 위한 것이 아니며, 법률적 자문을 대체하기 위한 것이다. GDPR에 대한 법률 자문을 구할 수 있습니다.

2018년 5월 25일부터 적용되는 [일반 데이터 보호](https://www.adobe.com/privacy/general-data-protection-regulation/what-is-gdpr.html)규정은 유럽 연합(EU)의 국경 내의 모든 개인(데이터 주체)에게 개인 데이터를 통제하도록 규정하고 있습니다. 또한 국제 비즈니스를 위한 규정 환경을 간소화합니다. 이 법은 데이터 관리자의 비즈니스 위치에 상관없이 개인 데이터를 처리할 때 EU의 경계 내에서 개인 데이터를 수집하거나, 행동을 감시하거나, 개인 데이터를 수집하는 모든 기업(데이터 관리자)에 적용됩니다.

Adobe Experience Cloud는 고객을 대신하여 수령하여 보관하는 모든 개인 데이터의 데이터 프로세서 역할을 합니다. 데이터 관리자는 Adobe Experience Cloud가 대신 처리하고 저장하는 개인 데이터를 결정합니다.

이 문서에서는  고객 속성이 Adobe Experience Platform 개인 정보 보호 서비스 API 및 개인 정보 서비스 UI를 사용하여 데이터 주체의 GDPR 데이터 액세스 및 삭제 권한을 지원하는 방법에 대해 설명합니다.

GDPR의 비즈니스 의미에 대한 자세한 내용은 [GDPR 및 비즈니스를 참조하십시오](https://www.adobe.com/kr/privacy/general-data-protection-regulation.html).

## 고객 속성에 대한 요청을 전송하는 [!UICONTROL 필수 설정]

고객 속성에 대한 데이터에 액세스하고 삭제를 요청하려면 [!UICONTROL 다음을 수행해야]합니다.

1. 다음을 확인합니다.

   * IMS 조직 ID
   * 작업을 수행하려는 CRS 데이터 소스의 별칭 ID
   * 작업할 프로필의 CRM ID
   IMS 조직 ID는 @AdobeOrg와 함께 추가된 24자 영숫자 문자열입니다. 마케팅 팀이나 내부 Adobe 시스템 관리자가 조직의 IMS 조직 ID를 모르는 경우 Adobe 고객 지원 센터(gdprsupport@adobe.com)에 문의하십시오. 개인 정보 API에 요청을 제출하려면 IMS 조직 ID가 필요합니다.

1. 개인정보 [!UICONTROL 보호 서비스에서]고객 속성에 액세스 및 삭제 요청을 제출하고 기존 요청의 상태를 확인할 수 있습니다.

## 고객 속성 JSON [!UICONTROL 요청의 필수 필드] 값

&quot;회사 컨텍스트&quot;:

* &quot;namespace&quot;: **imsOrgID**
* &quot;value&quot;: &lt;*귀하의 IMS 조직 ID 값*>

&quot;사용자&quot;:

* &quot;key&quot;: &lt;*보통 고객*&#x200B;이름>

* &quot;action&quot;: 액세스 **또는** **삭제**

* &quot;사용자 ID&quot;:

   * &quot;namespace&quot;: &lt;*CRS 데이터 소스의 별칭 ID*>

   * &quot;type&quot;: **integrationCode**

   * &quot;value&quot;: &lt;*CRM ID*>

* &quot;include&quot;: **CRS** (요청에 적용되는 Adobe 제품)

* &quot;규제&quot;: **gdpr** (요청에 적용되는 개인 정보 보호 규정)

## JSON 요청의 예

```
{
  "companyContexts": [
    {
      "namespace": "imsOrgID",
      "value": "<IMS_ORG_ID>"
    }
  ],
  "users": [
    {
      "key": "<KEY>",
      "action": [
        "<access/delete>"
      ],
      "userIDs": [
        {
          "namespace": "<Alias ID of CRS Data Source>",
          "type": "integrationCode",
          "value": "<CRM ID>"
        }
      ]
    }
  ],
  "regulation": "<gdpr/ccpa/pdpa>",
  "include": [
    "CRS"
  ]
}
```

## 액세스 요청을 위해 반환된 데이터 필드

```
attributes:
{
"value”:<*value*>,
"key”:<*key*>,
"displayName”:<*displayName*>
}
```
