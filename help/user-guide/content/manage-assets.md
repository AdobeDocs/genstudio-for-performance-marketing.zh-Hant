---
title: 管理資產和體驗
description: 簡化並增強對品牌核准資產的管理，以便在您的數位行銷歷程中使用和重複使用。
feature: Content Management, Content Attributes
exl-id: e2ce8797-6d3b-46d4-b12f-f5f80e26c669
source-git-commit: 67a760051b513dfd2bd6e69c886598efd7142090
workflow-type: tm+mt
source-wordcount: '1409'
ht-degree: 1%

---

# 管理資產和體驗

Adobe GenStudio for Performance Marketing [!DNL Content]簡化並增強品牌核准資產的管理，以便在您的數位行銷歷程中使用和重複使用。

## [!DNL Content]相簿

相簿會根據選取的檢視，顯示已核准資產、體驗或範本的詳細目錄。 表格左上方的篩選（漏斗）切換會開啟&#x200B;**[!UICONTROL 篩選]**&#x200B;功能表，您可以從許多類別中選取，以篩選相簿中顯示的內容。 在&#x200B;_[!UICONTROL Assets]_&#x200B;檢視中，按一下搜尋（放大鏡）圖示以使用關鍵字尋找資產。

下列顯示對[!UICONTROL Assets]相簿中字詞`space`的搜尋：

![搜尋空間的Assets檢視](/help/assets/content-assets-filter.png "搜尋具有空間屬性的資產")

### 搜尋內容

篩選和搜尋介面快速且回應迅速，並提供高生產力的搜尋優先體驗。 每個[!DNL Content]檢視都會提供篩選選項，以縮小搜尋範圍，找出理想的資產、體驗或範本。 針對資產和體驗，您可以選取行銷活動和特定准則，例如為特定產品製作的內容。

有以[准則](/help/user-guide/guidelines/overview.md)、[關鍵字](asset-details.md#user-defined-metadata)和[屬性類別](/help/user-guide/insights/attributes.md#categories)為基礎的篩選器，可縮小搜尋結果的範圍。 例如，您可能會想要尋找特定檔案型別或主題的資產，以協助您為行銷活動建立新的體驗。 或者，您可以根據使用者名稱或團隊成員名稱來篩選內容：

- **[!UICONTROL 上傳者]**：將&#x200B;_[!UICONTROL Assets]_&#x200B;清單限製為只顯示您或特定人員上傳的資產。
- **[!UICONTROL 建立者]**：限制&#x200B;_[!UICONTROL 體驗]_&#x200B;清單，以僅顯示您或特定人員建立的體驗。
- **[!UICONTROL 範本]**：限制&#x200B;_[!UICONTROL 體驗]_&#x200B;清單僅顯示使用所選範本建立的體驗。

如果看不到某些篩選選項，則表示存放庫中沒有符合對應中繼資料條件的範本。 請確定範本已正確加上中繼資料標籤，如此才能透過這些篩選器探索範本。

**若要搜尋要重複使用的內容**：

1. 在&#x200B;_[!DNL Content]_中，選取&#x200B;**[!UICONTROL Assets]**區段。

1. 從&#x200B;**[!UICONTROL 位置]**&#x200B;清單中選取資產存放庫，或確認您所檢視的資產存放庫是否正確。 `GenStudio assets`是預設存放庫。

   >[!IMPORTANT]
   >
   >_位置_&#x200B;清單只有在您[連線至AEM存放庫](connect-aem-repo.md)時才能使用。

1. 按一下&#x200B;**[!UICONTROL 搜尋]** （放大鏡）以輸入關鍵字或說明。

1. 從&#x200B;_[!UICONTROL 篩選器]_&#x200B;清單中選取類別，以縮小搜尋範圍。 例如，如果您正在尋找PNG檔案，請按一下&#x200B;**[!UICONTROL 檔案格式]**&#x200B;並選擇&#x200B;**PNG**。

   縮小搜尋範圍愈多，可用的篩選選項愈少。 按一下&#x200B;**[!UICONTROL 全部清除]**&#x200B;以移除所有篩選器。

1. 選取要完整檢視和詳細資訊清單的資產。

   按一下「**[!UICONTROL 下載]**」（向下箭頭）以在本機工作站中使用資產。

### 位置

依預設，您透過[!DNL Create]程式或上傳新增至[!DNL Content]的資產會儲存在`GenStudio assets`存放庫中。 `GenStudio assets`存放庫是GenStudio for Performance Marketing中的讀寫存放庫。 這表示您可以儲存、編輯和刪除`GenStudio assets`存放庫中的資產。

右側&#x200B;_[!UICONTROL Assets]_&#x200B;相簿上方的&#x200B;**[!UICONTROL 位置]**&#x200B;清單可讓您從已連線的Adobe Experience Manager (AEM) [!DNL Assets Content Hub]存放庫中進行選取。

![存放庫的位置清單](/help/assets/content-location-selection.png "選取內容存放庫"){width="350"}

選取AEM存放庫時，相簿會顯示該存放庫中的資產詳細目錄，好讓您可以善用這些存放庫中已核准的資產，作為內容建立的輸入專案。 篩選器選項會變更，以反映[!DNL AEM Assets Content Hub]中設定的類別。

如需將[!DNL AEM Assets Content Hub]存放庫新增到AEM的指引，請參閱[連線GenStudio for Performance Marketing存放庫](connect-aem-repo.md)。

AEM存放庫為唯讀，這表示您可以存取內容，但無法將草稿、新資產或中繼資料儲存至AEM存放庫。 資產、體驗和範本的所有草稿和最終更新都會使用新的[系統中繼資料](asset-details.md#system-metadata)儲存到`GenStudio assets`存放庫。

{{note-aem-assets}}

AEM存放庫可能會強制執行某些授權要求，例如資產過期。 這些資產可能無法在[!DNL Create]工作流程中使用。 您可能需要更新或更換過期的資產，才能維持專案的連續性。 請洽詢您的[!DNL AEM Assets Content Hub]管理員，以取得這些資產的協助。

## Assets管理

在[!UICONTROL Content]中，您可以輕鬆儲存、擷取及管理您的數位資產。 善用`GenStudio assets`存放庫和AEM存放庫，可確保您的資產有良好的組織且可供各種行銷活動存取。 此多存放庫方法可讓您靈活控制各環境中的資產使用情況，確保行銷工作中僅使用已核准和最新的資產。

下表列出資產、體驗和範本可用的管理任務：

| 任務 | 資產 | 體驗 | 範本 |
| --------------------------------------------------------- | :----: | :---------: | :-------: |
| [檢視詳細資料](/help/user-guide/content/asset-details.md) | ✓ | ✓ | ✓ |
| [建立體驗](/help/user-guide/create/overview.md) |        |             | ✓ |
| 在Adobe Express中編輯[](#edit-in-express) | ✓ |             |           |
| [匯出以啟動](#export-for-activation) |        | ✓ |           |
| [重新整理](/help/user-guide/content/use-templates.md#refresh-template) |   |      | ✓ |
| [下載](#download-assets) | ✓ |             | ✓ |
| [刪除](#delete-assets) | ✓ | ✓ | ✓ |

### 新增資產

將資產新增至[!DNL Content]時，預設會儲存在`GenStudio assets`存放庫中。 _[!UICONTROL 新增資產]_&#x200B;按鈕僅在&#x200B;_[!UICONTROL 位置]_&#x200B;是`GenStudio assets`存放庫時可用。

![位置欄位](/help/assets/content-location.png "位置欄位"){width="350"}

**若要新增一或多個資產**：

1. 在&#x200B;_[!DNL Content]_中，按一下&#x200B;**[!UICONTROL 新增資產]**。

1. 在&#x200B;_新增您核准的資產_&#x200B;檢視中，將一或多個檔案拖放至放置區。 您可以選擇使用&#x200B;**[!UICONTROL 瀏覽]**&#x200B;從本機檔案選取，或是從Dropbox或Microsoft OneDrive匯入檔案。

1. 在&#x200B;_新增詳細資料_&#x200B;區段中，選取&#x200B;**[!UICONTROL 促銷活動名稱]**&#x200B;或輸入新名稱。

1. 若要改善可發現性，請在&#x200B;**更多詳細資料**&#x200B;區段中新增選用的詳細資料，例如&#x200B;_品牌名稱_、_角色_、_地區_&#x200B;和&#x200B;_關鍵字_。

   您提供的詳細資料越多，就越能體驗GenStudio for Performance Marketing的強大功能。 從清單中選取一或多個詳細資訊，或輸入適用的新詳細資訊，例如關鍵字。 您新增的每個詳細資訊都會顯示在清單下方。 按一下&#x200B;**`x`**&#x200B;以移除詳細資料。

   您新增的任何詳細資料都會套用至此動作中新增的所有資產。

   檢視[中繼資料詳細資料](/help/user-guide/content/asset-details.md#system-metadata)。

1. 按一下&#x200B;**[!UICONTROL 新增資產]**。

1. 當資產上傳完成時，按一下&#x200B;**完成**。

1. 若要檢視您上傳的新資產，請按一下畫布底部的&#x200B;_可用新資產_&#x200B;通知中的&#x200B;**[!UICONTROL 重新整理]**。

### 下載資產

**若要下載資產**：

1. 在&#x200B;_[!DNL Content]_中，選取資產或範本。 按一下資產可開啟資產聚焦檢視。

1. 在資產檢視中，按一下右上角的&#x200B;**[!UICONTROL 下載]**&#x200B;圖示（向下箭頭）。

1. 下載作業會開始將資產復本放在您的預設下載位置。

### 刪除資產

**若要刪除資產**：

1. 在&#x200B;_[!DNL Content]_中，選取資產、體驗或範本。 按一下資產可開啟資產聚焦檢視。

1. 在資產檢視中，按一下右上角的&#x200B;**[!UICONTROL 刪除]** （垃圾桶）。

1. 在&#x200B;_刪除資產_&#x200B;快顯視窗中，驗證資產並按一下&#x200B;**[!UICONTROL 刪除]**。

## 匯出以啟動

您可以匯出核准的體驗，以與目標頻道相容的格式加以啟用。

**匯出體驗**：

1. 在&#x200B;_[!DNL Content]_中，選取體驗。 按一下體驗會開啟詳細資料檢視，或按一下捷徑功能表(`...`)。

1. 按一下&#x200B;**[!UICONTROL 匯出以啟動]** （箭號指向的方塊）。

1. 在&#x200B;_匯出以啟動_&#x200B;快顯視窗中，選取其中一個可用的格式：

   - 電子郵件： `HTML`，`CSV`
   - 中繼廣告、橫幅廣告和顯示廣告： `HTML`、`JPEG`、`PNG`

請參閱[啟用](/help/user-guide/activation/overview.md)。

## 在Express中編輯

您可以使用Adobe Express直接在GenStudio for Performance Marketing中編輯影像資產(JPG或PNG)。 由Adobe Express ]_支援的_[!UICONTROL &#x200B;畫布提供便利的功能，讓您在不離開GenStudio應用程式的情況下增強影像。 您可以輕鬆移除背景、套用產生式填色、調整效果和裁切影像。

>[!BEGINSHADEBOX]

使用[!DNL Edit in Adobe Express]功能增強影像的條件：

- 支援的MIME型別包括`image/png`和`image/jpeg`
- 最小影像尺寸為50x50畫素
- 最大影像尺寸為8000x8000畫素
- 大小上限為40MB （40,000,000位元組）

>[!ENDSHADEBOX]

**若要使用Express**&#x200B;編輯資產：

1. 在&#x200B;_[!DNL Content]_中，選取影像資產。 按一下資產可開啟資產聚焦檢視。

1. 在資產檢視中，按一下右上角的&#x200B;**[!UICONTROL 在Adobe Express中編輯]**&#x200B;圖示。

1. 在&#x200B;_[!UICONTROL Powered by Adobe Express]_&#x200B;畫布中，使用左側面板上的Express控制項來增強影像。

1. 當您對更新的影像感到滿意時，請按一下右上角的&#x200B;**[!UICONTROL 儲存復本]**。

1. 選取檔案格式(JPG或PNG)，然後按一下「儲存副本」****。

1. 在&#x200B;_[!UICONTROL 儲存資產]_&#x200B;快顯視窗中，更新&#x200B;**[!UICONTROL 資產名稱]**。

   - 選取&#x200B;**[!UICONTROL 與原始資產相同的詳細資料]**，以將資產詳細資料結轉到新影像。

   - 展開&#x200B;**[!UICONTROL 更多詳細資料]**&#x200B;區段以更新准則和其他中繼資料。

   >[!TIP]
   >
   >您提供的詳細資料越多，就越能體驗GenStudio for Performance Marketing的強大功能。 從清單中選取一或多個詳細資訊，或輸入適用的新詳細資訊，例如關鍵字。 您新增的每個詳細資訊都會顯示在清單下方。 按一下&#x200B;**`x`**&#x200B;以移除詳細資料。

1. 按一下「**[!UICONTROL 儲存]**」。
