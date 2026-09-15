---
title: 建立Meta廣告體驗 — 輪播廣告
description: 瞭解如何在[!DNL GenStudio for Performance Marketing]中建立多卡片Meta輪播廣告體驗、管理卡片，以及產生品牌內概念。
role: User
source-git-commit: 1b407c1c66a2426b21cbbf423774ebdff16a7dec
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 1%
---

# 建立Meta輪播廣告體驗

Meta輪播廣告是一種付費廣告格式，可顯示2到10張可滑動卡片，每張卡片都有自己的影像或影片、標題和連結。

本頁涵蓋轉盤廣告專屬的步驟。 如需此頁面不重複的共用步驟，例如選擇範本、新增引數、修訂變體及發佈，請參閱[建立Meta廣告體驗](/help/user-guide/create/create-meta-ad.md)。

## 先決條件

在建立轉盤廣告之前，請確定您有一個範本，其所有頁面都共用一個外觀比例，即1:1或4:5。 每個範本頁面會變成一張卡片。 如需詳細資訊，請參閱[Meta廣告範本指導方針](/help/user-guide/templates/meta-template.md)。

## 選擇輪播格式

選取範本並開啟「畫布」後，在提示抽屜中選擇輪播格式。

1. 在&#x200B;_[!DNL Create your ads]_&#x200B;面板中，展開&#x200B;_[!UICONTROL &#x200B;引數&#x200B;]_。
1. 從&#x200B;**[!UICONTROL 格式]**&#x200B;下拉式功能表中，選取&#x200B;**[!UICONTROL 轉盤廣告]**。

   ![在「格式」下拉式清單設為「轉盤」廣告和卡片清單時，建立「廣告」面板](./carousel-format-cards.png){width="70%" zoomable="yes"}

如果您從單頁範本開始，[!DNL GenStudio for Performance Marketing]會複製頁面，以符合最少兩張卡片的要求。 如果範本頁面並非全部共用一個外觀比例，則格式切換器會遭到封鎖，直到您使用具有相同外觀比例的範本為止。

## 管理卡片

產生之前，請先在提示匣中建立卡片組。 若要新增更多卡片，請複製現有卡片。

* **若要複製卡片**，請從卡片選項中選取&#x200B;**[!UICONTROL 複製]**。
* **若要重新排序卡片**，請拖曳卡片控點到新位置。
* **若要刪除卡片**，請從卡片選項中選取&#x200B;**[!UICONTROL 刪除]**。 無法刪除最後兩張卡片，因為輪播需要至少兩張卡片。

針對每張卡片，選取一個影像，並視需要設定可覆寫上層產品的每一張卡片產品。 您可以個別選取每個卡片一個影像。 稍後會在[!DNL Activate]中設定每個卡片目的地URL。 如需詳細資訊，請參閱[啟動Meta廣告](/help/user-guide/activation/activate-meta-ad.md)。

## 撰寫傳送提示

您的提示會表示輪播的意圖，因此請說明卡片彼此之間的關係。 輪播複製可遵循下列兩種方式之一：

* **模組化：**&#x200B;每個卡片都是獨立廣告，沒有跨卡片的複製流程。 將此方法用於一組相關但獨立的訊息，例如數個產品。
* **循序：**&#x200B;復本會跨卡片連線以講述故事、逐步順序或操作說明。 當卡片彼此建置時，請使用此方法。

您也可以說明輪播是否提供單一產品或多項產品，以及任何卡片詳細資料。

例如，此提示會說明包含多個產品的模組化輪播：

```properties
Create a multi-product carousel for our end-of-summer skincare sale. For each card, lead with the product's core benefit and emphasize the sale value.
```

此提示說明循序輪播如何跨五張卡片講述故事：

```properties
Create a narrative carousel for our compliance alert-management platform. Start with shared intro text about the cost of alert fatigue. Across five cards, build the story: rising review costs, too many low-value alerts, false positives as the hidden cost driver, a solution that cuts false positives by more than 50%, and a closing learn-more call to action.
```

如需提示基本資訊，請參閱[撰寫有效的提示](/help/user-guide/effective-prompts.md)。

## 產生和檢閱概念

在您設定卡片和提示後，產生輪播並檢閱結果。

1. 選取&#x200B;**[!UICONTROL 產生]**。

   [!DNL GenStudio for Performance Marketing]會產生四個輪播概念。 每個概念都是完整的多卡片輪播，並有自己的品牌分數。

   ![四個產生的輪播概念，每個都有品牌分數和編輯按鈕](./carousel-concepts.png){width="80%" zoomable="yes"}

1. 選取概念，然後選取&#x200B;**[!UICONTROL 編輯]**&#x200B;以開啟以進行編輯。
1. 使用箭頭在卡片之間移動，然後編輯文字或選取&#x200B;**[!UICONTROL 交換]**&#x200B;以變更卡片的影像。 如需編輯的詳細資訊，請參閱[管理變體](/help/user-guide/create/manage-variants.md)。

如果您在產生卡片之前重新排序卡片，畫布會立即更新。 如果您在產生後重新排序提示抽屜中的卡片，則變更只會在您再次產生後套用，並且會出現再生警告。

## 瞭解每張卡片及共用欄位

有些轉盤欄位會個別套用至每個卡片，有些則會套用至整個廣告。 下表說明每個欄位在Meta輪播廣告中的行為。

| 欄位 | 範圍 |
|---|---|
| 標題 | 每張卡片 |
| 說明 | 每一張卡片，選擇性，設定於[!DNL Activate] |
| call to action | 在廣告間共用 |
| 主要文字 | 在廣告間共用 |
| 媒體 | 每一張卡片（影像、視訊或混合） |
| 影像上文字 | 每張卡片 |
| 目的地URL | 每一張卡片，設定在[!DNL Activate] |

## 發佈、匯出和啟動

當輪播準備就緒時，請以與其他Meta廣告相同的方式發佈和匯出。 輪播會儲存為符合一個概念的單一體驗。 「匯出」會傳送CSV檔案以及卡片媒體。 請參閱[[!DNL Content]](/help/user-guide/content/overview.md)以瞭解如何儲存已發佈的體驗。 若要在Meta啟用輪播，請參閱[啟用Meta廣告](/help/user-guide/activation/activate-meta-ad.md)。
