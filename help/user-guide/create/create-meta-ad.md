---
title: 建立Meta廣告體驗
description: 瞭解如何使用Adobe GenStudio for Performance Marketing建立品牌上Meta廣告體驗（適用於Facebook或Instagram）。
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 42111bbf-70cd-4fd2-a7a9-15abe072d720
source-git-commit: d3ddbefc47d3289041783a1a277aa2e855d13ccb
workflow-type: tm+mt
source-wordcount: '1393'
ht-degree: 0%

---

# 建立Meta廣告體驗

此教學課程示範如何使用GenStudio for Performance Marketing [產生品牌化](/help/user-guide/create/meta-experiences.md)Meta廣告體驗[[!DNL Create]](/help/user-guide/create/overview.md) （左側導覽區域中的繪圖筆刷圖示）。

開始產生Meta廣告體驗之前，請務必[在GenStudio for Performance Marketing中納入指引](/help/user-guide/guidelines/add-guidelines.md)，並熟悉[建立提示](/help/user-guide/effective-prompts.md)的基本知識。

## 選擇範本

若要開始產生新的Meta廣告體驗，請使用可用的範本為您的內容提供架構。 請參閱[Meta廣告範本指導方針](/help/user-guide/templates/meta-template.md)，以取得支援的Meta廣告外觀比例相關資訊。

選取範本時，您可以選擇使用其中一個已上傳的範本或入門範本。

**若要選擇Meta廣告範本**：

1. 在&#x200B;_[!DNL Create]_中，按一下&#x200B;**[!UICONTROL Meta廣告]**。
1. 選取&#x200B;**[!UICONTROL 自訂範本]**&#x200B;以瀏覽您上傳的範本，或選取&#x200B;**[!UICONTROL 入門範本]**&#x200B;以瀏覽預先建立的範本。

   如果您打算將視訊資產新增至您的Meta變體，則必須選擇入門範本。 它們會預先載入系統定義的內容區域，以方便視訊的使用。

1. 按一下以選取範本，然後按一下&#x200B;**[!UICONTROL 使用]**。

   此動作會開啟畫布，這是內容建立的中心樞紐。

## 新增引數

在提示抽屜中新增[指南](/help/user-guide/guidelines/overview.md)和&#x200B;_引數_&#x200B;中的資產，可強化內容產生程式，是準備產生Meta廣告的重要步驟。

如果您使用具有預先定義指引（例如[!DNL Brands]、[!DNL Personas]或[!DNL Products]）的範本，這些指引適用於您的變體。 如有需要，您可以加以變更。

**若要新增引數和資產**：

1. 按一下&#x200B;_引數_&#x200B;圖示以展開提示抽屜。
1. 在&#x200B;_引數_&#x200B;區段中，選取指導方針 — [!DNL Brands]、[!DNL Personas]和[!DNL Products] — 以通知內容建立。

   ![選擇角色](/help/assets/persona-select-meta.png){width="300" align="center" zoomable="yes"}

   如果這些功能表中沒有可用的品牌、角色或產品，請[將准則新增至您的GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md)。

1. 新增內容（影像或視訊）以用於體驗&#x200B;*和*，以影響內容產生：
   * 按一下&#x200B;**[!UICONTROL 從內容中選取]**&#x200B;以從您的[!DNL Content]存放庫選取資產、篩選並選取一或多個影像。

     如果您使用的範本有視訊區段，系統會預先選取並篩選視訊內容(.mp4)。 將滑鼠指標暫留在視訊上，檢視自動播放的預覽。

     ![選擇視覺內容](/help/assets/content-select-meta.png){width="500" zoomable="yes"}

     若要使用已連線[!DNL AEM Assets Content Hub]存放庫中的資產，請從&#x200B;_位置_&#x200B;下拉式選單中選擇存放庫。 篩選並選取一或多個影像。

   * 或者，將影像拖放至&#x200B;**[!UICONTROL 從內容選取]**&#x200B;區段，以上傳一或多個新資產。

1. 按一下&#x200B;**[!UICONTROL 使用]**。

新增完引數後，您可以再次按一下&#x200B;_引數_&#x200B;圖示來收合提示抽屜。

## 輸入提示

選取准則後，請使用自然語言製作提示，以開始為您新的Meta廣告體驗產生內容。 詳細提示產生比模糊或模稜兩可的提示更高的品質輸出。

請參閱[撰寫有效提示](/help/user-guide/effective-prompts.md)，深入瞭解撰寫提示的相關資訊。

**若要輸入提示**：

1. 在&#x200B;_「描述您要產生的體驗」_&#x200B;提示方塊中輸入提示。
1. 按一下&#x200B;**[!UICONTROL 產生]**。

   請參閱[管理視訊](#manage-videos)，瞭解其產生方式及管理方式。

依預設，會產生四個變數（全部由您新增的提示、指引和內容所推動），並顯示在畫布中。

產生的內容會以漸進方式載入，當Meta體驗的每個區段產生時，都會顯示在畫布中。 請參閱[Meta體驗](/help/user-guide/create/meta-experiences.md#progressive-loading)，瞭解如何在畫布中載入這些變更。

## 選擇Meta廣告頻道

產生Meta廣告時，您可以選擇Facebook或Instagram廣告。

切換右側功能表列（Facebook和Instagram圖示）中的Meta廣告頻道選項（在&#x200B;**Facebook**&#x200B;和&#x200B;**Instagram**&#x200B;之間），以檢視和管理每個頻道的變體。

[修改Meta廣告](#revise-generated-variants)時，您可以變更Facebook和Instagram廣告的外觀比例。

## 修訂產生的變體

在選取要傳送以進行核准或發佈至[!DNL Content]的內容之前，您可以編輯Meta廣告或從產生的廣告集中刪除變體。

若要反白要修訂的各個圖層，請按一下可編輯的欄位或影像，然後按一下&#x200B;_[!UICONTROL 檢檢視層]_。

**若要修訂產生的變體**：

* **若要[編輯Meta廣告草稿名稱](/help/user-guide/create/manage-variants.md#change-draft-name)**，請按一下畫布頂端的&#x200B;_未命名的草稿_&#x200B;標題，然後輸入新標題。
* **若要[手動編輯Meta廣告](/help/user-guide/create/manage-variants.md#manually-edit-text)**，請按一下任何廣告區段(例如主旨列、
頁首或內文)，並視需要編輯。
* **若要變更或選取call to action**，請按一下call-to-action按鈕，然後從可用的按鈕文字選項中選取。 在&#x200B;_連結_&#x200B;中，輸入call-to-action文字的URL。
* **若要在變體中[套用文字格式](/help/user-guide/create/manage-variants.md#manually-edit-text)**，請按一下變體的影像上文字或內嵌連結，然後按一下&#x200B;**[!UICONTROL 格式化文字]**。
<!-- **To [change or select the Call to action](/help/user-guide/create/manage-variants.md#revise-call-to-action)**, click the call-to-action button and select _[!UICONTROL Rephrase]_ or _[!UICONTROL Add link]_. -->
* **若要[新增連結至變體中的影像](/help/user-guide/create/manage-variants.md#add-image-link)**，請按一下影像資產（如果影像目前不存在，則按一下影像資產區域），然後按一下連結圖示。
* **若要[變更廣告](/help/user-guide/create/manage-variants.md#change-aspect-ratio)**&#x200B;的大小與外觀比例，請按一下&#x200B;_[!UICONTROL 調整大小]_&#x200B;按鈕（在畫布左邊有按鈕圖示的方塊），然後選取要套用至所有變體的新大小與外觀比例。 變數會複製並調整大小。
* **若要[重新產生變體](/help/user-guide/create/manage-variants.md#re-generate-sections)**&#x200B;的區段，請按一下可編輯的文字欄位並使用&#x200B;_[!UICONTROL 建議的編輯]_&#x200B;選項，或輸入新的提示並按一下&#x200B;**[!UICONTROL 產生]**。
* **若要[新增或交換變體中的影像](/help/user-guide/create/manage-variants.md#swap-image)**，請按一下影像資產（如果影像目前不存在，則按一下影像資產區域），然後按一下&#x200B;**[!UICONTROL 從內容交換]**&#x200B;圖示。
* **若要[裁切或重新定位影像](/help/user-guide/create/manage-variants.md#crop-assets)**，請按一下影像，按一下&#x200B;**[!UICONTROL 編輯]** （鉛筆圖示），然後按一下&#x200B;**[!UICONTROL 裁切]**。 調整影像大小和位置。
* **要[使用[產生式展開]以調整影像大小並符合您的工作範本](/help/user-guide/create/manage-variants.md#use-generative-expand)**，按一下影像，按一下[編輯]**[!UICONTROL （鉛筆圖示），然後]**&#x200B;展開&#x200B;**[!UICONTROL 。]**&#x200B;調整影像以符合所需的外觀比例和範本。
* **若要[為變體中的影像新增替代文字](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)**，請按一下影像資產，並使用&#x200B;_替代文字_&#x200B;選項來手動新增或產生每個影像的替代文字。
* **若要[新增協助工具標籤](/help/user-guide/create/manage-variants.md#add-accessibility-labels)至您的變體**，請按一下影像或call-to-action連結，然後提供簡短說明，說明連結或按鈕的作用。
* **若要[刪除Meta廣告](/help/user-guide/create/manage-variants.md#delete-variant)**，請按一下變體的選項功能表，然後按一下&#x200B;**[!UICONTROL 刪除變體]**。

### 管理影片

將滑鼠停留在每個影片上，檢視循環的自動播放。

視訊會在產生期間重新設定影格，以符合選取的外觀比例。 按一下&#x200B;**[!UICONTROL 重新設定視訊]**&#x200B;並切換為關閉視訊，即可回覆成未重新設定影格的視訊。

## 提交產生回饋

若要[提交關於產生輸出品質的意見反應](/help/user-guide/create/manage-variants.md#generation-feedback)，請按一下選項圖示（三個點）並選取&#x200B;**[!UICONTROL 輸出良好]**&#x200B;或&#x200B;**[!UICONTROL 輸出不良]**。

## 驗證內容檢查對齊方式

若要最佳化產生的變體，並確保嚴格遵守品牌識別、平台指引及協助工具標準，請利用&#x200B;[_內容檢查_&#x200B;面板](/help/user-guide/guidelines/brand-validation.md#content-check-panel)的強大功能。 此面板會顯示完整的內容檢查詳細資訊，並闡明改善領域。

**若要對變體**&#x200B;執行內容檢查：

1. 按一下右側動作列中的&#x200B;_內容檢查_&#x200B;面板圖示以開啟&#x200B;[_內容檢查_&#x200B;面板](/help/user-guide/guidelines/brand-validation.md#content-check-panel)。 檢視&#x200B;*需要稽核*&#x200B;和&#x200B;*通過*&#x200B;檢查的摘要，以檢視哪些區段和准則需要改進。

   ![_內容檢查_&#x200B;面板](/help/assets/content-check-panel.png){height="400" zoomable="yes"}

1. [手動修訂變體](#revise-generated-variants)以確保您的變體與執行的內容檢查緊密對齊。

請參閱[品牌驗證](/help/user-guide/guidelines/brand-validation.md)。

## 取得檢閱和核准

使用核准面板（可在畫布的右側動作列上以圖示方式存取），以取得稽核、追蹤稽核評論及取得利害關係人的核准。

**若要取得稽核與核准**：

1. [啟動核准要求](/help/user-guide/approvals/request-review.md)以徵求[草擬的Meta廣告體驗核准](/help/user-guide/approvals/approve-content.md)。

   ![傳送草稿以供檢閱和核准](/help/assets/send-approval-meta.png){width="450" zoomable="yes"}

1. [在稽核程式期間移除或新增稽核者](/help/user-guide/approvals/review-and-edit.md#manage-approvals)。
1. [存取內容以供檢閱](/help/user-guide/approvals/review-and-edit.md#access-content-for-review)並檢視修訂要求。
1. 編輯每次評論的草稿，並[發佈您的Meta廣告體驗](#publish-and-export-experience)。

如需詳細資訊，請參閱[檢閱與核准](/help/user-guide/approvals/overview.md)。

## 發佈和匯出體驗

若要讓產生的Meta廣告可供目前和未來使用，請將它發佈至[!UICONTROL 內容]，並匯出以用於您的行銷活動。

1. **若要發佈新的Meta廣告體驗**，請按一下頂端工具列或核准流程中的&#x200B;**[!UICONTROL 發佈]**。
1. **若要匯出您新的Meta廣告體驗**，請按一下頂端工具列中的「**[!UICONTROL 匯出]**」。
   1. 選取格式 — HTML和影像或CSV和影像(JPG或PNG) — 按一下「匯出&#x200B;**[!UICONTROL 」]**。

如需詳細資訊，請參閱[[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content)。

## 連線Meta

您可以將GenStudio for Performance Marketing連線至Meta，接收進階分析和內容效能的深入分析。

請參閱[Meta廣告連線](/help/user-guide/connectors/meta-ads.md)。
