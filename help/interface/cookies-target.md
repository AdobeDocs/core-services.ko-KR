---
description: Adobe Target에서 어떻게 쿠키를 사용하여 어떤 온라인 콘텐츠 및 오퍼가 방문자와 밀접한 관련이 있는지 테스트하는 기능을 웹 사이트 운영자에게 제공하는지 알아봅니다.
solution: Experience Cloud,Analytics,Target
title: Adobe Target 쿠키
uuid: 44f7e32e-8d99-4682-8b54-8364d001b403
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: c4399cc0-8333-47b8-b830-2ba7359f464a
source-git-commit: f229ec33ff721527e6a4c920ea63eabb4102935a
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 15%

---

# Adobe Target 쿠키

[!DNL Adobe Target] 은 쿠키를 사용하여 웹 사이트 운영자가 어떤 온라인 콘텐츠 및 오퍼가 방문자와 관련이 있는지 테스트할 수 있도록 합니다.

>[!NOTE]
>
>이 문서의 정보는 [[!DNL Target] at.js JavaScript 라이브러리](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html?lang=ko-KR){target=_blank} 만 해당.
>
>에 사용된 쿠키에 대한 정보 [!DNL Target] 를 사용한 구현 [[!DNL Adobe Experience Platform Web SDK]](https://experienceleague.adobe.com/docs/experience-platform/edge/home.html?lang=ko-KR){target=_blank}, see "Does the [!DNL Adobe Experience Platform Web SDK] use cookies? If so, what cookies does it use?" in [Frequently Asked questions in the DNL Platform Web SDK overview guide](https://experienceleague.adobe.com/docs/experience-platform/edge/web-sdk-faq.html){target=_blank}.
>
>필요한 경우 쿠키 지속 시간을 제외하고 이 문서에서 설명한 설정을 변경할 수 있습니다. [계정 담당자에게 문의하십시오.](https://experienceleague.adobe.com/docs/target/using/cmp-resources-and-contact-information.html){target=_blank} 쿠키 설정을 변경하는 경우.
>
>[!DNL Target] 사용자는 사용자 지정된 서드파티 쿠키를 만들 수도 있습니다.

## 자사 쿠키

다음 자사 쿠키는 고객의 도메인에 저장됩니다.

| Cookie | 세부 사항 |
| --- | --- |
| mbox | 방문자에 대한 익명 식별자를 저장합니다.<P>**쿠키 도메인**: mbox를 제공하는 도메인입니다. 이 쿠키는 회사 도메인에서 제공되므로 쿠키는 자사 쿠키입니다. 예: `mycompany.com`. 도메인 이름에 다음과 같은 국가 코드가 포함되어 있는 경우 `mycompany.co.uk`, 클라이언트 서비스와 협력하여 이 코드를 지원하도록 at.js를 구성하십시오. 필요한 경우 쿠키 도메인 사용자 지정에 대한 자세한 내용은 &quot;`cookieDomain`&quot; 아래에 [targetGlobalSettings](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html?lang=ko-KR){target=_blank} 다음에서 *[!DNL Adobe Target]개발자 안내서*.<P>**서버 도메인**: `clientcode.tt.omtrdc.net`, 클라이언트 코드 사용 [!DNL Target] 계정입니다.<P>**쿠키 지속 시간**: 쿠키는 마지막 로그인부터 2년 동안 방문자의 브라우저에 유지됩니다. 쿠키 지속 시간은 변경할 수 없습니다.<P>쿠키는 방문자가 경험하는 방식을 관리하기 위해 일부 값을 유지합니다 [!DNL Target] 활동:<P>**세션 ID**: 지정된 사용자 세션에 대한 고유 식별자. 30분 동안 활동이 없으면 기본적으로 세션이 만료됩니다. 생성하는 경우 `sessionId` 자신(예: [서버측 구현](https://experienceleague.adobe.com/docs/target-dev/developer/server-side/server-side-overview.html){target=_blank}) 다음을 확인하십시오.<ul><li>세션 ID는 인쇄 가능한 모든 문자열이 될 수 있습니다. 단, 공백, 물음표( ? ), 슬래시( / )는 제외됩니다.</li><li>세션 ID는 1자에서 128자 사이여야 합니다.</li><li>특정 세션의 경우 쿠키의 값이 여러 요청에서 동일하게 유지되어야 합니다.</li><li>병렬 세션이 없어야 합니다(고유). `sessionIds`)을 클릭하여 제품에서 사용할 수 있습니다.</li></ul>에지 클러스터의 특정 노드에 대한 라우팅은 세션 ID를 사용하여 수행됩니다.<ul><li>세션은 서버측에서 30분 동안 활성화됩니다. 따라서 특정 항목에 다른 세션 ID를 사용해서는 안 됩니다 `tntId/thirdPartyId` 을(를) 사용한 마지막 요청 후 30분 이내 `tntId/thirdPartyId`. 그렇지 않으면, 프로필 변경 사항이 일관되지 않고 예측할 수 없습니다.</li><li>새 세션 ID는 방문자가 30분 동안 활동이 없으면 사용해야 합니다.</li><li>여러 개에 동일한 세션 ID 사용 `tntIds/thirdPartyIds` 로 식별되는 프로필에 예측 불가능한 변경 사항을 초래할 수 있음 `tntId/thirdPartyIDs`.</li></ul>참고: 다음을 참조하십시오 [동시 요청 수 제한](https://experienceleague.adobe.com/docs/target/using/troubleshoot/target-limits.html?lang=en#content-delivery){target=_blank} (특정 세션 ID의 경우)<P>**pc ID**: 방문자 브라우저의 반영구 ID입니다. 쿠키가 수동으로 삭제될 때까지 지속됩니다.<P>**check**: 방문자가 쿠키를 지원하는지 여부를 확인하는 데 사용되는 간단한 테스트 값입니다. 방문자가 페이지를 요청할 때마다 설정합니다.<P>**disable**: 방문자의 로드 시간이 at.js 파일에 구성된 시간을 초과하는 경우 설정됩니다. 기본적으로 이 시간 초과는 1시간 동안 지속됩니다. |
| at_check | 브라우저에서 쿠키 읽기/쓰기 기능이 활성화되어 있는지 확인하는 임시 쿠키. |
| mboxEdgeCluster | 이 쿠키는 다음과 같은 경우에만 존재합니다. [overrideMboxEdgeServer 설정](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html?lang=ko-KR){target=_blank} 이(가) (으)로 설정됨 `true`. |

이러한 자사 쿠키에서는 HTTPOnly를 사용할 수 없습니다. at.js JavaScript 라이브러리는 이러한 쿠키를 읽고 써야 합니다. 이러한 쿠키는 at.js에 의해 만들어지며 서버에서 설정되지 않습니다.

다음 `secure` 설정은 다음을 사용하여 이러한 모든 쿠키에서 활성화할 수 있습니다. `secureOnly: true` at.js 구현에서의 구성.

## 서드파티 쿠키

다음 타사 쿠키가에 저장됩니다. `tt.omtrdc.net`:

| Cookie | 세부 사항 |
| --- | --- |
| customerclientcode!mboxPC | 이 쿠키는 도메인 간 사용이 활성화된 경우 존재합니다. |
| customerclientcode!mboxSession | 이 쿠키는 도메인 간 사용이 활성화된 경우 존재합니다. |

이러한 서드파티 쿠키는 즉시 사용할 수 있으며 [!DNL Target] 에지 서버.

다음 `secure` 설정을 모든 쿠키에서 `secureOnly: true` at.js 구현에서의 구성.