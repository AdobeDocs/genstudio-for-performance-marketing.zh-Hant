---
title: Activate概述
description: 瞭解如何使用Adobe CX Enterprise和協力廠商應用程式啟用內容。
level: Beginner
feature: Ad Activation
exl-id: 365fe253-d189-467e-a723-f54cd74ff60b
TQID: https://experienceleague.adobe.com/-Nal0YqjTzKw4g2SM3IuMf0a13e87CWdTqBZPd0dBkU
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
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%
---
# Adobe GenStudio for Performance Marketing啟用

GenStudio for Performance Marketing [!DNL Activate]是您準備並傳送廣告體驗至付費廣告頻道（例如Meta或LinkedIn）的地方。 _啟用_&#x200B;會採用已核准的廣告體驗及其資產、套用特定管道所需的設定，然後以非使用中狀態、關閉狀態直接傳送給該管道。 從那裡，您可以在廣告上線之前，在管道自己的廣告管理員中進行最終審查。

[!DNL Activate]會將您的體驗直接提供給頻道，因此您不需要匯出檔案或手動將其上傳到頻道自己的廣告管理員。

GenStudio系統管理員或編輯器必須連線每個付費廣告頻道的廣告帳戶，您才能為該頻道啟用廣告體驗。

## 啟用功能

使用[!DNL Activate]為其目標付費廣告頻道準備廣告體驗。 在單一啟用表格中，針對多個付費廣告頻道大量啟動[體驗](create-activation.md)。 然後，[管理您的啟用](manage-activations.md)以檢視每個啟用體驗的狀態和詳細資訊。

>[!VIDEO](https://video.tv.adobe.com/v/3503538?learn=on)

### 從內容啟用核准的體驗

從[!DNL Content]選取一或多個已核准、已發佈的體驗，或從[!DNL Activate]登陸頁面開始。 與舊版[!DNL Activate]不同，單一啟用表格可同時包含多個付費廣告管道的體驗，依廣告格式和管道進行整理。

>[!NOTE]
>
>[!DNL Content]會呼叫&#x200B;**頻道**&#x200B;中的目的地，例如Meta或LinkedIn。 [!DNL Activate]會呼叫相同目的地的&#x200B;**平台** （例如，在&#x200B;**[!UICONTROL 平台設定]**&#x200B;中）。 這兩個詞指的是一樣的。

### 設定廣告和平台設定詳細資料

啟用表格中的每一列代表一個廣告。 核准的創意資產、標題和正文會被鎖定，因為它們已通過稽核和核准。 您可以編輯其餘欄位，例如call-to-action文字、目的地URL以及平台設定詳細資訊，例如廣告帳戶、行銷活動和廣告集。 一次編輯一列的欄位，或選取多個列以大量編輯共用欄位。

### 檢閱您的體驗並發佈至其廣告頻道

確認每一列顯示[!UICONTROL 準備啟動]。 [!DNL Activate]將遺漏或無效的欄位標示為旗標、不相容的動作呼叫，以及重複的追蹤ID標示為[!UICONTROL 需要注意]。 當每一列準備就緒時，按一下&#x200B;**[!UICONTROL 傳送至Platform]**&#x200B;以發佈表格中的所有廣告。 [!DNL Activate]會近乎即時報告每個廣告的狀態，而成功發佈的廣告會包含目的地平台原生廣告管理員中該廣告的深層連結。 失敗的廣告會傳回錯誤訊息，並可重試。
