---
title: Meta廣告範本指引
description: 搭配Adobe GenStudio for Performance Marketing使用Meta廣告範本時，請遵循最佳實務作法。
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: e69039b0-272d-4f39-b0e4-916be710fd5f
source-git-commit: 3251d81a6bfb0c1f7d2bf3c5bd319ad4e2237699
workflow-type: tm+mt
source-wordcount: '375'
ht-degree: 1%

---

# Meta廣告範本指引

Meta廣告範本可協助您在Meta平台上建立視覺上一致且有效的廣告。 您可以遵循建議的設計實務並使用支援的欄位，確保您的範本已針對GenStudio for Performance Marketing最佳化。 本指南說明如何架構、自訂和準備Meta廣告範本，以順暢整合併取得高影響力的結果。

自訂Meta廣告範本以搭配GenStudio for Performance Marketing使用時，請遵循下列設計最佳實務：

- 使用360畫素寬度作為欄版面
- 影像的最低解析度為1080 x 1080畫素
- 僅需要一個影像欄位
- 請&#x200B;**不**&#x200B;使用相對字型大小
- 請&#x200B;**不**&#x200B;定義檢視區
- 請&#x200B;**不**&#x200B;使用JavaScript
- 請&#x200B;**不**&#x200B;覆寫CSS中的HTML元素
- 使用`<img>`標籤而非`background-image`
- 使用遮罩來改善背景影像的文字可讀性
- 只能使用一個區段，以產生一組範本元素

## 可辨識的欄位名稱

自訂Meta廣告範本時，請套用這些必填欄位的內容預留位置：

- `image` (必要，從JPEG、PNG或GIF內容中選取)
- `on_image_text` （出現在影像上的文字）

GenStudio for Performance Marketing會自動產生下列欄位。 您不需要為下列專案套用內容預留位置：

- `headline`
- `body`
- `cta`

請參閱[內容預留位置](/help/user-guide/templates/customize-template.md#content-placeholders)，進一步瞭解如何在範本中使用欄位名稱。

## 支援的外觀比例

| 外觀比例 | 尺寸（畫素） | 備註 |
|------------------|----------------------------|-----------------------------------------------------------------------|
| 正方形1:1 | 1080 x 1080 | 適用於大多數Meta版位的標準；建議用於廣泛的相容性。 |
| 縱向4:5 | 1080 x 1350 | 針對行動饋送最佳化；提供更垂直的空間。 |
| 劇本9:16 | 1080 x 1920 | 適用於劇本和膠捲；填滿整個行動熒幕。 |
| 橫向1.91:1 | 1080 x 566 | 最適合連結廣告和新聞摘要位置；廣泛格式。 |
| 自訂 | 最小50 x 50 （寬度） | 僅在需要時使用；可能會導致裁切或縮放。 |

如果廣告不是以其中一個外觀比例設計，GenStudio for Performance Marketing會自動將影像裁切成適當的大小。

## 範本範例

+++範例： Meta廣告範本

<!-- Does this need to be a precise size? -->

以下是Meta廣告範本的基本範例。 標題包含用於樣式的內嵌CSS。 本文使用[內容預留位置](#content-placeholders) （例如`image`和`on_image_text`）來指示GenStudio for Performance Marketing可以在何處產生內容。

```html {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Adobe</title>
        <style>
            .ad-container {
            font-family: Helvetica, sans-serif;
            position: relative;
            text-align: center;
            height: 100%;
            }
            .ad-image {
            width: 100%;
            height: 100%;
            object-fit: cover;
            }
            .ad-text {
            position: absolute;
            top: 0;
            left: 0;
            margin: 1em;
            background-color: rgba(0, 0, 0, 0.5);
            color: white;
            padding: 1em;
            font-size: 75px;
            }
        </style>
    </head>
    <body>
        <div class="ad-container">
            <img src="{{image}}" alt="Ad Image" class="ad-image" />
            <div class="ad-text">{{on_image_text}}</div>
        </div>
    </body>
</html>
```

+++
