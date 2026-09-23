---
title: 最佳化您的啟用
description: 瞭解如何最佳化協力廠商付費廣告頻道的啟用。
level: Intermediate
feature: Ad Activation
exl-id: 5bc624c2-d064-4190-8761-ed05d0629d1f
TQID: https://experienceleague.adobe.com/-D3DGxTpZ-0J-grE5-jKPrptf4C1Z-OE1t0DCoqhRLQ
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
source-git-commit: db0cebfe795569d9913757d190db853097a00405
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 1%
---
# 最佳化啟用

啟用付費廣告頻道的廣告體驗涉及兩個主要階段：

* 針對啟用表格中的每一列設定廣告和平台設定詳細資訊

* 將您的啟用發佈至其指定的付費廣告管道的廣告管理員

設定和啟用您的廣告體驗時遵循最佳實務，有助於將傳送至目標頻道期間的潛在複雜度或錯誤降至最低。

## 最佳做法

以下是一些常見的最佳實務及其可避免的錯誤。

* **對每一列使用唯一的追蹤識別碼**

  [!DNL Activate]會將重複的追蹤ID標示為[!UICONTROL 需要注意]，而且除非受影響格式和Platform資料表中的每一列都有唯一的追蹤ID，否則不會允許您發佈。 每個&#x200B;**[!UICONTROL 追蹤ID]**&#x200B;欄位都會預先填入體驗名稱，因此跨廣告格式或平台共用體驗的列都會以相同的值開始。 檢查並解決這些重複專案，而不僅僅是大量編輯所引入的專案。 如果您大量編輯多個列的追蹤ID，請確認您想要將相同的值套用至每個選取的列。

* **使用有效、完整的目的地URL**

  無效的URL可能會觸發錯誤。 範例錯誤： _您輸入的URL不指向網站。 請輸入有效的URL，然後再試一次。 (100)_

* **請確定您的應用程式正確處理權杖過期時間**

  應用程式必須視需要請求新權杖。 再次登入或重新整理工作階段，以重新驗證並取得新的存取Token。 範例錯誤： _驗證存取Token時發生錯誤：工作階段已失效，因為使用者已變更其密碼，或Facebook已基於安全性原因變更工作階段。 (190)_

* **檢閱您的廣告集，並確定在任何時候只有一個廣告在作用中**

  如果您需要啟用多個Meta廣告，請為每個廣告建立個別的動態Creative廣告集。 範例錯誤： _動態Creative廣告集最多允許一個使用中的廣告。 不允許使用者在同一個動態Creative廣告集下建立多個廣告。 (100)_

* **將套用的規則數目與平台**&#x200B;所指定的數目相符

  付費管道希望套用的規則數目符合其指定格式。  如有必要，請調整規則數量，以符合平台所指定的值。 範例錯誤： _廣告AssetFeed的format有X目標規則：格式名稱，但此格式應為X目標規則。 (100)_

* **選擇與您的廣告集目標相容的call-to-action (CTA)**

  與Dynamic Creative廣告集中的目標不相容的呼叫動作會觸發錯誤。 範例錯誤： _動態call to action廣告集中的目標Y不支援Creative型別X。 (100)_

* **請確定目標廣告集的上限支援廣告體驗的數量**

  確認目標廣告集的廣告限制可容納您啟用的廣告體驗。 如有必要，請從廣告集中移除任何不必要或非作用中的廣告，以維持在此限制內。 或者，建立新的廣告集以啟動其他廣告。 範例錯誤： _您已達到行銷活動、廣告集或每個廣告帳戶的廣告限制。 每個廣告集最多可包含50個廣告。 這包括暫停/非作用中/關閉的廣告。 (100)_

* **請確定平台支援您選取的CTA型別**

  確認您的體驗包含支援的CTA型別。 範例錯誤： _(#100)無效的call to action型別(100)_
