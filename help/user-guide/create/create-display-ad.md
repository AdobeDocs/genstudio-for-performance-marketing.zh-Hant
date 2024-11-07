---
title: 建立顯示廣告體驗
description: 瞭解如何在Adobe [!DNL GenStudio] 中建立效能行銷的顯示廣告體驗。
feature: Brands Service, Guidelines, Content Generation, Generative AI, Create, Experiences, Variant Generation
role: User
level: Beginner
recommendations: noDisplay
source-git-commit: 5cd6abba1f56c9a2875c7e7dc5b94a353fc5e78e
workflow-type: tm+mt
source-wordcount: '849'
ht-degree: 0%

---

# 建立顯示廣告體驗

此教學課程示範如何使用GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md)產生品牌化[顯示廣告體驗](display-ad-experiences.md) （左側導覽區域中的繪圖筆刷圖示）。

若要設計吸引人的顯示廣告體驗，建議您[將指引新增至GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md)，並在開始前檢閱[撰寫提示的基本知識](/help/user-guide/effective-prompts.md)。

## 選擇範本

若要建立顯示廣告體驗，請使用可用的範本為您的內容提供架構。

**若要選擇顯示廣告範本**：

1. 在&#x200B;_[!DNL Create]_中，按一下_「您今天要建立什麼？」中的&#x200B;**[!UICONTROL 顯示廣告]**_節。
1. 使用&#x200B;_篩選器_&#x200B;旁的搜尋選項來尋找特定的顯示廣告範本。
1. 在&#x200B;_選取範本_&#x200B;檢視中，按一下顯示廣告範本。
1. 按一下&#x200B;**[!UICONTROL 使用]**。

   畫布是作為內容建立的中心樞紐，隨即顯示。

## 新增引數

在提示抽屜中新增[指南](/help/user-guide/guidelines/overview.md)和&#x200B;_引數_&#x200B;中的資產，會增加內容產生程式的費用，是產生顯示廣告體驗的必要準備步驟。

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

## 修訂產生的顯示廣告

在選取要傳送給核准或發佈至[!DNL Content]的內容之前，您可以編輯顯示廣告區段和文字欄位，或刪除產生的變體。

**若要修訂產生的變體**：

* **若要[編輯顯示廣告草稿名稱](/help/user-guide/create/manage-variants.md#change-draft-name)**，請按一下畫布頂端的&#x200B;_未命名的草稿_&#x200B;標題，然後輸入新標題。
* **若要[手動編輯顯示廣告](/help/user-guide/create/manage-variants.md#manually-edit-text)**，請連按兩下任何顯示廣告區段或欄位（例如主旨列、標題或內文）並視需要編輯。
* **若要[變更廣告](/help/user-guide/create/manage-variants.md#change-aspect-ratio)**&#x200B;的大小與外觀比例，請按一下&#x200B;_[!UICONTROL 調整大小]_&#x200B;按鈕（在畫布左邊有按鈕圖示的方塊），然後選取要套用至所有變體的新大小與外觀比例。 變數會複製並調整大小。
* **若要[裁切或重新定位影像](/help/user-guide/create/manage-variants.md#crop-assets)**，請將滑鼠停留在影像上，按一下顯示的裁切圖示，然後調整影像大小和位置。 按一下「**[!UICONTROL 套用]**」。

<!-- # Preview for device
When revising and preparing email experiences, you can toggle between previews for desktop and mobile views to ensure coherence and visual appeal of draft variants.
**To preview variants for desktop and mobile devices** toggle the device preview option—between **desktop** and **mobile**—in the right menu bar (computer and phone icons) to preview how variants appear. -->

## 提交產生回饋

若要[提交關於產生輸出品質的意見反應](/help/user-guide/create/manage-variants.md#generation-feedback)，請按一下選項圖示（三個點）並選取&#x200B;**[!UICONTROL 輸出良好]**&#x200B;或&#x200B;**[!UICONTROL 輸出不良]**。

## 驗證品牌一致性

若要最佳化產生的廣告，並確保嚴格遵守品牌識別，請利用&#x200B;[_品牌驗證面板_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel)&#x200B;的強大功能，該面板會顯示完整的品牌驗證詳細資訊，並闡明改善領域。

**若要驗證品牌一致性**：

1. 按一下頂端功能表列中的品牌驗證圖示，開啟&#x200B;[_品牌驗證面板_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel)。 您可以檢視片段的詳細資訊和需要改進的准則。

1. 切換每個廣告，瞭解如何改善產生的內容，使其更加與品牌保持一致。
1. [手動修訂廣告](#revise-generated-display-ads)，以確保您的電子郵件與品牌緊密一致。

請參閱[品牌驗證](/help/user-guide/guidelines/brand-validation.md)。

## 取得檢閱和核准

使用「核准」面板（可從畫布的頂端功能表列存取）來取得稽核、追蹤稽核評論，以及取得利害關係人的核准。

**若要取得稽核與核准**：

1. [啟動核准要求](/help/user-guide/approvals/request-review.md)以徵求[草擬電子郵件體驗的核准](/help/user-guide/approvals/approve-content.md)。
1. [在稽核程式期間移除或新增稽核者](/help/user-guide/approvals/review-and-edit.md#manage-approvals)。
1. [存取內容以供檢閱](/help/user-guide/approvals/review-and-edit.md#access-content-for-review)並檢視修訂要求。
1. 編輯每次稽核評論的草稿，並[發佈您的顯示廣告體驗](#publish-and-export-experience)。

檢視[檢閱與核准](/help/user-guide/approvals/overview.md)。

## Publish和匯出體驗

若要讓產生的顯示廣告可供目前和未來使用，請將它發佈至[!UICONTROL Content]，並匯出以用於您的行銷活動。

1. **若要發佈您的新顯示廣告體驗**，請按一下頂端工具列或核准流程中的&#x200B;**[!UICONTROL Publish]**。
   1. 選取&#x200B;_[!UICONTROL [!DNL Campaigns]]_並新增_[!UICONTROL &#x200B;更多詳細資料&#x200B;]_（如有需要）。
   1. 點擊&#x200B;**[!UICONTROL 發佈]**。

      ![Publish a顯示廣告](/help/assets/publish-displayad.png){width="450" zoomable="yes"}

1. **若要匯出您的新顯示廣告體驗**，請按一下頂端工具列中的[匯出]。****
   1. 選取格式(僅限JPG)，然後按一下「匯出」****。

請參閱[[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content)。
