---
title: 啟用ChatGPT廣告
description: 瞭解如何啟用ChatGPT廣告體驗。
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
source-wordcount: '272'
ht-degree: 0%
---
# 啟用ChatGPT廣告

Adobe GenStudio for Performance Marketing支援啟用ChatGPT廣告體驗。

**支援的格式**：聊天卡。

您可以在GenStudio for Performance Marketing中[建立ChatGPT體驗](/help/user-guide/create/create-chatgpt-ad.md)，然後選取它以啟動。

啟用ChatGPT廣告會遵循啟用其他付費廣告頻道所需的[相同的一般步驟](create-activation.md)。 本頁涵蓋ChatGPT的特定先決條件和設定欄位。 在GenStudio for Performance Marketing中啟用ChatGPT體驗後，請使用OpenAI廣告管理員來執行最終檢查並啟動廣告。

GenStudio的系統管理員和編輯人員可以啟用廣告體驗。

## 先決條件

* OpenAI Ads帳戶和該帳戶的API金鑰。
* 目標ChatGPT行銷活動和廣告群組必須已存在於OpenAI廣告管理員中。 GenStudio for Performance Marketing不會建立新的行銷活動或廣告群組。

## 連線您的ChatGPT帳戶

在貴組織啟用體驗之前，GenStudio系統管理員必須先將您的OpenAI Ads帳戶連結至GenStudio for Performance Marketing：

1. 在OpenAI廣告管理員中，移至&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL API金鑰]** > **[!UICONTROL 建立新金鑰]**。
1. 在GenStudio for Performance Marketing中，移至&#x200B;**[!UICONTROL 更多]** > **[!UICONTROL 設定]** > **[!UICONTROL ChatGPT]** > **[!UICONTROL 連線]** > **[!UICONTROL 新增帳戶]**。
1. 輸入您的OpenAI Ads帳戶名稱，貼上您的API金鑰，然後按一下&#x200B;**[!UICONTROL [新增帳戶]]**。

## ChatGPT設定欄位

核准的資產、標題（標題）和正文已鎖定，且無法在啟用期間進行編輯，因為它們已在[!DNL Content]中通過稽核和核准。 您可以編輯：

* **文字欄位**：目標URL、追蹤ID （用作平台廣告名稱）
* **平台設定欄位**： OpenAI Ads帳戶、OpenAI行銷活動、OpenAI廣告群組

目標URL必須使用有效的`https://`格式，例如`https://www.example.com`。
