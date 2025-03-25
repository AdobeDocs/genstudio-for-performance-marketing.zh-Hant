---
title: 範本的最佳實務
description: 搭配Adobe GenStudio for Performance Marketing使用範本時，請遵循最佳實務作法。
level: Intermediate
role: Developer, User
feature: Media Templates, Content Generation, Brand Personalization
exl-id: 3ff24fec-e836-4202-80f8-ba165e173b75
source-git-commit: daada794dd39c9bd2aea7815d887821454d162fc
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 0%

---

# 使用範本的最佳實務

範本提供包括預先設定版面和設計元素的起點，大幅減少產生新內容所需的時間和精力。

搭配GenStudio for Performance Marketing使用範本時，請使用下列建議：

1. 瞭解[範本元素](#know-about-template-elements)
1. 設定[頻道准則](#configure-channel-guidelines)，以有效個人化內容
1. 使用[協助工具標準](accessibility-for-templates.md)進行設計，以獲得最佳體驗
1. 遵循[特定管道的範本准則](#follow-channel-specific-template-guidelines)

>[!TIP]
>
>在[使用範本](use-templates.md)中進一步瞭解基本範本元素和程式。 深入探討[自訂範本](customize-template.md)以用於您的下一個行銷活動。

## 瞭解範本元素

請熟悉範本的各個部分，當作最佳作法。 每種範本型別使用不同元素來建立通道特定內容建立的結構。 若要自訂您的範本，請使用欄位名稱，取代您需要GenStudio for Performance Marketing產生內容的這些元素。

請參閱[範本元素](use-templates.md#template-elements)。

## 設定頻道准則

在GenStudio for Performance Marketing中使用範本之前，請先設定每個品牌的管道指南。 管道指引直接影響使用範本時產生的內容型別。 例如，您可以在電子郵件內文中設定字元限制。

![主體規格](/help/assets/channel-email-body.png)

請參閱[頻道准則](/help/user-guide/guidelines/brands.md#channel-guidelines)。

## 遵循特定頻道的範本准則

建立範本時，請確保它們符合預期通道的特定需求。 建立可容納每個管道的版面和視覺需求的範本。 有些一般准則適用於任何範本，例如：

- 使用簡潔且回應式的HTML和內嵌CSS
- 使用Adobe或Google字型
- 請&#x200B;**不**&#x200B;使用JavaScript

使用每種範本型別時，請考量下列提示和限制，以確保最佳效能和相容性：

>[!BEGINTABS]

>[!TAB 電子郵件]

自訂電子郵件範本以搭配GenStudio for Performance Marketing使用時，請遵循下列設計最佳實務：

- 使用Adobe或Google字型
- 使用簡潔且回應式的HTML和內嵌CSS
- 請&#x200B;**不**&#x200B;使用JavaScript
- 請&#x200B;**不**&#x200B;在主體或容器中使用固定寬度
- 請&#x200B;**不**&#x200B;使用base64編碼處理影像，因為它會大幅增加範本大小

**限制**：

- 使用[區段](customize-template.md#sections-or-groups)：
   - 基本範本（僅一個區段）可以產生一組範本元素。
   - 複雜範本（多個區段）最多可以產生三組範本元素。
- 範本中允許的最大欄位為20
- HTML檔案大小上限為102 KB

**可辨識的欄位名稱**：

對於電子郵件，會自動包含`subject`欄位。 在下列欄位中使用內容預留位置：

- `pre_header`
- `headline`
- `body`
- `cta`
- `image` (從JPEG、PNG或GIF內容中選取)
- `brand_logo`

請參閱[內容預留位置](customize-template.md#content-placeholders)，進一步瞭解如何在範本中使用欄位名稱。

>[!TAB 中繼廣告]

自訂中繼廣告範本以搭配GenStudio for Performance Marketing使用時，請遵循下列設計最佳實務：

- 使用360畫素寬度作為欄版面
- 影像的最低解析度為1080 x 1080畫素
- 請&#x200B;**不**&#x200B;使用相對字型大小
- 請&#x200B;**不**&#x200B;定義檢視區
- 請&#x200B;**不**&#x200B;使用JavaScript
- 請&#x200B;**不**&#x200B;覆寫CSS中的HTML元素
- 使用`<img>`標籤而非`background-image`
- 使用遮罩來改善背景影像的文字可讀性

**限制**：

- 使用[區段](customize-template.md#sections-or-groups)：
   - 只能使用一個區段，以產生一組範本元素。

**支援的外觀比例**：

- 正方形1:1 （1080 x 1080畫素）
- 垂直4:5 （1080 x 1350畫素）
- 內文9:16 （1080 x 1920畫素）
- 自訂影像大小： （50 x 50畫素最小影像寬度）

**可辨識的欄位名稱**：

對於中繼廣告，`headline`、`body`和`CTA`欄位會自動產生。 在下列欄位中使用內容預留位置：

- `image` (從JPEG、PNG或GIF內容中選取)
- `on_image_text`
- `brand_logo`

請參閱[內容預留位置](customize-template.md#content-placeholders)，進一步瞭解如何在範本中使用欄位名稱。

>[!TAB 橫幅和顯示廣告]

自訂橫幅和顯示廣告範本以搭配GenStudio for Performance Marketing使用時，請遵循下列設計最佳實務：

- 使用Adobe或Google字型
- 準備以超薄尺寸顯示的優異資產
- 請&#x200B;**不**&#x200B;使用內嵌或編碼的背景影像
- 使用已上傳至GenStudio for Performance Marketing內容存放庫的背景影像（`image`欄位）
- 請&#x200B;**不**&#x200B;使用JavaScript

**限制**：

- 使用[區段](customize-template.md#sections-or-groups)：
   - 只能使用一個區段，以產生一組範本元素。

**支援的維度**：

- 垂直： （畫素）
   - 300 x 600
   - 160 x 600&#x200B;
- 水準： （畫素）
   - 300 x 250
   - 728 x 90
   - 336 x 280
   - 320 x 50
   - 970 x 250&#x200B;
- 自訂： （畫素）
   - 50 x 50至2000 x 2000

**可辨識的欄位名稱**：

對於橫幅和顯示廣告，會自動產生`CTA`欄位。 在下列欄位中使用內容預留位置：

- `headline`
- `body`
- `image` (從JPEG、PNG或GIF內容中選取)

請參閱[內容預留位置](customize-template.md#content-placeholders)，進一步瞭解如何在範本中使用欄位名稱。

>[!TAB LinkedIn廣告]

[!BADGE Beta]{type=Informative tooltip="此功能目前在Beta中，因此某些功能可能會受到限制或有所變更。"}

自訂LinkedIn廣告範本以搭配GenStudio for Performance Marketing使用時，請遵循下列設計最佳實務：

**限制**：

- 使用[區段](customize-template.md#sections-or-groups)：
   - 只能使用一個區段，以產生一組範本元素。
- 影像大小上限為5 MB
- 標題最多70個字元
- 介紹文字上限150個字元

**支援的外觀比例**：

- 正方形1:1
   - 桌上型電腦或行動裝置
   - 最小：360 x 360畫素
   - 最大：4320 x 4320畫素
- 水準1.91:1
   - 案頭
   - 最小：640 x 360畫素
   - 最大：7680 x 4320畫素
- 垂直1:1.91
   - 行動
   - 最小：360 x 640畫素
   - 最大：2430 x 4320畫素
- 垂直2.3
   - 行動
   - 最小：360 x 640畫素
   - 最大：2430 x 4320畫素
- 垂直4.5 （建議）
   - 行動
   - 最小：360 x 640畫素
   - 最大：2430 x 4320畫素

**可辨識的欄位名稱**：

對於LinkedIn廣告，`headline`、`introductory_text`和`CTA`欄位會自動產生。 在下列欄位中使用內容預留位置：

- `image` (從JPEG、PNG或GIF內容中選取)
- `on_image_text`
- `brand_logo`

請參閱[內容預留位置](customize-template.md#content-placeholders)，進一步瞭解如何在範本中使用欄位名稱。

>[!ENDTABS]
