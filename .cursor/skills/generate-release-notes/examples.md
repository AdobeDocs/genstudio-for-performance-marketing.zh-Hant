---
source-git-commit: c9b8177a564cfcdfd2b63cd28fa22eb93a52d3a7
workflow-type: tm+mt
source-wordcount: '80'
ht-degree: 0%

---
# 發行說明範例

[help/user-guide/release-notes.md](../../help/user-guide/release-notes.md)的貼上就緒模式。 讓色調和結構與周圍的檔案相符。

## 最低正面內容範例（僅限新頁面）

僅在&#x200B;**建立**&#x200B;新的發行說明頁面時才使用。 如果檔案已經存在，請保留其完整的標題。

```yaml
---
title: Adobe GenStudio for Performance Marketing release notes
description: Learn about the latest features and enhancements to Adobe GenStudio for Performance Marketing.
recommendations: noDisplay
role: User
exl-id: 32f5104e-ae15-4092-8a34-642fc641baf9
---
```

## 功能區段（使用Beta）

```markdown
### Generative Expand AI functionality

[!BADGE Beta]{type=Informative tooltip="This feature is currently in Beta, so some functionality may be limited or subject to change."}

Now, in GenStudio for Performance Marketing [!DNL Create] you can use [Generative Expand AI capabilities](/help/user-guide/create/manage-variants.md#use-generative-expand) to expand the dimensions of images and add generative content to fit your ad templates in paid media variants.
```

## 功能區段（文字說明檔案連結）

```markdown
### Compatible assets filter

A new filter in the [!DNL Insights] module automatically hides [unsupported image and video assets](/help/user-guide/insights/published-experiences.md#ad-formats) from ad previews, eliminating visual clutter and broken tiles. This enhancement ensures users only see media that's actually available and ready to use, creating a cleaner and more reliable experience.
```

## 修正和增強功能（專案符號）

```markdown
### Fixes and enhancements

* Added support for [publishing ad experiences](/help/user-guide/activation/activate-linkedin-ad.md) from GenStudio for Performance Marketing into LinkedIn Campaign Manager. [!DNL Activate] supports detailed LinkedIn ad previews before publishing to LinkedIn Campaign Manager.
```

僅將此子區段用於專案&#x200B;**明確**&#x200B;在原始資料中標示為修正或增強功能。

## 封存的區塊（舊版的發行說明）

```markdown
+++Notes from 2025.05.15

### Fixes and enhancements

* Enabled functionality for [adding alternative (alt) text](/help/user-guide/create/manage-variants.md#add-alt-text-for-images) to an image for an individual variant.
* Added a [new Meta aspect ratio](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) —Landscape 1.19:1 (1080 pixel width).
* Now you can choose more than one experience for export or download. See [Export experiences](/help/user-guide/content/manage-assets.md#export-experiences).

+++
```
