---
description: 드래그 앤 드롭을 사용하여 업로드하지 않는 경우에는 FTP를 통해 Experience Cloud로 고객 속성 데이터를 업로드할 수 있습니다.
keywords: 고객 속성;핵심 서비스
seo-description: 드래그 앤 드롭을 사용하여 업로드하지 않는 경우에는 FTP를 통해 Experience Cloud로 고객 속성 데이터를 업로드할 수 있습니다.
seo-title: 선택 사항 - FTP를 통해 데이터 파일 업로드
solution: Experience Cloud
title: 선택 사항 - FTP를 통해 데이터 파일 업로드
uuid: 5df565dd-b6f8-420e-981f-4b6fc6f7d0e4
translation-type: ht
source-git-commit: f8b48077d936e289d66c1a93a96fe9ebaa4f0136

---


# 선택 사항 - FTP를 통해 데이터 파일 업로드

드래그 앤 드롭을 사용하여 업로드하지 않는 경우에는 FTP를 통해 Experience Cloud로 고객 속성 데이터를 업로드할 수 있습니다.

Experience Cloud에서 고객 속성 소스 및 FTP 계정을 만든 후에 데이터를 업로드할 수 있습니다. 속성 소스당 FTP 계정을 1개 만듭니다. 업로드한 파일은 해당 계정의 루트 폴더에 저장됩니다. 데이터는 `.csv` 형식이어야 하며 업로드가 완료되었음을 나타내는 두 번째 `.fin` 파일도 있어야 합니다.

>[!IMPORTANT]
>
>파일을 업로드하기 전에 [고객 속성을 업로드하기 위한 데이터 파일 요구 사항](../attributes/crs-data-file.md#concept_DE908F362DF24172BFEF48E1797DAF19)을 검토하십시오.


고객 속성 FTP 사이트로의 파일 업로드는 FTP 또는 SFTP를 통해 수행될 수 있습니다.

* SFTP 연결을 지원하는 클라이언트가 필요합니다.
* [여기](https://marketing.adobe.com/resources/help/ko_KR/whitepapers/ftp/?f=ftp_sftp_cert_auth) 설명된 대로 사용자 이름/암호 또는 암호 없음을 사용하여 SFTP와 연결할 수 있습니다.



<!-- <p>Error states - get with Matt and Dave </p> 
<p>What are the most common reasons for doing this? Retail? Do a use case example, then show an AN example. </p> 
<p>You create one FTP per attribute source. Files go to the root folder in that account. The file type .fin is user-created. (For example, upload a .csv then a .fin of the same name, which signals you have completed the upload. https://wiki.corp.adobe.com/display/marketingcloud/Customer+Record+Services#CustomerRecordServices-FileFormats (leverage for doc). Possibly link from FTP File Reqs page to a help file about naming conventions. Need a new file type page for this. Similar content here: https://marketing.adobe.com/resources/help/en_US/reference/c_general_file_structure.html and here: https://marketing.adobe.com/resources/help/en_US/whitepapers/ftp/ftp_datasources.html </p> 
<p>Drag-n-drop and zip functionality for uploads - 1/21/2015. S/b less than 100 megs for drag and drop zip file. Fin file not required for drag/drop. </p> 
<p>Preview Data - shows the last upload (?) </p> 
<p>Need a link to the "instructions" on that information icon with the image. </p> 
<p>Workflow: Drag and drop, validate schema, configure subscription, save/activate. </p> -->
**FTP를 통해 데이터 파일 업로드**

1. [고객 속성 소스를 만들고 데이터 파일 업로드...](../attributes/t-crs-usecase.md#task_BCC327B2A0EF4A1BBB2934013AB92B78).

   FTP 사이트 [!DNL ftp.adobe.com/<sftpname>]에 로그인되어 있는지 확인하십시오.

1. **[!UICONTROL 작업]** &gt; **[!UICONTROL 파일 업로드]**&#x200B;를 클릭합니다.

1. `.fin` 파일을 업로드하여 검색할 수 있게 만듭니다.

   파일 형식 `.fin`은 사용자가 만드는 파일이며 업로드가 완료되었음을 나타냅니다. 빈 메모장 파일일 수 있습니다. 예를 들어 [!DNL crs123.csv]를 업로드하는 경우 [!DNL crs123.fin]도 업로드하게 됩니다.

   업로드가 성공적으로 수행되면 두 파일이 모두 **processed** 폴더로 이동됩니다.


   파일 이름 및 구조에 대한 중요 정보를 보려면 [고객 속성을 업로드하기 위한 데이터 파일 요구 사항](../attributes/crs-data-file.md#concept_DE908F362DF24172BFEF48E1797DAF19)을 참조하십시오.
