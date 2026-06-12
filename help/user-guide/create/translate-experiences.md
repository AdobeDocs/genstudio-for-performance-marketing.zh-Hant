---
title: 翻譯和本地化體驗
description: 瞭解如何在Adobe GenStudio for Performance Marketing的HTML畫布上將核准的電子郵件和付費媒體體驗翻譯成多種語言。
feature: Create Canvas, Content Generation
role: User
level: Beginner
source-git-commit: bc59f6f5dce0c4f22228bcd06c2f5e60a4311e04
workflow-type: tm+mt
source-wordcount: '767'
ht-degree: 2%

---

# 翻譯體驗並將其本地化

Adobe [!DNL GenStudio for Performance Marketing]在HTML畫布中提供立即可用的翻譯，讓全球和區域行銷人員無需外部翻譯工具，即可將已核准的體驗擴充為多種語言。

此功能預設使用Azure Open AI。 您的組織也可以透過[翻譯延伸模組](/help/extensibility/deploy-app.md#find-translation-extensions)連線偏好的翻譯服務。

從[!DNL Content]中儲存的核准體驗開始翻譯。 來源體驗可以是任何語言。 每個翻譯的變體都會在[!DNL Create]畫布上開啟為可編輯的草稿，您可匯出、傳送以供稽核及發佈為個別體驗。

## 支援的體驗

HTML畫布上的現成翻譯支援：

* [電子郵件體驗](/help/user-guide/create/email-experiences.md)
* 付費媒體體驗，包括[Meta](/help/user-guide/create/meta-experiences.md)、[LinkedIn](/help/user-guide/create/linkedin-experiences.md)和[顯示](/help/user-guide/create/display-ad-experiences.md)廣告

## 開始之前

確認您要翻譯的體驗是&#x200B;**已核准**，且可在[!DNL Content] _[!UICONTROL 體驗]_&#x200B;相簿中取得。 草稿或檢閱中的體驗不符合翻譯來源資格。

如果您的組織註冊自訂翻譯擴充功能，GenStudio for Performance Marketing會使用該服務，而非預設的Azure Open AI翻譯。 請參閱[尋找翻譯延伸模組](/help/extensibility/deploy-app.md#find-translation-extensions)。

## 從[!DNL Create]翻譯 {#translate-from-create}

從[!DNL Create]登陸頁面開始翻譯，將核准的體驗當地語系化。

![在建立登陸頁面](./translate-create-workflow.png){width="600" zoomable="yes"}上翻譯及本地化復本

**從[!DNL Create]**&#x200B;翻譯：

1. 在[!DNL Create]中，捲動至&#x200B;_內容建立_&#x200B;區段。
1. 按一下&#x200B;**[!UICONTROL 翻譯與本地化復本]**。
1. 選取您要翻譯的已核准電子郵件或付費媒體體驗。 按一下&#x200B;**[!UICONTROL 使用]**&#x200B;按鈕。
1. 從支援的語言清單中選取目標語言。 按一下&#x200B;**[!UICONTROL 翻譯]**。

轉譯的變體會出現在畫布上。

## 從[!DNL Content]翻譯 {#translate-from-content}

當您瀏覽已核准的體驗時，也可以從[!DNL Content]開始翻譯。

### 從體驗收藏館

![翻譯內容收藏館中的體驗動作](./translate-content-gallery.png){width="500" zoomable="yes"}

**若要從體驗庫**&#x200B;翻譯：

1. 在[!DNL Content]中，開啟&#x200B;**[!UICONTROL 體驗]**&#x200B;索引標籤。
1. 找到您要翻譯的已核准體驗。
1. 按一下體驗卡上的選項（三個點）選單。
1. 按一下&#x200B;**[!UICONTROL 翻譯]**。
1. 從支援的語言清單中選取目標語言。 按一下&#x200B;**[!UICONTROL 翻譯]**。

## 在畫布上處理翻譯

在HTML畫布上，無法編輯來源體驗，因為它已核准。 電子郵件來源體驗似乎已鎖定。 您可以直接在畫布上編輯翻譯後的變體文字。 如需編輯變體副本的指引，請參閱[管理變體](/help/user-guide/create/manage-variants.md)。

翻譯的體驗不會執行品牌驗證或顯示品牌分數。 來源體驗已使用品牌指南建立、審查和核准。

翻譯的體驗不支援片段重新產生。

### 刪除翻譯的語言

**若要從畫布移除翻譯語言**：

1. 在[!DNL Create]畫布上，按一下翻譯後變體標題上的選項（三個點）功能表。
1. 按一下&#x200B;**[!UICONTROL 刪除]**。

![從畫布中刪除翻譯語言](./remove-translation-variant.png){width="500" zoomable="yes"}

翻譯的語言會從畫布中移除。

### 重新整理付費媒體翻譯

編輯已翻譯的付費媒體副本後，您可以重新載入原始翻譯輸出。

**若要重新整理付費媒體翻譯**：

1. 在[!DNL Create]畫布上，開啟已編輯翻譯變體上的選項功能表。
1. 按一下&#x200B;**[!UICONTROL 重新整理翻譯]**。

>[!NOTE]
>
>重新整理翻譯適用於付費媒體體驗。 電子郵件翻譯目前不支援重新整理翻譯。

## 匯出、檢閱和發佈

在畫布上載入翻譯後，您可以匯出、傳送它們以供核准，以及將已核准的變體發佈到[!DNL Content]。

**若要匯出翻譯的體驗**：

1. 在[!DNL Create]畫布上，按一下工具列中的&#x200B;**[!UICONTROL 匯出]**。
1. 選取匯出格式。
   * 電子郵件： **CSV和影像**&#x200B;或僅限&#x200B;**HTML**
   * 付費媒體： **CSV + JPG**、**CSV + PNG**&#x200B;或&#x200B;**HTML +影像**
1. 按一下&#x200B;**[!UICONTROL 匯出]**。

您也可以[從 [!DNL Content]](/help/user-guide/content/manage-assets.md#export-experiences)匯出體驗。

**若要要求檢閱與核准**：

1. 在[!DNL Create]畫布上，按一下&#x200B;**[!UICONTROL 要求核准]**。
1. 至少指派一位核准者並傳送請求。

如需稽核工作流程的詳細資訊，請參閱[要求稽核和核准](/help/user-guide/approvals/request-review.md)。

**若要發佈已核准的翻譯**：

1. 核准者核准轉譯的變體後，請按一下&#x200B;**[!UICONTROL 發佈]**。
1. 在發佈視窗中，確認中繼資料，例如行銷活動名稱、時間範圍、地區和關鍵字。

請參閱[發佈核准的內容](/help/user-guide/approvals/publish-content.md)。

每個已發佈的翻譯都會另存至[!DNL Content]做為個別體驗。

## 翻譯的體驗中繼資料

已發佈的翻譯包含中繼資料，可將每個變體連結回其來源，包括：

* **標題** — 遵循模式`Translation from "<source title>" <channel>`，例如`Translation from "Summer campaign" Meta`
* **建立者** — 啟動翻譯的使用者
* **建立日期** — 翻譯日期
* **已翻譯的來源** — [!DNL Content]中的來源體驗連結
* **翻譯自** — 來源語言

## 限制

當您在HTML畫布上翻譯體驗時，請記住下列限制：

* 來源體驗必須已核准並儲存在[!DNL Content]。
* 品牌驗證不會在轉譯的變體上執行。
* 翻譯的體驗不支援片段重新產生。
* 重新整理翻譯僅適用於付費媒體。

## 相關資訊

* [電子郵件體驗](/help/user-guide/create/email-experiences.md)
* [Meta體驗](/help/user-guide/create/meta-experiences.md)
* [顯示廣告體驗](/help/user-guide/create/display-ad-experiences.md)
* [管理資產和體驗](/help/user-guide/content/manage-assets.md)
* [尋找翻譯延伸模組](/help/extensibility/deploy-app.md#find-translation-extensions)
