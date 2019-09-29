---
source-git-commit: 58ccef353b492b1c2adfbb8c2471e1f92263e6e4
translation-type: tm+mt

---
# 지침

**참고: 이 페이지(또는 readme.md 페이지)는 고객 대면 설명서에 게시되지 않습니다.**

## TOC

+ 사용 안내서의 루트에 있는 `TOC.md`는 이 솔루션에 대한 안내서에 포함된 주제 구성을 제공합니다.
+ 모든 사용 안내서는 고유한 각각의 `TOC.md`를 보유하며, 필요한 경우 모든 페이지/주제를 정렬할 수 있습니다.
+ 모든 사용 안내서의 첫 페이지는 `overview.md`입니다.

## 사용 안내서

+ 사용 안내서 소개는 `overview.md`라고 합니다.
+ 사용 안내서의 각 주제에는 고유한 디렉토리가 있습니다.
   + 안내서에 *구현*&#x200B;이라는 주제가 있으면 해당 디렉토리가 `/implementation`입니다.
+ 모든 이미지 자산은 사용 안내서의 루트에 있는 `/assets`에 저장됩니다.
   + `/assets` 디렉토리의 모든 이미지는 현지화됩니다.
   + `/no-localize` 디렉토리에 있는 모든 이미지는 현지화되지 않습니다. loc 버전에서 특정 자산이 불필요하게 재생되지 않는지 확인하는 데 사용할 수 있습니다.

## 사용 안내서 수준 메타데이터

+ 사용 안내서를 설명하는 메타데이터는 `TOC.md`에 저장됩니다. 여기에는 다음 항목이 포함되어 있습니다.
   + product - 제품/기능의 이름.
   + cloud - 이 제품이 속한 클라우드.
   + audience - 안내서가 타깃팅된 대상 또는 원형.
   + user-guide - 사용자 안내서의 이름.

## 페이지 수준 메타데이터

+ 문서를 설명하는 데 필요한 메타데이터는 각 개별 페이지의 일부로 저장됩니다. 여기에는 다음 항목이 포함되어 있습니다.
   + title - 페이지의 제목.
   + description - 페이지에 대한 설명.
   + seo-title - SEO 대체 제목.
   + seo-description - SEO 목적의 대체 제목.
   + short-title - (선택적 필드).
   + index - yes / no - 페이지가 Adobe의 검색 플랫폼으로 인덱싱됨.
   + translate - yes / no - 이 페이지가 현지화됨.
   + version - 주로 AEM 및 캠페인에 사용되며 제품 버전을 나타냄.
   + private-feature-pack - 주로 AEM에 사용됨.
   + beta - 제품이 베타 버전입니까?
   + redirect - 필요한 경우, 새 페이지에 대한 참조를 만드는 데 사용 가능.
   + doc-type: 참조(기본값) / 문제 해결 / 개발자 / 자습서 / kb / 백서.

## 추가 정보

자세한 게시 지침, 스타일 안내서, 샘플 및 기타 리소스는 [공동 작업 설명서 Repo](https://git.corp.adobe.com/AdobeDocs/collaborative-doc-instructions)를 참조하십시오.
