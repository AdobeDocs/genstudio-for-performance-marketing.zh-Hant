---
title: 建立顯示廣告體驗
description: 瞭解如何在Adobe [!DNL GenStudio] 中建立效能行銷的顯示廣告體驗。
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 7d5e777b-7a30-48f4-b253-9823e38eecce
source-git-commit: f49a2bd241f98dda23f6612f8c699ec49d222a12
workflow-type: tm+mt
source-wordcount: '1052'
ht-degree: 0%

---

# 建立顯示廣告體驗

此教學課程示範如何使用GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md)產生品牌化[顯示廣告體驗](display-ad-experiences.md) （左側導覽區域中的繪圖筆刷圖示）。

若要設計吸引人的顯示廣告體驗，建議您[將指引新增至GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md)，並在開始前檢閱[撰寫提示的基本知識](/help/user-guide/effective-prompts.md)。

## 選擇範本

若要建立顯示廣告體驗，請使用可用的範本為您的內容提供架構。 請參閱[範本最佳實務](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines)，以取得支援的顯示廣告維度相關資訊。

**若要選擇顯示廣告範本**：

1. 在&#x200B;_[!DNL Create]_&#x200B;中，按一下&#x200B;**[!UICONTROL 顯示廣告]**。
1. 使用&#x200B;_篩選器_&#x200B;旁的搜尋選項來尋找特定的顯示廣告範本。
1. 在&#x200B;_選取範本_&#x200B;檢視中，按一下顯示廣告範本。
1. 按一下&#x200B;**[!UICONTROL 使用]**。

   畫布是作為內容建立的中心樞紐，隨即顯示。

## 新增引數

在提示抽屜中新增[指南](/help/user-guide/guidelines/overview.md)和&#x200B;_引數_&#x200B;中的資產，會增加內容產生程式的費用，是產生顯示廣告體驗的必要準備步驟。

如果您使用具有預先定義指引（[!DNL Brands]、[!DNL Personas]或[!DNL Products]）的範本，這些指引適用於您的變體。 如有需要，您可以加以變更。

**若要新增引數和資產**：

1. 按一下&#x200B;_引數_&#x200B;圖示以展開提示抽屜。
1. 在&#x200B;_引數_&#x200B;區段中，選取指導方針 — [!DNL Brands]、[!DNL Personas]和[!DNL Products] — 以通知內容建立。

   如果這些功能表中沒有可用的品牌、角色或產品，請[將准則新增至您的GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md)。

1. 若要新增要在體驗&#x200B;*和*&#x200B;中使用的內容，以影響內容產生：
   * 按一下&#x200B;**[!UICONTROL 從「內容」選取]**，從[!DNL Content]存放庫選取資產（影像）、篩選並選取一或多個影像。

     若要使用已連線[!DNL AEM Assets Content Hub]存放庫中的資產，請從&#x200B;_位置_&#x200B;下拉式選單中選擇存放庫。 篩選並選取一或多個影像。

   * 或者，將資產拖放至&#x200B;**[!UICONTROL 從內容選取]**&#x200B;區段，以上傳一或多個新資產。
1. 按一下&#x200B;**[!UICONTROL 使用]**。

當您完成新增引數時，請再次按一下&#x200B;_引數_&#x200B;圖示來收合提示抽屜。

## 輸入提示

選取准則後，請使用自然語言製作提示，以開始為您的新顯示廣告體驗產生內容。 若要提高所產生顯示廣告體驗的品質，請務必製作詳盡的描述性提示。

![輸入提示](/help/assets/prompt-displayad.png){width="650" zoomable="yes"}

請參閱[撰寫有效提示](/help/user-guide/effective-prompts.md)，深入瞭解撰寫提示的相關資訊。

**若要輸入提示**：

1. 在&#x200B;_「描述您要產生的體驗」_&#x200B;提示方塊中輸入提示。
1. 按一下&#x200B;**[!UICONTROL 產生]**。

依照預設，會產生四個變數（由您新增的提示、指引和內容所驅動），並顯示在畫布中。

## 修訂產生的變體

在選取要傳送給核准或發佈至[!DNL Content]的內容之前，您可以編輯顯示廣告區段和文字欄位，或刪除產生的變體。

若要反白要修訂的各個圖層，請按一下可編輯的欄位或影像，然後按一下&#x200B;_[!UICONTROL 檢檢視層]_。

**若要修訂產生的變體**：

* **若要[編輯顯示廣告草稿名稱](/help/user-guide/create/manage-variants.md#change-draft-name)**，請按一下畫布頂端的&#x200B;_未命名的草稿_&#x200B;標題，然後輸入新標題。
* **若要[手動編輯顯示廣告](/help/user-guide/create/manage-variants.md#manually-edit-text)**，請連按兩下任何顯示廣告區段或欄位（例如主旨列、標題或內文）並視需要編輯。
* **若要[重新產生變體](/help/user-guide/create/manage-variants.md#re-generate-sections)**&#x200B;的區段，請按一下可編輯的文字欄位並使用&#x200B;_[!UICONTROL 建議的編輯]_&#x200B;選項，或在_[!UICONTROL 產生新文字_區段]中輸入新提示，然後按一下&#x200B;**[!UICONTROL 產生]**。
* **若要[新增或交換變體中的影像](/help/user-guide/create/manage-variants.md#swap-image)**，請按一下影像資產（如果影像目前不存在，則按一下影像資產區域），然後按一下&#x200B;**[!UICONTROL 從內容交換]**&#x200B;圖示。
* **若要[新增連結至變體中的影像](/help/user-guide/create/manage-variants.md#add-image-link)**，請按一下影像資產（如果影像目前不存在，則按一下影像資產區域），然後按一下連結圖示。
* **若要[為變體中的影像新增替代文字](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)**，請按一下影像資產，並使用&#x200B;_替代文字_&#x200B;選項來手動新增或產生每個影像的替代文字。
* **若要[變更廣告](/help/user-guide/create/manage-variants.md#change-aspect-ratio)**&#x200B;的大小與外觀比例，請按一下&#x200B;_[!UICONTROL 調整大小]_&#x200B;按鈕（在畫布左邊有按鈕圖示的方塊），然後選取要套用至所有變體的新大小與外觀比例。 變數會複製並調整大小。
* **若要[裁切或重新定位影像](/help/user-guide/create/manage-variants.md#crop-assets)**，請將滑鼠停留在影像上，按一下顯示的裁切圖示，然後調整影像大小和位置。 按一下「**[!UICONTROL 套用]**」。

<!-- # Preview for device
When revising and preparing email experiences, you can toggle between previews for desktop and mobile views to ensure coherence and visual appeal of draft variants.
**To preview variants for desktop and mobile devices** toggle the device preview option—between **desktop** and **mobile**—in the right menu bar (computer and phone icons) to preview how variants appear. -->

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

1. [啟動核准要求](/help/user-guide/approvals/request-review.md)以徵求[草擬顯示廣告體驗](/help/user-guide/approvals/approve-content.md)的核准。
1. [在稽核程式期間移除或新增稽核者](/help/user-guide/approvals/review-and-edit.md#manage-approvals)。
1. [存取內容以供檢閱](/help/user-guide/approvals/review-and-edit.md#access-content-for-review)並檢視修訂要求。
1. 編輯每次稽核評論的草稿，並[發佈您的顯示廣告體驗](#publish-and-export-experience)。

檢視[檢閱與核准](/help/user-guide/approvals/overview.md)。

## 發佈和匯出體驗

若要讓產生的顯示廣告可供目前和未來使用，請將它發佈至[!UICONTROL Content]，並匯出以用於您的行銷活動。

1. **若要發佈您的新顯示廣告體驗**，請按一下頂端工具列或核准流程中的&#x200B;**[!UICONTROL 發佈]**。
   1. 選取&#x200B;_[!UICONTROL [!DNL Campaigns]]_&#x200B;並新增&#x200B;_[!UICONTROL &#x200B;更多詳細資料&#x200B;]_（如有需要）。
   1. 點擊&#x200B;**[!UICONTROL 發佈]**。

      ![發佈顯示廣告](/help/assets/publish-displayad.png){width="450" zoomable="yes"}

1. **若要匯出您的新顯示廣告體驗**，請按一下頂端工具列中的[匯出]。**&#x200B;**
   1. 選取格式(HTML和影像、PNG或JPG)，然後按一下「匯出」**&#x200B;**。

      匯出的HTML應放置在預先定義的Web屬性中，例如範本或`div`容器。 如果沒有這些設定的尺寸，獨立檢視影像時，影像可能會扭曲。

請參閱[[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content)。
