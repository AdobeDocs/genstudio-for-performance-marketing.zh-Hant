---
title: 資產詳細資訊
description: Adobe GenStudio for Performance Marketing會使用豐富的中繼資料儲存已核准的內容，以供搜尋和效能追蹤。
feature: Attributes, Assets
exl-id: 2be5cfee-f315-4ad6-8cf0-a8d3929b9ba3
source-git-commit: a2c2a39a8ed69a36c7126312ac42f6e02dd0598e
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 0%

---

# 資產詳細資訊

Adobe GenStudio for Performance Marketing會以豐富的中繼資料儲存已核准的內容，以便探索性和效能追蹤。

每個資產（包括體驗和範本）都有關聯的&#x200B;_詳細資料_ （中繼資料），以協助識別、追蹤、使用內容效能和從中學習。

**若要檢視資產詳細資訊**：

1. 在&#x200B;_[!DNL Content]_中，選取資產、體驗或範本。 按一下資產可開啟資產聚焦檢視。

1. 在資產檢視中，檢閱右側的&#x200B;_[!UICONTROL 詳細資料]_&#x200B;區段。

   >[!TIP]
   >
   >如果看不到&#x200B;_[!UICONTROL 詳細資料]_&#x200B;區段，請按一下&#x200B;**[!UICONTROL 資訊]** (i)圖示。

   資產詳細資料包含在建立或上傳程式期間套用的中繼資料。 資產中繼資料型別包含[系統中繼資料](#system-metadata)和[使用者定義的中繼資料](#user-defined-metadata)。

>[!NOTE]
>
>AEM存放庫中的Assets會顯示不同的中繼資料。 請參閱[設定資產可見性](connect-aem-repo.md#step-4-configure-asset-visibility)以瞭解如何設定[!DNL AEM Assets Content Hub]資產詳細資訊。

## 在Express中編輯

您可以使用Adobe Express直接在GenStudio for Performance Marketing中編輯影像資產(JPG或PNG)。 _[!UICONTROL Powered by Adobe Express]_&#x200B;畫布提供便利的功能，讓您在不離開GenStudio應用程式的情況下增強影像。 您可以輕鬆移除背景、套用產生式填色、調整效果和裁切影像。

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

   - 展開&#x200B;**[!UICONTROL 更多詳細資料]**&#x200B;區段以更新行銷活動、准則和其他中繼資料。

   >[!TIP]
   >
   >您提供的詳細資料越多，就越能體驗GenStudio for Performance Marketing的強大功能。 從清單中選取一或多個詳細資訊，或輸入適用的新詳細資訊，例如關鍵字。 您新增的每個詳細資訊都會顯示在清單下方。 按一下&#x200B;**`x`**&#x200B;以移除詳細資料。

1. 按一下「**[!UICONTROL 儲存]**」。

## 系統中繼資料

上傳資產時，會自動收集部分資產中繼資料。 您無法編輯預設的系統中繼資料。

為資產儲存和擷取的預設中繼資料包括檔案名稱、維度、來源等。

### 產生的標籤

當您在[!DNL Content]中儲存已核准的資產時，GenStudio for Performance Marketing會使用Adobe的AI和機器學習功能來研究該資產，並根據資產功能套用標籤。 例如，貓的圖片可能會產生屬性標籤，例如`pet photography`或`cat`，以及識別圖片中主要顏色的顏色標籤。 您無法編輯偵測到並自動套用的標籤。

如需影像、視訊和文字功能的詳細清單，請參閱[!DNL Insights] [屬性類別](/help/user-guide/insights/attribute-category.md)。

### 產生的內容中繼資料

用來產生新資產或體驗的資訊會成為中繼資料，例如所使用的提示。 內容獲得核准後，您就無法編輯提示，但您可以用它作為產生新內容的起點。

## 使用者定義的中繼資料

使用者定義的中繼資料會將行銷內容新增至資產內容，讓行銷人員瞭解如何使用及參與資產。

當您[上傳資產](/help/user-guide/content/manage-assets.md#add-assets)時，您可以將GenStudio for Performance Marketing中存在的一組選用資產詳細資料定義為中繼資料。 包含更多詳細資訊可改善搜尋和篩選中的資產識別功能。

### 中繼資料詳細資料

下表詳細說明您建立資產時可以定義的中繼資料（資產詳細資訊）。

| 欄位 | 說明 |
| ------------- | ----------- |
| 行銷活動（專案名稱） | 隨資產擷取並儲存的預設中繼資料 |
| [!DNL Brands] | [[!DNL Brands]](/help/user-guide/guidelines/brands.md)已新增至GenStudio for Performance Marketing並發佈以供使用 |
| [!DNL Products] | [[!DNL Products]](/help/user-guide/guidelines/products.md)已新增至GenStudio for Performance Marketing以供使用 |
| [!DNL Personas] | [[!DNL Personas]](/help/user-guide/guidelines/personas.md)已新增至GenStudio for Performance Marketing以供使用 |
| 頻道 | 資產使用的GenStudio for Performance Marketing內容型別，例如電子郵件和中繼廣告 |
| 時間範圍 | 使用資產的時間範圍，例如季、季、年等。 範例： `Winter 2023` |
| 地區 | 使用資產的區域。 範例： `North America`， `APAC`， `Italy` |
| 語言 | 使用資產的語言。 範例： `Spanish` |
| 關鍵字 | 用於進一步識別資產特徵和用途的關鍵字 |

<!-- ## History

Expand the _[!UICONTROL History]_ section to view a timeline of approvals and activity.

list other activity, show screenshot?
-->
