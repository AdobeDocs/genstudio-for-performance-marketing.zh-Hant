---
title: 使用範本
description: 瞭解如何在Adobe GenStudio for Performance Marketing中有效使用範本來簡化您的創意流程。
feature: Templates, Content
exl-id: 7705bb79-19ca-4c16-8f8b-95bf8687e96d
source-git-commit: 61a939ae81eb5ff61d741bb1092e9e4c82119f7e
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 0%

---

# 使用範本

GenStudio for Performance Marketing可讓內容建立者使用&#x200B;_範本_&#x200B;快速產生一致的品牌上行銷內容。 範本提供起點，包含預先設定的版面和設計元素，可大幅減少產生新內容所需的時間和精力。

## 範本元素

範本是使用HTML和內嵌CSS定義的一組指示，可用於產生電子郵件或中繼廣告體驗。

以下是範本中使用的元素清單，以及有關其特性的部分詳細資訊。

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

- **CTA （呼叫動作）**

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

## 設定頻道准則

在GenStudio for Performance Marketing中使用範本之前，最佳實務是為每個品牌設定[管道指引](../guidelines/brands.md#channel-guidelines)。 管道指引直接影響使用範本時產生的內容型別。 例如，您可以在電子郵件內文中設定字元限制。

![主體規格](/help/assets/channel-email-body.png)

## 自訂範本

您[透過插入產生AI用來插入內容的內容預留位置或欄位，自訂範本](customize-template.md)以用於GenStudio for Performance Marketing。 GenStudio for Performance Marketing可辨識特定欄位，例如「`body`」欄位，並遵守為所選品牌設定的管道准則。

>[!TIP]
>
>遵循建置範本的[協助工具准則](accessibility-for-templates.md)，以便您可以觸及更多對象並提供最佳體驗。

## 上傳範本

準備GenStudio for Performance Marketing的範本時，請使用[自訂範本](customize-template.md)作為指南。 請參閱範本的[協助工具准則](accessibility-for-templates.md)，以取得為所有對象提供更佳體驗的指引。

**若要新增範本**：

1. 在&#x200B;_[!DNL Content]_中，選取&#x200B;**[!UICONTROL 範本]**區段。

1. 按一下&#x200B;**[!UICONTROL 新增範本]**。

1. 在&#x200B;_[!UICONTROL 新增您核准的範本]_&#x200B;窗格中，瀏覽以尋找HTML範本檔案，或將HTML範本檔案拖曳至放置空間。 按一下「**[!UICONTROL 下一步]**」。

1. 在&#x200B;_[!UICONTROL 檢閱發現的欄位]_&#x200B;窗格中，檢閱偵測到的欄位。 確認您使用正確的範本，以及所有詳細資料皆如預期般顯示。 按一下「**[!UICONTROL 下一步]**」。

   電子郵件範本的範例預覽：

   ![偵測到預覽欄位](../../assets/template-detected-fields.png){width="650"}

   >[!TIP]
   >
   >如果範本不正確，請按一下[上一步] ****&#x200B;並返回上一步。 上傳修正的範本檔案。

1. 在&#x200B;_[!UICONTROL 提供範本詳細資料及上傳]_&#x200B;窗格中，命名您的範本並選取&#x200B;**[!UICONTROL 管道]**&#x200B;型別。

   需要範本名稱和管道型別。 其他需求可能包括：

   - **Meta**：需要外觀比例
   - **顯示廣告**：需要Dimension

1. 新增儘可能多的詳細資訊，以改善搜尋和篩選中的範本識別。

1. 按一下&#x200B;**[!UICONTROL 「完成」]**。

## 使用範本建立

在GenStudio for Performance Marketing中尋找並使用現有範本，以建立更多體驗。

**若要使用範本建立體驗**：

1. 在&#x200B;_[!DNL Content]_中，選取&#x200B;**[!UICONTROL 範本]**區段。

   ![內容範本清單](../../assets/content-templates.png){width="650" zoomable="yes"}

1. 選取完整檢視和詳細資訊清單的範本。

1. 從右上角按一下&#x200B;**[!UICONTROL 建立體驗]** （繪圖筆刷）以使用範本。

1. 繼續[建立](/help/user-guide/create/overview.md)體驗。
