---
title: LinkedIn範本指導方針
description: 搭配Adobe GenStudio for Performance Marketing使用LinkedIn範本時，請遵循最佳實務作法。
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 85432185-8311-411b-b57b-f482c3d45854
source-git-commit: c0f45fb0ffc61d20611693498f1b12d3946ca6ca
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 2%

---

# LinkedIn範本准則

LinkedIn範本提供結構化方式，可建立和自訂LinkedIn行銷活動的廣告創意。 這些准則可確保您的廣告符合LinkedIn的規格，同時簡化GenStudio for Performance Marketing的創作流程。 本指南可協助您準備LinkedIn桌上型電腦和行動平台一致的品牌和有效效能。

自訂LinkedIn廣告範本以搭配GenStudio for Performance Marketing使用時，請遵循下列設計最佳實務：

- 僅需要一個影像欄位
- 影像大小上限為5 MB
- 標題最多70個字元
- 介紹文字上限150個字元
- 只能使用一個區段，以產生一組範本元素

## 可辨識的欄位名稱

自訂LinkedIn範本時，請套用這些必要欄位的內容預留位置：

- `image` (必要，從JPEG、PNG或GIF內容中選取)
- `on_image_text` （出現在影像上的文字）

GenStudio for Performance Marketing會自動產生下列欄位。 您不需要為下列專案套用內容預留位置：

- `headline`
- `introductory_text`
- `cta` (Call to action)

請參閱[內容預留位置](/help/user-guide/content/customize-template.md#content-placeholders)，進一步瞭解如何在範本中使用欄位名稱。

## 支援的外觀比例

| 外觀比例 | Platform | 最小大小（畫素） | 大小上限(px) | 備註 |
|-------------------|-----------------|---------------|----------------|-------------------------------------------------------------------------------------|
| 正方形1:1 | 桌上型電腦、行動裝置 | 360 x 360 | 4320 x 4320 | 最通用。 適用於跨裝置和位置的一致外觀。 |
| 水準1.91:1 | 桌上型電腦 | 640 x 360 | 7680 x 4320 | 標準橫向格式。 通常用於贊助內容和動態消息廣告。 |
| 垂直1:1.91 | 行動 | 360 x 640 | 2430 x 4320 | 高垂直格式。 針對行動檢視進行最佳化，提供更優異的畫面顯示效果。 |
| 垂直2:3 | 行動 | 360 x 640 | 2430 x 4320 | 略低於1:1.91。適用於行動優先的行銷活動。 |
| 垂直4:5 | 行動 | 360 x 640 | 2430 x 4320 | 建議行動裝置使用。 平衡可見度和內容，通常會產生較高的影響力。 |

<!-- Potentially add an example

## Template example

+++Example: LinkedIn template

+++

-->
