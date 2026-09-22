---
title: AI助理工具參考
description: 瞭解AI助理可以搭配[!DNL GenStudio for Performance Marketing]使用的深入分析、建立、啟用和意見回饋工具。
role: User
source-git-commit: 6fb7ddb7549ea6bcd66b6139fbde9ebe12ddaa22
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 15%
---

# AI助理工具參考

此參考資料說明連線的AI助理員可以搭配[!DNL GenStudio for Performance Marketing]使用的工具。 可用的工具清單取決於貴組織的設定。

在啟動工作流程之前，請詢問您的AI助理可以存取哪些工具。

## 功能區域

| 區域圖 | 用途 | 行為 |
|---|---|---|
| Insights | 查詢付費媒體效能並擷取創意建議。 | 唯讀。 |
| 建立 | 從快速範本或見解建議彙整草稿，然後管理稽核。 | 讀取和寫入。 在Creative Cloud中建立檔案。 |
| 啟動 | 解決發佈目標並發佈已核准的體驗。 | 寫入和破壞。 可以發佈即時廣告並產生廣告支出。 |
| 回饋 | 傳送產品意見回饋給[!DNL GenStudio for Performance Marketing]團隊。 | 寫入。 |

大部分的深入分析工具涵蓋`meta`、`linkedin`和`innovid`。 轉換量度工具涵蓋`meta`和`linkedin`。

建立支援`meta`、`linkedin`、`display`、`tiktok`和`youtube`。 啟用支援`META`、`LINKEDIN`和`GOOGLECM360`。

## 分析工具

### get_insights_capabilities

傳回為您的組織啟用的見解管道、作業和自訂轉換量度。 可用性不明時，請先使用此工具。

此工具會傳回功能中繼資料，而非行銷活動、廣告或量度值。

### get_insights_summary

傳回所選日期範圍內單一管道的整體績效量度和趨勢。

| 參數 | 必要 | 說明 |
|---|---|---|
| `channel` | 是 | `meta`、`linkedin`或`innovid`。 |
| `startDate` | 無 | 開始日期為`YYYY-MM-DD`格式。 預設值為30天前。 |
| `endDate` | 無 | 結束日期為`YYYY-MM-DD`格式。 預設值為今天。 |
| `metrics` | 無 | 要繪製圖表的量度，例如`spend`、`ctr`、`cpc`、`cpm`、`impressions`、`clicks`或`conversions`。 |

### list_insights_campaigns

傳回行銷活動績效量度的可排序表格和總計列。

| 參數 | 必要 | 說明 |
|---|---|---|
| `channel` | 是 | `meta`、`linkedin`或`innovid`。 |
| `startDate`, `endDate` | 無 | 日期範圍`YYYY-MM-DD`格式。 預設為過去30天。 |
| `search` | 無 | 行銷活動名稱篩選器。 |
| `sortBy` | 無 | 排序欄位，例如`spend`、`impressions`、`clicks`、`ctr`、`cpc`、`cpm`或`name`。 |
| `limit`, `offset` | 無 | 頁面大小和分頁位移。 |

### list_insights_ads

傳回廣告層級效能。 對可排序表格使用預設瀏覽模式，或對高和低效廣告使用層級模式。

| 參數 | 必要 | 說明 |
|---|---|---|
| `channel` | 是 | `meta`、`linkedin`或`innovid`。 |
| `tier` | 無 | `all`、`high`或`low`。 預設為 `all`。 |
| `mainMetric` | 條件式 | `high`或`low`層級模式所需的排名量度。 |
| `campaigns` | 無 | 用來限制結果的促銷活動識別碼。 |
| `search` | 無 | 廣告名稱篩選。 |
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
| `ads` | 是 | 要說明的廣告，包括`list_insights_ads`傳回的識別碼。 |
| `mainMetric` | 是 | 用來排名廣告的量度。 |
| `campaigns` | 無 | 用來定義比較母體的促銷活動識別碼。 |
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
| `tagSource` | 無 | `ad_tags`或`campaign_tags`。 |
| `sortBy` | 無 | 用來排序結果的量度。 |
| `search` | 無 | 標籤值篩選器。 |
| `startDate`, `endDate` | 無 | 日期範圍`YYYY-MM-DD`格式。 |

### get_insights_custom_metrics

傳回為組織設定的自訂轉換量度。 在`get_insights_conversion_metrics`之前使用它。

此工具會傳回量度識別碼，而非量度值。

### get_insights_conversion_metrics

傳回Meta和LinkedIn已設定的轉換量度值和趨勢。

| 參數 | 必要 | 說明 |
|---|---|---|
| `channels` | 否 | 支援的轉換管道。 預設為 `meta`。 |
| `metrics` | 無 | `get_insights_custom_metrics`傳回的量度識別碼。 |
| `campaigns` | 無 | 用來限制結果的促銷活動識別碼。 |
| `startDate`, `endDate` | 無 | 日期範圍`YYYY-MM-DD`格式。 |

### get_insights_recommendations

根據您組織的效能資料傳回提議的創意變更。 當選取的範圍不含合格廣告時，請求無法傳回任何建議。

| 參數 | 必要 | 說明 |
|---|---|---|
| `channels` | 是 | 一或多個支援的管道。 |
| `campaigns` | 無 | 用來限制結果的促銷活動識別碼。 |
| `search` | 無 | 行銷活動名稱篩選器。 |
| `recommendationId` | 無 | 用來擷取一個詳細建議的識別碼。 |
| `limit`, `offset` | 無 | 頁面大小和分頁位移。 |

## 建立工具

在體驗準備好啟動之前，建立工具以從Adobe Express範本組合草稿並管理稽核。

### list_express_templates

列出具有篩選條件和Facet計數的可用快速範本。

| 參數 | 必要 | 說明 |
|---|---|---|
| `channel` | 否 | `meta`、`display`、`linkedin`、`tiktok`、`youtube`或`__unspecified__`。 |
| `query` | 無 | 範本的搜尋字詞。 |
| `aspectRatios`, `keywords`, `languages`, `mediaFormat`, `regions`, `timeframes` | 無 | 範本Facet篩選器。 |
| `sortBy`, `order` | 無 | 排序欄位和順序。 |
| `limit`, `offset` | 無 | 頁面大小和分頁位移。 |

### describe_express_template

傳回範本中可編輯的文字欄位和影像位置。

| 參數 | 必要 | 說明 |
|---|---|---|
| `templateId` | 是 | 快速範本識別碼。 |

### list_cta_options

傳回某個管道所允許的call-to-action值。

| 參數 | 必要 | 說明 |
|---|---|---|
| `channel` | 是 | `linkedin`、`meta`、`display`、`tiktok`或`youtube`。 |

### create_draft

從具有一或多個體驗的快速範本建立可編輯的草稿。

| 參數 | 必要 | 說明 |
|---|---|---|
| `templateId` | 是 | 快速範本識別碼。 |
| `prompt` | 是 | Creative摘要並複製與草稿一起儲存的指示。 |
| `experiences` | 是 | 每個體驗的管道、內容欄位和選用範本欄位覆寫。 |
| `name` | 無 | 檔名稱。 |

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
| `emails` | 是 | 一或多個共同作業人員電子郵件地址。 |
| `role` | 是 | `editor`或`viewer`。 |
| `message` | 無 | 邀請訊息。 |

### request_draft_approval

傳送草稿給一或多人進行核准。

| 參數 | 必要 | 說明 |
|---|---|---|
| `draftId` | 是 | 草稿資產識別碼。 |
| `emails` | 是 | 一或多個稽核者電子郵件地址。 |

### list_experiences

傳回已核准且發佈且準備好啟用的體驗。 不包含草稿。

| 參數 | 必要 | 說明 |
|---|---|---|
| `channel` | 否 | 體驗管道篩選器。 |
| `createdByMe` | 無 | 將結果限製為目前使用者建立的體驗。 |
| `campaignNames` | 無 | 確切的行銷活動名稱篩選器。 |
| `creatorEmail` | 無 | 建立者電子郵件篩選器。 |
| `createdAtFrom`, `createdAtTo` | 無 | 建立日期範圍。 |
| `language` | 無 | BCP 47語言標籤。 |
| `limit`, `cursor` | 無 | 頁面大小和分頁遊標。 |

## 啟動工具

啟用工具解決付費媒體目標並發佈已核准的體驗。 發佈作業無法透過這些工具還原，且可能會產生廣告支出。

### configure_activation_target

必要時解析及驗證付費媒體帳戶、行銷活動、廣告集和Facebook頁面。

| 參數 | 必要 | 說明 |
|---|---|---|
| `platform` | 是 | `META`、`LINKEDIN`或`GOOGLECM360`。 |
| `platformAccountId` | 無 | 付費媒體帳戶識別碼。 省略它以探索帳戶。 |
| `campaignId` | 無 | Meta或LinkedIn的行銷活動識別碼。 |
| `adsetId` | 無 | Meta廣告集或LinkedIn促銷活動識別碼。 |
| `pageId` | 無 | 適用於Meta的Facebook頁面識別碼。 |

### create_activation

從核准的體驗和驗證的目標發佈即時、單一影像廣告。

| 參數 | 必要 | 說明 |
|---|---|---|
| `platform` | 是 | `META`、`LINKEDIN`或`GOOGLECM360`。 |
| `targetId` | 是 | 由`configure_activation_target`傳回的已驗證目標。 |
| `experienceId` | 是 | `list_experiences`傳回已核准的體驗識別碼。 |
| `assetId` | 無 | 具有多個合格變體的體驗的變體識別碼。 |
| `name` | 無 | 廣告位置顯示名稱。 |

呼叫`create_activation`兩次會建立兩個個別的廣告，而非更新第一個廣告。

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
- **檢閱轉換量度：**&#x200B;呼叫`get_insights_custom_metrics`，然後使用傳回的量度識別碼呼叫`get_insights_conversion_metrics`。
- **將建議轉換為草稿：**&#x200B;呼叫`get_insights_recommendations`，然後呼叫`create_draft_from_recommendation`。
- **從範本建置：**&#x200B;呼叫`list_express_templates`、`describe_express_template`和`list_cta_options`，然後呼叫`create_draft`。
- **發佈核准的體驗：**&#x200B;呼叫`list_experiences`，然後呼叫`configure_activation_target`和`create_activation`。

## 相關功能

- [AI助理概述](overview.md)
- [連線AI助理](connect-ai-assistants.md)
- [使用AI助理](use-ai-assistants.md)
