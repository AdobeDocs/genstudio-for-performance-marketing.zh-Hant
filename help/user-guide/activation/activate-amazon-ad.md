---
title: 啟用Amazon Ads
description: 瞭解如何啟用Amazon Ads體驗。
feature: Ad Activation
exl-id: 539cb43c-a9d8-4473-8a7d-e81967111741
TQID: https://experienceleague.adobe.com/4L4JHcYLSsoQ50QbCW7Mof52h5jpz3z8n0UL8CaqLA8
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
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%
---
# 啟用Amazon Ads

Adobe GenStudio for Performance Marketing支援為Amazon Ads啟用廣告體驗。

**支援的格式**：靜態顯示。

啟用Amazon廣告體驗會遵循啟用其他付費廣告頻道所需的[相同一般步驟](create-activation.md)。 本頁說明Amazon Ads的專屬先決條件和設定欄位。 在GenStudio for Performance Marketing中啟用體驗後，請使用Amazon Ads檢閱體驗並啟動廣告。

GenStudio的系統管理員和編輯人員可以啟用廣告體驗。

## 先決條件

* 存取目標Amazon Ads帳戶。
* 該帳戶的管理員存取權，可讀取和寫入Amazon Ads。

Amazon Ads會在不同的帳戶內組織行銷活動和廣告，每個帳戶都包含一個創意資料庫。 目標帳戶必須已存在於Amazon Ads中；GenStudio for Performance Marketing會發佈廣告體驗至該帳戶的創意程式庫，但不會建立帳戶。

## 連線您的Amazon Ads帳戶

GenStudio系統管理員必須先將您的Amazon Ads帳戶連線至GenStudio for Performance Marketing，您的組織才能在創意程式庫中發佈資產。 您必須擁有該帳戶的管理員存取權，才能讀取和寫入Amazon Ads。 請參閱[連線付費媒體帳戶](/help/user-guide/connectors/connect-channel.md)。

同步完成後，您可以檢視新增的帳戶。

## Amazon Ads設定欄位

核准的資產已鎖定，且無法在啟用期間進行編輯，因為它們已在[!DNL Content]中通過檢閱和核准。 您可以編輯：

* **文字欄位**：追蹤識別碼（用來作為平台創意名稱）
* **平台設定欄位**：帳戶

當啟用完成時，您的創意體驗會在Amazon Ads中傳送至所選帳戶的創意資料庫。
