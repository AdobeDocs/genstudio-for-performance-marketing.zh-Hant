---
title: 資料管理
description: 瞭解GenStudio for Performance Marketing中用於深入分析的資料擷取和儲存。
feature: Insights
level: Experienced
role: Admin
last-substantial-update: 2025-1-7
source-git-commit: 5dbe645f2ccf033f515da22ffdcce86edcb9fb24
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---

# 資料管理

GenStudio for Performance Marketing使用Adobe Experience Platform (AEP)來擷取和儲存支援[!DNL Insights]的量度和中繼資料。 AEP使用&#x200B;_結構描述_&#x200B;來定義資料結構，並使用&#x200B;_資料集_&#x200B;來儲存和管理資料集合。

## 資料連線

GenStudio for Performance Marketing會使用Customer Journey Analytics (CJA)建立與一個或多個AEP資料集的連線，以彙總多個資料來源。 CJA使用這些資料連線來建立資料檢視，以便分析具有[!DNL Insights]的量度。

>[!BEGINSHADEBOX]

**資料連線的重要資訊**

如果您是[Adobe系統管理員](/help/user-guide/user-roles.md#adobe-system-administrator-vs-genstudio-system-manager)，則您可能擁有可存取支援GenStudio for Performance Marketing的AEP沙箱管理和資料湖元件的權益。

>[!WARNING]
>
>在AEP中重設生產沙箱會刪除所有資料連線，並導致[!DNL Insights]停止運作。

請謹慎操作，請勿刪除GenStudio for Performance Marketing以可靠操作所需的下列資料連線：

- 以`GS Insights`為前置詞的AEP資料集
- 以`GS Insights`為前置詞的AEP結構描述、類別和欄位群組
- 自訂欄位群組`timestamp for metadata`
- AEP連線：前置詞為`GS Insights`的資料流程
- AEP連線： GS Insights帳戶

在刪除AEP中的任何資料元件之前，請參閱&#x200B;_Customer Journey Analytics_&#x200B;指南中的[刪除關聯](https://experienceleague.adobe.com/en/docs/analytics-platform/using/technotes/deletion)。

>[!ENDSHADEBOX]

## 資料保留原則

GenStudio for Performance Marketing會保留13個月的管道資料。 此保留原則包含在初始連線期間擷取的6個月資料，以確保完整的歷史資料分析和報告。

請參閱[連線頻道廣告帳戶](/help/user-guide/insights/connect-channel.md)。
