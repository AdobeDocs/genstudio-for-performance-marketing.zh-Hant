---
title: 適用於Adobe GenStudio for Performance Marketing的GenStudio Photoshop
description: 瞭解如何安裝、設定和使用GenStudio for Performance Marketing適用的GenStudio Photoshop。
feature: Generative AI
role: User
exl-id: e3f57acd-f2dd-4957-aa5e-c97595a29899
TQID: https://experienceleague.adobe.com/9p-ohsF1gIVKv3vwjnP9o675l3gJT3tVxx34PefFzCQ
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: e0aa398c-6185-4e77-8cf7-2561c578c181
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 8c7ac98d651195c28a2c82341c68d40b067b2c76
workflow-type: tm+mt
source-wordcount: 847
ht-degree: 92%

---

# 適用於GenStudio for Performance Marketing的GenStudio Photoshop

GenStudio Photoshop會在Adobe Photoshop中新增面板，讓您產生品牌內內容。

本頁面說明如何安裝和設定外掛程式，以及如何使用外掛程式。

此外掛程式的功能包括：

* 使用Adobe ID登入GenStudio for Performance Marketing執行個體
* 將GenStudio for Performance Marketing內容產生欄位對應至Photoshop檔案中的文字圖層
* 指定品牌、產品、角色和文字提示以產生內容
* 或者，新增影像以取代範本影像
* 預覽產生的品牌內內容變化
* 將產生的內容套用至目前檔案中的對應圖層
* 建立品牌內內容翻譯
* 將產生的[!DNL Experiences]匯出至GenStudio for Performance Marketing

>[!VIDEO](https://video.tv.adobe.com/v/3478831?captions=chi_hant&learn=on)

## 安裝外掛程式

請依照下列指示安裝外掛程式。

### 先決條件

* Creative Cloud案頭應用程式
* Photoshop，最低版本25.6.0

### 安裝步驟

1. 從Adobe Exchange的Creative Cloud Marketplace下載並更新外掛程式。
1. 在Adobe Exchange中搜尋&#x200B;**GenStudio Photoshop**。
1. 依照提示安裝外掛程式。

### 解除安裝外掛程式

1. 啟動Creative Cloud案頭應用程式。
1. 按一下&#x200B;**[!UICONTROL 外掛程式]**&#x200B;選項。
1. 按一下適用於Creative Cloud的GenStudio卡片上的省略符號&#x200B;**[!UICONTROL (...)]**&#x200B;以取得選項。
1. 選擇&#x200B;**解除安裝**。

## 建立範本

若要產生內容，您必須從GenStudio for Performance Marketing檔案建立Photoshop範本。

若要建立GenStudio就緒範本：

1. 在Photoshop中開啟檔案。
1. 識別產生內容的文字圖層。
1. 以欄位名稱慣例格式重新命名圖層： `{<name_of_generated_field>}`。 例如：`{body}`、`{headline}`、`{cta}`。
1. 重新命名範本型別[&#128279;](../../user-guide/templates/customize-template.md#recognized-field-names)的管道所需的所有欄位的圖層。

| 頻道 | 產生所需的欄位 | 用於產生的選用欄位 |
| --- | --- | --- |
| LinkedIn | `{on_image_text}`, `{image}` | `{headline}`, `{introductory_text}`, `{cta}`, `{website_url}` |
| Meta | `{on_image_text}`, `{image}` | `{body}`, `{headline}`, `{cta}`, `{website_url}`, `{display_link}` |
| 顯示 | `{body}`, `{image}` | `{headline}`, `{cta}`, `{website_url}` |

請注意，多個圖層可以共用相同的欄位指定，但每個圖層只能指定一個欄位。 例如，如果檔案中有多個工作區域：

* 您可以指定每個工作區域中的`{headline}`圖層。
* 您可以在單一工作區域指定多個`{headline}`圖層。
* 您無法指定單一圖層同時接收`{headline}`和`{cta}`欄位名稱。

### 範本大小要求

#### Meta範本

對於Instagram和Facebook貼文：

* 寬度：1080畫素（固定）
* 高度：1080畫素或1350畫素

若為Instagram和Facebook故事：

* 寬度：1080畫素（固定）
* 高度：1920畫素

外掛程式會根據範本的高度來決定所產生體驗的顏色。

#### 顯示範本

沒有固定大小的要求。 顯示範本支援任何大小。

#### LinkedIn範本

* 寬度：1200畫素（固定）
* 高度：1200畫素、628畫素、2292畫素、1800畫素或1500畫素

檔案現在已準備好與外掛程式搭配使用。

## 產生新內容

1. 開啟Photoshop。
1. 開啟您已建立的GenStudio就緒範本檔案（請參閱上述指示），或使用GenStudio for Performance Marketing入門範本： `branding-template-acrobat-handlebars.psd`。
1. 在&#x200B;**[!UICONTROL 外掛程式]** > **[!UICONTROL GenStudio]**&#x200B;開啟外掛程式面板。
1. 按一下&#x200B;**[!UICONTROL 登入]**&#x200B;按鈕。 如果系統提示要開啟URL的許可權，可選擇勾選&#x200B;**記住我的選擇**，然後按一下&#x200B;**[!UICONTROL 允許]**。
1. 使用網頁瀏覽器以可存取GenStudio for Performance Marketing的設定檔登入。
1. 選取要套用至您已開啟之範本的管道（Meta、LinkedIn或Display）。
   ![頻道選取](./ps-select-channel.png){width="300" zoomable="yes"}
1. 選取用於產生內容的[!DNL Brand]、[!DNL Persona]和[!DNL Product]內容。
   ![品牌、角色和產品選取](./ps-select-box.png){width="300" zoomable="yes"}
1. 選取要產生的變數數目。
1. 使用「**[!UICONTROL 選取內容]**」下的按鈕，從您的資產中瀏覽並選擇影像。 最近新增的40個資產會先出現，您可以搜尋其他資產。 選取的影像會自動調整大小以符合您的範本。
1. 在&#x200B;**[!UICONTROL 文字提示]**&#x200B;方塊中提供內容的文字提示。
1. 按一下&#x200B;**[!UICONTROL 產生]**&#x200B;按鈕。 變化會顯示在外掛程式面板的卡片上。

新檔案會新增至您的Photoshop工作區，且產生的內容會套用至範本欄位。 這些檔案的名稱具有編號的變數尾碼。

## 翻譯內容

產生副本後，使用者可以將內容翻譯成支援的語言。

1. 使用外掛程式產生廣告復本後，請按一下&#x200B;**[!UICONTROL 翻譯]**。
1. 選取翻譯的一或多個語言。
1. 按一下&#x200B;**[!UICONTROL 翻譯]**&#x200B;按鈕。

新檔案會新增至您的Photoshop工作區，且產生的內容會套用至範本欄位。 這些檔案的名稱具有編號的變數尾碼。

## 將體驗匯出至GenStudio

使用者可選取在內容產生或翻譯後匯出。 匯出的體驗會填入GenStudio for Performance Marketing的內容區段中。

![內容區段中所顯示的匯出資產](./content-assets.png){width="90%"}

## 將Figma框架轉換為Photoshop

圖形框架可以轉換為Photoshop檔案並匯出以用於GenStudio Photoshop。 若要瞭解如何轉換框架，請參閱Figma外掛程式頁面中的[將Figma框架轉換成Photoshop](figma-plugin.md#convert-figma-frames-to-photoshop)區段。

## 疑難排解

如果在產生的變化中未取代文字或影像，請考量這些最佳實務和提示。

### 對應的欄位

如果未取代文字或影像，則確認欄位正確對應為大括弧`{}` （不是括弧`()`）。

### 確認字型是否可用

文字欄位的字型必須可在您的電腦上使用，才能在產生期間進行取代。 確認檔案中使用的所有字型在您的電腦上均可用，尤其是當檔案是在其他電腦上建立時。

### 欄位對應例外

{{$include /help/_includes/field-mapping-exceptions.md}}
