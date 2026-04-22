---
title: Content Credentials for Organizations
description: Learn about how to apply and review Content Credentials in GenStudio for Performance Marketing.
level: Intermediate
feature: Content Management, Content Attributes
exl-id: 9fc1e428-7fa7-4f00-84ba-51c9318766f4
TQID: https://experienceleague.adobe.com/ATpH1AXBAhr5tJDVkgx0ZaK20YYBmP7NQF0BUCtGiGw
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: ad3738c7-91ac-48ed-a914-fd0b03f89396
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: f321b88b-6bb7-49cc-a16a-ae2b665ebd32
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 7aed06dbb249cfc7e0f15d792563699e63b1a390
workflow-type: tm+mt
source-wordcount: 723
ht-degree: 0%

---

# Content Credentials for organizations

Learn how tamper-proof credentials for content that prove brand authenticity and drive compliance are embedded directly in your marketing workflow.

>[!WARNING]
>
> This feature is currently in beta and is only available to organizations that have been granted access. If interested, please reach out to your Adobe account team representative or [use this link to request enrollment](https://www.feedbackprogram.adobe.com/c/a/5aWPEOthrDv22Mf9CyekOy?source=qr).

## Get started with Content Credentials {#content-credentials}

>[!CONTEXTUALHELP]
>id="gspm_content_credentials"
>title="Content Credentials in [!DNL GenStudio for Performance Marketing]"
>abstract="Tamper-proof credentials for content that prove brand authenticity and drive compliance can be embedded directly in your marketing workflow."

After Content Credentials have been activated in the Admin Console, GenStudio for Performance Marketing users can turn on Content Credentials for all assets globally in the app. If the global option to apply credentials is turned off, users have the choice to apply Content Credentials for each individual asset.

Once content is published, Content Credentials will be visible on external platforms, like LinkedIn.

Administrators are responsible for uploading a valid X.509 certificate within the Admin Console. This step ensures that the enterprise&#39;s digital signature is properly configured and ready for use in supported Adobe DX applications.

>[!NOTE]
>
>Control over this setting might transition to the Admin Console in the future, streamlining the management of Content Credentials across applications and enhancing administrative oversight.

## What are Content Credentials? 

Content Credentials are a durable, industry-standard type of metadata with details about how content was made and identity information about the creators. Content Credentials can be viewed when the content is published online to supporting platforms, or by using tools like [Adobe&#39;s Inspect tool](https://contentauthenticity.adobe.com/inspect) or the [Adobe Content Authenticity Chrome browser extension](https://helpx.adobe.com/creative-cloud/help/cai/adobe-content-authenticity-chrome-browser-extension.html).  

Applying Content Credentials can help increase transparency about how content was made and can help your users connect themselves to their content.

[Learn more about Content Credentials](https://helpx.adobe.com/tw/creative-cloud/help/content-credentials.html) at Adobe.

## Brand signature and asset tracking

Brand-signed content plays a significant role in promoting brand integrity and user trust. 在Admin Console中正確設定憑證後，組織便可以在Adobe應用程式中，使用唯一的品牌簽章簽署內容。 這項真實性保證是使用不可見的浮水印和指紋技術來維護，這有助於在內容的整個生命週期中保持簽名的耐久性。

除了品牌簽署外，企業也可以直接將資產ID附加至其內容。 這有助於有效率地追蹤資產，尤其是在社群媒體平台上分享或張貼資產時。 透過合併資產ID，組織可以追蹤其內容的原始和發佈路徑，強化監督和問責。

## 行銷工作流程中的Content Credentials

您可以直接在GenStudio for Performance Marketing中，在整個行銷工作流程中套用Content Credentials，從匯入和內容探索，到啟用和匯出。 您也會找到內容上顯示的認證，以供整個應用程式檢閱。

### 匯入和探索

在內容庫中，認證會顯示在匯入的資產上。

縮圖右上角的Content Credential徽章表示「品牌簽署」內容。

![具有認證的匯入資產](./images/import-discovery1.png)

選取已簽署的內容會顯示詳細的中繼資料：已發佈的品牌、錄製程式、使用的工具、時間戳記。

可依認證狀態篩選內容。

![資產上的認證資料](./images/import-discovery2.jpg)

### 建立和選取

Content Credential徽章會顯示在畫布資產選擇器中。

在選取體驗的資產以在整個編輯過程中維護來源鏈時，會保留認證中繼資料。

畫布資產選擇器中的![Content Credential徽章](./images/creation-selection1.png)

### 編輯和轉換

從草稿匯出期間，已修改的資產會自動重新簽署，而新的認證會連結至原始資產。

已匯出資產上的![認證資料](./images/edit-and-transformation1.png){width="60%"}

### 檢閱和核准

在「稽核並核准」預覽中，右側邊欄會顯示資產的認證狀態。

![已核准資產的認證資料](./images/review-and-approve1.png){width="60%"}

當檢閱者檢查資產時，會顯示每個變體的認證詳細資料。 使用者按一下&#x200B;**[!UICONTROL 儲存至內容]**&#x200B;時，核准的體驗會重新簽署。

![已核准資產的認證資料](./images/review-and-approve2.png)

### 啟用和匯出

在啟用期間，認證狀態會顯示在Experience選擇器中。

已啟動資產上的![認證資料](./images/activate-export1.png){width="60%"}

匯出的檔案將會內嵌C2PA相容的認證。

所有支援的格式(JPEG、PNG、MP4)都能維持認證完整性。

已匯出資產上的![認證資料](./images/activate-export2.png)
