---
title: 屬性總覽
description: 瞭解如何評估Adobe GenStudio for Performance Marketing中特定屬性的效能。
feature: Insights, Attributes
exl-id: 9d05c128-50d5-415a-ae60-7023c36c06ad
source-git-commit: 2abd2d874fb9ce515c9ec15bd6130b5a4dc8bd48
workflow-type: tm+mt
source-wordcount: '785'
ht-degree: 0%

---

# 屬性總覽

[!DNL Insights] _[!UICONTROL 屬性]_&#x200B;檢視會顯示所選管道帳戶在廣告行銷活動中使用的屬性清單。

{{connect-insights}}

_[!UICONTROL 屬性]_&#x200B;表格是使用[!UICONTROL 屬性]名稱來組織。 您可以使用&#x200B;**[!UICONTROL 影像]**&#x200B;按鈕和&#x200B;**[!UICONTROL 影片]**&#x200B;按鈕，在清單型別之間切換。 按一下表格右上方的設定(cog)圖示，以切換可檢視欄。

表格左上方的篩選器（漏斗）圖示會開啟&#x200B;**[!UICONTROL 篩選器]**&#x200B;功能表，您可從中選取[!UICONTROL 帳戶]和[!UICONTROL 屬性類別]，以篩選表格中的屬性。 下列範例顯示`Lighting Condition`類別中的屬性清單。

![屬性篩選器和資料表](/help/assets/insights-attributes-filter.png){zoomable="yes"}

{{$include /help/_includes/download-insights.md}}

## 屬性詳細資料

屬性可協助透過資產的內在細節來識別資產，例如顏色、構成、視覺元素和其他屬性。

在屬性詳細資料檢視中，您可以檢視哪些體驗使用選取的屬性。 詳細資料包括總屬性效能以及與每個體驗相關的效能測量結果劃分。

![屬性績效量度](/help/assets/insights-attribute-details.png){zoomable="yes"}

GenStudio for Performance Marketing會偵測某些功能，並將適當的屬性套用至資產或體驗作為標籤。 請參閱[類別](#categories)，檢視這些標籤的範例。 若要檢視與體驗相關聯的所有屬性，請按一下表格右側上方的設定(cog)圖示，以選取&#x200B;**[!UICONTROL 屬性]**&#x200B;欄。

## 類別

GenStudio for Performance Marketing可辨識影像、影片和文字的特定功能，並將功能標籤套用至資產。 _類別_&#x200B;是共用特定特徵的一組功能。 例如，_影像方向_&#x200B;類別有`landscape`、`portrait`或`square`值。

您無法編輯偵測到並自動套用的標籤。

如需影像、視訊和文字功能的詳細清單，請參閱[屬性類別](/help/user-guide/insights/attribute-category.md)。

## 屬性效能

見解量度可協助您評估哪些屬效能激發更多客戶參與。

下表提供[!UICONTROL 屬性]表格檢視中關鍵數位行銷量度的定義與深入分析。 每個量度都包含與資產相關的簡短定義、量度的計算方式，以及有助於瞭解其對廣告促銷活動之重要性和影響的一或多個深入分析。

| 量度 | 定義 | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL 屬性]** | 屬性名稱。 | 按一下任何關鍵量度的欄標題來排序表格。 |
| **[!UICONTROL 類別]** | 代表屬性固有品質的[類別](#categories)。 |  |
| **[!UICONTROL #影像]** | 具有此屬性的影像數。 | 「屬性」表格中的計數可能與「屬性詳細資訊」檢視中的計數不同。 如果管道來源（例如中繼）和GenStudio使用的摘要計算略有不同，則會出現這種差異。 |
| **[!UICONTROL #影片]** | 具有此屬性的視訊數量。 | 「屬性」表格中的計數可能與「屬性詳細資訊」檢視中的計數不同。 如果管道來源（例如中繼）和GenStudio使用的摘要計算略有不同，則會出現這種差異。 |
| **[!UICONTROL 曝光次數]** | 每次將具有此屬性的影像或影片載入管道時的計數，無論互動或檢視為何。 | 高曝光數可表示廣泛的可見度，但如需真正的效能深入分析，請將其與其他參與量度關聯起來。 |
| **[!UICONTROL 點按]** | 使用者與此屬性之影像或視訊互動的次數。 | 點按次數高表示對內容有強烈的興趣和參與，這可能有效並觸及適當的對象。 |
| **[!UICONTROL CTR ]**<br>_點進率_ | 導致點按具有此屬性的影像或影片的曝光百分比(%)。<br>**計算**： `clicks`除以`impressions` | 高點進率表示內容與訊息和設計的對象高度相關且充滿動力，並有效鎖定對象的興趣。 |
| **[!UICONTROL CPM ]**<br>_每千成本_ | 具有此屬性的影像或視訊的每1,000次廣告印象成本。<br>**計算**：總金額`spent`除以範圍，然後乘以1000 | 低值可能表示具有成本效益的可見度，尤其是與高點進率配對時。 |
| **[!UICONTROL CPA ]**<br>_每個動作的成本_ | 完成特定客戶動作（例如購買或訂閱）所花費的平均成本。<br>**計算**：總金額`spent`除以已完成的客戶動作數目 | 協助識別可產生寶貴客戶動作的屬性。 |
| **[!UICONTROL CPC ]**<br>_每次點按成本_ | 具有此屬性的影像或影片每次點按的相關平均成本。<br>**計算**：總金額`spent`除以`clicks` | 平均成本降低可能表示廣告支出符合成本效益，尤其是與轉換率增加相比。 |
| **[!UICONTROL 支出]** | 與指定期間內的屬性相關的預算支出金額。 | 在短時間內發生高支出量可能表示快速使用，這可能導致資源提早耗盡。 根據關鍵績效指標追蹤支出金額，協助監控整體投資報酬率。 |
