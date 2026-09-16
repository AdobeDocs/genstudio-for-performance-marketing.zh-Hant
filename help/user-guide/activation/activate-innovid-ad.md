---
title: 啟用無罪廣告
description: 瞭解如何啟用無痕體驗。
feature: Ad Activation
exl-id: ebb2aa9e-8efb-45b0-9ba2-7b27b8888708
TQID: https://experienceleague.adobe.com/VTzk2CDlTqawM1ckdHPVzs2ES-y0Ui0mkOLnVD88bJk
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
    internal-label: Insights
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
    internal-label: Assets
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
    internal-label: Experiences
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%
---
# 啟動無訊息廣告

Adobe GenStudio for Performance Marketing支援將廣告體驗啟用為Innovid。

**支援的格式**：靜態顯示、HTML5壓縮顯示。

啟用無罪體驗會遵循啟用其他付費廣告頻道所需的[相同的一般步驟](create-activation.md)。 本頁涵蓋Innovid專屬的先決條件和設定欄位。 在GenStudio for Performance Marketing中啟用體驗後，使用Innovid檢閱體驗並啟動廣告。

GenStudio的系統管理員和編輯人員可以啟用廣告體驗。

## 先決條件

* 存取目標Innovid帳戶。
* 該帳戶的管理員存取權，可讀取和寫入Innovid。

Innovid會在不同的帳戶內組織行銷活動和廣告，每個帳戶都有一個創意資料庫。 Innovid中必須已存在目標創意程式庫；GenStudio for Performance Marketing會發佈廣告體驗至該創意程式庫，但不建立帳戶或創意程式庫。

## 連線您的Innovid帳戶

GenStudio系統管理員必須先將您的Innovid帳戶連線至GenStudio for Performance Marketing，您的組織才能在創意程式庫中發佈資產。 您必須擁有該帳戶的管理員存取權，才能在Innovid中讀取和寫入。 請參閱[連線付費媒體帳戶](/help/user-guide/connectors/connect-channel.md)。

同步完成後，您可以檢視新增的帳戶。

## 無效的設定欄位

核准的資產已鎖定，且無法在啟用期間進行編輯，因為它們已在[!DNL Content]中通過檢閱和核准。 您可以編輯：

* **文字欄位**：追蹤識別碼（用來作為平台創意名稱）
* **平台設定欄位**：帳戶、Creative資料庫、概念名稱

當啟用完成時，您的創意體驗會傳送至在Innovid中選取的創意程式庫。
