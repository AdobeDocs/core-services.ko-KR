---
title: "[!DNL Customer Attributes] 개인 정보 보호 규정 지원"
description: 개인정보 보호 규정을 위한 고객 속성 지원에 대해 알아봅니다.
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 02417c0c-6780-4699-9470-f1685c3cd25d
source-git-commit: f229ec33ff721527e6a4c920ea63eabb4102935a
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 77%

---

# [!DNL Customer Attributes] 개인정보 보호 규정 지원

이 페이지에서는 다음 방법에 대해 설명합니다. [!DNL Customer Attributes] 는 일반 데이터 보호 규정(GDPR)을 지원합니다.

>[!IMPORTANT]
>
>이 문서의 콘텐츠는 법률적인 조언이 아니며, 법률적인 조언을 대체하지 않습니다. GDPR에 대한 법률 자문을 구하십시오.

2018년 5월 25일부터 적용되는 [개인정보 보호 규정](https://business.adobe.com/privacy/general-data-protection-regulation.html)은 유럽 연합(EU)의 국경 내의 모든 개인(데이터 주체)이 개인 데이터를 통제하도록 규정하고 있습니다. 또한 국제 비즈니스를 위한 규정 환경을 간소화합니다. 이 법은 데이터 관리자의 비즈니스 위치에 상관없이 개인 데이터를 처리할 때 EU의 경계 내에서 개인 데이터를 수집하거나, 행동을 모니터링하거나, 개인 데이터를 수집하는 모든 기업(데이터 관리자)에 적용됩니다.

Adobe Experience Cloud는 고객을 대신하여 수신하여 보관하는 모든 개인 데이터에 대한 데이터 처리자의 역할을 합니다. 귀하는 정보 통제자로서 Adobe Experience Cloud가 귀하를 대신하여 처리하고 저장하는 개인 데이터를 결정합니다.

이 문서에서는 다음 방법을 설명합니다 [!DNL Customer Attributes] 는 Adobe Experience Platform Privacy Service API 및 Privacy Service UI를 사용하여 데이터 주체의 GDPR 데이터 액세스 및 삭제 권한을 지원합니다.

GDPR의 비즈니스 의미에 대한 자세한 내용은 [GDPR 및 비즈니스](https://business.adobe.com/privacy/general-data-protection-regulation.html)를 참조하십시오.

## 다음에 대한 요청을 전송하기 위한 필수 설정 [!DNL Customer Attributes]

다음에 대한 데이터에 액세스하고 삭제를 요청하려면 [!DNL Customer Attributes], 다음을 수행해야 합니다.

1. 다음 항목을 확인하십시오.

   * [조직 ID](#organizations.md)
   * 작업을 수행하려는 CRS 데이터 소스의 별칭 ID
   * 작업할 프로필의 CRM ID

   [조직 ID](#organizations.md)는 @AdobeOrg가 추가된 24자 영숫자 문자열입니다. Privacy API에 요청을 제출하려면 조직 ID가 필요합니다. ID를 찾을 수 없는 경우 Adobe 고객 지원 센터(`gdprsupport@adobe.com`)에 문의하십시오.

1. 위치 [!UICONTROL Privacy Service]에 액세스 및 삭제 요청을 제출할 수 있습니다. [!DNL Customer Attributes]을 클릭하고 기존 요청의 상태를 확인합니다.

## 의 필수 필드 값 [!DNL Customer Attributes] JSON 요청

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

* &quot;regulation&quot;: **gdpr**(요청에 적용되는 개인정보 보호 규정)

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
"value":<*value*>,
"key":<*key*>,
"displayName":<*displayName*>
}
```
