---
title: 啟動Meta廣告
description: 瞭解如何啟用Meta廣告體驗。
feature: Ad Activation
exl-id: 157df612-a774-422c-bca3-2fde9e9d1c88
TQID: https://experienceleague.adobe.com/hDR0ngNiGnCXCCOgNhVG8gX4kHGrNvfybPbuMLwYk7U
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
    internal-label: Guidelines
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
source-wordcount: '382'
ht-degree: 0%
---
# 啟動Meta廣告

Adobe GenStudio for Performance Marketing支援將Meta廣告體驗啟動至Instagram和Facebook。

**支援的格式**：影像、視訊、輪播。

[在GenStudio for Performance Marketing中建立Meta體驗](/help/user-guide/create/create-meta-ad.md)，然後選取它以進行啟用。

啟用Meta廣告會遵循啟用其他付費廣告頻道所需的[相同一般步驟](create-activation.md)。 本頁說明Meta專屬的先決條件和設定欄位。 在GenStudio for Performance Marketing中啟用Meta體驗後，請使用[Meta Ads Manager](https://adsmanager.facebook.com/)檢閱體驗並啟動廣告。

與其他管道不同，Meta廣告可以在單一廣告中包含多個外觀比例。 如果您的體驗有多個外觀比例，[!DNL Activate]仍只會為其產生一列，而不是每個外觀比例產生一列。

GenStudio的系統管理員和編輯人員可以啟用廣告體驗。

## 先決條件

確認您連線的Meta廣告帳戶擁有在Meta廣告平台的這些元件中管理廣告的完整許可權：

* Meta廣告帳戶
* Facebook頁面
* Meta行銷活動
* Meta廣告集
* Instagram設定檔（選填）

目標Meta行銷活動和廣告集必須已存在於Meta廣告管理員中。 GenStudio for Performance Marketing目前不會建立行銷活動或廣告集。

## 連線您的Meta帳戶

在貴組織啟用體驗之前，GenStudio系統管理員必須將您的Meta帳戶連結至GenStudio for Performance Marketing。 此連線可讓資料在GenStudio for Performance Marketing和Meta之間流動，以啟用啟用啟用程式。 請參閱[連線至Meta Ads](/help/user-guide/connectors/meta-ads.md)。

若要選取Instagram帳戶，請在Meta Business Manager中確認您要使用的[Instagram帳戶已連線至上線期間選取的相同廣告帳戶](/help/user-guide/connectors/meta-ads.md#connect-an-instagram-account)。 如果缺少此連線，Instagram帳戶在啟用期間可能不會顯示在&#x200B;**[!UICONTROL Instagram設定檔]**&#x200B;下拉式功能表中。

同步完成後，您可以檢視新增的帳戶。 大量資料需要更長的時間才能同步。

## Meta設定欄位

核准的資產、標題和正文已鎖定，且無法在啟用期間進行編輯，因為它們已在[!DNL Content]中通過稽核和核准。 您可以編輯：

* **文字欄位**：說明、Call-to-action、目的地URL、URL引數、追蹤ID （用作Meta廣告名稱）
* **平台設定欄位**：廣告帳戶、Facebook頁面、Instagram設定檔、Meta行銷活動、Meta廣告集
