---
title: Adobe GenStudio for Performance Marketing審查與核准
description: 瞭解GenStudio for Performance Marketing檢閱和核准程式。
feature: Approval
exl-id: c83f47c0-e8ae-4c54-84b3-c50f67d6b3c2
source-git-commit: ce08231cb723bec3d80a732837b72a435d3b552d
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 0%

---

# Adobe GenStudio for Performance Marketing審查與核准

檢閱和核准工作流程可確保所有利害關係人（從創意團隊到法律專家）能夠有效地檢閱和核准行銷活動資產和體驗，包括創作AI生產的品牌資產。

## [!DNL Review and Approval]工作流程優點

* **支援健全的反複產生AI內容建立**。 在組織中建立與部署品牌一致的內容是一項反覆無常的工作。 GenStudio for Performance Marketing創作AI功能可支援快速建立數百種資產變體。 每個稽核者在核准資產草稿之前，可能會要求對該資產草稿進行多項變更。 稽核者越多，所有利害關係人在最終變體上達成共識前的潛在反複專案數量就越多。

* **支援創意完整性**。 核准可讓內容建立者參與核准程式，以保護品牌資產的創意完整性。 透過讓創意利害關係人（例如內容製作人和創意總監）參與稽核和核准程式，您可確保最終輸出符合您的願景和品牌識別。

* **遵守Campaign目標與法律規定**。 核准程式可協助確認內容是否支援行銷活動目標。 這可確保所有行銷資料符合法律和法規標準，將風險和潛在法律問題降至最低。

## 檢閱和核准生命週期

稽核與核准工作流程的主要階段包括：

* [要求您建立內容的檢閱與核准](./request-review.md)
* [檢閱和編輯內容](./review-and-edit.md)
* [核准內容](./approve-content.md)
* [發佈內容](./publish-content.md)

## 誰可以要求檢閱或核准內容？

如果您已建立資產或體驗，您可以要求組織核准鏈結中的其他人正式檢閱您的工作並加上註解。 雖然任何GenStudio for Performance Marketing組織成員都可以檢閱草稿，但只有指定的核准者才能對草稿加上註解或核准草稿。

## 關於[!DNL Content]個草稿

_草稿_&#x200B;是未經過檢閱和核准程式的資產或體驗的初步版本。 草稿狀態會識別草稿處於稽核與核准流程中的位置。 唯一的草稿識別碼可識別每個草稿。 此ID在草稿獲得核准並發佈到[!DNL Content]之前有效。 草稿的稽核評論和核准與此個別草稿ID相關聯。

當草稿完成檢閱和核准程式並發佈到[!DNL Content]時，草稿ID會過期，並且GenStudio for Performance Marketing不會儲存關聯的評論和核准狀態。 草稿URL已無效。

草稿狀態會擷取內容草稿在稽核及核准流程中的狀態。 建立檢閱中資產的GenStudio for Performance Marketing內容編輯人員會收到任何草稿或核准變更請求的通知。 核准者變更草稿狀態，以指出草稿是否需要進一步修訂或可以核准。 所有指定的核准者都必須先核准資產或體驗，才能發佈。

可用的草稿狀態：

**已通知**：內容編輯已透過通知核准者草稿已準備好檢閱來開始檢閱和核准程式。
**需要工作**：表示有一或多個核准者已要求變更內容草稿。 無法儲存此狀態的內容至[!DNL Content]。
**已核准**：所有指定的核准者皆已核准資產或體驗。 內容編輯器現在可以將中繼資料新增到資產或體驗中，並將其儲存到[!DNL Content]。

## 通知

GenStudio for Performance Marketing產品內通知會即時更新核准者和內容編輯器，以變更資產狀態和`@mention`個註解。 通知可支援在多個稽核、編輯和核准週期中快速反複執行。

內容編輯者和核准者可以註冊，在Slack中接收這些通知。 請參閱[在Experience Cloud](https://experienceleague.adobe.com/en/docs/core-services/interface/features/account-preferences#slack)中訂閱服務。

核准參與者採取的動作會觸發自動產品內通知和電子郵件通知。 當您開始核准流程時，指定的核准者會收到電子郵件和產品內通知。 每當核准者新增`@mention`個註解或做出決定時，您就會與產品內通知和電子郵件通知一起進入回圈。 通知包括內容草稿的連結。

如果您已啟動內容的稽核和核准流程，您將會收到所有核准和稽核註釋的通知。 但是，核准者只會收到包含他們與`@mention`的評論的通知。
