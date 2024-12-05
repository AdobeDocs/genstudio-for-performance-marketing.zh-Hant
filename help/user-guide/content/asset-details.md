---
title: 資產詳細資訊
description: Adobe GenStudio for Performance Marketing會使用豐富的中繼資料儲存已核准的內容，以供搜尋和效能追蹤。
feature: Attributes, Assets
exl-id: 2be5cfee-f315-4ad6-8cf0-a8d3929b9ba3
source-git-commit: 088bc6df481fb1e961a7df3c79515642ec39767d
workflow-type: tm+mt
source-wordcount: '509'
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

下列影像資產包含描述檔案型別、大小和其他特性的系統中繼資料、一個使用者定義的關鍵字以及數個AI偵測到的屬性和顏色。

具有多個標籤之資產的![詳細資料](/help/assets/content-asset-details.png)

>[!NOTE]
>
>AEM存放庫中的Assets會顯示不同的中繼資料。 請參閱[設定資產可見性](connect-aem-repo.md#step-4-configure-asset-visibility)以瞭解如何設定[!DNL AEM Assets Content Hub]資產詳細資訊。

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
| [!UICONTROL 時間範圍] | 使用資產的時間範圍，例如季、季、年等。 範例： `Winter 2023` |
| 地區 | 使用資產的區域。 範例： `North America`， `APAC`， `Italy` |
| 語言 | 使用資產的語言。 範例： `Spanish` |
| 關鍵字 | 用於進一步識別資產特性及用途的使用者定義關鍵字 |

<!-- ## History

Expand the _[!UICONTROL History]_ section to view a timeline of approvals and activity.

list other activity, show screenshot?
-->
