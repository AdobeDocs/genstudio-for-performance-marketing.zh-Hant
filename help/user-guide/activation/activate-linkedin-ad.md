---
title: 啟動LinkedIn廣告
description: 瞭解如何啟用LinkedIn廣告體驗。
feature: Ad Activation
exl-id: edc95319-36c3-4cbf-a5c0-865b49482b50
TQID: https://experienceleague.adobe.com/1mcxWePqYd8tYp3e1D2UTSeBHSvPj4WrqeSyiUCxD8c
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
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%
---
# 啟動LinkedIn廣告

Adobe GenStudio for Performance Marketing支援將LinkedIn廣告體驗啟用至[LinkedIn行銷活動管理員](https://business.linkedin.com/marketing-solutions)。

**支援的格式**：單一影像、單一視訊。

您可以在GenStudio for Performance Marketing中[建立LinkedIn體驗](/help/user-guide/create/create-linkedin.md)，然後選取它以啟動。

啟用LinkedIn廣告會遵循啟用其他付費廣告頻道所需的[相同的一般步驟](create-activation.md)。 本頁說明LinkedIn專屬的先決條件和設定欄位。 在GenStudio for Performance Marketing中啟用LinkedIn體驗後，請使用LinkedIn行銷活動管理員來檢閱體驗並啟動廣告。

GenStudio的系統管理員和編輯人員可以啟用廣告體驗。

## 先決條件

* 具有管理行銷活動和廣告之完整許可權的LinkedIn行銷活動管理員帳戶。 此帳戶必須包含現有的行銷活動。
* LinkedIn廣告帳戶擁有在LinkedIn頁面上建立廣告和發佈內容的完整許可權。

目標LinkedIn行銷活動和廣告集必須已存在於LinkedIn行銷活動管理員中。 GenStudio for Performance Marketing不會建立行銷活動或廣告集。

>[!NOTE]
>
>LinkedIn已重新命名其行銷活動階層：LinkedIn行銷活動管理員先前稱為&#x200B;**行銷活動群組**&#x200B;的專案現在稱為&#x200B;**行銷活動**，而先前稱為&#x200B;**行銷活動**&#x200B;的專案現在稱為&#x200B;**廣告集**。 [!DNL Activate]中的&#x200B;**[!UICONTROL LinkedIn行銷活動]**&#x200B;和&#x200B;**[!UICONTROL LinkedIn廣告集]**&#x200B;設定欄位使用目前的術語。

GenStudio for Performance Marketing目前支援「單一影像」和「單一視訊」LinkedIn廣告，兩者每個貼文都只會包含一個影像或視訊。 如果您的體驗包含多個外觀比例，[!DNL Activate]會在啟用表格中為每個比例產生個別的列，以便每個列都可以作為自己的廣告執行；刪除您不需要的任何列。

## 連線您的LinkedIn帳戶

GenStudio系統管理員或編輯器必須先將LinkedIn廣告帳戶連線至GenStudio for Performance Marketing，您的組織才能啟用體驗。 您必須擁有廣告帳戶和LinkedIn設定檔頁面的完整管理員存取權，才能成功連線。 您只需在&#x200B;**[!UICONTROL 設定]**&#x200B;中連線廣告帳戶一次。 之後，任何可以存取該執行個體的人都可以使用此功能。

此連線可讓資料在GenStudio for Performance Marketing和LinkedIn之間流動，以啟用啟用啟用程式。

同步完成後，您可以檢視新增的帳戶。 大量資料需要更長的時間才能同步。

## LinkedIn設定欄位

核准的資產、標題和簡介文字已鎖定，且無法在啟用期間進行編輯，因為它們已在[!DNL Content]中通過稽核和核准。 您可以編輯：

* **文字欄位**：說明、Call-to-action、目的地URL、URL引數、追蹤ID （用作平台廣告名稱）
* **平台設定欄位**： LinkedIn廣告帳戶、LinkedIn行銷活動、LinkedIn廣告集
