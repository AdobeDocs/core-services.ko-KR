---
description: ' [!DNL Adobe Target] 이(가) 쿠키를 사용하여 어떤 온라인 콘텐츠 및 오퍼가 방문자와 관련이 있는지 테스트하는 기능을 웹 사이트 운영자에게 제공하는 방법에 대해 알아봅니다.'
solution: Experience Cloud,Analytics,Target
title: Adobe Target 쿠키
uuid: 44f7e32e-8d99-4682-8b54-8364d001b403
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: c4399cc0-8333-47b8-b830-2ba7359f464a
source-git-commit: 95ca3a8e172166d7901873e0dc2e096e0bba7cd2
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 8%

---

# [!DNL Adobe Target] 쿠키

[!DNL Adobe Target]은(는) 쿠키를 사용하여 웹 사이트 운영자가 어떤 온라인 콘텐츠 및 오퍼가 방문자와 관련이 있는지 테스트할 수 있도록 합니다.

>[!NOTE]
>
>이 문서의 정보는 [[!DNL Target] at.js JavaScript 라이브러리](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html?lang=ko){target=_blank}에만 적용됩니다.
>
>[[!DNL Adobe Experience Platform Web SDK]](https://experienceleague.adobe.com/docs/experience-platform/edge/home.html?lang=ko){target=_blank}을(를) 사용하여 [!DNL Target] 구현에 사용된 쿠키에 대한 자세한 내용은 &quot;[!DNL Adobe Experience Platform Web SDK]에서 쿠키를 사용합니까? 그렇다면 어떤 쿠키를 사용합니까?&quot; [[!DNL Platform Web SDK 개요 안내서의 FAQ]](https://experienceleague.adobe.com/docs/experience-platform/edge/web-sdk-faq.html?lang=ko){target=_blank}에서 참조하십시오.
>
>필요한 경우 쿠키 지속 시간을 제외하고 이 문서에서 설명한 설정을 변경할 수 있습니다. 쿠키 설정을 변경할 때 [계정 담당자에게 문의](https://experienceleague.adobe.com/docs/target/using/cmp-resources-and-contact-information.html?lang=ko){target=_blank}합니다.
>
>[!DNL Target]명의 사용자가 사용자 지정된 서드파티 쿠키를 만들 수도 있습니다.

## 자사 쿠키

다음 자사 쿠키는 고객의 도메인에 저장됩니다.

| Cookie | 세부 사항 |
| --- | --- |
| mbox | 방문자에 대한 익명 식별자를 저장합니다.<P>**쿠키 도메인**: mbox를 제공하는 도메인입니다. 이 쿠키는 회사 도메인에서 제공되므로 쿠키는 자사 쿠키입니다. 예: `mycompany.com` 도메인 이름에 `mycompany.co.uk`과(와) 같은 국가 코드가 포함되어 있는 경우 클라이언트 서비스와 작업하여 이 코드를 지원하도록 at.js를 구성하십시오. 필요한 경우 쿠키 도메인을 사용자 지정하는 방법에 대한 자세한 내용은 *[!DNL Adobe Target]개발자 안내서*&#x200B;의 [targetGlobalSettings](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html?lang=ko){target=_blank}에서 &quot;`cookieDomain`&quot;을(를) 참조하십시오.<P>**서버 도메인**: `clientcode.tt.omtrdc.net`, [!DNL Target] 계정에 대해 클라이언트 코드 사용.<P>**쿠키 지속 시간**: 쿠키는 마지막 로그인부터 2년 동안 방문자의 브라우저에 유지됩니다. 쿠키 지속 시간은 변경할 수 없습니다.<P>쿠키는 방문자가 [!DNL Target] 활동을 경험하는 방식을 관리하기 위해 일부 값을 유지합니다.<P>**세션 ID**: 지정된 사용자 세션의 고유 식별자입니다. 30분 동안 활동이 없으면 기본적으로 세션이 만료됩니다. `sessionId`을(를) 직접 생성하는 경우(예: [서버측 구현](https://experienceleague.adobe.com/docs/target-dev/developer/server-side/server-side-overview.html?lang=ko){target=_blank}의 경우) 다음을 확인하십시오.<ul><li>세션 ID는 인쇄 가능한 모든 문자열이 될 수 있습니다. 단, 공백, 물음표( ? ), 중괄호( { } ) 또는 슬래시( / )를 사용할 수 있습니다.</li><li>세션 ID는 1자에서 128자 사이여야 합니다.</li><li>특정 세션의 경우 쿠키의 값이 여러 요청에서 동일하게 유지되어야 합니다.</li><li>특정 시점에 지정된 방문자에 대해 병렬 세션(개별 `sessionIds`)이 있어서는 안 됩니다.</li></ul>에지 클러스터의 특정 노드에 대한 라우팅은 세션 ID를 사용하여 수행됩니다.<ul><li>세션은 서버측에서 30분 동안 활성화됩니다. 따라서 `tntId/thirdPartyId`에 대해 마지막으로 요청한 후 30분 이내에 특정 `tntId/thirdPartyId`에 대해 다른 세션 ID를 사용해서는 안 됩니다. 그렇지 않으면, 프로필 변경 사항이 일관되지 않고 예측할 수 없습니다.</li><li>새 세션 ID는 방문자가 30분 동안 활동이 없으면 사용해야 합니다.</li><li>여러 `tntIds/thirdPartyIds`에서 동일한 세션 ID를 사용하면 `tntId/thirdPartyIDs`에서 식별하는 프로필에 예측 불가능한 변경 사항을 초래할 수 있습니다.</li></ul>참고: 지정된 세션 ID는 [동시 요청 수 제한](https://experienceleague.adobe.com/docs/target/using/troubleshoot/target-limits.html?lang=ko#content-delivery){target=_blank}을 참조하십시오.<P>**pc ID**: 방문자 브라우저의 반영구 ID입니다. 쿠키가 수동으로 삭제될 때까지 지속됩니다.<P>**check**: 방문자가 쿠키를 지원하는지 확인하는 데 사용되는 간단한 테스트 값입니다. 방문자가 페이지를 요청할 때마다 설정합니다.<P>**disable**: 방문자의 로드 시간이 at.js 파일에 구성된 시간을 초과하는 경우 설정합니다. 기본적으로 이 시간 초과는 1시간 동안 지속됩니다. |
| at_check | 브라우저에서 쿠키 읽기/쓰기 기능이 활성화되어 있는지 확인하는 임시 쿠키. |
| mboxEdgeCluster | 이 쿠키는 [overrideMboxEdgeServer 설정](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html?lang=ko){target=_blank}이(가) `true`(으)로 설정된 경우에만 존재합니다. |

이러한 자사 쿠키에서는 HTTPOnly를 사용할 수 없습니다. at.js JavaScript 라이브러리는 이러한 쿠키를 읽고 써야 합니다. 이러한 쿠키는 at.js에 의해 만들어지며 서버에서 설정되지 않습니다.

at.js 구현의 `secureOnly: true` 구성을 사용하여 이러한 모든 쿠키에 대해 `secure` 설정을 활성화할 수 있습니다.

## 서드파티 쿠키

다음 타사 쿠키가 `tt.omtrdc.net`에 저장되어 있습니다.

| Cookie | 세부 사항 |
| --- | --- |
| customerclientcode!mboxPC | 이 쿠키는 도메인 간 사용이 활성화된 경우 존재합니다. |
| customerclientcode!mboxSession | 이 쿠키는 도메인 간 사용이 활성화된 경우 존재합니다. |

이러한 타사 쿠키는 기본적으로 HTTPOnly이며 [!DNL Target] Edge Server에 의해 설정됩니다.

at.js 구현의 `secureOnly: true` 구성을 사용하여 모든 쿠키에 대해 `secure` 설정을 활성화할 수 있습니다.