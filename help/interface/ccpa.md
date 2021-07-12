---
title: '캘리포니아 소비자 개인 정보 보호법을 위한 고객 속성 지원 '
description: 캘리포니아 소비자 개인 정보 보호법을 위한 고객 속성 지원에 대해 알아보기
feature: 고객 속성
topic: 관리
role: Admin
level: Experienced
exl-id: 320defc7-2cd5-4481-955d-77cf6fbfef6d
source-git-commit: 1fb1abc7311573f976f7e6b6ae67f60ada10a3e7
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 100%

---

# 캘리포니아 소비자 개인 정보 보호법을 위한 고객 속성 지원

이 페이지에서는 CPA(캘리포니아 소비자 개인 정보 보호법)에 대한 [!UICONTROL 고객 속성] 지원에 대해 설명합니다.

>[!IMPORTANT]
>
>이 문서의 콘텐츠는 법률적인 조언이 아니며, 법률적인 조언을 대체하지 않습니다. (CCPA)에 대한 법률 자문을 구하십시오.

CCPA는 2020년 1월 1일에 발효되는 캘리포니아 주의 새로운 개인 정보 보호법입니다. CCPA는 캘리포니아 주민에게 개인 정보에 대한 새로운 권리를 제공하고 캘리포니아에서 사업을 하는 특정 업체들에 데이터 보호 책임을 부과합니다. CCPA는 개인 정보를 액세스하고 삭제할 수 있는 권한을 비롯하여 서드파티에 대한 개인 정보 “판매” 자격이 되는 특정 활동을 거부할 수 있는 권한을 소비자에게 제공합니다.

기업은 Adobe Experience Cloud가 기업을 대신하여 처리하고 저장하는 개인 데이터를 결정합니다.

서비스 제공업체로서 Adobe Experience Cloud는 귀사가 Experience Cloud 제품 및 서비스 사용에 적용되는 CCPA에 따른 의무를 이행할 수 있도록 지원을 제공합니다. 이 지원에는 개인 정보 액세스 및 삭제 요청 관리가 포함됩니다.

이 문서에서는 [!UICONTROL 고객 속성]이 Adobe Experience Platform Privacy Service API 및 Privacy Service UI를 사용하여 데이터 주체의 CCPA 데이터 액세스 및 삭제 권한을 지원하는 방법에 대해 설명합니다.

CCPA를 위한 Adobe 개인정보보호 서비스에 대한 자세한 내용은 [Adobe 개인정보보호 센터](https://www.adobe.com/privacy/ccpa.html)를 참조하십시오.

## [!UICONTROL 고객 속성]에 대한 요청을 전송하기 위한 필수 설정

[!UICONTROL 고객 속성]에 대한 데이터에 액세스하고 삭제를 요청하려면 다음을 수행해야 합니다.

1. 다음을 확인합니다.

   * IMS 조직 ID
   * 작업을 수행하려는 CRS 데이터 소스의 별칭 ID
   * 작업할 프로필의 CRM ID

   IMS 조직 ID는 @AdobeOrg가 추가된 24자 영숫자 문자열입니다. 마케팅 팀이나 내부 Adobe 시스템 관리자가 조직의 IMS 조직 ID를 모르는 경우에는 Adobe 고객 지원 센터(gdprsupport@adobe.com)에 문의하십시오. Privacy API에 요청을 제출하려면 IMS 조직 ID가 필요합니다.

1. [!UICONTROL 개인정보보호 서비스]에서 고객 속성에 액세스 및 삭제 요청을 제출하고 기존 요청의 상태를 확인할 수 있습니다.

## [!UICONTROL 고객 속성 ]JSON 요청의 필수 필드 값

&quot;company context&quot;:

* &quot;namespace&quot;: **imsOrgID**
* &quot;value&quot;: &lt;*IMS 조직 ID 값*>

&quot;users&quot;:

* &quot;key&quot;: &lt;*일반적으로 고객의 이름*>

* &quot;action&quot;: **access** 또는 **delete**

* &quot;user IDs&quot;:

   * &quot;namespace&quot;: &lt;*CRS 데이터 소스의 별칭 ID*>

   * &quot;type&quot;: **integrationCode**

   * &quot;value&quot;: &lt;*CRM ID*>

* &quot;include&quot;: **CRS**(요청에 적용되는 Adobe 제품)

* &quot;regulation&quot;: **ccpa**(요청에 적용되는 개인정보 보호 규정)

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
