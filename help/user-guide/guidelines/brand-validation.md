---
title: Adobe GenStudio for Performance Marketing中的品牌驗證
description: 瞭解GenStudio for Performance Marketing中的內建品牌驗證系統。
feature: Brand Personalization, Variant Generation, Compliance, Content Generation, Content Review, Generative AI
exl-id: 2e777186-3b7e-46a6-9d37-7c7b7c2aa7ae
source-git-commit: 6a33f7e3a769eda459f70e6ab4e8559064ede2b4
workflow-type: tm+mt
source-wordcount: '781'
ht-degree: 0%

---

# 品牌驗證

在GenStudio for Performance Marketing中，品牌驗證是與產生AI功能和指導方針 — [[!DNL Brands]](/help/user-guide/guidelines/brands.md)、[[!DNL Products]](/help/user-guide/guidelines/products.md)和[[!DNL Personas]](/help/user-guide/guidelines/personas.md) — 共同運作的基本元件。 這可確保所有內容符合您的品牌識別、ADA標準和個別通路平台指引。

GenStudio for Performance Marketing會針對不同方面執行品牌驗證和其他內容檢查，包括：

* 已定義或預設[!DNL Brand]指南
* 平台指南
* [協助工具支援](/help/user-guide/guidelines/brand-validation.md#supporting-your-accessibility-strategy)
<!-- * Ethical considerations related to gender, ethnicity, race, disability status, and age in AI-generated content -->


## 內容檢查摘要

可透過畫布中每個變體的&#x200B;_內容檢查_&#x200B;摘要圖示，存取產生內容之每個專案的品牌驗證摘要和其他內容檢查資訊。

_內容檢查_&#x200B;摘要顯示：

* 以通過驗證的[[!DNL Brand]](brands.md)個准則[與測試過的准則數目相較之下，計算出](overview.md)的符合性百分比
* 平台指引的`Pass`或`Fail`個結果，例如Meta或LinkedIn
* ADA協助工具標準的`Pass`或`Fail`個結果

![內容檢查摘要](/help/assets/content-check-summary.png){width="400" zoomable="yes"}

按一下百分比以檢視變體的相容性。 當您編輯變體或其他內容時，分數會自動更新。 您可以按一下[檢視並修正問題] __，確保進一步合規性。

請參閱[改善品牌一致性](#improve-brand-alignment)。

## 內容檢查面板

從右側的動作列&#x200B;_或_&#x200B;按一下&#x200B;_內容檢查_&#x200B;摘要圖示&#x200B;[_時，_&#x200B;內容檢查](#content-check-summary)面板會在畫布的右側開啟。 此面板提供詳細的品牌驗證、平台指引和無障礙標準資訊，並闡明改善的機會。

![內容檢查面板](/help/assets/content-check-panel.png){width="400" zoomable="yes"}

_內容檢查_&#x200B;面板會顯示影像和變體區段的驗證和[相容性資訊](/help/user-guide/guidelines/overview.md#compliance)：

* 代表&#x200B;_、平台指引及協助工具標準的_&#x200B;內容檢查[!DNL Brand]摘要資訊
* _需要檢閱_&#x200B;區段，顯示失敗准則的數目以及每個需要修訂之准則的詳細資訊
* _通過_&#x200B;區段，顯示通過准則的數目以及有關每個通過准則的詳細資訊

請參閱[改善品牌一致性](#improve-brand-alignment)，瞭解如何改善&#x200B;_內容檢查_&#x200B;面板分數。

### 內容型別

在&#x200B;_內容檢查_&#x200B;面板中，您可以切換要執行哪些准則和協助工具標準檢查。 按一下面板頂端的&#x200B;_內容型別_&#x200B;圖示（層級圖示）以開啟或關閉：

* **[!DNL Brand]** — 執行與[!DNL Brand]准則相關的檢查
* **平台指南** — 執行與特定通道平台(例如Meta)相關的檢查
* **協助工具** — 執行與ADA協助工具標準相關的檢查

若要&#x200B;**為您要執行的檢查設定內容型別**，請按一下以關閉或開啟可用的型別，然後按一下&#x200B;**套用**。

## 改善品牌一致性

若要最大化產生內容的效能並維持一致的品牌識別，請使用&#x200B;[_內容檢查_&#x200B;摘要](#content-check-summary)和&#x200B;[_內容檢查_&#x200B;面板](#content-check-panel)。 您可以手動修改特定區段，以符合您的[[!DNL Brand] 指南](brands.md)、平台指南檢查及協助工具標準檢查。

**若要改善產生之變體的品牌一致性**：

1. 按一下右側動作列中的&#x200B;_內容檢查_&#x200B;面板圖示，以檢視驗證和協助工具資訊。

   您可以看到&#x200B;_需要檢閱_&#x200B;和&#x200B;_通過_&#x200B;檢查的摘要，以檢視哪些需要改進。

   >[!NOTE]
   >
   > _內容檢查_&#x200B;面板中註記的&#x200B;_品牌聲音_&#x200B;指引適用於整個變體，而非個別區段。 系統會強調顯示整個內容變體，以利提出改善建議。

1. 按一下以修正目前不相容的准則。
1. 按一下以展開並檢查每個需要在可用區段（例如&#x200B;_標題_、_色彩_&#x200B;和&#x200B;_品牌語音_）中檢閱的檢查。

   使用為每個檢查提供的推理來指導您修訂影像和變體。

1. 進行必要的修訂後，請按一下[重新檢查分數] ****&#x200B;來重新檢查並驗證您的變更，以確保它們符合您的品牌識別、平台指引及協助工具標準。

   內容檢查程式會再次執行。 如果修訂專案通過驗證，則會在畫布底部顯示綠色橫幅，以確認分數已更新。 如果重新檢查後沒有變更，橫幅會確認分數沒有變更。 修訂變體的&#x200B;_內容檢查_&#x200B;摘要圖示中的百分比也會顯示您的進度。

1. 繼續修訂區段，以確保整個變體通過驗證和協助工具檢查。 使用畫布中個別變體旁的箭頭，導覽至每個變體。

## 支援協助工具策略

GenStudio for Performance Marketing包含內容檢查，旨在協助客戶支援其自己的協助工具最佳實務。

此功能包括下列內容檢查：

* 影像提供`<alt>`屬性。
* 產生的文字與背景的對比為4.5:1。
* 避免以不尋常或受限制的方式使用字詞或短語，包括習語和行話。
* 縮寫的擴充形式或含義可供使用。
* 在初中教育層級可讀取內容。

雖然客戶需自行負責其法律和協助工具合規性，但仍鼓勵客戶將這些功能用作為其更廣泛協助工具策略的一部分。
