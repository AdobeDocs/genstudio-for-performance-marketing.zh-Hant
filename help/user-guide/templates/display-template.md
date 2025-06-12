---
title: 顯示廣告範本准則
description: 搭配Adobe GenStudio for Performance Marketing使用顯示廣告和橫幅範本時，請遵循最佳實務作法。
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 076239b3-9444-48f9-bdd6-ef2b757bdf0d
source-git-commit: 4760da26d20e91489a74bb238e07f0d3b426c0a1
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# 顯示廣告範本准則

顯示範本是預先設計的版面，用於建立吸引目光的橫幅和顯示廣告。 它們提供彈性的架構，整合影像、文字和call to action，確保在製作多個廣告變化時的一致性和效率。 準備要在GenStudio for Performance Marketing中使用的範本時，請確定所有資產已針對Web顯示最佳化，並符合必要的檔案格式和大小。

自訂橫幅和顯示廣告範本以搭配GenStudio for Performance Marketing使用時，請遵循下列設計最佳實務：

- 使用Adobe或Google字型
- 準備以超薄尺寸顯示的優異資產
- 僅需要一個影像欄位
- 請&#x200B;**不**&#x200B;使用內嵌或編碼的背景影像
- 使用已上傳至GenStudio for Performance Marketing內容存放庫的背景影像（`image`欄位）
- 請&#x200B;**不**&#x200B;使用JavaScript
- 只能使用一個區段，以產生一組範本元素

## 可辨識的欄位名稱

自訂橫幅或顯示廣告範本時，請為下列必填欄位使用內容預留位置：

- `headline`
- `sub_headline`
- `body`
- `image` (必要，從JPEG、PNG或GIF內容中選取)

GenStudio for Performance Marketing會自動產生下列欄位。 您不需要為下列專案套用內容預留位置：

- `cta`

請參閱[內容預留位置](/help/user-guide/content/customize-template.md#content-placeholders)，進一步瞭解如何在範本中使用欄位名稱。

## 支援的維度

必須設定寬度x高度（畫素）。

| 方向 | 尺寸（畫素） | 備註 |
|--------------|-------------------------------------------------------------|------------------------------------------------------------------|
| 垂直 | 300 x 600<br>160 x 600 | 摩天大樓和半頁橫幅共用 |
| 水準 | 300 x 250<br>728 x 90<br>336 x 280<br>320 x 50<br>970 x 250 | 標準排行榜、中等矩形和橫幅大小 |
| 自訂 | 50 x 50至2000 x 2000 | 用於非標準或唯一版位；檢查平台限制 |

<!-- Potentially add an example

## Template example

+++Example: Display ad template

+++

-->
