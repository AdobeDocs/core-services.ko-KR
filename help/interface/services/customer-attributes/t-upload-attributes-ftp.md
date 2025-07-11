---
description: FTP를 통해 Experience Cloud에 고객 속성 데이터를 업로드하는 방법을 알아봅니다.
solution: Experience Cloud
title: FTP를 통한 고객 속성 데이터 파일 업로드
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: ed9e4a8f-493a-4a0f-a87e-674c7da95b99
source-git-commit: 2f126877f6a5f090884ebe093f35e4f6d90b4df6
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 71%

---

# 선택 사항 - FTP를 통한 데이터 파일 업로드

드래그 앤 드롭을 사용하여 업로드하지 않는 경우에는 FTP를 통해 Experience Cloud으로 고객 속성 데이터를 업로드할 수 있습니다.

Experience Cloud에서 고객 속성 소스 및 FTP 계정을 만든 후에 데이터를 업로드할 수 있습니다. 속성 소스당 FTP 계정을 1개 만듭니다. 업로드한 파일은 해당 계정의 루트 폴더에 저장됩니다. 데이터는 `.csv` 형식이어야 하며, 업로드가 완료되었음을 나타내는 두 번째 `.fin` 파일도 있어야 합니다.

>[!IMPORTANT]
>
>파일을 업로드하기 전에 [고객 특성을 업로드하기 위한 데이터 파일 요구 사항](crs-data-file.md)을 검토하십시오.

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

   파일 이름 및 구조에 대한 중요한 정보가 필요하면 [고객 특성을 업로드하기 위한 데이터 파일 요구 사항](crs-data-file.md)을 참조하십시오.
