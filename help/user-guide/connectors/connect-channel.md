---
title: 連線付費媒體
description: Connect a channel account to activate and monitor your ads and media with Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Admin, Data Engineer
feature: Reporting and Insights
exl-id: e699041e-b462-45b3-8c4c-4de0d52cf0e6
source-git-commit: 2844914d25d9bc3a2be7f47d0cd7f26f7c921555
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---

# Connect paid media accounts

_[!DNL Data connectors]_enable seamless integration between GenStudio for Performance Marketing and your paid media network accounts. By connecting to third-party channel accounts, you can exchange critical data, such as campaign performance metrics in [[!DNL Insights]](/help/user-guide/insights/overview.md), and you can deliver fresh ad placements with [[!DNL Activate]](/help/user-guide/activation/overview.md). This integration allows GenStudio for Performance Marketing to manage your media and ads while receiving valuable insights, including impressions, clicks, and conversions, from your active campaigns.

**若要連線到付費媒體帳戶**：

1. 按一下省略符號&#x200B;**[!UICONTROL ...左下方導覽區顯示更多]**。

1. 選取&#x200B;**[!UICONTROL 設定]**，並附上cog圖示。

1. 在&#x200B;_[!UICONTROL 設定]_&#x200B;中，從&#x200B;_[!UICONTROL 資料聯結器]_&#x200B;區段選擇聯結器型別，然後按一下&#x200B;**[!UICONTROL 連線]**。

   如果有已連線的帳戶，您可以按一下&#x200B;_已連線的帳戶_，檢視帳戶名稱、詳細資料和狀態的清單。

1. 檢視您選取的[聯結器型別](#connector-types)、檢閱先決條件，然後繼續連線步驟。

## 付費媒體連線

GenStudio for Performance Marketing supports various connector types to integrate with your preferred marketing platforms. Each connector type has specific prerequisites and set-up steps to complete for a successful connection.

### Meta ads connect

>[!BEGINSHADEBOX]

**必要條件**：

- Facebook/中繼廣告帳戶
- 存取具有`View performance`許可權層級的中繼廣告帳戶，以存取報表和檢視廣告
- 移除瀏覽器中的任何快顯封鎖程式

>[!ENDSHADEBOX]

**若要連線中繼廣告帳戶**：

1. 在&#x200B;_Data Connectors_&#x200B;區段中，按一下&#x200B;_中繼廣告_&#x200B;卡片上的&#x200B;**[!UICONTROL 連線]**。

1. 登入您的Facebook帳戶。

   您可能必須移除快顯視窗封鎖程式，然後使用&#x200B;**[!UICONTROL 重新整理]**&#x200B;再試一次。

1. 遵循Facebook驗證指示。

1. In the _[!UICONTROL Facebook Login for Business]_ pop-up (Meta to Adobe symbol), step through the following selections.

   - Verify the account information and click **[!UICONTROL Continue as]**
   - Grant access to select Pages and click **[!UICONTROL Continue]**
   - 授與選取企業的存取權，然後按一下[繼續] ****
   - 選擇加入一或多個Instagram帳戶，然後按一下&#x200B;**[!UICONTROL 繼續]**
   - 檢閱選取專案並按一下&#x200B;**[!UICONTROL 儲存]**

1. 在&#x200B;_[!UICONTROL 中繼廣告]_&#x200B;檢視中，選取一或多個帳戶並按一下&#x200B;**[!UICONTROL 選取]**。

_[!UICONTROL 中繼廣告帳戶]_&#x200B;檢視會列出`Account name`、`Added by`、`Date added`和`Status`。 使用&#x200B;**[!UICONTROL 新增帳戶]**&#x200B;將更多帳戶新增至清單。

## 資料擷取

最初，GenStudio for Performance Marketing會匯入最近六個月的歷史資料。 此做法可確保您立即存取相關的深入分析，以分析趨勢、評估績效及做出明智的決策。 The ingestion process may take one to five days depending on the volume of data in your account.

>[!BEGINSHADEBOX]

**資料擷取與保留原則**

GenStudio for Performance Marketing會保留13個月的管道資料。 此保留原則包含在初始連線期間擷取的6個月資料，以確保完整的歷史資料分析和報告。

>[!ENDSHADEBOX]
