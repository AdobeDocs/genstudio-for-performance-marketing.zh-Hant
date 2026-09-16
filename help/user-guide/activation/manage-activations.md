---
title: 管理啟用
description: 瞭解如何使用Adobe GenStudio for Performance Marketing管理啟用的體驗。
feature: Ad Activation
exl-id: 7cf340d4-37ab-4906-9aad-088a26db0818
TQID: https://experienceleague.adobe.com/ird0IiW8L5Axjj2FmEjlUcD1sPaNCNfxj9XNqGfQWiI
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 1%
---
# 管理啟用

您的啟用表格會顯示在[!DNL Activate]登陸頁面上。 每個表格都會列出其廣告及其狀態：

| 狀態 | 含義 |
|---|---|
| [!UICONTROL 需要注意] | 啟用表格中至少有一個廣告遺失或無效的欄位，例如不相容的call to action或重複的追蹤ID。 |
| [!UICONTROL 準備啟動] | 啟用表格中的所有廣告都會通過驗證，並準備發佈。 |
| [!UICONTROL 待處理] | 整個啟用表格已提交，且正在由目的地平台處理。 |
| [!UICONTROL 已發佈] | 已成功發佈整個啟用表格。 |
| [!UICONTROL 失敗] | 目的地平台已拒絕表格中至少一個廣告。 將滑鼠懸停在狀態工具提示上，可檢視平台的錯誤訊息。 |

您可以按一下右上角的&#x200B;**[!UICONTROL 再試一次]**，以自動重試失敗的啟用。

已發佈的列會因重新提交而遭到鎖定，且在目的地平台的原生廣告管理員中，包含該廣告的深層連結，因此您可以直接跳至目的地平台以進行檢閱或啟動。

## 詳細資料檢視

按一下廣告列，即可開啟其啟用詳細資訊的焦點檢視。 唯讀詳細資料檢視會擷取已啟用廣告的定義詳細資訊，包括失敗的啟用，以及衍生自GenStudio for Performance Marketing和目的地平台的資訊：

* **發佈時間和日期**：從目的地平台發佈的時間和日期
* **廣告ID**：由目的地平台指派並用於追蹤的ID，其包含平台原生廣告管理員中已發佈廣告的深層連結
* **廣告詳細資料**：用於廣告的已核准資產、復本和中繼資料
* **平台設定**：用來啟用廣告的帳戶、行銷活動和其他平台設定欄位

失敗的啟動詳細資料檢視包含失敗的原因。
