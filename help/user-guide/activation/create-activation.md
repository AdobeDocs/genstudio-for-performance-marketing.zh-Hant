---
title: 啟用工作流程
description: 瞭解廣告體驗的啟用工作流程。
feature: Ad Activation
exl-id: 17e1bade-d52a-4953-a85c-c10d093e73d6
source-git-commit: 6ee58b22761be357bb9ff753cf9e5bd5b431c513
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 0%

---

# 啟用工作流程

_[!DNL Activate]_支援頻道特定格式的廣告體驗啟用，例如中繼廣告體驗。

GenStudio for Performance Marketing體驗是行銷活動元件（例如廣告），針對付費廣告頻道或電子郵件上的特定對象量身打造。 廣告體驗包含三個主要元件：

* **媒體資產**：媒體資產是廣告體驗中包含的影像(GIF、PNG、JPEG)。 啟用目前支援靜態影像。
為您的廣告體驗選取影像資產需要選擇適當的外觀比例。 外觀比例定義影像寬度和高度之間的比例關係，對於廣告投放的有效性至關重要。 付費媒體管道對其平台上的每個廣告投放仔細指定有效的外觀比例。 將影像資產新增至您的啟用時，您必須根據體驗的最終廣告投放位置選取外觀比例。 檔案型別僅限於JPEG、PNG和GIF。

* **文字**：文字包含廣告中包含的所有形式副本，包括標題、內文和行動號召元素。

* **中繼資料**：您可以指派給內容的使用者定義屬性。 中繼資料可強化效能分析、篩選和追蹤。 使用者通常看不到。

建立啟動涉及針對指定的頻道位置和行銷活動調整這些廣告元件的每個元件。 GenStudio for Performance Marketing支援將單一體驗啟用至一個付費頻道。

## 工作流程階段

雖然不重複的位置要求定義了每個付費頻道，但所有廣告啟用都共用相同的高層級步驟。 為任何付費管道啟用體驗有三個核心階段：

* **將GenStudio for Performance Marketing連線至您的目標頻道**。 GenStudio系統管理員必須連線您的管道帳戶，您才能啟用體驗。

* **準備您的使用體驗**。 準備工作包括以適當的外觀比例為您的特定廣告投放選擇媒體資產，並為行動號召元素和正文指派文字。 您也可以新增資訊性中繼資料，協助使用者在啟用後搜尋體驗。 每個廣告頻道位置都會針對位置中包含的視覺資產指定有效的外觀比例。

* **檢閱您的體驗並發佈至目標頻道**。  使用建立啟用工作流程中的&#x200B;_預覽_&#x200B;面板，在最終完成啟用之前，評估您選擇的廣告版位和文字元素。 您的最終發佈前稽核會在目的地頻道的廣告管理應用程式中進行。 例如，在GenStudio for Performance Marketing中啟動中繼廣告體驗後，您必須登入Meta Ads Manager、檢閱您的廣告體驗，然後選取其特定屬性，才能發佈。

一旦體驗在其目標廣告頻道上線，_[!DNL Insights]_就可以追蹤和分析其效能資料。

## 支援的管道

每個付費媒體頻道都有獨特的啟用工作流程。 選取付費管道以取得啟用准則：

* [Meta](activate-meta-ad.md)
