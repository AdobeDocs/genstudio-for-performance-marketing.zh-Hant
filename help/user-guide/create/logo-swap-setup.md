---
title: 在範本中設定圖志交換
description: 設定範本中的品牌標誌預留位置，以啟用 [!DNL GenStudio for Performance Marketing]中的標誌交換。
feature: Create Canvas
role: User
level: Intermediate
source-git-commit: 98cb7ba338878495e6d7b68f3b8c620abae10127
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 2%

---

# 在範本中設定圖志交換

本指南說明如何在範本中設定品牌標誌預留位置，以啟用[!DNL GenStudio for Performance Marketing]中的[標誌交換功能](/help/user-guide/create/logo-swap.md)。 請依照這些准則來確保預留位置在各種影像大小和外觀比例中正確顯示。

## 快速設定

針對您的標誌影像使用下列基本範本程式碼：

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="my-logo"
>
```

必填：

- `src="{{brand_logo}}"` — 啟用圖志交換功能。
- `style="{{defaultLogo}}"` — 套用預留位置邊框樣式。

可選：

- `class="my-logo"` — 您用於調整大小和樣式的自訂CSS類別。

## 瞭解預留位置邊框

未選取標誌時，`{{brand_logo}}`會包含透明的1×1畫素影像。 `{{defaultLogo}}`樣式會自動套用外框，使預留位置可見：

```css
outline: clamp(1px, 0.1em, 5px) dashed #FFF;
```

邊框行為：

- 顯示預設預留位置時顯示。
- 更換標誌後會自動消失。
- 根據父字型大小縮放。

### 邊框大小

`clamp()`函式會調整外框粗細以符合範本大小：

| 父字型大小 | 大綱大小 |
| --- | --- |
| 10px | 1px （分鐘） |
| 16px | 1.6px |
| 24px | 2.4px |
| 32px | 3.2px |
| 50px+ | 5px （最大值） |

公式： `0.1em`等於繼承字型大小的10%，夾在`1px`和`5px`之間。

## 自訂預留位置邊框

您可以使用CSS類別來覆寫預設大綱。 `{{defaultLogo}}`樣式會套用基本外框，而您的類別可以自訂顏色、寬度和樣式。

範本HTML：

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-custom-border"
>
```

範本CSS：

```css
.logo-custom-border {
  outline-color: #0066CC !important;
  outline-width: 2px !important;
  outline-style: dotted !important;
}
```

>[!NOTE]
>自訂外框樣式只會影響預留位置。 一旦更換標誌，所有外框樣式都會自動移除。

## 設定建議的標誌大小

若要確保預留位置可見並避免版面位移，請在CSS類別中設定明確的大小：

範本HTML：

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-standard"
>
```

範本CSS：

```css
.logo-standard {
  width: 120px;
  height: 60px;
}
```

## 控制標誌定位

使用`object-fit`和`object-position`控制標誌在其容器內的縮放方式。

### 標誌置中（最常見）

標誌會縮放以符合150×80畫素，水平與垂直皆置中。

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-centered"
>
```

```css
.logo-centered {
  width: 150px;
  height: 80px;
  object-fit: contain;
  object-position: center center;
}
```

### 標誌靠左對齊

標誌會縮放以符合，對齊左邊緣，垂直置中。

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-left"
>
```

```css
.logo-left {
  width: 200px;
  height: 60px;
  object-fit: contain;
  object-position: left center;
}
```

### 右上角的標誌

標誌縮放以符合，位於右上角。

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-top-right"
>
```

```css
.logo-top-right {
  width: 100px;
  height: 100px;
  object-fit: contain;
  object-position: right top;
}
```

## 完整範例

### 最小設定

```html
<img src="{{brand_logo}}" style="{{defaultLogo}}">
```

>[!NOTE]
>此設定可以運作，但預留位置可能幾乎不可見，因為透明的1×1畫素影像會縮疊到其自然大小。 使用包含`width`和`height`的CSS類別作為可見的預留位置。

### 建議的設定

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="brand-logo"
>
```

```css
.brand-logo {
  width: 120px;
  height: 60px;
  object-fit: contain;
  object-position: center center;
}
```

### 使用自訂邊框的進階設定

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="sponsor-logo"
>
```

```css
.sponsor-logo {
  width: 180px;
  height: 90px;
  object-fit: contain;
  object-position: left center;
  outline-color: #0066CC !important;
  outline-width: 2px !important;
  outline-style: solid !important;
}
```

### 彈性設定，具有大小限制

針對回應式範本或各種標誌大小使用`min-*`和`max-*`屬性。

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-flexible"
>
```

```css
.logo-flexible {
  min-width: 20px;
  min-height: 20px;
  max-width: 200px;
  max-height: 100px;
  object-fit: contain;
  object-position: center center;
}
```

運作方式：

- `min-width`和`min-height`保持預留位置可見。
- `max-width`和`max-height`防止過大的標誌破壞版面。
- 標誌會依比例在這些邊界內縮放。

## CSS屬性參考

| 類別 | 屬性 | 值 | 用途 |
| --- | --- | --- | --- |
| 必要(HTML) | `src` | `{{brand_logo}}` | 啟用圖志交換功能。 |
| 必要(HTML) | `style` | `{{defaultLogo}}` | 套用預留位置大綱。 |
| 建議（CSS類別） | `width` | `120px` | 設定最大標誌寬度。 |
| 建議（CSS類別） | `height` | `60px` | 設定最大標誌高度。 |
| 建議（CSS類別） | `object-fit` | `contain` | 縮放標誌而不裁切。 |
| 建議（CSS類別） | `object-position` | `center center` | 控制標誌對齊方式。 |
| 選用（CSS類別） | `outline-color` | `#FF0000` | 變更外框顏色。 |
| 選用（CSS類別） | `outline-width` | `3px` | 變更外框粗細。 |
| 選用（CSS類別） | `outline-style` | `solid` | 變更大綱樣式。 |
| 彈性調整（CSS類別） | `min-width` | `20px` | 確保預留位置可見性。 |
| 彈性調整（CSS類別） | `min-height` | `20px` | 確保預留位置可見性。 |
| 彈性調整（CSS類別） | `max-width` | `200px` | 防止溢位。 |
| 彈性調整（CSS類別） | `max-height` | `100px` | 控制配置界限。 |

## 最佳做法

執行：

- 一律包含`{{brand_logo}}`和`{{defaultLogo}}`。
- 定義`width`和`height`，以顯示預留位置。
- 使用CSS類別進行大小調整和大綱自訂。
- 使用`object-fit: contain`保留標誌外觀比例。
- 使用不同大小和外觀比例的圖志進行測試。

請勿：

- 使用`border`而非`outline` （不會自動隱藏邊框）。
- 在內嵌樣式中放置大小屬性。
- 省略大小限制（預留位置會以1×1畫素呈現）。
- 使用`object-fit: cover` （它可能會裁切標誌）。

## 疑難排解

邊框不可見：

- 確定已包含`style="{{defaultLogo}}"`。
- 確認已在您的CSS類別中定義`width`和`height`。

預留位置太小(1px)：

- 將明確的`width`和`height`新增到您的CSS類別。

交換後邊框沒有消失：

- 在您的CSS類別中使用大綱屬性，而非`border`。

會裁切標誌：

- 使用`object-fit: contain`而非`cover`。

標誌太小或太大：

- 調整您CSS類別中的`width`和`height`。

未顯示自訂邊框：

- 確認`{{defaultLogo}}`在`style`屬性中。
- 將自訂`outline-*`屬性放入CSS類別中。
