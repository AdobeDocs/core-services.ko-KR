---
description: Adobe Experience Cloud에서 업로드되고 사용되는 PII(개인 식별 정보)와 관련된 고려 사항 및 우수 사례입니다.
keywords: customer attributes;core services
seo-description: Adobe Experience Cloud에서 업로드되고 사용되는 PII(개인 식별 정보)와 관련된 고려 사항 및 우수 사례입니다.
seo-title: 개인 정보 고려 사항 - 고객 속성
solution: Experience Cloud
title: 개인 정보 고려 사항 - 고객 속성
uuid: 5666dc4e-55fa-4196-9985-cf530cfb9247
translation-type: tm+mt
source-git-commit: ae97db27349940a8df7ee2ba6678683f57585678

---


# 개인 정보 고려 사항 - 고객 속성

Adobe Experience Cloud에서 업로드되고 사용되는 PII(개인 식별 정보)와 관련된 고려 사항 및 우수 사례입니다.


<!-- <p>https://wiki.corp.adobe.com/display/omtrplatform/Visitor+Enrichment+and+privacy#VisitorEnrichmentandprivacy-INFORMATIONASSOCIATIONOPTIONS </p> -->


* 이름과 성
* 집 또는 기타 실제 주소
* 이메일 주소
* 전화 번호
* 사회 보장 번호
* 개인에게 실제로 또는 온라인으로 연결하도록 하는 기타 식별자 (위치마다 다릅니다. 비즈니스를 수행하는 모든 위치에 대한 개인 정보 및 PII와 관련된 현지 법률 및 규정을 확인하고 준수하십시오.)


Adobe는 광고주가 해당 사이트를 방문하거나 애플리케이션을 사용하는 소비자에 대한 행동 정보를 수집할 수 있는 도구를 제공합니다. 또한 광고주가 다른 정보 관리 시스템 내에서 유지할 수 있는 오프라인 또는 외부 고객 레코드로 이 정보를 개선할 수 있도록 합니다.

광고주가 이렇게 하는 한 가지 일반적인 이유는 소비자에게 적합한 마케팅 및 광고 결정을 내릴 때 사용할 수 있도록 이 정보를 개선하기 위해서입니다. Adobe Analytics 및 Target에서 광고주는 개인에게 연락하는 데 사용할 수 없도록 해시 처리한 후에만 전자 메일 주소와 같은 PII(개인 식별 정보)를 업로드할 수 있습니다. 해시 처리된 정보는 여전히 분석 및 마케팅 용도로 사용할 수 있습니다. 다시 말해서 Adobe는 광고주가 의료 기록, 금융 계좌 정보 및 미성년자에 대한 정보 등의 민감한 개인 정보를 Adobe에 보내지 못하게 합니다.

Adobe는 이러한 유형의 마케팅 및 광고 결정 시 고객 개인 정보를 고려할 수 있다는 것을 알고 있습니다. Adobe에서 광고주가 소비자의 기대를 충족하도록 도와주는 내장된 개인 정보 컨트롤을 제공하는 것도 바로 이러한 이유 때문입니다. Adobe는 광고주가 마케팅 목적으로 사용하기 적합한 정보를 고려하고 어떤 상황에서 광고주가 이러한 정보를 사용할 수 있는지 신중히 고려할 것을 권장합니다.

**우수 사례**

Adobe Analytics 또는 Target에 PII를 업로드할 때 고객은 PII를 해시 처리한 후 Adobe에 업로드하는 것이 좋습니다. 해시 처리된 정보는 여전히 분석 및 마케팅 용도로 사용할 수 있습니다. 다시 말해서 Adobe는 광고주가 의료 기록, 금융 계좌 정보 및 미성년자에 대한 정보 등의 민감한 개인 정보를 Adobe Analytics 및 Target에 보내지 못하게 합니다.

Adobe는 광고주가 마케팅 목적으로 사용하기 적합한 정보를 고려하고 어떤 상황에서 광고주가 이러한 정보를 사용할 수 있는지 신중히 고려할 것을 권장합니다.

소비자 개인 정보 관련 법률이 유동적이므로 Adobe는 광고주가 다음과 같은 세 가지 일반적인 원칙을 따를 것을 권장합니다.

1. 개인 정보 보호 정책에서 명시한 대로 행동합니다.
1. 개인 정보 보호 정책에서 수행하는 행동을 말합니다.
1. 소비자를 놀라게 하지 않도록 합니다.

이러한 점을 고려해서, Adobe는 광고주가 검색 활동을 PII에 연결할 때 소비자가 인증을 받았음을 나타내는 공지 또는 개인화 환경을 제공할 것을 권장합니다. 웹 사이트 제목 내의 인사말을 예로 들 수 있습니다. 또한 Adobe는 광고주가 PII에 연결하는 검색 정보 유형과 검색 정보가 PII에 연결되는 상황을 개인 정보 정책에 명시할 것을 권장합니다. 마지막으로 Adobe는 광고주가 소비자에게 제공하는 옵트아웃 선택 옵션을 검토하여 인증되지 않은 프로필 정보 게시물 옵트아웃을 사용할지 여부 및 사용하는 방법을 이해할 것을 강력히 권장합니다.

<!-- <p> <b>Vinay Geol</b> should help craft privacy regarding how all MAC uses privacy/cookies. Privacy implications around each part of the workflow. Moving from CRM to MAC. Can it include PII? What is PII? What isn't PII? </p> 
<p>CRM data is Known Data or Info. Going to combine with activity that occurs when visitor was not authenticated. PII wiki: </p> 
<p>https://wiki.corp.adobe.com/display/omtrplatform/Visitor+Enrichment+and+privacy#VisitorEnrichmentandprivacy-INFORMATIONASSOCIATIONOPTIONS </p> 
<p>Refactoring of implementation docs as it relates to privacy and cookies. </p> 
<p>Add content to t-publish-audience-segment, as follows: </p> 
<p> Audiences are not filtered based on the authentication state of a visitor. If a visitor can browse your site in un-authenticated and authenticated states, actions that occur when a visitor is un-authenticated can still cause a visitor to be included in an audience. Please review <link> to understand the full privacy implications of audience sharing. </p> 
<p>That "link" goes to a topic dedicated to PII, with this text: </p> 
<p> - Adobe Analytics allows its advertisers to upload personally identifiable information (PII) such as email addresses. When uploading PII to Adobe Analytics, Adobe recommends that the customer should hash PII prior to uploading it to Adobe. Hashed information can still be used for analysis and for marketing purposes. As a reminder, Adobe prohibits advertisers from sending sensitive personal information to Adobe Analytics, such as medical records, financial account information, and information about minors. </p> 
<p> - Adobe recommends its advertisers carefully consider which information is appropriate to use for marketing purposes and in which circumstances the advertiser has permission to use such information. </p> 
<p> - As consumer privacy law remains in flux, Adobe recommends that advertisers respect three common tenets: 1) Do what you say (in your privacy policy); 2) Say what you do (in your privacy policy); and 3) Don't surprise your consumers. </p> 
<p> - With these expectations in mind, Adobe recommends that when an advertiser associates browsing activities to PII, the advertiser provide notices/personalization indicating that the consumer is authenticated. An example of this is including a 'Hello, Jane' greeting within the header of the website. Adobe also recommends that advertisers describe in its privacy policy what type of browsing information it associates with PII and under what circumstances browsing information is associated with PII. Lastly, Adobe strongly recommends advertisers review the opt out choices they provide their consumers to understand whether and how they can use unauthenticated profile information post opt out. </p> 
<p>Possibly revamp the cookies to include privacy, with best practices: https://docs.adobe.com/content/help/en/core-services/interface/ec-cookies/cookies-privacy.html </p> -->
