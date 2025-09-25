---
title: 資料管理
description: 瞭解GenStudio for Performance Marketing中 [!DNL Insights] 的資料擷取和儲存。
feature: Reporting and Insights
level: Experienced
role: Admin, Data Architect
last-substantial-update: 2025-1-7
exl-id: a5ab44d6-75c0-405b-82ad-9c65f6094bd6
source-git-commit: 44fedfdc3902b4f993d656ae6360a32e27a62520
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---

# 資料管理

GenStudio for Performance Marketing使用Adobe Experience Platform (AEP)來擷取及儲存支援[!DNL Insights]的量度和中繼資料。 AEP使用&#x200B;_結構描述_&#x200B;來定義資料結構，並使用&#x200B;_資料集_&#x200B;來儲存和管理資料集合。

## 資料連線

GenStudio for Performance Marketing使用Customer Journey Analytics (CJA)，透過建立與一個或多個AEP資料集的連線來彙總多個資料來源。 CJA使用這些資料連線來建立資料檢視，以分析具有[!DNL Insights]的量度。

>[!BEGINSHADEBOX]

**資料連線的重要資訊**

如果您是[Adobe系統管理員](/help/user-guide/user-roles.md#adobe-system-administrator-vs-genstudio-system-manager)，則可能會擁有可存取支援GenStudio for Performance Marketing的AEP沙箱管理和Data Lake元件的權益。

>[!WARNING]
>
>在AEP中重設生產沙箱會刪除所有資料連線，並導致[!DNL Insights]停止運作。

請謹慎操作，請勿刪除GenStudio for Performance Marketing以可靠操作所需的下列資料連線：

- 前置詞為`GS Insights`的AEP資料集
- 以`GS Insights`為首碼的AEP結構描述、類別和欄位群組
- 自訂欄位群組`timestamp for metadata`
- AEP連線：前置詞為`GS Insights`的資料流程
- AEP連線： GS Insights帳戶

在刪除AEP中的任何資料元件之前，請參閱[Customer Journey Analytics](https://experienceleague.adobe.com/zh-hant/docs/analytics-platform/using/technotes/deletion)指南中的&#x200B;_刪除關聯_。

>[!ENDSHADEBOX]

## 資料保留原則

GenStudio for Performance Marketing會保留13個月的管道資料。 此保留原則包含在初始連線期間擷取的6個月資料，以確保完整的歷史資料分析和報告。

請參閱[連線付費媒體帳戶](/help/user-guide/connectors/connect-channel.md)。
