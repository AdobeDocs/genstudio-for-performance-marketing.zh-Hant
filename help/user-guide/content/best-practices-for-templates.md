---
title: 範本的最佳實務
description: 搭配Adobe GenStudio for Performance Marketing使用範本時，請遵循最佳實務作法。
feature: Templates, Content
last-substantial-update: 2024-12-09T00:00:00Z
source-git-commit: 7ba2ecfbdd6853934be5210685bf447848715d28
workflow-type: tm+mt
source-wordcount: '0'
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

建立可容納每個管道的版面和視覺需求的範本。 使用每種範本型別時，請考量下列提示和限制，以確保最佳效能和相容性：

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
- `image` （從內容中選取）
- `brand_logo`

請參閱[內容預留位置](customize-template.md#content-placeholders)，進一步瞭解如何在範本中使用欄位名稱。

>[!TAB 中繼廣告]

自訂中繼廣告範本以搭配GenStudio for Performance Marketing使用時，請遵循下列設計最佳實務：

- 使用360畫素寬度作為欄版面
- 影像的最低解析度為1080 x 1080畫素
- 請&#x200B;**不**&#x200B;使用相對字型大小
- 請&#x200B;**不**&#x200B;定義檢視區
- 請&#x200B;**不**&#x200B;使用JavaScript
- 請&#x200B;**不**&#x200B;覆寫CSS中的HTML專案
- 對背景影像使用下列設定：

  新增`object-fit: cover`值至`background-image` CSS類別：

  ```css
  .background-image {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
  ```

**限制**：

- 使用[區段](customize-template.md#sections-or-groups)：
   - 只能使用一個區段，以產生一組範本元素。

**支援的外觀比例**：

- 正方形1:1 （1080 x 1080畫素）
- 垂直4:5 （1080 x 1350畫素）
- 內文9:16 （1080 x 1920畫素）

**可辨識的欄位名稱**：

對於中繼廣告，`headline`、`body`和`CTA`欄位會自動產生。 在下列欄位中使用內容預留位置：

- `image` （從內容中選取）
- `on-image-text`
- `brand_logo`

請參閱[內容預留位置](customize-template.md#content-placeholders)，進一步瞭解如何在範本中使用欄位名稱。

>[!TAB 顯示廣告]

自訂顯示廣告範本以搭配GenStudio for Performance Marketing使用時，請遵循下列設計最佳實務：

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

**可辨識的欄位名稱**：

在下列欄位中使用內容預留位置：

- `headline`
- `body`
- `cta`
- `image` （從內容中選取）

請參閱[內容預留位置](customize-template.md#content-placeholders)，進一步瞭解如何在範本中使用欄位名稱。

>[!ENDTABS]
