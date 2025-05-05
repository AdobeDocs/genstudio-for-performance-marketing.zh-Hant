---
title: 連線付費媒體
description: 連線管道帳戶，以使用Adobe GenStudio for Performance Marketing啟用和監控您的廣告和媒體。
level: Intermediate
role: Admin, Data Engineer
feature: Reporting and Insights
exl-id: e699041e-b462-45b3-8c4c-4de0d52cf0e6
source-git-commit: cf4be61925761c9630cb8ea5c995d017b3938a31
workflow-type: tm+mt
source-wordcount: '689'
ht-degree: 0%

---

# 連線付費媒體帳戶

_[!DNL Data connectors]_&#x200B;可讓GenStudio for Performance Marketing與您的付費媒體網路帳戶緊密整合。 透過連線到協力廠商管道帳戶，您可以交換關鍵資料，例如[[!DNL Insights]](/help/user-guide/insights/overview.md)中的行銷活動績效量度，並且可以透過[[!DNL Activate]](/help/user-guide/activation/overview.md)傳遞新的廣告位置。 此整合可讓GenStudio for Performance Marketing管理您的媒體和廣告，同時從您的作用中行銷活動接收有價值的深入分析，包括曝光數、點按數和轉換。

**若要連線到付費媒體帳戶**：

1. 按一下省略符號&#x200B;**[!UICONTROL ...左下方導覽區顯示更多]**。

1. 選取&#x200B;**[!UICONTROL 設定]**，並附上cog圖示。

1. 在&#x200B;_[!UICONTROL 設定]_&#x200B;中，從&#x200B;_[!UICONTROL 資料聯結器]_&#x200B;區段選擇聯結器型別，然後按一下&#x200B;**[!UICONTROL 連線]**。

   如果有已連線的帳戶，您可以按一下&#x200B;_已連線的帳戶_，檢視帳戶名稱、詳細資料和狀態的清單。

1. 檢視您選取的[聯結器型別](#connector-types)、檢閱先決條件，然後繼續連線步驟。

## 付費媒體連線

GenStudio for Performance Marketing支援各種聯結器型別，以便與您偏好的行銷平台整合。 每種聯結器型別都有特定的先決條件和設定步驟，才能完成成功的連線。

### Google Campaign Manager 360連線

>[!BEGINSHADEBOX]

**必要條件**：

- Google Campaign Manager 360帳戶
- 移除瀏覽器中的任何快顯封鎖程式

>[!ENDSHADEBOX]

**若要連線Google Campaign Manager 360帳戶**：

1. 在&#x200B;_Data Connectors_&#x200B;區段中，按一下&#x200B;_Google Campaign Manager 360_&#x200B;卡片上的&#x200B;**[!UICONTROL 連線]**。

1. 登入您的Google Campaign Manager 360帳戶。

   您可能必須移除快顯視窗封鎖程式，然後使用&#x200B;**[!UICONTROL 重新整理]**&#x200B;再試一次。

1. 閱讀條款與條件，然後按一下&#x200B;**[!UICONTROL 允許]**&#x200B;以授與存取權。

1. 在&#x200B;_[!UICONTROL Google行銷活動管理員360]_&#x200B;檢視中，選取一或多個廣告商並按一下&#x200B;**[!UICONTROL 選取]**。

_[!UICONTROL Google行銷活動管理員360帳戶]_&#x200B;檢視會列出`Account name`、`Added by`、`Date added`和`Status`。 使用&#x200B;**[!UICONTROL 新增帳戶]**&#x200B;將更多帳戶新增至清單。

### 中繼廣告連線

當您將&#x200B;_Meta Business_&#x200B;設定檔連線至GenStudio for Performance Marketing時，可確保順暢存取您企業頁面、Meta Ads帳戶和其他中繼資產的廣告資料。

>[!BEGINSHADEBOX]

**必要條件**：

- 可存取所有中繼服務（例如中繼廣告帳戶和Facebook商業設定檔）的Facebook/中繼登入
- 存取具有`View performance`許可權層級的中繼廣告帳戶，以存取報表和檢視廣告，包括下列專案
   - 與[!DNL Insights]一起使用所需的許可權：

      - `pages_show_list`
      - `ads_read`
      - `ads_management`
      - `pages_read_engagement`

   - 與[!DNL Activate]一起使用所需的許可權：

      - `ads_management`
      - `ads_read`
      - `business_management`
      - `instagram_basic`
      - `instagram_content_publish`
      - `pages_manage_ads`
      - `pages_manage_posts`
      - `pages_show_list`

- 移除瀏覽器中的任何快顯封鎖程式

>[!ENDSHADEBOX]

**若要連線中繼廣告帳戶**：

1. 在&#x200B;_Data Connectors_&#x200B;區段中，按一下&#x200B;_中繼廣告_&#x200B;卡片上的&#x200B;**[!UICONTROL 連線]**。

1. 登入您的Facebook帳戶。

   您可能必須移除快顯視窗封鎖程式，然後使用&#x200B;**[!UICONTROL 重新整理]**&#x200B;再試一次。

1. 遵循Facebook驗證指示，驗證帳戶資訊，然後按一下&#x200B;**[!UICONTROL 繼續為……]**

1. 在&#x200B;_[!UICONTROL 商務用Facebook登入]_ (Meta至Adobe符號)中，逐步執行下列選取專案以授予GenStudio for Performance Marketing存取權：

   - 選取一或多個中繼企業設定檔，然後按一下&#x200B;**[!UICONTROL 繼續]**
   - 選取一或多個中繼頁面，然後按一下&#x200B;**[!UICONTROL 繼續]**
   - 選取一或多個Instagram帳戶，然後按一下&#x200B;**[!UICONTROL 繼續]**
   - 檢閱選取專案並按一下&#x200B;**[!UICONTROL 儲存]**

1. 收到帳戶已連線的驗證後，請按一下&#x200B;**[!UICONTROL 取得]**。

   此步驟可確保GenStudio for Performance Marketing取得所有廣告、中繼資料和量度的存取權，以發揮最佳效能。

1. 在&#x200B;_[!UICONTROL 中繼廣告]_&#x200B;中，選取一或多個要包含在[!DNL Insights]中的帳戶，然後按一下&#x200B;**[!UICONTROL 選取]**。

1. 收到&#x200B;_平台已連線_&#x200B;的確認之後，請按一下&#x200B;**[!UICONTROL 檢視帳戶]**。

   _[!UICONTROL 中繼廣告帳戶]_&#x200B;檢視會列出`Account name`、`Added by`、`Date added`和`Status`。

使用&#x200B;**[!UICONTROL 新增帳戶]**&#x200B;將更多帳戶新增至清單。 當您新增連結到相同中繼企業設定檔的帳戶時，授權流程可能會略有不同。 在連線過程中，您只選取新的中繼廣告帳戶。

## 資料擷取

最初，GenStudio for Performance Marketing會匯入最近六個月的歷史資料。 此做法可確保您立即存取相關的深入分析，以分析趨勢、評估績效及做出明智的決策。 擷取程式可能需要一到五天，視您帳戶中的資料量而定。

>[!BEGINSHADEBOX]

**資料擷取與保留原則**

GenStudio for Performance Marketing會保留13個月的管道資料。 此保留原則包含在初始連線期間擷取的6個月資料，以確保完整的歷史資料分析和報告。

>[!ENDSHADEBOX]
