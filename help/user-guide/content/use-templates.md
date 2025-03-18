---
title: 使用範本
description: 瞭解如何在Adobe GenStudio for Performance Marketing中有效使用範本來簡化您的創意流程。
feature: Media Templates
exl-id: 7705bb79-19ca-4c16-8f8b-95bf8687e96d
source-git-commit: 19d0b8b929e293179a091cc7b5a6a1268b0abbbd
workflow-type: tm+mt
source-wordcount: '1157'
ht-degree: 0%

---

# 使用範本

GenStudio for Performance Marketing可讓內容建立者使用&#x200B;_範本_&#x200B;快速產生一致的品牌上行銷內容。 範本提供起點，包含預先設定的版面和設計元素，可大幅減少產生新內容所需的時間和精力。

雖然GenStudio for Performance Marketing不支援直接在應用程式中建立範本，但您可以使用熱門設計工具(例如Adobe InDesign、Illustrator或Express)輕鬆設計和準備範本。 設計完成後，您可以加以調整以用於GenStudio for Performance Marketing。 請依照下列步驟開始使用範本：

1. **設計您的範本**：使用您偏好的設計工具，以元素](#template-elements)建立[範本的視覺版面，例如頁首、標題、內文、CTA、影像和頁尾。

2. **為您的範本撰寫程式碼**：將您的設計轉換為HTML和內嵌CSS，以確保在各種裝置間保持乾淨且有回應。 請考慮[協助工具准則](accessibility-for-templates.md)，以協助達到您預期的最大受眾。

3. **準備GenStudio for Performance Marketing**：使用Handlebars範本語言調整您的HTML範本。 插入預留位置以指示GenStudio for Performance Marketing應在何處動態產生內容。 瞭解如何[自訂GenStudio for Performance Marketing的範本](customize-template.md)。

依照這些步驟，您可以建立專業且有效的範本，這些範本即可在GenStudio for Performance Marketing中使用，讓您快速有效率地製作品牌內內容。

## 範本元素

範本是使用HTML和內嵌CSS定義的一組指示，可用來產生電子郵件、社交廣告或顯示廣告體驗。 範本元素提供內容建立的結構。

以下是範本中使用的元素清單，以及有關其特性的部分詳細資訊：

| **元素** | **頻道** | **說明** |
|----------------------|------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Preheader** | 電子郵件 | 電子郵件中的次要主旨列（通常介於40到50個字元之間），可強化主要主旨列。 在開啟電子郵件之前，它會在收件匣中主旨旁邊顯示。 |
| **標頭** | 電子郵件 | 收件者在開啟電子郵件時看到的電子郵件頂端區段會設定語調，並提供所包含內容的內容。 |
| **標題** | 中繼廣告、橫幅和顯示廣告、LinkedIn | 收件者看到的第一個內容應該足以吸引吸引讀者興趣。 |
| **簡介文字** | LinkedIn | 主要訊息會傳達核心訊息，類似於內文。 最多可使用150個字元，包括空格、最多四個表情符號和標點符號。 |
| **內文** | 電子郵件、中繼廣告、橫幅和顯示廣告 | 廣告的主要文字傳達核心訊息。 它應該吸引人、提供資訊和具有說服力，以鼓勵對象採取所需的行動。 |
| **號召性用語** | 電子郵件、中繼廣告、橫幅和顯示廣告、LinkedIn | 行動號召按鈕使用片語和連結來鼓勵收件者採取特定動作，例如按一下連結或進行購買。 |
| **影像** | 電子郵件、中繼廣告、橫幅和顯示廣告、LinkedIn | 提升視覺吸引力、分解文字，並支援訊息。 影像應高品質且吸引目光。 |
| **頁尾** | 電子郵件 | 電子郵件的底部區段包含其他內容，例如聯絡詳細資訊、社群媒體連結、免責宣告和取消訂閱選項。 |
| **文字覆蓋** | 中繼廣告 | 放置在影像上的文字，用以支援和增強標題與內文內容。 |

>[!TIP]
>
>檢視GenStudio for Performance Marketing支援的每種管道型別範本的[可辨識欄位名稱](customize-template.md#recognized-field-names)。

## 自訂範本

您[透過插入產生AI用來插入內容的內容預留位置或欄位，自訂範本](customize-template.md)以用於GenStudio for Performance Marketing。 GenStudio for Performance Marketing可辨識特定欄位，例如「`body`」欄位，並遵守為所選品牌設定的管道准則。

>[!TIP]
>
>遵循[協助工具准則](accessibility-for-templates.md)和[最佳實務](/help/user-guide/content/best-practices-for-templates.md)，以便您可以觸及更多對象並提供最佳體驗。

## 管理範本

_[!DNL Templates]_相簿會顯示您為在GenStudio for Performance Marketing中產生體驗而自訂的範本詳細目錄。 您可以依管道型別（例如電子郵件、顯示廣告、中繼廣告和LinkedIn廣告）篩選範本。

![內容範本清單](/help/assets/content-templates-filter.png "搜尋LinkedIn範本"){width="650" zoomable="yes"}

### 新增範本

在上傳範本之前，請依照[自訂範本](customize-template.md)指南，確保範本已完全準備就緒並可以在GenStudio for Performance Marketing中使用。

**若要新增範本**：

1. 在&#x200B;_[!DNL Content]_中，選取&#x200B;**[!UICONTROL 範本]**區段。

1. 按一下&#x200B;**[!UICONTROL 新增範本]**。

1. 在&#x200B;_[!UICONTROL 新增您核准的範本]_&#x200B;窗格中，瀏覽HTML範本檔案或將HTML範本檔案拖曳至放置空間。 按一下「**[!UICONTROL 下一步]**」。

1. 在&#x200B;_[!UICONTROL 檢查偵測到的欄位]_&#x200B;窗格中，檢閱欄位。 確認您使用正確的範本，以及所有詳細資料皆如預期般顯示。

   電子郵件範本的範例預覽：

   ![偵測到預覽欄位](/help/assets/template-detected-fields.png){width="650" zoomable="yes"}

   >[!TIP]
   >
   >如果範本不正確，請按一下[上一步] ****&#x200B;並返回上一步。 上傳修正的範本檔案。 或使用[範本程式碼編輯器](/help/user-guide/content/code-editor.md)進行簡單的更正。

1. 當您對範本預覽感到滿意時，請按一下&#x200B;**[!UICONTROL [下一步]]**。

1. 在&#x200B;_[!UICONTROL 提供範本詳細資料及上傳]_&#x200B;窗格中，命名您的範本並選取&#x200B;**[!UICONTROL 管道]**&#x200B;型別。

   需要範本名稱和管道型別。 其他需求可能包括：

   - **Meta**：需要外觀比例
   - **橫幅和顯示廣告**：需要維度

1. 新增儘可能多的詳細資訊，以改善搜尋和篩選中的範本識別。

1. 按一下&#x200B;**[!UICONTROL 「完成」]**。

### 重新整理範本

範本可能包含靜態檔案，例如圖示或標誌。 建立範本預覽後未儲存[靜態內容](/help/user-guide/content/customize-template.md#static-content)。 GenStudio for Performance Marketing會繼續參考範本中提供的來源連結。 使用重新整理以更新這些資產最新版本的範本預覽。

**若要重新整理範本**：

1. 在&#x200B;_[!DNL Content]_中，選取&#x200B;**[!UICONTROL 範本]**區段。

1. 按一下範本以取得完整檢視和詳細資訊清單。

1. 按一下右上角的&#x200B;**[!UICONTROL 重新整理]** （圓圈箭頭）以重新整理範本中使用的所有資產。

### 使用範本建立體驗

在GenStudio for Performance Marketing中尋找並使用現有範本，以建立更多體驗。

**若要使用範本建立體驗**：

1. 在&#x200B;_[!DNL Content]_中，選取&#x200B;**[!UICONTROL 範本]**區段。

1. 按一下範本以取得完整檢視和詳細資訊清單。

1. 從右上角按一下&#x200B;**[!UICONTROL 建立體驗]** （繪圖筆刷）以使用範本。

1. 繼續[建立](/help/user-guide/create/overview.md#create-use-cases)體驗。

## AJO和Marketo的範本

您可以上傳在Adobe Journey Optimizer (AJO)或Marketo中建立的範本。 GenStudio for Performance Marketing會偵測應用程式特有的模式並忽略它們，保留原始表單以繼續用於AJO或Marketo。 您不需要變更原始AJO或Marketo語法。

可辨識的應用程式模式包括：

- **AJO**： `{{profile.*}}`，`{{context.*}}`
- **Marketo**： `{{my.*}}`，`{{lead.*}}`，`{{system.*}}`

>[!BEGINSHADEBOX]

**必備條件**

- 應用程式(AJO、Marketo)和GenStudio for Performance Marketing必須屬於相同的IMS組織才能整合
- 使用者必須具有「共同作業人員」角色（最低層級）或以上層級

>[!ENDSHADEBOX]

接著，[使用預留位置自訂您的範本](/help/user-guide/content/customize-template.md)，以指示GenStudio for Performance Marketing應在何處為您產生內容。 [將範本](#add-a-template)新增至[!DNL Content]存放庫並驗證範本。 使用程式碼編輯器進行任何細微的更正。
