---
title: 使用範本
description: 瞭解如何在Adobe GenStudio for Performance Marketing中有效使用範本來簡化您的創意流程。
feature: Templates, Content
exl-id: 7705bb79-19ca-4c16-8f8b-95bf8687e96d
source-git-commit: 62ab3849296195ca4d9525cb5688f74ce8bede54
workflow-type: tm+mt
source-wordcount: '960'
ht-degree: 0%

---

# 使用範本

GenStudio for Performance Marketing可讓內容建立者使用&#x200B;_範本_&#x200B;快速產生一致的品牌上行銷內容。 範本提供起點，包含預先設定的版面和設計元素，可大幅減少產生新內容所需的時間和精力。

雖然GenStudio for Performance Marketing不支援直接在應用程式中建立範本，但您可以使用熱門設計工具(例如Adobe InDesign、Illustrator或Express)輕鬆設計和準備範本。 設計完成後，您可以加以調整以用於GenStudio for Performance Marketing。 請依照下列步驟開始使用範本：

1. **設計您的範本**：使用您偏好的設計工具，以元素](#template-elements)建立[範本的視覺版面，例如頁首、標題、內文、CTA、影像和頁尾。

2. **為您的範本編碼**：將您的設計轉換為HTML和內嵌CSS，以確保它在各種裝置間保持乾淨和回應。 請考慮[協助工具准則](accessibility-for-templates.md)，以協助達到您預期的最大受眾。

3. **準備GenStudio for Performance Marketing**：使用Handlebars範本語言調整您的HTML範本。 插入預留位置以指示GenStudio for Performance Marketing應在何處動態產生內容。 瞭解如何[自訂GenStudio for Performance Marketing的範本](customize-template.md)。

依照這些步驟，您可以建立專業且有效的範本，這些範本即可在GenStudio for Performance Marketing中使用，讓您快速有效率地製作品牌內內容。

## 範本元素

範本是以HTML和內嵌CSS定義的一組指示，可用來產生電子郵件、社交廣告或顯示廣告體驗。 範本元素提供內容建立的結構。

以下是範本中使用的元素清單，以及有關其特性的部分詳細資訊：

- **Preheader**

   - 充當電子郵件中的次要主旨列，增強主要主旨列
   - 40到50個字元之間
   - 在開啟電子郵件之前，顯示在收件匣中主旨旁邊
   - 用於電子郵件範本

- **標頭**

   - 收件者開啟電子郵件時看到的電子郵件頂端區段
   - 設定色調，並為包含的內容提供內容
   - 用於電子郵件範本

- **標題**

   - 收件者看到的第一個內容
   - 應該吸引人才能引起興趣
   - 用於中繼廣告範本

- **內文**

   - 傳送主要訊息的主要內容區域
   - 可包含文字、影像和其他媒體
   - 用於電子郵件和中繼廣告範本

- **號召性用語**

   - 呼叫動作按鈕使用片語和連結
   - 鼓勵收件者採取特定動作，例如按一下連結或進行購買
   - 用於電子郵件和中繼廣告範本

- **影像**

   - 增強視覺吸引力
   - 分解文字
   - 支援訊息
   - 應該高品質且搶眼
   - 用於電子郵件和中繼廣告範本

- **頁尾**

   - 底部區段包含其他內容，例如聯絡詳細資訊、社群媒體連結、免責宣告和取消訂閱選項
   - 用於電子郵件範本

- **文字覆蓋**

   - 影像上的文字
   - 用於支援及提升標題與內文
   - 用於中繼廣告範本

>[!TIP]
>
>檢視GenStudio for Performance Marketing支援的每種管道型別範本的[可辨識欄位名稱](customize-template.md#recognized-field-names)。

## 自訂範本

您[透過插入產生AI用來插入內容的內容預留位置或欄位，自訂範本](customize-template.md)以用於GenStudio for Performance Marketing。 GenStudio for Performance Marketing可辨識特定欄位，例如「`body`」欄位，並遵守為所選品牌設定的管道准則。

>[!TIP]
>
>遵循[協助工具准則](accessibility-for-templates.md)和[最佳實務](/help/user-guide/content/best-practices-for-templates.md)，以便您可以觸及更多對象並提供最佳體驗。

## 管理範本

[!DNL Templates]相簿會顯示您為在GenStudio for Performance Marketing中產生體驗而自訂的範本詳細目錄。 您可以依管道型別（例如電子郵件、顯示廣告和中繼廣告）篩選範本。

![內容範本清單](/help/assets/content-templates.png){width="650" zoomable="yes"}

### 新增範本

在上傳範本之前，請依照[自訂範本](customize-template.md)指南，確保範本已完全準備就緒並可以在GenStudio for Performance Marketing中使用。

**若要新增範本**：

1. 在&#x200B;_[!DNL Content]_中，選取&#x200B;**[!UICONTROL 範本]**區段。

1. 按一下&#x200B;**[!UICONTROL 新增範本]**。

1. 在&#x200B;_[!UICONTROL 新增您核准的範本]_&#x200B;窗格中，瀏覽以尋找HTML範本檔案，或將HTML範本檔案拖曳至放置空間。 按一下「**[!UICONTROL 下一步]**」。

1. 在&#x200B;_[!UICONTROL 檢閱發現的欄位]_&#x200B;窗格中，檢閱偵測到的欄位。 確認您使用正確的範本，以及所有詳細資料皆如預期般顯示。 按一下「**[!UICONTROL 下一步]**」。

   電子郵件範本的範例預覽：

   ![偵測到預覽欄位](/help/assets/template-detected-fields.png){width="650"}

   >[!TIP]
   >
   >如果範本不正確，請按一下[上一步] ****&#x200B;並返回上一步。 上傳修正的範本檔案。

1. 在&#x200B;_[!UICONTROL 提供範本詳細資料及上傳]_&#x200B;窗格中，命名您的範本並選取&#x200B;**[!UICONTROL 管道]**&#x200B;型別。

   需要範本名稱和管道型別。 其他需求可能包括：

   - **Meta**：需要外觀比例
   - **顯示廣告**：需要Dimension

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
