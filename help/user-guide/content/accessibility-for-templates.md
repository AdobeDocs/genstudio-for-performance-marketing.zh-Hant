---
title: 建立無障礙範本
description: 在Adobe GenStudio for Performance Marketing中建立範本，這些範本可觸及更多對象並提供最佳體驗。
feature: Media Templates
exl-id: eaaa5d9f-ad45-4fd0-826d-c250deb6d238
source-git-commit: 28c128ad6f3d173b7516a6b1309555c12e6a4e2d
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---

# 建立無障礙範本

Adobe致力於為所有受眾提供最佳體驗。 如需進一步閱讀，請參閱Adobe[&#128279;](https://www.adobe.com/trust/accessibility/initiatives.html)的協助工具方案。

在GenStudio for Performance Marketing中，您可以上傳資產和範本，以針對各種體驗建立內容。 遵循協助工具標準有助於您的內容觸及到最大的目標受眾。

使用下列建議，以使用最佳協助工具標準準備您的範本。

## 替代文字

為非文字內容（例如影像）提供替代文字。

```html
<img alt="Collage of ideas, books, man holding giant pencil, computer" src="card-create-assets.png">
```

![創意拼貼、書籍、拿著巨鉛筆的男人、電腦](/help/assets/card-create-assets.png){width="400"}

自訂範本時，請針對`alt`和`aria-label`屬性使用內容預留位置：

- [替代文字](/help/user-guide/content/customize-template.md#alternative-text)
- [協助工具標籤](/help/user-guide/content/customize-template.md#accessibility-label)

## 字型

使用容易閱讀的字型。 例如，Sans Serif字型具有整潔的區塊式外觀，這有助於提高可讀性。

提供文字和背景之間的適當對比。 避免使用在深色背景產生深色文字，而在淺色背景產生淺色文字的字型顏色。 考量最佳比率的對比准則：

- 文字和影像：對比率至少為4.5:1
- 大型文字的大型文字和影像：至少3:1的對比率

## 連結目的（僅限連結）

建立說明連結目的和位置的清楚連結文字。

例如，使用「按一下這裡」或「閱讀更多」之類的連結文字無法清楚說明連結的用途：

```html
<a href="product-site.html">Click here</a>
```

作為最佳作法，您應該使用清楚說明連結前往位置的文字。 較佳的範例可能會使用連結來源的標題及用途：

```html
<a href="product-site.html">Explore Product Site</a>
```

## 語言

許多產品和服務都會以創意或獨特的方式使用語言。 避免使用行話、長句子和複雜片語。 使用與目標受眾相容的清晰、簡潔、易讀語言。

- 儘可能使用清楚的說明、內嵌定義或相關的範例。 翻譯獨特的白話可能很困難。

- 拼出或連結至首度縮寫或縮寫例項的定義。 縮寫可能很難翻譯。

- 儘可能使用視覺元素來補充文字或複雜的想法。
