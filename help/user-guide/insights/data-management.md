---
title: 數據管理
description: 瞭解 GenStudio 中用於 [!DNL Insights] 績效營銷的數據攝取和儲存。
feature: Reporting and Insights
level: Experienced
role: Admin, Data Architect
last-substantial-update: 2025-1-7
exl-id: a5ab44d6-75c0-405b-82ad-9c65f6094bd6
source-git-commit: 8e61fa5c08102c5dd9905e693d7f129105d9f633
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---

# 數據管理

GenStudio for Performance Marketing 使用 Adobe Experience Platform （AEP） 進行數據攝取和儲存指標，並中繼資料此功能 [!DNL Insights]。 AEP 使用架構&#x200B;_來_&#x200B;定義用於存儲和管理數據集合的數據結構和&#x200B;_數據集_。

## 數據連線

GenStudio for Performance Marketing 使用 Customer Journey Analytics （CJA） 通過創建與一個或多個 AEP 數據集的連接來彙總多個數據源。 CJA 使用這些資料連接建立資料檢視，以便使用 [!DNL Insights].

>[!BEGINSHADEBOX]

**有關數據連接的重要資訊**

如果您是 [Adobe Systems 系統管理員](/help/user-guide/user-roles.md#adobe-system-administrator-vs-genstudio-system-manager)，您可能擁有允許訪問支援 GenStudio for Performance Marketing 的 AEP 沙箱管理和數據湖元件的權利。

>[!WARNING]
>
>在 AEP 中重置生產沙箱會刪除所有數據連接並導致 [!DNL Insights] 停止工作。

請謹慎使用，不要刪除 GenStudio for Performance Marketing 可靠運行所需的以下數據連接：

- 前置詞為 AEP 數據集 `GS Insights`
- AEP 架構、類別和欄位群組，前綴為 `GS Insights`
- 自訂欄位群組 `timestamp for metadata`
- AEP 連接：前置綴為 `GS Insights`
- AEP 連接：GS Insights 帳戶

在 AEP 中刪除任何數據元件之前，請參閱[刪除](https://experienceleague.adobe.com/en/docs/analytics-platform/using/technotes/deletion)_Customer Journey Analytics_&#x200B;指南中的含義。

>[!ENDSHADEBOX]

## 數據保留原則

GenStudio for Performance Marketing 會將通道數據保留 13 個月。 此保留原則包括在初始連接期間引入的 6 個月数据，確保全面的歷史資料分析和報告。

請参閱 [連接通道廣告帳戶](/help/user-guide/connectors/connect-channel.md)。
