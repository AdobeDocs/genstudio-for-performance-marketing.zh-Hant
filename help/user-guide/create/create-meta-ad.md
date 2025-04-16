---
title: 建立中繼廣告體驗
description: 瞭解如何使用Adobe GenStudio for Performance Marketing建立Facebook或Instagram的品牌內中繼廣告體驗。
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 42111bbf-70cd-4fd2-a7a9-15abe072d720
source-git-commit: a9da9ba1e93335896640e52837cc7226ec8e4bef
workflow-type: tm+mt
source-wordcount: '1102'
ht-degree: 0%

---

# 建立中繼廣告體驗

此教學課程示範如何使用GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md)產生品牌化[中繼廣告體驗](/help/user-guide/create/meta-experiences.md) （左側導覽區域中的繪圖筆刷圖示）。

開始產生中繼廣告體驗之前，請務必[在GenStudio for Performance Marketing中納入指引](/help/user-guide/guidelines/add-guidelines.md)，並熟悉[建立提示](/help/user-guide/effective-prompts.md)的基本知識。

## 選擇範本

若要開始產生新的中繼廣告體驗，請使用可用的範本為您的內容提供框架。 請參閱[範本最佳實務](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines)，以取得支援的中繼廣告外觀比例的相關資訊。

**若要選擇中繼廣告範本**：

1. 在&#x200B;_[!DNL Create]_中，按一下&#x200B;**[!UICONTROL 中繼廣告]**。
1. 使用&#x200B;_篩選器_&#x200B;旁的搜尋選項來尋找特定的中繼廣告範本。
1. 按兩下以選取範本，然後按兩下 **[!UICONTROL 使用]**。

   此作將打開畫布，它是創建內容的中心樞紐。

## 新增參數

[在提示抽屜的参数&#x200B;_中添加_&#x200B;指南](/help/user-guide/guidelines/overview.md)和資產可增強內容生成過程，並且是準備生成元廣告的關鍵步驟。

如果您使用的是具有預定義準則---[!DNL Brands][!DNL Personas]或[!DNL Products]---這些準則適用於您的變體的範本。您可以視需要加以變更。

**若要新增引數和資產**：

1. 按一下&#x200B;_引數_&#x200B;圖示以展開提示抽屜。
1. 在&#x200B;_引數_&#x200B;區段中，選取指導方針 — [!DNL Brands]、[!DNL Personas]和[!DNL Products] — 以通知內容建立。

   ![選擇角色](/help/assets/persona-select.png){width="600" zoomable="yes"}

   如果這些功能表中沒有可用的品牌、角色或產品， [請將指南添加到您的 GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md)。

1. 新增內容以用於體驗&#x200B;*和*，以影響內容產生：
   * 按一下&#x200B;**[!UICONTROL 從「內容」選取]**，從[!DNL Content]存放庫選取資產（影像）、篩選並選取一或多個影像。

     ![選擇視覺內容](/help/assets/content-select-meta.png){width="500" zoomable="yes"}

     若要使用已連線[!DNL AEM Assets Content Hub]存放庫中的資產，請從&#x200B;_位置_&#x200B;下拉式選單中選擇存放庫。 篩選並選取一或多個影像。

   * 或者，將資產拖放至&#x200B;**[!UICONTROL 從內容選取]**&#x200B;區段，以上傳一或多個新資產。
1. 按一下&#x200B;**[!UICONTROL 使用]**。

新增完引數後，您可以再次按一下&#x200B;_引數_&#x200B;圖示來收合提示抽屜。

## 輸入提示

選取准則後，使用自然語言製作提示，以開始為您新的中繼廣告體驗產生內容。 詳細提示產生比模糊或模稜兩可的提示更高的品質輸出。

請參閱[撰寫有效提示](/help/user-guide/effective-prompts.md)，深入瞭解撰寫提示的相關資訊。

**要輸入提示**：

1. 在 _「描述您要生成的體驗」_ 提示框中輸入提示。
1. 按一下&#x200B;**[!UICONTROL 產生]**。

默認情況下，四個變體（全部由您添加的提示、指南和內容推動）將生成並顯示在畫布中。

生成的內容會逐步載入 - 隨著元體驗的每個部分的生成，它們將顯示在畫布中。 請參閱 [Meta體驗](/help/user-guide/create/meta-experiences.md#progressive-loading) 以瞭解這些變更在畫布中的載入方式。

## 選擇中繼廣告頻道

產生中繼廣告時，您可以在Facebook或Instagram廣告之間選擇。

在右側功能表欄（Facebook 和 Instagram 圖示）中切換 Meta 廣告通道選項 **（在 Facebook** 和 **Instagram** 之間），以查看和管理每個通道的變體。

修改 Meta 廣告](#revise-generated-variants)時[，您可以更改 Facebook 和 Instagram 廣告的外觀比例。

## 修改生成的變型

在選擇要發送以供審批或發佈 [!DNL Content] 的內容之前，您可以編輯 Meta 廣告或從生成的廣告集中刪除變體。

若要反白要修訂的各個圖層，請按一下可編輯的欄位或影像，然後按一下&#x200B;_[!UICONTROL 檢檢視層]_。

**若要修訂產生的變體**：

* **若要[編輯中繼廣告草稿名稱](/help/user-guide/create/manage-variants.md#change-draft-name)**，請按一下畫布頂端的&#x200B;_未命名的草稿_&#x200B;標題，然後輸入新標題。
* **若要[手動編輯中繼廣告](/help/user-guide/create/manage-variants.md#manually-edit-text)**，請按一下任何廣告區段(例如主旨列、
頁首或內文)，並視需要編輯。
* **若要變更或選取呼叫動作**，請按一下call-to-action按鈕，然後從可用的按鈕文字選項中選取。 在&#x200B;_連結_&#x200B;中，輸入call-to-action文字的URL。
<!-- **To [change or select the Call to action](/help/user-guide/create/manage-variants.md#revise-call-to-action)**, click the call-to-action button and select _[!UICONTROL Rephrase]_ or _[!UICONTROL Add link]_. -->
* **要向變體](/help/user-guide/create/manage-variants.md#add-image-link)**&#x200B;中的圖像添加連結，請按兩下[圖像資產（如果圖像當前不存在，則按兩下圖像資產區域），然後按下連結圖示。
* **要重新生成變體的一部分，請按下[可編輯文字欄位並使用建議的編輯&#x200B;]_選項，_[!UICONTROL 或輸入新提示並按兩下**[!UICONTROL &#x200B;生成&#x200B;]**。](/help/user-guide/create/manage-variants.md#re-generate-sections)**
* **要在变體](/help/user-guide/create/manage-variants.md#swap-image)**&#x200B;中添加或交換圖像，請按兩下[圖像資產（如果當前不存在圖像，則按兩下圖像資產區域），然後按兩下&#x200B;**[!UICONTROL “從內容]**&#x200B;交換”圖示。
* **若要裁剪或重新定位圖像](/help/user-guide/create/manage-variants.md#crop-assets)**，請將[滑鼠懸停在圖像上，按兩下出現的裁剪圖示，然後調整圖像大小和刊登。
* **要刪除 Meta 廣告，請按下[變體的選項選單，然後按下**[!UICONTROL &#x200B;刪除變體&#x200B;]**。](/help/user-guide/create/manage-variants.md#delete-variant)**

## 提交產生回饋

若要[提交關於產生輸出品質的意見反應](/help/user-guide/create/manage-variants.md#generation-feedback)，請按一下選項圖示（三個點）並選取&#x200B;**[!UICONTROL 輸出良好]**&#x200B;或&#x200B;**[!UICONTROL 輸出不良]**。

## 驗證內容檢查對齊情況

為了優化生成的變體並確保嚴格遵守品牌識別、平臺指南和輔助功能標準，善用內容檢查&#x200B;_面板](/help/user-guide/guidelines/brand-validation.md#content-check-panel)的強大[_&#x200B;功能。此面板顯示全面的內容檢查詳細資訊並闡明改進區域。

**要對多屬性**&#x200B;執行內容檢查，請執行以下作：

1. 按一下右側動作列中的&#x200B;_內容檢查_&#x200B;面板圖示以開啟&#x200B;[_內容檢查_&#x200B;面板](/help/user-guide/guidelines/brand-validation.md#content-check-panel)。 檢視&#x200B;*需要稽核*&#x200B;和&#x200B;*通過*&#x200B;檢查的摘要，以檢視哪些區段和准則需要改進。

   ![_內容檢查_&#x200B;面板](/help/assets/content-check-panel.png){height="400" zoomable="yes"}

1. [手動修訂變體](#revise-generated-variants)以確保您的變體與執行的內容檢查緊密對齊。

請參閱[品牌驗證](/help/user-guide/guidelines/brand-validation.md)。

## 取得檢閱和核准

使用核准面板（可在畫布的右側動作列上以圖示方式存取），以取得稽核、追蹤稽核評論及取得利害關係人的核准。

**若要取得稽核與核准**：

1. [啟動核准要求](/help/user-guide/approvals/request-review.md)以徵求[草擬中繼廣告體驗的核准](/help/user-guide/approvals/approve-content.md)。

   ![傳送草稿以供檢閱和核准](/help/assets/send-approval-meta.png){width="450" zoomable="yes"}

1. [在稽核程式期間移除或新增稽核者](/help/user-guide/approvals/review-and-edit.md#manage-approvals)。
1. [存取內容以供檢閱](/help/user-guide/approvals/review-and-edit.md#access-content-for-review)並檢視修訂要求。
1. 編輯每個評論評論的草稿，並 [發佈您的 Meta 廣告體驗](#publish-and-export-experience)。

有關詳細資訊，請參閱 [審核和批准](/help/user-guide/approvals/overview.md) 。

## Publish和導出體驗

要使生成的 Meta 廣告可供當前和未來使用，請將其發佈內容並匯出以用於您的行銷廣告系列。

1. **要發佈您的新 Meta 廣告體驗**，請按兩下頂部工具列中的Publish ]**，或在審批流程中按兩下**[!UICONTROL 。
1. **若要匯出您新的中繼廣告體驗**，請按一下頂端工具列中的&#x200B;**[!UICONTROL 匯出]**。
   1. 選取格式 — HTML和影像或CSV和影像(JPG或PNG) — 按一下「匯出&#x200B;**[!UICONTROL 」]**。

有關詳細資訊，請參閱 [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) 。

## 連接元

您可以將效果行銷的GenStudio 連接到元維琪，以接收有關內容績效的高級分析和見解。

請參閱 [元廣告連接](/help/user-guide/connectors/connect-channel.md#meta-ads-connect)。
