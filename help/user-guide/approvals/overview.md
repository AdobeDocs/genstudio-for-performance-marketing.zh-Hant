---
title: Adobe GenStudio for Performance Marketing審查與核准
description: 瞭解GenStudio for Performance Marketing檢閱和核准程式。
level: Beginner
feature: Content Review, Content Management
exl-id: c83f47c0-e8ae-4c54-84b3-c50f67d6b3c2
source-git-commit: 7955796949c17f7cd877b115cba45c58cdd614a7
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 0%

---

# Adobe GenStudio for Performance Marketing審查與核准

檢閱和核准工作流程可確保所有利害關係人（從創意團隊到法律專家）能夠有效地檢閱和核准行銷活動資產和體驗，包括創作AI生產的品牌資產。

>[!NOTE]
>
> 此功能也可作為[與Adobe Workfront Proof](/help/user-guide/approvals/proof-integration.md)的整合提供。 此整合在GenStudio for Performance Marketing畫布中提供校訂功能。 透過Workfront Proof整合，GenStudio for Performance Marketing可獲得更結構化、透明和合作的稽核流程，協助團隊更自信、更明確地從草稿走向最終。

## 檢閱和核准工作流程優點

* **支援健全的反複產生AI內容建立**。 在組織中建立與部署品牌一致的內容是一項反覆無常的工作。 GenStudio for Performance Marketing創作AI功能可支援快速建立數百種資產變體。 每個稽核者在核准資產草稿之前，可能會要求對該資產草稿進行多項變更。 稽核者越多，所有利害關係人在最終變體上達成共識前的潛在反複專案數量就越多。

* **支援創意完整性**。 核准可讓內容建立者參與核准程式，以保護品牌資產的創意完整性。 透過讓創意利害關係人（例如內容製作人和創意總監）參與稽核和核准程式，您可確保最終輸出符合您的願景和品牌識別。

* **遵守行銷活動目標與法律規定**。 核准程式可協助確認內容是否支援行銷活動目標。 這可確保所有行銷資料符合法律和法規標準，將風險和潛在法律問題降至最低。

* **與Adobe Workfront校訂整合**。 使用者可以從GenStudio for Performance Marketing存取Workfront Proof強大的檢閱及核准功能。 在GenStudio for Performance Marketing中檢閱的內容會同步至Workfront Proof，且檢閱評論和狀態會保留。 [整合亮點](/help/user-guide/approvals/proof-integration.md)識別校訂如何延伸GenStudio for Performance Marketing的核准工作流程。

## 檢閱和核准生命週期

稽核與核准工作流程的主要階段包括：

* [要求您建立之內容的檢閱與核准](/help/user-guide/approvals/request-review.md)。 GenStudio for Performance Marketing簡化了請求核准和管理核准者的流程。 Workfront Proof核准範本可進一步簡化這項工作。

* [檢閱和編輯內容](/help/user-guide/approvals/review-and-edit.md)。 通知可讓內容建立者持續瞭解請求的變更和核准。 修訂內容會觸發新的自動核准週期。

* [核准內容](/help/user-guide/approvals/approve-content.md)。 指定的核准者將內容標示為已核准或準備好發佈。

* [發佈內容](/help/user-guide/approvals/publish-content.md)。 將核准的內容發佈至[!DNL Content]可讓貴組織中的其他人使用或參考。

## 關於內容草稿

_草稿_&#x200B;是尚未完成檢閱及核准程式的資產或體驗的初步版本。 草稿狀態會識別草稿處於稽核與核准流程中的位置。 唯一的草稿識別碼可識別每個草稿。 在草稿獲得核准並發佈到[!DNL Content]之前，此ID有效。 草稿的稽核評論和核准與此個別草稿ID相關聯。 GenStudio內容草稿沒有版本設定。

當草稿完成複查與核准程式，並發佈至[!DNL Content]時，草稿ID就會過期。 GenStudio for Performance Marketing不會儲存關聯的評論和核准狀態。 草稿URL已無效。

草稿狀態會擷取內容草稿在稽核與核准流程中的狀態。 建立檢閱中資產的GenStudio for Performance Marketing內容編輯人員會收到任何草稿或核准變更請求的通知。 核准者變更草稿狀態，以指出草稿是否需要進一步修訂或可以核准。 所有指定的核准者都必須先核准資產或體驗，才能發佈。

可用的草稿狀態：

**已通知**：內容編輯已透過通知核准者草稿已準備好進行稽核來啟動稽核與核准程式。
**需要工作**：表示有一或多個核准者已要求變更內容草稿。 無法儲存此狀態的內容至[!DNL Content]。
**已核准**：所有指定的核准者皆已核准資產或體驗。 內容編輯器現在可以將中繼資料新增到資產或體驗中，並將其儲存到[!DNL Content]。

>[!NOTE]
>
> 草稿對應至Workfront Proof整合之使用者的&#x200B;_校訂_。 [草稿和校樣](/help/user-guide/approvals/proof-integration.md#drafts-and-proofs)在持續性和版本設定方面有所不同。

## 核准角色

_檢閱者_&#x200B;可以新增註解，但無法核准內容。 檢閱者的參與有所幫助，但並非必要。 _核准者_&#x200B;必須先核准內容，才能進行核准程式。 Workfront Proof整合支援更多使用者角色。

## 通知

GenStudio for Performance Marketing產品內通知會即時更新核准者和內容編輯器，以變更資產狀態和`@mention`個註解。 通知可支援在多個稽核、編輯和核准週期中快速反複執行。

內容編輯者和核准者可以註冊，在Slack中接收這些通知。 請參閱[在Experience Cloud中訂閱服務](https://experienceleague.adobe.com/en/docs/core-services/interface/services/customer-attributes/subscription)。

核准參與者採取的動作會觸發自動產品內通知和電子郵件通知。 當您開始核准流程時，指定的核准者會收到電子郵件和產品內通知。 每當核准者新增`@mention`個註解或做出決定時，您就會與產品內通知和電子郵件通知一起進入回圈。 通知包括內容草稿的連結。

如果您已啟動內容的稽核與核准流程，您將會收到所有核准與稽核註解的通知。 但是，核准者只會收到包含他們與`@mention`的評論的通知。
