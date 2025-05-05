---
title: 建立LinkedIn體驗
description: 瞭解如何使用 品牌 GenStudio for Performance Marketing Adobe Systems創建符合LinkedIn體驗。
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
badgeBeta: label="試用版" tooltip="此功能目前正在Beta中，因此某些功能可能會受到限制或可能發生變化。"
recommendations: noDisplay
exl-id: abe10fc8-d6d5-4cad-9273-400b622f22b7
source-git-commit: d5019f1cdceccb8ce2fdd86c54cf2d36673a90aa
workflow-type: tm+mt
source-wordcount: '914'
ht-degree: 0%

---

# 建立LinkedIn體驗

本教學課程演示如何使用 [&#128279;](/help/user-guide/create/meta-experiences.md)GenStudio 進行績效營銷[[!DNL Create]](/help/user-guide/create/overview.md)（左側導覽區域中的畫筆圖示）生成符合品牌準則的LinkedIn體驗。

在開始生成LinkedIn廣告之前，[請務必在 GenStudio 中為效果行銷添加指南](/help/user-guide/guidelines/add-guidelines.md)並學習創建提示[&#128279;](/help/user-guide/effective-prompts.md)的基礎知識。

## 選擇一個範本

若要生成新的LinkedIn體驗，需要一個範本來提供內容框架。 有關支援的LinkedIn外觀比例的資訊，請參閱 [範本](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) 的最佳實踐。

**要選擇LinkedIn範本**：

1. 在&#x200B;_[!DNL Create]_&#x200B;中，按一下&#x200B;**[!UICONTROL LinkedIn]**。
1. 使用&#x200B;_篩選器_&#x200B;旁的搜尋選項來尋找特定範本。
1. 按一下以選取範本，然後按一下[使用]。**&#x200B;**

   此動作會開啟畫布，這是內容建立的中心樞紐。

## 新增引數

[在提示抽屜的参数&#x200B;_中添加_&#x200B;指南](/help/user-guide/guidelines/overview.md)和資產可增強內容生成過程，並且是準備生成LinkedIn體驗的關鍵步驟。

**若要新增参数和資產**：

1. 按兩下「 _參數」_ 圖示以展開提示抽屜。
1. 在“参数”__&#x200B;部分中，選擇準則 （、[!DNL Personas][!DNL Brands]） 和 [!DNL Products]— 以通知內容創建。

   ![選擇角色](/help/assets/persona-select.png){width="600" zoomable="yes"}

   如果這些功能表中沒有可用的品牌、角色或產品，請[將准則新增至您的GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md)。

1. 新增內容以便在體驗 *中使用并* 影響內容產生：
   * 按兩下從 **[!UICONTROL 內容]** 中選擇以從 [!DNL Content] 存放庫中選擇資產（圖像），過濾並選擇一個或多個圖像。

     ![選擇視覺內容](/help/assets/content-select-meta.png){width="500" zoomable="yes"}

     要使用已連接[!DNL AEM Assets Content Hub]存放庫中的資產，請從位置&#x200B;__&#x200B;下拉菜單中選擇存放庫。篩選並選擇一個或多個圖像。

   * 或者，將資產拖放到“ **[!UICONTROL 從內容]** 中選擇”部分以上傳一個或多個新資產。
1. 按兩下 **[!UICONTROL 使用]**。

添加完參數后，可以通過再次按兩下 _「參數_ 」圖示來摺疊提示抽屜。

## 輸入提示

選擇指南后，使用自然語言制作提示，以開始為新LinkedIn體驗生成內容。 詳細的提示可確保您收到良好的品質和有用的輸出。

請參閱 [編寫有效提示](/help/user-guide/effective-prompts.md) 以瞭解有關編寫提示的詳細資訊。

**若要輸入提示**：

1. 在&#x200B;_「描述您要產生的體驗」_&#x200B;提示方塊中輸入提示。
1. 按一下&#x200B;**[!UICONTROL 產生]**。

依預設，會產生四個變數（全部由您新增的提示、指引和內容所推動），並顯示在畫布中。

產生的內容會以漸進方式載入 — 當LinkedIn體驗的每個區段產生時，都會顯示在畫布中。 請參閱[LinkedIn體驗](/help/user-guide/create/linkedin-experiences.md#progressive-loading)，瞭解如何在畫布中載入這些變更。

## 修改產生的LinkedIn廣告

在傳送變體以供核准或發佈到[!DNL Content]之前，您可以編輯LinkedIn廣告或從產生的廣告集中刪除變體。

**若要修訂產生的變體**：

* **若要[編輯LinkedIn廣告草稿名稱](/help/user-guide/create/manage-variants.md#change-draft-name)**，請按一下畫布頂端的&#x200B;_未命名的草稿_&#x200B;標題，然後輸入新標題。
* **若要[手動編輯LinkedIn廣告](/help/user-guide/create/manage-variants.md#manually-edit-text)**，請按一下任何廣告區段（例如主旨列、標題或內文）並視需要編輯。
* **要更改或選擇號召性用語**，請按兩下號召性用語按鈕，然後從可用的按鈕文本選項中進行選擇。 在“連結”_中_，輸入號召性用語文本的URL。
* **要重新生成變體的一部分，請按下[可編輯的文字欄位並使用建議的&#x200B;]_編輯選項，_[[!UICONTROL 或在 _[!UICONTROL 生成新text_ 部分中]輸入新提示，然後按兩下**&#x200B;[!UICONTROL &#x200B;生成&#x200B;]&#x200B;**。]](/help/user-guide/create/manage-variants.md#re-generate-sections)**
* **若要裁剪或重新定位圖像[&#128279;](/help/user-guide/create/manage-variants.md#crop-assets)**，請將滑鼠懸停在圖像上，按兩下出現的裁剪圖示，然後調整圖像大小和刊登。
* **要 [刪除LinkedIn廣告](/help/user-guide/create/manage-variants.md#delete-variant)**，請單擊多屬性的選項功能表，然後按下 **[!UICONTROL 刪除多屬性]**。

## 提交生成反饋

要提交有關生成輸出品質的反饋，請按下[選項圖示（三個點），然後選擇&#x200B;**[!UICONTROL 良好輸出]**&#x200B;或&#x200B;**[!UICONTROL 差輸出]**。](/help/user-guide/create/manage-variants.md#generation-feedback)

## 驗證內容檢查對齊方式

若要最佳化產生的變體，並確保嚴格遵守品牌識別、平台指引及協助工具標準，請利用&#x200B;[_內容檢查_&#x200B;面板](/help/user-guide/guidelines/brand-validation.md#content-check-panel)的強大功能。 此面板會顯示完整的內容檢查詳細資訊，並闡明改善領域。

**若要對變體**&#x200B;執行內容檢查：

1. 按一下右側動作列中的&#x200B;_內容檢查_&#x200B;面板圖示以開啟&#x200B;[_內容檢查_&#x200B;面板](/help/user-guide/guidelines/brand-validation.md#content-check-panel)。 檢視&#x200B;*需要稽核*&#x200B;和&#x200B;*通過*&#x200B;檢查的摘要，以檢視哪些區段和准則需要改進。

   ![_內容檢查_ 面板](/help/assets/content-check-panel.png){height="400" zoomable="yes"}

1. [手動修改多屬性](#revise-generated-variants) ，以確保您的多屬性與執行的內容檢查緊密一致。

請参閱 [品牌驗證](/help/user-guide/guidelines/brand-validation.md)。

## 獲得評論和批准

使用「核准」面板（可從畫布的頂端功能表列存取）來取得稽核、追蹤稽核評論，以及取得利害關係人的核准。

**要獲得審核和批准**，請執行以下作：

1. [Launch批准請求](/help/user-guide/approvals/request-review.md) ，以徵求 [草擬的 Meta 廣告體驗](/help/user-guide/approvals/approve-content.md)的批准。

   ![傳送草稿以供審閱和批准](/help/assets/send-approval-meta.png){width="450" zoomable="yes"}

1. [在審核過程中移除或添加審閱者](/help/user-guide/approvals/review-and-edit.md#manage-approvals) 。
1. [存取 內容 進行審核](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) ，並視圖修訂請求。
1. 編輯每個評論評論的草稿，並 [發佈您的 Meta 廣告體驗](#publish-and-export-experience)。

有關詳細資訊，請參閱 [審核和批准](/help/user-guide/approvals/overview.md) 。

## Publish和導出體驗

要使生成的LinkedIn廣告可供當前和將來使用，請將其發佈內容，然後匯出以用於行銷廣告系列。

1. **若要發佈新體驗**，請按兩下 **[!UICONTROL 頂部工具列中或審批流程中的Publish]** 。
1. **要導出新體驗**，請按兩下 **[!UICONTROL 頂部工具列中的導出]** 。
   1. 選取格式(JPG、PNG或GIF)，然後按一下「匯出」**&#x200B;**。

如需詳細資訊，請參閱[[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content)。
