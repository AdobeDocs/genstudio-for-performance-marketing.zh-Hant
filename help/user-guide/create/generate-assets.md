---
title: 產生影像
description: 在Adobe [!DNL GenStudio] 中建立符合參考影像樣式的影像，以進行效能行銷。
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
badgeBeta: label="Beta" tooltip="此功能目前在Beta中，因此某些功能可能會受到限制或有所變更。"
role: User
level: Beginner
recommendations: noDisplay
exl-id: c1118ada-7fee-43cd-aff4-eab69539afb4
source-git-commit: 47195c08f500e50a01db127c6badc461c10afaf9
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 0%

---

# 產生影像

使用GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) （繪圖筆刷圖示），您就可以產生&#x200B;_[!DNL On-brand images]_&#x200B;個從選取的影像中汲取靈感的產生資產，擷取其視覺效果和整體美感。<!-- [two types of images](#image-types) using GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (paintbrush icon)—_[!DNL On-brand images]_ and _[!DNL Similar images]_. -->

若要設計吸引目光且有效的影像，建議您[在GenStudio for Performance Marketing中新增准則](/help/user-guide/guidelines/add-guidelines.md)，並檢閱撰寫提示的[基本知識](/help/user-guide/effective-prompts.md)。

## 影像型別

_[!DNL On-brand images]_&#x200B;是從選定影像中汲取靈感的已產生資產，擷取其視覺效果和整體美感。 這些影像是使用[!DNL Content]中已提供的影像以及精心製作的提示來建立，以指導設計。 它們嚴格遵守品牌指導方針和在產生過程中選擇的引數。

_[!DNL On-brand images]_<!-- and _[!DNL Similar images]_ -->整合設定准則、引數，以及[精心打造的提示](/help/user-guide/effective-prompts.md)，以提供吸引目光的影像資產。

<!-- * _[!DNL Similar images]_—Image assets created with strong similarity to an existing selected image available in [!DNL Content]. When generating similar images, GenStudio for Performance Marketing redesigns the selected image, giving slight variations on the content to provide variety and nuance. -->

## 產生品牌內影像

您可以使用定義的指導方針、引數和選取的參考影像來產生[!DNL On-brand images]。 這些元素以及您的提示會引導產生一致的[!DNL On-brand image]變數。

### 選擇參考影像

若要建立&#x200B;_[!DNL On-brand images]_，請選取儲存在[!DNL Content]中的現有影像。 如需有關支援的[維度的資訊，請參閱](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines)範本最佳實務[!DNL on-brand image]。

**若要選擇參考影像**：

1. 在&#x200B;_[!DNL Create]_&#x200B;中，按一下&#x200B;**[!UICONTROL 品牌上影像]**。
1. 使用&#x200B;_篩選器_&#x200B;旁的搜尋選項來尋找特定影像。

   ![選取參考影像](/help/assets/select-img.png){width="400" zoomable="yes"}

   若要使用已連線[!DNL AEM Assets Content Hub]存放庫中的資產，請從&#x200B;_位置_&#x200B;下拉式選單中選擇存放庫。 篩選並選取一個影像。

1. 在&#x200B;_選取影像_&#x200B;檢視中，按一下影像。

   選取影像的大小最多可達10MB。

1. 按一下&#x200B;**[!UICONTROL 使用]**。

   畫布是作為內容建立的中心樞紐，隨即顯示。

### 新增引數

納入[指南](/help/user-guide/guidelines/overview.md)和引數可強化內容產生程式，是產生[!DNL on-brand image]的重要準備步驟。

**若要新增指引和引數**：

1. 在&#x200B;_基本_&#x200B;索引標籤中，選取[!DNL Brand]以通知內容建立。

   如果此功能表中沒有可用品牌，請[將准則新增至您的GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md)。

1. 從&#x200B;_[!UICONTROL 影像類別]_&#x200B;選取最適合您所需結果的影像類別。

   如果選取[!DNL Brand]，則可以使用影像類別。 選項由選取的[!DNL Brand]決定。

<!-- 1. _(Optional)_ Select a custom model from _[!UICONTROL Model]_.

   Models are available if you access to [custom models in Firefly](https://adobedx.slack.com/archives/CMF1JGMLY/p1743534402774569). The _Models_ list will be blank if you do not have access. -->

1. 從&#x200B;_[!UICONTROL 外觀比例]_&#x200B;中選取所需的外觀比例。
1. 按一下&#x200B;**[!UICONTROL 樣式參考]**&#x200B;中的&#x200B;_[!UICONTROL 從內容選取]_&#x200B;以新增參考影像。 您選取的影像會影響您產生的影像的視覺美感和深度。

   若要使用已連線[!DNL AEM Assets Content Hub]存放庫中的資產，請從&#x200B;_位置_&#x200B;下拉式選單中選擇存放庫。 篩選並選取一個影像。

1. 在&#x200B;_進階_&#x200B;索引標籤中，選取&#x200B;_內容型別_。

   已根據所選[!DNL Brand]—_Art_&#x200B;或&#x200B;_Photo_ — 的影像類別預先選取此專案，且無法編輯。

1. 以&#x200B;_[!UICONTROL 視覺強度]_&#x200B;調整影像現有視覺特性的整體強度。

### 輸入提示

選取引數後，使用自然語言製作提示，以開始於品牌影像上產生。

請參閱[撰寫有效的提示](/help/user-guide/effective-prompts.md)。

**若要輸入提示**：

1. 在提示方塊中輸入提示。
1. 按一下&#x200B;**[!UICONTROL 產生]**。

依預設，會產生四個變數（由您新增的提示、引數和內容所驅動），並顯示在畫布中。

### 在Adobe Express中編輯

產生影像變體後，您可以使用Adobe Express直接在Adobe GenStudio for Performance Marketing中編輯它們。

**若要使用Adobe Express編輯個別影像**：

1. 將滑鼠停留在產生的影像變體上，然後按一下「在Adobe Express中編輯」__。

   出現&#x200B;_Powered by Adobe Express_&#x200B;視窗。

1. 執行影像編輯，例如[裁切影像](https://helpx.adobe.com/express/create-and-edit-images/edit-images/crop-images.html)、[移除物件](https://helpx.adobe.com/express/create-and-edit-images/create-and-modify-with-generative-ai/remove-objects-generative-fill.html)以及套用效果。

   請參閱[Adobe Express檔案](https://helpx.adobe.com/express/user-guide.html)，瞭解如何使用Adobe Express在GenStudio for Performance Marketing中修訂影像。

1. 按一下&#x200B;_[!UICONTROL 套用變更]_&#x200B;以儲存您的編輯。
1. 視需要繼續編輯個別影像變體，並套用變更以儲存進度。

### 驗證內容檢查對齊方式

若要最佳化產生的變體，並確保嚴格遵守品牌識別、平台指引及協助工具標準，請利用&#x200B;[_內容檢查_&#x200B;面板](/help/user-guide/guidelines/brand-validation.md#content-check-panel)的強大功能。 此面板會顯示完整的內容檢查詳細資訊，並闡明改善領域。

**若要執行內容檢查**：

1. 按一下右側動作列中的&#x200B;_內容檢查_&#x200B;面板圖示以開啟&#x200B;[_內容檢查_&#x200B;面板](/help/user-guide/guidelines/brand-validation.md#content-check-panel)。 檢視&#x200B;*需要稽核*&#x200B;和&#x200B;*通過*&#x200B;檢查的摘要，以檢視哪些區段和准則需要改進。

   ![_內容檢查_&#x200B;面板](/help/assets/content-check-img.png){width="500" zoomable="yes"}

1. 修訂影像變體以確保您的變體與執行的內容檢查緊密對齊。

請參閱[品牌驗證](/help/user-guide/guidelines/brand-validation.md)。

<!-- ## Generate Similar images

You can quickly generate images similar to a selected image within [!DNL Content] from the [!DNL Create] home.

**To create _[!DNL Similar images]_**:

1. In _[!DNL Create]_, click **[!UICONTROL Similar images]**.
1. Use the search option, adjacent to _Filter_, to find a specific image.

   To use assets from a connected [!DNL AEM Assets Content Hub] repository, choose a repository from the _Location_ drop-down menu. Filter and select one image.

1. In the _Select image_ view, click on an image.
1. Click **[!UICONTROL Use]**.

   The Canvas, which serves as the central hub for content creation, is displayed. Four image variations similar to the original selected image appear.

   ![Generate similar images](/help/assets/generate-similar.png){width="400" zoomable="yes"} -->

## 發佈和匯出影像

產生的影像草稿會顯示在&#x200B;_首頁的_ Recents[!DNL Create]區段中。

若要讓產生的影像可供目前和未來使用，請將它們發佈至[!UICONTROL 內容]，然後匯出以用於您的行銷活動。

1. **若要發佈您的新影像**，請按一下頂端工具列中的&#x200B;**[!UICONTROL 發佈]**。
   1. 如有需要，_[!UICONTROL 新增詳細資料]_，例如&#x200B;_[!UICONTROL 行銷活動]_&#x200B;或&#x200B;_[!UICONTROL 管道]_。
   1. 點擊&#x200B;**[!UICONTROL 發佈]**。

1. **若要匯出您的新影像**，請按一下頂端工具列中的&#x200B;**[!UICONTROL 匯出]**。
   1. 選取格式(JPG或PNG)，然後按一下&#x200B;**[!UICONTROL 匯出]**。

請參閱[[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content)。
