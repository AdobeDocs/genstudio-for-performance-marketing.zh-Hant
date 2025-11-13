---
title: 建立電子郵件體驗
description: 瞭解如何在Adobe GenStudio for Performance Marketing中建立電子郵件體驗。
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 34446202-da98-45ff-869a-b43496a477f8
source-git-commit: 4658a759f5a4e03c54f645cfa1d1bbcc84fe1d91
workflow-type: tm+mt
source-wordcount: '1084'
ht-degree: 0%

---

# 建立電子郵件體驗

此教學課程示範如何使用GenStudio for Performance Marketing [產生品牌化](/help/user-guide/create/email-experiences.md)電子郵件體驗[[!DNL Create]](/help/user-guide/create/overview.md) （在左側導覽區域中繪製筆刷圖示）。

若要建立有效的電子郵件體驗，建議您[在GenStudio for Performance Marketing中新增准則](/help/user-guide/guidelines/add-guidelines.md)，並在開始之前[先梳理製作提示字元](/help/user-guide/effective-prompts.md)的基本知識。

## 選擇範本

若要建立新的電子郵件體驗，請使用可用的範本為您的內容提供架構。

**若要選擇電子郵件範本**：

1. 在&#x200B;_[!DNL Create]_&#x200B;中，按一下&#x200B;**[!UICONTROL 電子郵件]**。
1. 使用&#x200B;_篩選器_&#x200B;旁的搜尋選項來尋找特定的電子郵件範本。
1. 按一下以選取電子郵件範本，然後按一下[使用]。**&#x200B;**

   內容建立的中心「畫布」隨即顯示。

## 新增引數

在提示抽屜中新增[指南](/help/user-guide/guidelines/overview.md)和&#x200B;_引數_&#x200B;中的資產，會增加內容產生程式的費用，是產生電子郵件體驗的必要準備步驟。

如果您使用具有預先定義指引（例如[!DNL Brands]、[!DNL Personas]或[!DNL Products]）的範本，這些指引適用於您的變體。 如有需要，您可以加以變更。

**若要新增引數和資產**：

1. 按一下&#x200B;_引數_&#x200B;圖示以展開提示抽屜。
1. 在&#x200B;_引數_&#x200B;區段中，選取指導方針 — [!DNL Brands]、[!DNL Personas]和[!DNL Products] — 以通知內容建立。

   ![選擇角色](/help/assets/persona-select.png){width="600" zoomable="yes"}

   如果這些功能表中沒有可用的品牌、角色或產品，請[將准則新增至您的GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md)。

1. 新增內容以用於體驗&#x200B;*和*，以影響內容產生：
   * 按一下&#x200B;**[!UICONTROL 從「內容」選取]**，從[!DNL Content]存放庫選取資產（影像）、篩選並選取一或多個影像。

     ![選擇視覺內容](/help/assets/content-select-email.png){width="500" zoomable="yes"}

     若要使用已連線[!DNL AEM Assets Content Hub]存放庫中的資產，請從&#x200B;_位置_&#x200B;下拉式選單中選擇存放庫。 篩選並選取一或多個影像。

   * 或者，將資產拖放至&#x200B;**[!UICONTROL 從內容選取]**&#x200B;區段，以上傳一或多個新資產。
1. 按一下&#x200B;**[!UICONTROL 使用]**。

   >[!NOTE]
   >如果您的電子郵件範本有多個區段，請在[!DNL Products]多區段電子郵件&#x200B;_中為每個電子郵件區段選取_&#x200B;和內容（視覺資產）。 多節電子郵件支援每個節一個視覺資產。 您只能從[!DNL Content]將視覺資產新增至多節電子郵件，而不能從本機來源拖放或上傳資產。
   >![為每個電子郵件區段新增內容和引數](/help/assets/parameters-multisection-email.png){width="450" zoomable="yes"}

當您完成新增引數時，可以再次按一下&#x200B;_引數_&#x200B;圖示來收合提示抽屜。

## 輸入提示

選取准則後，請使用自然語言製作提示，以開始為您的新電子郵件體驗產生內容。 詳細提示產生比模糊或模稜兩可的提示更高的品質輸出。

請參閱[撰寫有效提示](/help/user-guide/effective-prompts.md)，深入瞭解撰寫提示的相關資訊。

**若要輸入提示**：

1. 在&#x200B;_「描述您要產生的體驗」_&#x200B;提示方塊中輸入提示。
1. 按一下&#x200B;**[!UICONTROL 產生]**。

依預設，會產生四個變數（全部由您新增的提示、指引和內容所推動），並顯示在畫布中。

產生的內容會以漸進方式載入 — 當電子郵件體驗的每個區段產生時，都會顯示在畫布中。 請參閱[電子郵件體驗](/help/user-guide/create/meta-experiences.md#progressive-loading)，瞭解如何在畫布中載入這些變更。

## 修訂產生的變體

在選取要傳送以進行核准或發佈至[!DNL Content]的內容之前，您可以編輯電子郵件區段或刪除產生之電子郵件集中的變體。

**若要修訂產生的變體**：

* **若要[編輯電子郵件草稿名稱](/help/user-guide/create/manage-variants.md#change-draft-name)**，請按一下畫布頂端的&#x200B;_未命名草稿_&#x200B;標題，然後輸入新標題。
* **若要[手動編輯電子郵件](/help/user-guide/create/manage-variants.md#manually-edit-text)**，請按一下任何可編輯的文字欄位（例如主旨列、標題或內文）並視需要編輯
* **若要[變更或選取Call to action](/help/user-guide/create/manage-variants.md#revise-call-to-action)**，請按一下call-to-action按鈕，然後選取&#x200B;_[!UICONTROL 重新片語]_&#x200B;或&#x200B;_[!UICONTROL 新增連結]_。
* **若要在變體中[套用文字格式](/help/user-guide/create/manage-variants.md#manually-edit-text)**，請按一下變體的影像上文字，然後按一下&#x200B;**[!UICONTROL 格式化文字]**。
* **若要[重新產生變體](/help/user-guide/create/manage-variants.md#re-generate-sections)**&#x200B;的區段，請按一下可編輯的文字欄位並使用&#x200B;_[!UICONTROL 建議的編輯]_&#x200B;選項，或輸入新的提示並按一下&#x200B;**[!UICONTROL 產生]**。
* **若要[新增或交換變體中的影像](/help/user-guide/create/manage-variants.md#swap-image)**，請按一下影像資產（如果影像目前不存在，則按一下影像資產區域），然後按一下&#x200B;**[!UICONTROL 從內容交換]**&#x200B;圖示。
* **若要[新增連結至變體中的影像](/help/user-guide/create/manage-variants.md#add-image-link)**，請按一下影像資產（如果影像目前不存在，則按一下影像資產區域），然後按一下連結圖示。
* **若要[為變體中的影像新增替代文字](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)**，請按一下影像資產，並使用&#x200B;_替代文字_&#x200B;選項來手動新增或產生每個影像的替代文字。
* **若要[新增協助工具標籤](/help/user-guide/create/manage-variants.md#add-accessibility-labels)至您的變體**，請按一下影像或call-to-action連結，然後提供簡短說明，說明連結或按鈕的作用。
* **若要[刪除電子郵件](/help/user-guide/create/manage-variants.md#delete-variant)**，請按一下以選取電子郵件標題（例如「電子郵件1/4」），然後按一下&#x200B;**[!UICONTROL 刪除變體]**。

## 提交產生回饋

若要[提交關於產生輸出品質的意見反應](/help/user-guide/create/manage-variants.md#generation-feedback)，請按一下選項圖示（三個點）並選取&#x200B;**[!UICONTROL 輸出良好]**&#x200B;或&#x200B;**[!UICONTROL 輸出不良]**。

## 裝置的預覽

修訂和準備電子郵件體驗時，您可以[在案頭和行動檢視的預覽之間切換](/help/user-guide/create/manage-variants.md#preview-for-device)，以確保草稿變體的一致性和視覺吸引力。

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

1. [啟動核准要求](/help/user-guide/approvals/request-review.md)以徵求[草擬電子郵件體驗的核准](/help/user-guide/approvals/approve-content.md)。
1. [在稽核程式期間移除或新增稽核者](/help/user-guide/approvals/review-and-edit.md#manage-approvals)。
1. [存取內容以供檢閱](/help/user-guide/approvals/review-and-edit.md#access-content-for-review)並檢視修訂要求。
1. 編輯每次稽核評論的草稿，並[發佈您的電子郵件體驗](#publish-and-export-experience)。

如需詳細資訊，請參閱[檢閱與核准](/help/user-guide/approvals/overview.md)。

## 發佈和匯出體驗

若要讓產生的電子郵件可供目前和未來使用，請將它發佈至[!UICONTROL Content]，並匯出以用於您的行銷活動。

1. **若要發佈您的新電子郵件體驗**，請按一下頂端工具列或核准流程中的&#x200B;**[!UICONTROL 發佈]**。
1. **若要匯出您的新電子郵件體驗**，請按一下頂端工具列中的[匯出]。**&#x200B;**
   1. 選取格式(僅限CSV和影像或HTML)，然後按一下「匯出」**&#x200B;**。

如需詳細資訊，請參閱[[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content)。
