---
source-git-commit: c3c6aa86f4f520d020f8928612d1be6be1599652
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 3%

---
# 參考：沖銷核發來源(MCP)

## 儀式頁面探索

| 模式 | 範例 |
|---------|---------|
| 標題 | **GenStudio**&#x200B;空間中的`YYYY/MM Release Ceremony` |
| 從Jira | 票證`description`中的Wiki連結（偏好設定） |
| CQL遞補 | `title ~ "2026/06 Release Ceremony" AND space = GenStudio` |

## 儀式功能群組

發行儀式Wiki最多包含&#x200B;**兩個**&#x200B;功能表格。 從&#x200B;**儲存** HTML剖析兩者。

### GA版本功能

- 章節標題： `GA Release Features` (`<h2>`)
- 子標題： `Feature Group:`含選擇性Floodgate連結
- 資料表資料行包含&#x200B;**型別** （`GA`、`Limited`、`EA`、`Beta`或空白）
- **KT檔案**&#x200B;欄： `<ac:link><ri:page ri:content-title="..."/></ac:link>`

每列擷取：

| 欄位 | 來源 |
|-------|--------|
| `featureDescription` | 資料列中的前`<td>` |
| `type` | 輸入欄儲存格文字 |
| `ktPageTitle` | KT欄中的`ri:content-title` |
| `jiraKeys` | `ac:macro ac:name="jira"` → `key`引數（僅限內部） |
| `releaseTier` | 當Type為`GA`時`ga`；繼承其他GA資料表值的型別 |

### Beta版本功能

- 章節標題： `Beta Release Features` （某些月份可能有&#x200B;**個缺席**）
- 第二個資料表；**no型別資料行** — 每一列都是Beta
- 與GA表格相同的KT和Jira擷取
- 在每個Beta區段列上設定`releaseTier: beta`和`requiresBetaBadge: true`

如果缺少Beta區段，請記錄零Beta列並繼續。

### 儲存HTML模式

```html
<ac:link><ri:page ri:content-title="Translation on HZ Canvas" /></ac:link>
<ac:structured-macro ac:name="jira" ...><ac:parameter ac:name="key">GS-23218</ac:parameter></ac:structured-macro>
```

## MCP工具用途

| 步驟 | 工具 | 參數 |
|------|------|------------|
| 票證 | `jira_getIssue` | `issueKey`，選擇性`expand: renderedFields` |
| 儀式 | `confluence_getContent` | `contentId`, `bodyMode: storage` |
| KT查閱 | `confluence_searchContent` | `cql: title = "<KT title>" AND space = GenStudio` |
| KT內文 | `confluence_getContent` | `contentId`, `bodyMode: text`, `maxBodyChars: 50000` |

剖析KT連結時，**不要**&#x200B;使用`bodyMode: text`作為儀式頁面。

## KT欄位對應（繪圖輸入）

對應至generate-release-notes；請勿逐字貼至public release notes。

| KT區段 | 使用 |
|------------|-----|
| 說明 | 核心功能 |
| 電梯間推介 | 價值主張 |
| 已提供的功能 | 具體行為 |
| 問題陳述 | 使用者問題（僅限內容） |
| 發行型別和日期 | GA / Beta /有限（內部）；磁碟機徽章決定 |

## 包含篩選器

不明時，向使用者確認範圍。 常見預設集：

| 預設集 | 包含 |
|--------|----------|
| `ga_only` | 型別= `GA`的GA表格列 |
| `ga_and_beta` | **未來月份的建議預設值** — 型別= `GA` **加上所有** Beta發行功能表格列的GA列 |
| `ga_plus_empty` | GA資料表：型別= `GA`或空白型別 |
| `all_except_pilot` | 使用`ga_and_beta`時，除了`Limited`以外的GA表格列；加上Beta區段 |
| `all_with_badges` | 所有GA表格列；Beta區段列一律會取得Beta徽章 |

## Beta徽章移交

| 條件 | `requiresBetaBadge` |
|-----------|---------------------|
| 來自&#x200B;**Beta發行功能**&#x200B;表格的資料列 | `true` |
| 型別= `Beta`的GA資料表列 | `true` |
| 型別= `GA`的GA資料表列 | `false` |

下游： [產生發行說明決定規則](../generate-release-notes/SKILL.md#decision-rules)和[Beta徽章片段](../generate-release-notes/SKILL.md#beta-badge)。

## 移交裝載（非正式）

傳遞以產生專案清單的發行說明：

```yaml
- featureDescription: "YouTube Shorts"
  releaseTier: ga
  requiresBetaBadge: false
  ktPageTitle: "YouTube Shorts (Create + Activate)"
  # extracted KT fields: description, elevatorPitch, featuresDelivered, ...
```
