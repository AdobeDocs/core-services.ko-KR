---
title: Customer Attributes Support for California Consumer Privacy Act
description: Customer Attributes Support for California Consumer Privacy Act
translation-type: tm+mt
source-git-commit: 8709449909ce4fbd441d77fb4bbfb0b7758e805d
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 4%

---


# California Consumer Privacy Act에 대한 고객 속성 지원

이 페이지에서는 CPA(California Consumer Privacy Act)에 대한 [!UICONTROL 고객 속성] 지원에 대해 설명합니다.

>[!IMPORTANT]
>
>이 문서의 내용은 법률적인 조언이 아니며, 법률적인 조언을 대체하지 않습니다. (CPA)에 대한 법률 자문을 구할 수 있습니다.

CPA는 2020년 1월 1일에 발효되는 캘리포니아 주의 새로운 개인 정보 보호법입니다. CPA는 캘리포니아 주민들에게 그들의 개인 정보에 대한 새로운 권리를 제공하고 캘리포니아에서 사업을 하는 특정 업체들에 데이터 보호 책임을 부과합니다. CPA는 소비자에게 개인 정보를 액세스하고 삭제할 수 있는 권한과 제3자에게 &quot;개인 정보 판매&quot;의 자격이 되는 특정 활동을 거부할 수 있는 권한을 제공합니다.

기업은 Adobe Experience Cloud가 귀하를 대신하여 처리하고 저장하는 개인 데이터를 결정합니다.

Adobe Experience Cloud는 서비스 제공업체로서, 개인 정보에 액세스하거나 삭제하기 위한 요청을 관리하는 것을 비롯하여 Experience Cloud 제품 및 서비스 사용에 적용되는 CPA에 따른 책임을 이행하도록 비즈니스를 지원합니다.

이 문서에서는 Adobe Experience Platform Privacy Service API 및 Privacy Service UI를 사용하여  고객 속성이 데이터 주체의 CPA 데이터 액세스 및 삭제 권한을 지원하는 방법에 대해 설명합니다.

CPA용 Adobe 개인정보 보호 서비스에 대한 자세한 내용은 [Adobe 개인정보 보호 센터를 참조하십시오](https://www.adobe.com/privacy/ccpa.html).

## 고객 속성에 대한 요청을 전송하는 데 필요한 [!UICONTROL 설정]

고객 속성에 대한 데이터에 액세스하고 삭제를 요청하려면 [!UICONTROL 다음을 수행해야]합니다.

1. 다음을 확인합니다.

   * IMS 조직 ID
   * 작업을 수행하려는 CRS 데이터 소스의 별칭 ID
   * 작업할 프로필의 CRM ID
   IMS 조직 ID는 @AdobeOrg와 함께 추가된 24자 영숫자 문자열입니다. 마케팅 팀이나 내부 Adobe 시스템 관리자가 조직의 IMS 조직 ID를 모르는 경우 Adobe 고객 지원 센터(gdprsupport@adobe.com)에 문의하십시오. 개인 정보 API에 요청을 제출하려면 IMS 조직 ID가 필요합니다.

1. 개인정보 [!UICONTROL 보호 서비스에서]고객 속성에 액세스 및 삭제 요청을 제출하고 기존 요청의 상태를 확인할 수 있습니다.

## JSON 요청에 [!UICONTROL 필요한] 필드 값

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

* &quot;규제&quot;: **ccpa** (요청에 적용되는 개인정보 보호 규정)

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
