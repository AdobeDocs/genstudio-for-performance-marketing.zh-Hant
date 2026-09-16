---
title: 啟動到交易台的廣告
description: 瞭解如何為交易台啟用靜態顯示廣告體驗。
feature: Ad Activation
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
subfeature_v2:
  - id: d87258a7-722c-4afd-b632-adddc447c7aa
    internal-label: Ad activation
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
    internal-label: Experiences
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%
---
# 啟動到交易台的廣告

Adobe GenStudio for Performance Marketing支援為Trade Desk啟用廣告體驗。

**支援的格式**：靜態顯示（僅限單一資產）。

啟用交易台的廣告遵循啟用其他付費廣告頻道所需的[相同的一般步驟](create-activation.md)，但有一個差異。 Trade Desk是受管理的企業服務，而非自助服務廣告平台，因此帳戶存取的運作方式與其他管道不同。 本頁涵蓋這些差異，以及Trade Desk的特定先決條件和設定欄位。

GenStudio的系統管理員和編輯人員可以啟用廣告體驗。

## 先決條件

* 現有的交易台即時帳戶。 在連線到GenStudio for Performance Marketing之前，請直接與交易台進行此設定。
* 交易台帳戶團隊已啟用的API存取。 對於交易台，您的帳戶團隊會使用API權杖代表您啟用此存取權，而不是使用其他付費廣告頻道使用的OAuth登入。
* 由The Trade Desk為GenStudio for Performance Marketing整合啟用的正確廣告商、座位和許可權。
* 來自您的交易台帳戶團隊的API權杖或認證，具有將創意發佈到目標廣告商帳戶的許可權。
* 已在交易台中的目的地行銷活動。 GenStudio for Performance Marketing會在該現有行銷活動中啟用廣告。

## 連線您的交易台帳戶

在貴組織啟用體驗之前，請與您的交易台帳戶團隊合作以啟用API存取，然後GenStudio系統管理員將帳戶連線到GenStudio for Performance Marketing：

1. 請聯絡您的交易台帳戶團隊，並請求存取許可權，以將創意內容從GenStudio for Performance Marketing發佈至您的交易台帳戶。 確認要用於啟用的廣告商ID、座位或合作夥伴詳細資訊。
1. 從交易台帳戶團隊取得API權杖或認證，並確認該權杖支援目標廣告商帳戶的創意發佈許可權。
1. 在GenStudio for Performance Marketing中，移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL 管道]**，然後按一下&#x200B;**[!UICONTROL 交易台]**&#x200B;圖磚上的&#x200B;**[!UICONTROL 連線]**。 輸入帳戶名稱、廣告商ID、API權杖或認證，然後儲存連線。

如果連線失敗，請與您的交易台帳戶團隊確認，已啟用API存取權，且代號具有正確的廣告商和座位許可權。

## 交易台設定欄位

核准的資產已鎖定，且無法在啟用期間進行編輯，因為它們已在[!DNL Content]中通過檢閱和核准。 您可以編輯：

* **文字欄位**：追蹤識別碼（用來作為平台創意名稱）
* **平台設定欄位**：帳戶、行銷活動

目前，啟用The Trade Desk僅支援單一資產靜態顯示廣告。
