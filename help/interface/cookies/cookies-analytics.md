---
description: Adobe Analytics는 쿠키를 사용하여 서로 다른 브라우저의 요청을 구분하고 응용 프로그램이 나중에 사용할 수 있도록 유용한 정보를 저장합니다. 또한 쿠키는 탐색 정보를 고객 기록과 연결하는 데 사용되기도 합니다.
keywords: cookies;privacy
seo-description: Adobe Analytics는 쿠키를 사용하여 서로 다른 브라우저의 요청을 구분하고 응용 프로그램이 나중에 사용할 수 있도록 유용한 정보를 저장합니다. 또한 쿠키는 탐색 정보를 고객 기록과 연결하는 데 사용되기도 합니다.
seo-title: Analytics 쿠키
solution: Marketing Cloud,Analytics,Target,Social
title: Analytics 쿠키
uuid: e2d3d61d-2708-48b2-a7e6-2331f2aed8e0
index: y
internal: n
snippet: y
translation-type: ht
source-git-commit: f59badcd3423ada51a3fe0c605158a009d5b1d64

---


# Analytics 쿠키{#analytics-cookies}

Adobe Analytics는 쿠키를 사용하여 서로 다른 브라우저의 요청을 구분하고 응용 프로그램이 나중에 사용할 수 있도록 유용한 정보를 저장합니다. 또한 쿠키는 탐색 정보를 고객 기록과 연결하는 데 사용되기도 합니다.

특히 Analytics는 쿠키를 사용하여 새 방문자를 익명으로 정의하고 클릭스트림 데이터를 분석하며 특정 캠페인이나 구매 주기 길이에 대한 응답 같은 웹 사이트의 활동 내역을 추적합니다.

* [쿠키 이름: s_ecid](../cookies/cookies-mc.md#section-32fd753c3fa54452acd62b021434919a)
* [쿠키 이름: AMCV_###@AdobeOrg](../cookies/cookies-mc.md#section-a12aa2a9296940ae82d8921b381b8fb0)
* [쿠키 이름: s_cc](../cookies/cookies-analytics.md#section-03aa90aa7e36427b8cb12dc4a0f0291e)
* [쿠키 이름: s_cc](../cookies/cookies-analytics.md#section-03aa90aa7e36427b8cb12dc4a0f0291e)
* [쿠키 이름: s_sq](../cookies/cookies-analytics.md#section-8abfff3a302d494f81a3cfb91e3b09ff)
* [쿠키 이름: s_vi](../cookies/cookies-analytics.md#section-5d50a078de444d12b7d927d68ff3b679)
* [쿠키 이름: s_fid](../cookies/cookies-analytics.md#section-65e33f9bfc264959ac1513e2f4b10ac7)
* [플러그인에 의해 설정되는 쿠키](../cookies/cookies-analytics.md#section-a6b1cae8454945fab9eea5c7884c40fc)

[퍼스트 파티 쿠키](/help/interface/cookies/cookies-first-party.md)에 대한 자세한 내용은 Analytics 도움말을 참조하십시오.

## 쿠키 이름: s_ecid {#section-32fd753c3fa54452acd62b021434919a}

| 특성 | 설명 |
|--- |--- |
| 저장되는 정보 | Experience Cloud ID(ECID) 또는 MID의 사본을 포함합니다. MID는 이 구문, s_ecid=MCMID를 따르는 키-값 쌍에 저장됩니다. | <ECID> |
| 만료 | 2년 |
| 사용 | 이 쿠키는 클라이언트가 AMCV 쿠키를 설정한 후에 고객의 도메인에 의해 설정됩니다. 이 쿠키의 목적은 자사 상태의 지속적인 ID 추적을 허용하는 것이며 AMCV 쿠키가 만료된 경우 참조 ID로 사용됩니다. 자세한 내용은 AMCV 쿠키를 확인하십시오. |
| 위치 | CNAME 고객에게만 해당됩니다. 타사 시나리오에 해당되지 않습니다. 쿠키는 CNAME 및 Analytics 이미지 요청에 사용된 동일한 도메인에 저장됩니다. |
| 크기 | 45바이트 |

## 쿠키 이름: s_cc {#section-03aa90aa7e36427b8cb12dc4a0f0291e}

| 특성 | 설명 |
|--- |--- |
| 저장되는 정보 | 이 쿠키는 활성화 여부를 확인하기 위해 JavaScript 코드로 설정하고 읽습니다(간단하게 "True"로 설정). |
| 만료 | 이 쿠키는 세션 쿠키로 브라우저를 닫으면 만료됩니다. |
| 사용 | 모든 계정에 대하여 하나의 쿠키만 사용됩니다. |
| 위치 | 이 쿠키는 페이지의 도메인에 저장됩니다. |
| 크기 | 4바이트 |

## 쿠키 이름: s_sq {#section-8abfff3a302d494f81a3cfb91e3b09ff}

| 특성 | 설명 |
|--- |--- |
| 저장되는 정보 | 이 쿠키는 사용자가 클릭했던 이전 링크에 대한 정보를 포함하고 있으며 ClickMap 기능과 Activity Map 기능을 사용하는 경우 JavaScript 코드로 설정하고 읽습니다. |
| 만료 | 이 쿠키는 세션 쿠키로 브라우저를 닫으면 만료됩니다. |
| 사용 | 모든 계정에 대하여 하나의 쿠키만 사용됩니다. |
| 위치 | 이 쿠키는 페이지의 도메인에 저장됩니다. |
| 크기 | 페이지 URL 크기에 따라 다르지만 일반적으로 100-200바이트입니다 |

## 쿠키 이름: s_vi {#section-5d50a078de444d12b7d927d68ff3b679}

| 특성 | 설명 |
|--- |--- |
| 저장되는 정보 | 고유 방문자 ID 시간/날짜 스탬프 |
| 만료 | 2년 |
| 사용 | 이 쿠키는 고유 방문자를 식별하는 데 사용됩니다. |
| 위치 | 타사 쿠키를 사용하는 경우 이 쿠키는 일반적으로 207.net인 이미지 요청 도메인에 저장되며 자사 쿠키를 사용하는 경우 사용자의 도메인에 저장됩니다. |
| 크기 | 44바이트 |

>[!NOTE]
>
>각각의 Analytics 방문자 ID는 Adobe 서버의 방문자 프로필과 연결됩니다. 방문자 프로필은 모든 방문자 ID 쿠키 만료와 관계없이 비활성 기간 1년 후 삭제됩니다.

## 쿠키 이름: s_fid {#section-65e33f9bfc264959ac1513e2f4b10ac7}

| 특성 | 설명 |
|--- |--- |
| 저장되는 정보 | 대체 고유 방문자 ID 시간/날짜 스탬프 |
| 만료 | 5년 |
| 사용 | 타사 쿠키 제한으로 인해 표준 s_vi 쿠키를 사용할 수 없는 경우 쿠키는 고유 방문자를 식별하는 데 사용됩니다. 퍼스트 파티 쿠키를 사용하는 구현에는 사용되지 않습니다. |
| 위치 | 이 쿠키는 도메인에 퍼스트 파티 쿠키로 저장됩니다. |
| 크기 | 33바이트 |

## 플러그인에 의해 설정되는 쿠키 {#section-a6b1cae8454945fab9eea5c7884c40fc}

추가 쿠키는 Analytics 플러그인 사용에 따라 설정할 수 있습니다. 이러한 쿠키는 고객이 다양한 상황에 사용할 수 있는 코드 스니펫입니다. 이러한 상황들로는 URL에서 값 검색, Analytics에 전달할 값 연결, 양식 포기 캡처 등이 있습니다. 각 플러그인에 의해 설정된 쿠키의 특성에 대해 알아보려면 ClientCare에 문의하십시오. 예로는 [!DNL s_vh]Set Once Per *및* Set and Get Last Value *플러그인과 함께 사용되는* 쿠키가 있습니다.

이메일 내에 배치된 코드와 같이 JavaScript 없이 이미지 요청에 전달된 전환 변수(eVarX)는 이메일 클라이언트와 웹 브라우저가 동일한 쿠키 공간을 공유하는 경우에만 올바르게 분류됩니다.
