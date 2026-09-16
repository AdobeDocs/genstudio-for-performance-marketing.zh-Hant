---
title: 啟動Google Campaign Manager 360廣告
description: 瞭解如何啟用Google Campaign Manager 360體驗。
feature: Ad Activation
exl-id: e4ee4e04-8dd0-4e05-a0f7-0ddca2fbb6be
TQID: https://experienceleague.adobe.com/pQbT2OC7-jK33HhJWgTBBtJrmEvr48mGkl8v-fTkOLQ
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
subfeature_v2:
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
    internal-label: Experiences
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%
---
# 啟動Google Campaign Manager 360廣告

Adobe GenStudio for Performance Marketing支援在Google Campaign Manager 360上啟用廣告體驗。

**支援的格式**：靜態顯示、視訊顯示、HTML5 Zip顯示。

啟用Google Campaign Manager 360廣告時，會依循啟用其他付費廣告頻道所需的[相同的一般步驟](create-activation.md)。 本頁說明Google Campaign Manager 360的先決條件和設定欄位。 在GenStudio for Performance Marketing中啟用體驗後，請使用Google Campaign Manager 360檢閱體驗並啟動廣告。

GenStudio的系統管理員和編輯人員可以啟用廣告體驗。

## 先決條件

* 可存取目標廣告商的Google Campaign Manager 360帳戶。
* 廣告商的管理員存取權，可讀取和寫入Campaign Manager 360。

Campaign Manager 360可在不同的廣告商內組織行銷活動和廣告，每個廣告商都包含創意資料庫。 目標廣告商必須已存在於Campaign Manager 360中；GenStudio for Performance Marketing會發佈廣告體驗至該廣告商的創意資料庫，但不建立廣告。

## 連線您的Google Campaign Manager 360帳戶

GenStudio系統管理員或編輯器必須先將您的Google Campaign Manager 360帳戶連線至GenStudio for Performance Marketing，您的組織才能在創意程式庫中發佈資產。 您必須擁有廣告商的管理員存取權，才能讀取和寫入Campaign Manager 360。 請參閱[連線付費媒體帳戶](/help/user-guide/connectors/connect-channel.md)。

同步完成後，您可以檢視新增的帳戶。

## Google Campaign Manager 360設定欄位

核准的資產已鎖定，且無法在啟用期間進行編輯，因為它們已在[!DNL Content]中通過檢閱和核准。 您可以編輯：

* **文字欄位**：追蹤識別碼（用來作為平台創意名稱）
* **平台設定欄位**：廣告商

啟用完成時，您的創意體驗會傳遞至Google Campaign Manager 360中選取的廣告商創意資料庫。
