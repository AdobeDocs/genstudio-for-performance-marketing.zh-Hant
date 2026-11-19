---
title: AI助理工具參考
description: 瞭解AI助理可以搭配[!DNL GenStudio for Performance Marketing]使用的深入分析、建立、規劃、啟用和意見回饋工具。
role: User
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 244293cf4f83acbc252f1d5f3495db403ed4a9bb
workflow-type: tm+mt
source-wordcount: '2265'
ht-degree: 13%
---

# AI助理工具參考

此參考資料說明連線的AI助理員可以搭配[!DNL GenStudio for Performance Marketing]使用的工具。 可用的工具清單取決於貴組織的設定。

在啟動工作流程之前，請詢問您的AI助理可以存取哪些工具。

## 功能區域

| 區域圖 | 用途 | 行為 |
|---|---|---|
| Insights | 查詢付費媒體和電子郵件效能，並擷取創意建議。 | 唯讀。 |
| 建立 | 尋找資產、從快速範本或見解建議彙整草稿，然後管理稽核。 | 讀取和寫入。 在Creative Cloud中建立檔案。 |
| 規劃 | 從簡報中擷取行銷活動詳細資料，並將其儲存至Workfront Planning。 | 擷取是唯讀的。 儲存會在Workfront Planning中建立記錄，且無法自動回覆。 |
| 啟動 | 解決發佈目標，並將核准的體驗傳送至平台。 | 寫入。 廣告會傳送至平台，並以關閉狀態發佈。 您可以分別開啟這些功能。 無法透過這些工具還原。 |
| 回饋 | 傳送產品意見回饋給[!DNL GenStudio for Performance Marketing]團隊。 | 寫入。 |

大部分的深入分析工具涵蓋`meta`、`linkedin`和`innovid`。 量度值工具涵蓋`meta`和`linkedin`。 電子郵件行銷活動報告涵蓋Adobe Journey Optimizer (`ajo`)和Adobe Campaign (`acc`)。

建立支援`meta`、`linkedin`、`display`、`tiktok`和`youtube`。 啟用支援`META`、`LINKEDIN`和`GOOGLECM360`。

## 分析工具

### get_insights_capabilities

傳回為您組織啟用的見解管道和報表作業。 可用性不明時，請先使用此工具。 支援的管道是`meta`、`linkedin`、`innovid`、`ajo`和`acc`。

此工具會傳回功能中繼資料，而非行銷活動、廣告或量度值。 若要尋找您組織的自訂量度金鑰，請使用`list_connected_channels_and_metrics`。

### list_connected_channels_and_metrics

傳回貴組織的作用中Meta、LinkedIn和Google Campaign Manager 360連線、支援的Insights管道和作業，以及設定的自訂轉換量度。 在呼叫`get_insights_metric_values`之前，使用它來尋找量度索引鍵。

此工具會傳回量度索引鍵、標籤和格式，而非量度值。 連線無法保證歷史報表資料可用。

| 參數 | 必要 | 說明 |
|---|---|---|
| `limit`, `offset` | 無 | 頁面大小和分頁位移。 省略兩者以傳回完整的目錄。 |

### get_insights_summary

傳回所選日期範圍內單一管道的整體績效量度和趨勢。

| 參數 | 必要 | 說明 |
|---|---|---|
| `channel` | 是 | `meta`、`linkedin`或`innovid`。 |
| `startDate` | 無 | 開始日期為`YYYY-MM-DD`格式。 預設值為30天前。 |
| `endDate` | 無 | 結束日期為`YYYY-MM-DD`格式。 預設值為今天。 |
| `metrics` | 無 | 要繪製圖表的量度： `spend`、`ctr`、`cpc`、`cpm`、`cpa`、`impressions`、`clicks`、`conversions`、`videoPlays`、`engagement`、`likes`、`comments`或`shares`。 預設值為`spend`、`ctr`、`cpc`和`cpm`。 |

### list_insights_campaigns

傳回行銷活動績效量度的可排序表格和總計列。

| 參數 | 必要 | 說明 |
|---|---|---|
| `channel` | 是 | `meta`、`linkedin`或`innovid`。 |
| `startDate`, `endDate` | 無 | 日期範圍`YYYY-MM-DD`格式。 預設為過去30天。 |
| `search` | 無 | 行銷活動名稱篩選器。 |
| `sortBy` | 無 | 排序欄位： `spend`、`impressions`、`clicks`、`ctr`、`cpc`、`cpm`或`name`。 預設為 `spend`。 結果一律以遞減順序排序。 |
| `limit`, `offset` | 無 | 頁面大小和分頁位移。 預設頁面大小為20。 |

### list_insights_email_campaigns

針對Adobe Journey Optimizer和Adobe Campaign，傳回電子郵件行銷活動及其傳送和參與量度的可排序表格。 對於廣告行銷活動，請使用`list_insights_campaigns`。

| 參數 | 必要 | 說明 |
|---|---|---|
| `channel` | 是 | `ajo`或`acc`。 |
| `startDate`, `endDate` | 無 | 日期範圍`YYYY-MM-DD`格式。 預設為結束日期前的前30天。 |
| `search` | 無 | 行銷活動名稱篩選器。 |
| `sortBy` | 無 | 排序欄位： `campaignName`、`emailsNumber`、`emailsDelivered`、`totalClicks`、`openRate`、`ctr`、`ctor`、`bounceRate`、`unsubscribeRate`或`spamComplaintRate`。 預設為 `emailsDelivered`。 結果一律以遞減順序排序。 |
| `limit`, `offset` | 無 | 頁面大小和分頁位移。 |

### list_insights_ads

傳回廣告層級效能。 對可排序表格使用預設瀏覽模式，或對高和低效廣告使用層級模式。

| 參數 | 必要 | 說明 |
|---|---|---|
| `channel` | 是 | `meta`、`linkedin`或`innovid`。 |
| `tier` | 無 | `all`、`high`或`low`。 預設為 `all`。 |
| `mainMetric` | 無 | `high`或`low`層級模式的排名量度： `ctr`、`cpc`、`cpm`、`cpa`、`spend`、`impressions`或`clicks`。 在瀏覽模式中忽略。 |
| `metrics` | 無 | 要針對層級模式中的每個廣告報告的其他量度。 |
| `campaigns` | 無 | 用來限制結果的行銷活動，最多50個。 每個行銷活動包含`channel`、`accountId`和`campaignId`。 |
| `search` | 無 | 廣告名稱篩選。 |
| `sortBy` | 無 | 瀏覽模式排序欄位： `spend`、`impressions`、`clicks`、`ctr`、`cpc`、`cpm`或`name`。 預設為 `spend`。 結果一律以遞減順序排序。 |
| `spendMin`, `spendMax` | 無 | 每個廣告的總支出界限。 僅限層級模式。 |
| `includeUnsupported` | 無 | 包含無法呈現其創意的廣告。 預設為 `false`。 |
| `startDate`, `endDate` | 無 | 日期範圍`YYYY-MM-DD`格式。 |
| `limit`, `offset` | 無 | 頁面大小和分頁位移。 |

層級模式傳回`get_insights_ad_attributes`所需的廣告識別碼。

### get_insights_ad_details

傳回一個廣告的創意中繼資料，包括復本、call to action、資產和版位。 它不會傳回效能量度。

| 參數 | 必要 | 說明 |
|---|---|---|
| `channel` | 是 | `meta`、`linkedin`或`innovid`。 |
| `accountId` | 是 | 付費媒體帳戶識別碼。 |
| `campaignId` | 是 | 促銷活動識別碼。 |
| `adId` | 是 | 廣告識別碼。 |
| `adgroupId` | 無 | 頻道使用廣告群組時的廣告群組識別碼。 |

### get_insights_ad_attributes

將所選廣告的創意特徵與管道平均進行比較。 在`list_insights_ads`識別高績效或低績效廣告之後使用它。

| 參數 | 必要 | 說明 |
|---|---|---|
| `ads` | 是 | 一到200個廣告需要說明。 每個廣告包含`channel`、`accountId`、`campaignId`和`adId`，以及選擇性的`adGroupId`和`performanceTier` （`high`或`low`）。 在階層模式中使用`list_insights_ads`傳回的識別碼。 |
| `mainMetric` | 是 | 用於排名廣告的量度： `ctr`、`cpc`、`cpm`、`cpa`、`spend`、`impressions`或`clicks`。 |
| `campaigns` | 無 | 用來定義比較母體的行銷活動，最多50個。 每個行銷活動包含`channel`、`accountId`和`campaignId`。 |
| `spendMin`, `spendMax` | 無 | 比較母體的支出界限。 |
| `startDate`, `endDate` | 無 | 日期範圍`YYYY-MM-DD`格式。 |

### get_insights_tag_categories

傳回貴組織在請求期間可用的標籤類別。 它會傳回類別名稱，而非效能量度。

| 參數 | 必要 | 說明 |
|---|---|---|
| `channels` | 是 | 一或多個支援的管道。 |
| `startDate`, `endDate` | 無 | 日期範圍`YYYY-MM-DD`格式。 |

### get_insights_ad_tags

傳回單一類別中標籤值（例如產品、區域或創意主題）的績效。

| 參數 | 必要 | 說明 |
|---|---|---|
| `channel` | 是 | `meta`、`linkedin`或`innovid`。 |
| `tagCategory` | 是 | `get_insights_tag_categories`傳回的類別。 |
| `tagSource` | 無 | `ad_tags`或`campaign_tags`。 預設為 `ad_tags`。 |
| `sortBy` | 無 | 排序欄位： `adsCount`、`spend`、`impressions`、`clicks`、`conversionCount`、`ctr`、`cpc`、`cpm`或`cpa`。 預設為 `adsCount`。 |
| `search` | 無 | 標籤值篩選器。 |
| `startDate`, `endDate` | 無 | 日期範圍`YYYY-MM-DD`格式。 |
| `limit`, `offset` | 無 | 頁面大小和分頁位移。 |

### get_insights_metric_values

針對Meta和LinkedIn，傳回組織追蹤量度的值和趨勢，例如潛在客戶、註冊或廣告支出回報率。

| 參數 | 必要 | 說明 |
|---|---|---|
| `channels` | 否 | `meta`、`linkedin`或兩者。 |
| `metrics` | 無 | `list_connected_channels_and_metrics`最多傳回20個量度索引鍵。 預設為您組織的預設可見集。 |
| `campaigns` | 無 | 用來限制結果的行銷活動，最多50個。 每個行銷活動包含`channel`、`accountId`和`campaignId`。 |
| `startDate`, `endDate` | 無 | 日期範圍`YYYY-MM-DD`格式。 預設為過去30天。 |

### get_insights_recommendations

根據您組織的效能資料傳回提議的創意變更。 當選取的範圍不含合格廣告時，請求無法傳回任何建議。

| 參數 | 必要 | 說明 |
|---|---|---|
| `channels` | 是 | 一或多個`meta`、`linkedin`或`innovid`。 |
| `campaigns` | 無 | 用來限制結果的行銷活動，最多50個。 每個行銷活動包含`channel`、`accountId`和`campaignId`。 |
| `search` | 無 | 行銷活動名稱篩選器。 |
| `recommendationId` | 無 | 一個建議的`adUid`，用來擷取其詳細資訊。 |
| `onlyWithPreview` | 無 | 排除沒有範例創意預覽的建議。 預設為 `true`。 |
| `limit`, `offset` | 無 | 頁面大小和分頁位移。 |

## 建立工具

在體驗準備好啟用之前，建立工具以尋找資產、從Adobe Express範本組合草稿，以及管理稽核。

### list_express_templates

列出具有篩選條件和Facet計數的可用快速範本。

| 參數 | 必要 | 說明 |
|---|---|---|
| `channel` | 否 | `meta`、`display`、`linkedin`、`tiktok`、`youtube`或`__unspecified__`。 |
| `query` | 無 | 範本的搜尋字詞。 |
| `activatableMimeType`, `aspectRatios`, `externalTemplateSource`, `isHTML5Template`, `keywords`, `languages`, `mediaFormat`, `regions`, `timeframes` | 無 | 範本Facet篩選器。 |
| `sortBy` | 無 | `modified`或`created`。 預設為 `modified`。 |
| `order` | 無 | `asc`或`desc`。 預設為 `desc`。 |
| `limit`, `offset` | 無 | 頁面大小和分頁位移。 |

### describe_express_template

傳回範本中可編輯的文字欄位和影像位置。

| 參數 | 必要 | 說明 |
|---|---|---|
| `templateId` | 是 | 快速範本識別碼。 |

### list_cta_options

傳回某個管道所允許的call-to-action值。 「顯示」會傳回空白清單，因為它接受自由格式文字。

| 參數 | 必要 | 說明 |
|---|---|---|
| `channel` | 是 | `linkedin`、`meta`、`display`、`tiktok`或`youtube`。 |
| `limit`, `offset` | 無 | 頁面大小和分頁位移。 省略兩者以傳回每個選項。 |

### search_assets

搜尋您GenStudio內容中的影像和影片。 使用它來選取草稿的現有資產。 衍生資產、外部資產和過期的資產會排除在外。 此工具不會上傳、編輯、刪除或產生資產，而且需要GenStudio內容權益。

| 參數 | 必要 | 說明 |
|---|---|---|
| `query` | 否 | 跨資產中繼資料的關鍵字或自然語言搜尋。 |
| `mediaTypes` | 無 | `image`、`video`或兩者。 預設包含兩者。 |
| `aspectRatios` | 無 | 外觀比例，例如`1:1`或`16:9`。 如果比率不可用，工具會傳回可用的選項。 |
| `brands`, `campaigns`, `products`, `personas`, `channels` | 無 | 依名稱篩選。 |
| `customMetadata` | 無 | 最多5個中繼資料欄位，每個欄位有一或多個值。 |
| `uploadedBy` | 無 | `me`或上傳程式電子郵件地址。 |
| `createdAtFrom`, `createdAtTo` | 無 | 以ISO 8601格式建立時間範圍。 |
| `aiGenerated` | 無 | 依AI產生狀態篩選。 |
| `contentCredentials` | 無 | 依Content Credentials狀態篩選。 |
| `limit`, `offset` | 無 | 頁面大小和分頁位移。 |

結果包含`create_draft`的穩定資產參考和短期已簽署URL。

### create_draft

從具有一或多個體驗的快速範本建立可編輯的草稿。 每個呼叫都會建立新的草稿。

| 參數 | 必要 | 說明 |
|---|---|---|
| `templateId` | 是 | 快速範本識別碼。 |
| `prompt` | 是 | Creative摘要並複製與草稿一起儲存的指示。 |
| `experiences` | 是 | 一或多個體驗。 請參閱下表。 |
| `name` | 無 | 檔名稱。 |
| `allowAssetReuse` | 無 | 允許跨多個體驗重複使用一個選取的資產。 預設為 `false`。 |

每個體驗都支援這些欄位：

| 欄位 | 必要 | 說明 |
|---|---|---|
| `channel` | 是 | `linkedin`、`meta`、`display`、`tiktok`或`youtube`。 |
| `title` | 無 | 體驗標題。 預設值為「概念&#x200B;*n*」。 |
| `headline` | Meta和LinkedIn | 主要標題。 |
| `body` | Meta、LinkedIn和TikTok | 內文。 對於LinkedIn，這是介紹性文字。 若為TikTok，此為主要文字。 |
| `description` | YouTube | 廣告說明。 Meta和LinkedIn的選用專案。 |
| `display_url` | Meta和LinkedIn | 在廣告中顯示URL。 |
| `destination_url` | 無 | 廣告連結到的URL。 |
| `cta` | 無 | 來自`list_cta_options`的Call-to-action文字。 |
| `templateFields` | 無 | 覆寫來自`describe_express_template`的具名範本元素。 每個覆寫都會設定文字、含尺寸的影像URL或視訊URL。 |
| `assetTemplateFields` | 無 | 範本中影像或視訊欄位的`search_assets`內容資產。 |

在建立具有固定call-to-action值的管道草稿之前，請使用`list_cta_options`。

### create_draft_from_recommendation

根據特定前瞻分析建議建立可編輯的草稿。

| 參數 | 必要 | 說明 |
|---|---|---|
| `channel` | 是 | `meta`或`linkedin`。 |
| `adUid` | 是 | 由`get_insights_recommendations`傳回的建議識別碼。 |
| `prompt` | 是 | 根據建議的Creative摘要。 |
| `name` | 無 | 檔名稱。 |

### list_recent_drafts

列出最近的Express範本草稿及其狀態和連結。

| 參數 | 必要 | 說明 |
|---|---|---|
| `limit`, `offset` | 無 | 頁面大小和分頁位移。 |

### get_draft_metadata

傳回草稿的名稱、管道、核准狀態、稽核者結果和共同作業人員存取權。

| 參數 | 必要 | 說明 |
|---|---|---|
| `draftId` | 是 | 草稿資產識別碼。 |

### share_draft

為共同作業人員提供草稿的檢視或編輯許可權，而不需請求核准。

| 參數 | 必要 | 說明 |
|---|---|---|
| `draftId` | 是 | 草稿資產識別碼。 |
| `emails` | 是 | 1至20個共同作業人員電子郵件地址。 |
| `role` | 是 | `editor`或`viewer`。 |
| `message` | 無 | 邀請訊息。 |

### request_draft_approval

傳送草稿給一或多人進行核准。

| 參數 | 必要 | 說明 |
|---|---|---|
| `draftId` | 是 | 草稿資產識別碼。 |
| `emails` | 是 | 1到20個稽核者電子郵件地址。 |

### list_experiences

傳回已核准且發佈且準備好啟用的體驗。 不包含草稿。

| 參數 | 必要 | 說明 |
|---|---|---|
| `channel` | 否 | `email`、`meta`、`meta_organic`、`display`、`ctv`、`linkedin`、`linkedin_organic`、`tiktok`、`chatgpt`或`youtube`。 |
| `createdByMe` | 無 | 將結果限製為目前使用者建立的體驗。 |
| `campaignNames` | 無 | 最多5個確切的行銷活動名稱篩選器。 |
| `creatorEmail` | 無 | 建立者電子郵件篩選器。 |
| `createdAtFrom`, `createdAtTo` | 無 | 建立日期範圍。 |
| `language` | 無 | BCP 47語言標籤。 |
| `limit`, `cursor` | 無 | 頁面大小（1-50、預設20）和分頁遊標。 |

## 計畫工具

計畫工具會將行銷活動簡介轉換為可檢視的行銷活動草稿，並儲存至Workfront Planning。

### extract_campaign_from_brief

從貼上的行銷簡報中擷取可檢視的行銷活動草稿。 此工具不會儲存任何記錄。 無法推斷缺少的事實和日期。

| 參數 | 必要 | 說明 |
|---|---|---|
| `briefText` | 是 | 一個行銷活動簡介的完整純文字，最多100,000個字元。 不支援檔案和連結。 |

結果包括行銷活動草稿、發現專案及支援的引號、建議的對象和警告。

### create_workfront_campaign

從您檢閱並核准的草稿中，使用連結的產品和角色建立Workfront規劃行銷活動。 此工具不是等冪，而且無法自動復原記錄。 在重試可能已成功的寫入作業之前檢查Workfront。

| 參數 | 必要 | 說明 |
|---|---|---|
| `campaignDraft` | 是 | 核准的草稿。 需要`name`。 選用欄位為`description`、`objective`、`keyMessaging`、`startDate`、`endDate` (`YYYY-MM-DD`)、`status`、`channels`、`products`和`personas`。 |
| `channelSelections` | 無 | 不明確管道名稱的核准選擇。 |
| `entitySelections` | 無 | 已核准現有產品和角色記錄。 使用`null`要求新記錄。 |
| `createMissingEntities` | 無 | 建立您選取為新產品和角色。 預設為 `false`。 |

如果產品、角色或管道模稜兩可，則工具會傳回選項以確認，且不會進行任何變更。

## 啟動工具

啟用工具解決付費媒體目標並將核准的體驗傳送至平台。 廣告會以關閉狀態發佈（Meta已暫停、LinkedIn草稿、行銷活動管理員360非作用中），因此您必須先個別開啟廣告，才能傳送廣告。 透過這些工具將廣告傳送至平台無法還原。

### configure_activation_target

必要時解析及驗證付費媒體帳戶、行銷活動、廣告集和Facebook頁面。

| 參數 | 必要 | 說明 |
|---|---|---|
| `platform` | 是 | `META`、`LINKEDIN`或`GOOGLECM360`。 |
| `platformAccountId` | 無 | 付費媒體帳戶識別碼。 省略它以探索帳戶。 |
| `campaignId` | 無 | Meta或LinkedIn的行銷活動識別碼。 不用於Campaign Manager 360。 |
| `adsetId` | 無 | Meta廣告集或LinkedIn促銷活動識別碼。 不用於Campaign Manager 360。 |
| `pageId` | 無 | 適用於Meta的Facebook頁面識別碼。 |

對於Campaign Manager 360，只需要廣告帳戶。

### create_activation

使用已驗證的目標，將已核准的體驗以廣告的形式傳送至平台。 廣告會以關閉狀態發佈。 Meta會為每個外觀比例建立一個含有第一個影像的廣告。 LinkedIn和Campaign Manager 360會為每個已解析的影像建立一個廣告。

| 參數 | 必要 | 說明 |
|---|---|---|
| `platform` | 是 | `META`、`LINKEDIN`或`GOOGLECM360`。 |
| `targetId` | 是 | 由`configure_activation_target`傳回的已驗證目標。 |
| `experienceId` | 是 | `list_experiences`傳回已核准的體驗識別碼。 |
| `name` | 無 | 廣告位置顯示名稱。 預設為體驗的廣告標題。 |

結果會列出已建立、已排入佇列及已略過的廣告數量，以及每個廣告的初始狀態及其在[!DNL GenStudio for Performance Marketing]中的連結。 `PENDING`的狀態表示工作已排入佇列，而非廣告正在傳遞。

撥打兩次`create_activation`會建立額外的廣告，而非更新第一個廣告。

## 意見回饋工具

### submit_mcp_feedback

傳送工具或工作流程的相關意見給[!DNL GenStudio for Performance Marketing]團隊。

| 參數 | 必要 | 說明 |
|---|---|---|
| `category` | 是 | `bug`、`feature_request`或`workflow_friction`。 |
| `comment` | 是 | 意見回饋的簡要說明。 |
| `tags` | 無 | 用來分類意見回饋的標籤。 |
| `tool_name` | 無 | 與意見反應關聯的工具。 |

## 常見工作流程

當一個工具為另一個工具提供識別碼或設定時，請使用以下順序：

- **診斷廣告：**&#x200B;在`high`或`low`層級模式中呼叫`list_insights_ads`，然後使用相同的排名量度呼叫`get_insights_ad_attributes`。
- **依標籤分析：**&#x200B;呼叫`get_insights_tag_categories`，然後使用傳回的類別呼叫`get_insights_ad_tags`。
- **檢閱追蹤的量度：**&#x200B;呼叫`list_connected_channels_and_metrics`，然後使用傳回的量度索引鍵呼叫`get_insights_metric_values`。
- **將建議轉換為草稿：**&#x200B;呼叫`get_insights_recommendations`，然後呼叫`create_draft_from_recommendation`。
- **從範本建置：**&#x200B;呼叫`list_express_templates`、`describe_express_template`和`list_cta_options`，然後呼叫`create_draft`。
- **從現有資產建置：**&#x200B;呼叫`search_assets`，然後將傳回的資產參考傳遞至`assetTemplateFields`中的`create_draft`。
- **將行銷活動簡報儲存至Workfront：**&#x200B;請致電`extract_campaign_from_brief`，檢閱草稿，然後致電`create_workfront_campaign`。
- **將核准的體驗傳送至平台：**&#x200B;呼叫`list_experiences`，然後呼叫`configure_activation_target`與`create_activation`。

## 相關功能

- [AI助理概述](overview.md)
- [連線AI助理](connect-ai-assistants.md)
- [使用AI助理](use-ai-assistants.md)
