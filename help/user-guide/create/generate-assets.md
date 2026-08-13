---
title: 產生影像變體
description: 在Adobe [!DNL GenStudio] 中建立符合參考影像樣式的影像，以進行效能行銷。
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
badgeBeta: label="Beta" tooltip="此功能目前在Beta中，因此某些功能可能會受到限制或有所變更。"
role: User
level: Beginner
recommendations: noDisplay
exl-id: c1118ada-7fee-43cd-aff4-eab69539afb4
TQID: https://experienceleague.adobe.com/NXtN00EKTe0lGI8jJMJWJfWx6mHoMQI1of1mJhgrR5U
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
  - id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2:
  - id: be495d08-ecd1-455f-951e-c22de504e667
  - id: de1f9646-abd3-4e21-9de2-df62ce55c8dc
  - id: dee4e9a9-78d1-4953-8179-f8da6117027d
  - id: e4a0febc-5163-4017-82ce-fc7594509fb6
  - id: f54ee13b-9545-4d68-9842-a12026e60aaf
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2:
  - id: cc72dcf1-72e1-48cc-b434-e7c27d62d67c
source-git-commit: 6d1053bf94b0a0ba65be90359e4d176e64dfffae
workflow-type: tm+mt
source-wordcount: 752
ht-degree: 0%

---

# 產生影像變體

使用GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) （繪圖筆刷圖示），您就可以產生&#x200B;_[!DNL Image variants]_&#x200B;個從選取的影像中汲取靈感的產生資產，擷取其視覺效果和整體美感。<!-- [two types of images](#image-types) using GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (paintbrush icon)—_[!DNL Image variants]_ and _[!DNL Similar images]_. -->

若要設計吸引目光且有效的影像，建議您[在GenStudio for Performance Marketing中新增准則](/help/user-guide/guidelines/add-guidelines.md)，並檢閱撰寫提示的[基本知識](/help/user-guide/effective-prompts.md)。

## 影像型別

_[!DNL Image variants]_&#x200B;是從選定影像中汲取靈感的已產生資產，擷取其視覺效果和整體美感。 這些影像是使用[!DNL Content]中已提供的影像以及精心製作的提示來建立，以指導設計。 它們嚴格遵守品牌指導方針和在產生過程中選擇的引數。

_[!DNL Image variants]_<!-- and _[!DNL Similar images]_ -->整合設定准則、引數，以及[精心打造的提示](/help/user-guide/effective-prompts.md)，以提供吸引目光的影像資產。

<!-- * _[!DNL Similar images]_—Image assets created with strong similarity to an existing selected image available in [!DNL Content]. When generating similar images, GenStudio for Performance Marketing redesigns the selected image, giving slight variations on the content to provide variety and nuance. -->

## 產生影像變體

您可以使用定義的指導方針、引數和選取的參考影像來產生[!DNL Image variants]。 這些元素以及您的提示會引導產生一致的[!DNL Image variants]。

### 選擇參考影像

若要建立&#x200B;_[!DNL Image variants]_，請選取儲存在[!DNL Content]中的現有影像。 請參閱[範本最佳實務](/help/user-guide/templates/best-practices-for-templates.md#follow-channel-specific-template-guidelines)，以取得支援的影像尺寸相關資訊。

**若要選擇參考影像**：

1. 在&#x200B;_[!DNL Create]_&#x200B;中，按一下&#x200B;**[!UICONTROL 產生影像變體]**。
   ![產生影像變體](./gen-image-variants.png){width="400" zoomable="yes"}
1. 若要選擇參考影像，請使用&#x200B;_[!UICONTROL 從內容中選取]_&#x200B;按鈕來尋找特定影像。
   ![從內容中選取](./gen-variant-select-from-content.png){width="200" zoomable="yes"}

   若要使用已連線[!DNL AEM Assets Content Hub]存放庫中的資產，請從&#x200B;_位置_&#x200B;下拉式選單中選擇存放庫。 篩選並選取一個影像。

   ![選取參考影像](/help/assets/select-img.png){width="400" zoomable="yes"}

1. 在&#x200B;_選取影像_&#x200B;檢視中，按一下影像以核取選取方塊。

   選取影像的大小最多可達10MB。 一次只能選取一個影像。

1. 按一下&#x200B;**[!UICONTROL 使用]**。

   畫布是作為內容建立的中心樞紐，隨即顯示。

### 新增引數

納入[指南](/help/user-guide/guidelines/overview.md)和引數可強化內容產生程式，是產生[!DNL Image variants]的重要準備步驟。

**若要新增指引和引數**：

1. 在&#x200B;_基本_&#x200B;索引標籤中，選取[!DNL Brand]以通知內容建立。

   如果此功能表中沒有可用品牌，請[將准則新增至您的GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md)。
1. 從&#x200B;_[!UICONTROL 模型]_&#x200B;選取要用於產生影像的模型。
1. 從&#x200B;_[!UICONTROL 外觀比例]_&#x200B;中選取所需的外觀比例。

### 輸入提示

選取引數後，使用自然語言製作提示以開始產生影像變體。

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

<!-- 
## Generate Similar images

You can quickly generate images similar to a selected image within [!DNL Content] from the [!DNL Create] home.

**To create _[!DNL Similar images]_**:

1. In _[!DNL Create]_, click **[!UICONTROL Similar images]**.
1. Use the search option, adjacent to _Filter_, to find a specific image.

   To use assets from a connected [!DNL AEM Assets Content Hub] repository, choose a repository from the _Location_ drop-down menu. Filter and select one image.

1. In the _Select image_ view, click on an image.
1. Click **[!UICONTROL Use]**.

   The Canvas, which serves as the central hub for content creation, is displayed. Four image variations similar to the original selected image appear.

   ![Generate similar images](/help/assets/generate-similar.png){width="400" zoomable="yes"} 
-->

## 發佈和匯出影像

產生的影像草稿會顯示在[!DNL Create]首頁的&#x200B;_Recents_&#x200B;區段中。

若要讓產生的影像可供目前和未來使用，請將它們發佈至[!UICONTROL 內容]，然後匯出以用於您的行銷活動。

1. **若要發佈您的新影像**，請按一下頂端工具列中的&#x200B;**[!UICONTROL 發佈]**。
   1. 如有需要，_[!UICONTROL 新增詳細資料]_，例如&#x200B;_[!UICONTROL 行銷活動]_&#x200B;或&#x200B;_[!UICONTROL 管道]_。
   1. 點擊&#x200B;**[!UICONTROL 發佈]**。

1. **若要匯出您的新影像**，請按一下頂端工具列中的&#x200B;**[!UICONTROL 匯出]**。
   1. 選取格式（JPG或PNG），然後按一下&#x200B;**[!UICONTROL 匯出]**。

請參閱[[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content)。
