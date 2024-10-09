---
title: 為Adobe GenStudio for Performance Marketing準備中繼廣告範本
description: 瞭解如何建立Adobe GenStudio for Performance Marketing的自訂中繼廣告範本。
level: Intermediate
feature: Templates, Content
exl-id: e69039b0-272d-4f39-b0e4-916be710fd5f
source-git-commit: ce08231cb723bec3d80a732837b72a435d3b552d
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# 為Adobe GenStudio for Performance Marketing準備中繼廣告範本

建立中繼廣告範本涉及為社群媒體量身打造的結構化方法。 設計和測試中繼廣告範本後，您就可以準備將其上傳和用於GenStudio for Performance Marketing。

## 新增准則

在準備中繼廣告範本之前，請確定您已將[指導方針](/help/user-guide/guidelines/overview.md)新增到您的GenStudio for Performance Marketing中，並填入相關品牌的完整資訊。 [品牌指導方針](/help/user-guide/guidelines/brands.md)直接影響產生的內容。

**範例**：如果您希望中繼廣告範本內文不超過500個字元，請將該要求新增至「內文」欄位的[頻道准則](/help/user-guide/guidelines/brands.md#channel-guidelines)。

如果未將准則新增至GenStudio for Performance Marketing，則會使用預設值。

## 設計範本

通常，設計人員會在設計程式(例如Adobe XD)中建立範本的視覺化設計。

檢視[範本元素](use-templates.md#template-elements)和[範本範例](/help/user-guide/content/customize-template.md#template-examples)。

### 廣告規格

GenStudio for Performance Marketing支援中繼廣告的這些外觀比例：

* 正方形(1:1)：1080 x 1080畫素
* 垂直(4:5)：1080 x 1350畫素
* 內文(9:16)：1080 x 1920畫素

如果廣告不是以其中一個外觀比例設計，GenStudio for Performance Marketing會自動將影像裁切成適當的大小。

## 測試中繼廣告範本

使用Meta的Creative Hub測試您的範本，以檢視廣告在不同位置（例如資訊源或內文）的外觀。

使用您的電子郵件傳遞或校訂平台來測試您的電子郵件，並確認其是否正確在不同電子郵件使用者端和裝置間呈現。

## 定義產生的內容區域

定義電子郵件範本中應動態填入GenStudio for Performance Marketing內容的區域。

若要定義產生的內容區域，請執行下列動作：

* 識別GenStudio for Performance Marketing應自動產生的範本文字元素，例如標題或CTA。
* 使用Handlebars語法在HTML範本中插入預留位置，以調整範本。

請參閱[內容預留位置](/help/user-guide/content/customize-template.md#content-placeholders)。

## 預覽範本

使用內建協助程式控制特定內容區域的可見度。 例如，在匯出的範本中加入連結的追蹤引數，同時保持整潔的預覽連結。

請參閱[範本預覽](/help/user-guide/content/customize-template.md#template-preview)。

## 上傳並使用範本

在設計、編碼、測試和預覽範本後，將其上傳至GenStudio for Performance Marketing以用於產生全新的行銷內容。

請參閱[使用範本](use-templates.md)。
