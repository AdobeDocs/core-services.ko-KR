---
description: FTP를 통해 고객 속성 데이터를 CX Enterprise로 업로드하는 방법을 알아봅니다.
solution: Experience Cloud
title: FTP를 통한 고객 속성 데이터 파일 업로드
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: ed9e4a8f-493a-4a0f-a87e-674c7da95b99
TQID: https://experienceleague.adobe.com/jI2dWXMmrrWxceVi-sZtzF5cTF11iy4d7QKkx71vF-I
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
feature_v2:
  - id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
subfeature_v2:
  - id: b75843fa-0a67-4a44-a6b1-cc627b0481dc
  - id: fef08361-6ac5-460c-93fe-d063e40b6a49
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 50012e2564e88e1a6e16578e3331136c7df0cb21
workflow-type: tm+mt
source-wordcount: 394
ht-degree: 51%

---

# FTP를 통한 데이터 파일 업로드 (선택 사항)

드래그 앤 드롭을 사용하여 업로드하지 않는 경우에는 FTP를 통해 고객 속성 데이터를 CX Enterprise로 업로드할 수 있습니다.

CX Enterprise에서 고객 속성 소스 및 FTP 계정을 만든 후에 데이터를 업로드할 수 있습니다. 속성 소스당 FTP 계정을 1개 만듭니다. 업로드한 파일은 해당 계정의 루트 폴더에 저장됩니다. 데이터는 `.csv` 형식이어야 하며, 업로드가 완료되었음을 나타내는 두 번째 `.fin` 파일도 있어야 합니다.

>[!IMPORTANT]
>
>파일을 업로드하기 전에 [고객 특성 데이터 파일 및 원본](crs-data-file.md)을 검토하십시오.

고객 속성 FTP 사이트로의 파일 업로드는 FTP 또는 SFTP를 통해 수행될 수 있습니다.

* SFTP 연결을 지원하는 클라이언트가 필요합니다.
* [여기](https://experienceleague.adobe.com/docs/analytics/export/ftp-and-sftp/secure-file-transfer-protocol/ftp-sftp-cert-auth.html?lang=ko)에 설명된 것처럼 사용자 이름/암호를 사용하거나 암호를 사용하지 않고 SFTP를 통해 연결할 수 있습니다.

**FTP를 통한 데이터 파일 업로드**

1. [고객 속성 소스를 만들고 데이터 파일 업로드...](t-crs-usecase.md).

   `ftp.adobe.com/<sftpname>`에서 FTP 사이트에 로그인했는지 확인하십시오.

1. **[!UICONTROL 작업]** > **[!UICONTROL 파일 업로드]**&#x200B;를 클릭합니다.

1. `.fin` 파일을 업로드하여 검색할 수 있게 만듭니다.

   파일 형식 `.fin` 은 사용자가 만드는 파일이며 업로드가 완료되었음을 나타냅니다. 빈 메모장 파일일 수 있습니다. 예를 들어 `crs123.csv`를 업로드하는 경우 `crs123.fin`도 업로드하게 됩니다.

   업로드가 성공적으로 수행되면 두 파일이 모두 **processed** 폴더로 이동됩니다.

   파일 이름 및 구조에 대한 중요한 정보가 필요하면 [고객 특성 데이터 파일 및 원본](crs-data-file.md)을 참조하세요.

## FTP 계정 설정

속성 소스당 하나의 FTP 계정을 설정합니다.

[!UICONTROL 파일 업로드 및 스키마 유효성 검사] 페이지에서 **[!UICONTROL FTP 설정]**&#x200B;을 클릭합니다.

![스키마 편집](assets/ftp-account.png)

업로드한 파일은 해당 계정의 루트 폴더에 저장됩니다. 데이터는 `.csv` 형식이어야 하며, 업로드가 완료되었음을 나타내는 두 번째 `.fin` 파일도 있어야 합니다.

문자열, 정수 및 숫자에 적용하는 이름은 [!DNL Analytics] 지표를 만드는 데 사용됩니다.

* 업로드된 `.csv` 파일에서 **[!UICONTROL 특성:]** 특성 데이터를 읽었습니다.

* **[!UICONTROL 유형:]** 다음과 같은 데이터 유형:

   * **문자열:** 일련의 문자들.

   * **정수:** 범자연수.

   * **숫자:** 최대 2개의 소수 자리를 가질 수 있습니다.

* **[!UICONTROL 표시 이름:]** 특성의 이름입니다. 예를들어 특성 *customer age*&#x200B;을(를) *customer Since*(으)로 변경할 수 있습니다.

* **[!UICONTROL 설명:]** 특성에 대한 설명입니다.

