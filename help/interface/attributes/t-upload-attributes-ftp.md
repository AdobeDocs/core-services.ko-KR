---
description: 드래그 앤 드롭을 사용하여 업로드하지 않는 경우에는 FTP를 통해 Experience Cloud로 고객 속성 데이터를 업로드할 수 있습니다.
keywords: Customer Attributes;core services
seo-description: 드래그 앤 드롭을 사용하여 업로드하지 않는 경우에는 FTP를 통해 Experience Cloud로 고객 속성 데이터를 업로드할 수 있습니다.
seo-title: 선택 사항 - FTP를 통해 데이터 파일 업로드
solution: Experience Cloud
title: 선택 사항 - FTP를 통해 데이터 파일 업로드
uuid: 5df565dd-b6f8-420e-981f-4b6fc6f7d0e4
translation-type: tm+mt
source-git-commit: 0bc7032d0052ba03beac1140dfbfd630e1802bfd
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# 선택 사항 - FTP를 통해 데이터 파일 업로드

드래그 앤 드롭을 사용하여 업로드하지 않는 경우에는 FTP를 통해 Experience Cloud로 고객 속성 데이터를 업로드할 수 있습니다.

Experience Cloud에서 고객 속성 소스 및 FTP 계정을 만든 후 데이터를 업로드할 수 있습니다. 속성 소스당 하나의 FTP 계정을 만듭니다. 업로드된 파일은 해당 계정의 루트 폴더에 저장됩니다. 데이터는 `.csv` 형식이어야 하며 업로드가 완료되었음을 나타내는 두 번째 `.fin` 파일도 있어야 합니다.

>[!IMPORTANT]
>
>Review [Data file requirements for uploading Customer Attributes](../attributes/crs-data-file.md#concept_DE908F362DF24172BFEF48E1797DAF19) before uploading the file.

고객 속성 FTP 사이트에 대한 파일 업로드는 FTP 또는 SFTP를 통해 수행할 수 있습니다.

* SFTP 연결을 지원하는 클라이언트가 필요합니다.
* 여기에 설명된 대로 사용자 이름/암호를 사용하거나 암호를 사용하지 않고 SFTP에 연결할 수 [있습니다](https://docs.adobe.com/help/en/analytics/export/ftp-and-sftp/secure-file-transfer-protocol/ftp-sftp-cert-auth.html).

**FTP를 통해 데이터 파일 업로드**

1. [고객 속성 소스를 만들고 데이터 파일 업로드...](../attributes/t-crs-usecase.md#task_BCC327B2A0EF4A1BBB2934013AB92B78).

   FTP 사이트 [!DNL ftp.adobe.com/<sftpname>]에 로그인되어 있는지 확인하십시오.

1. Click **[!UICONTROL Actions]** > **[!UICONTROL File Upload]**.

1. `.fin` 파일을 업로드하여 검색할 수 있게 만듭니다.

   파일 형식 `.fin`은 사용자가 만드는 파일이며 업로드가 완료되었음을 나타냅니다. 빈 메모장 파일일 수 있습니다. 예를 들어 [!DNL crs123.csv]를 업로드하는 경우 [!DNL crs123.fin]도 업로드하게 됩니다.

   업로드에 성공하면 두 파일이 모두 **처리된 폴더로 이동됩니다**.

   See [Data file requirements for uploading Customer Attributes](../attributes/crs-data-file.md#concept_DE908F362DF24172BFEF48E1797DAF19) for important information about file names and structure.
