---
title: 為Adobe GenStudio for Performance Marketing準備電子郵件範本
description: 瞭解如何建立Adobe GenStudio for Performance Marketing的自訂電子郵件範本。
level: Intermediate
feature: Templates, Content
exl-id: 8b1e8d32-5a23-45ce-a2d4-ae6de3698c45
source-git-commit: 478815d74a742cdc05d3f1faebf27d5adc04d417
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# 為Adobe GenStudio for Performance Marketing準備電子郵件範本

通常，設計人員會在設計程式(例如Adobe XD)中建立範本的視覺化設計。 設計、編碼和測試電子郵件範本後，您就可以準備將其上傳和用於GenStudio for Performance Marketing。

請參閱[範本元素](use-templates.md#template-elements)。

## 新增准則

在準備中繼廣告範本之前，請確定您已將[指導方針](/help/user-guide/guidelines/overview.md)新增到您的GenStudio for Performance Marketing中，並填入相關品牌的完整資訊。 [品牌指導方針](/help/user-guide/guidelines/brands.md)直接影響產生的內容。

**範例**：如果您希望電子郵件範本內文不超過500個字元，請將該要求新增至「內文」欄位的[頻道准則](/help/user-guide/guidelines/brands.md#channel-guidelines)。

如果未將准則新增至GenStudio for Performance Marketing，則會使用預設值。

## 為電子郵件範本編碼

設計範本後，會使用HTML和內嵌CSS對其進行編碼。 程式碼應該對各種裝置而言是乾淨和回應式的。

請參閱[範本範例](/help/user-guide/content/customize-template.md#template-examples)。

### 多節電子郵件

您可以在內容產生期間使用[結構化提示](/help/user-guide/effective-prompts.md#structured-prompts)來指示GenStudio for Performance Marketing在電子郵件的每個區段產生不同的內容。

例如，如果電子郵件範本中的區段以`Pod`—`Pod1`和`Pod2`為前置詞，用於產生內容的結構化提示可以包含這些電子郵件區段的特定指示。 GenStudio for Performance Marketing會將提示中的區段特定指示與相關電子郵件區段進行比對，並產生與指示一致的內容。

請參閱[結構化提示](/help/user-guide/effective-prompts.md#structured-prompts)。

## 測試電子郵件範本

使用您的電子郵件傳遞或校訂平台來測試您的電子郵件，並確認其是否正確在不同電子郵件使用者端和裝置間呈現。

測試以確保您的電子郵件範本滿足下列要求：

* 使用CSS媒體查詢調整不同熒幕大小的版面
* 按鈕可供點按，並導覽至所需位置
* 電子郵件範本在行動裝置上可讀取和使用

## 定義產生的內容區域

定義電子郵件範本中應動態填入GenStudio for Performance Marketing內容的區域。

若要定義產生的內容區域，請執行下列動作：

* 識別GenStudio for Performance Marketing應自動產生的範本文字元素，例如標題或CTA。
* 使用Handlebars語法在HTML範本中插入預留位置，以調整範本。

請參閱[內容預留位置](/help/user-guide/content/customize-template.md#content-placeholders)。

## 預覽範本

使用內建協助程式控制特定內容區域的可見度。 例如，您可以在匯出的範本中加入連結的追蹤引數，同時保持整潔的預覽連結。

請參閱[範本預覽](/help/user-guide/content/customize-template.md#template-preview)。

## 上傳並使用範本

在設計、編碼、測試和預覽範本後，您可以將其上傳至GenStudio for Performance Marketing以用於產生全新的行銷內容。

請參閱[使用範本](use-templates.md)。
