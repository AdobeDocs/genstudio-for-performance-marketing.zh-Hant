---
name: consume-release-sources
description: ""
source-git-commit: c3c6aa86f4f520d020f8928612d1be6be1599652
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 1%

---


# 沖銷核發來源(Jira + Confluence MCP)

**下游草擬：** [產生發行說明](../generate-release-notes/SKILL.md) →選用的[波蘭發行說明](../polish-release-notes/SKILL.md)

**剖析參考：** [reference.md](reference.md)

**目標輸出檔案（僅限下游）：** [help/user-guide/release-notes.md](../../help/user-guide/release-notes.md)

## 先決條件

- **Jira MCP** (`jira_getIssue`， `jira_searchIssues`)已驗證
- **Confluence MCP** (`confluence_getContent`， `confluence_searchContent`)已驗證
- 來自分支名稱(`GS-#####`)、使用者輸入或票證說明的Jira票證金鑰

## 工作流程檢查清單

1. [ ] **解析Jira票證** — `jira_getIssue`與`issueKey`。 閱讀儀式wiki連結和發行月的`description`。
2. [ ] **尋找儀式頁面** — 使用票證中的Wiki URL；備援CQL： `title ~ "YYYY/MM Release Ceremony" AND space = GenStudio`。
3. [ ] **擷取儀式內文** — `confluence_getContent`具有`bodyMode: storage` （必要；`text`遺失KT連結和資料表結構）。
4. [ ] **剖析功能群組** — 從&#x200B;**GA發行功能**&#x200B;和&#x200B;**Beta發行功能**&#x200B;擷取資料列（請參閱[reference.md](reference.md#ceremony-feature-groups)）。
5. [ ] **套用包含篩選器** — 每個使用者範圍（請參閱[reference.md](reference.md#inclusion-filters)）；確認Beta列計數（可能為零）。
6. [ ] **解析KT頁面** — 每個KT標題`confluence_searchContent`；使用`bodyMode: text`的`confluence_getContent`。
7. [ ] **擷取KT欄位** — 說明、電梯間推介、已傳遞的功能、問題陳述、發行型別和日期。
8. [ ] **設定Beta旗標** — `requiresBetaBadge: true`，適用於Beta區段列或型別為`Beta`的GA表格列。
9. [ ] **將**&#x200B;交給[產生發行說明](../generate-release-notes/SKILL.md)，並包含結構化資料列清單（已寄出的副本中沒有wiki/Jira參照）。

## Beta標籤（移交以產生技能）

當`requiresBetaBadge: true`時，下游`###`區段必須立即包含在標題下：

```markdown
[!BADGE Beta]{type=Informative tooltip="This feature is currently in Beta, so some functionality may be limited or subject to change."}
```

請勿為Beta新增斜體排程免責宣告；徽章是支援的模式。

## 已出貨版本注意事項中禁止使用

內部ID、Wiki URL、KT引文和Jira金鑰只會保留在此擷取階段。 根據[產生發行說明禁止的內容](../generate-release-notes/SKILL.md#prohibited-content)，在公開頁面中摘要使用者面對的結果。

## 遞補

如果MCP呼叫失敗，請要求使用者貼上儀式和KT內容，然後使用[reference.md KT欄位對應](../generate-release-notes/reference.md#internal-sources-kt-and-release-wikis)繼續產生發行說明。

## 其他資源

- [reference.md](reference.md) — 儀式剖析、CQL、包含篩選器、MCP引數
- [generate-release-notes](../generate-release-notes/SKILL.md) — 封存、草稿、連結、品質檢查
- [polish-release-notes](../polish-release-notes/SKILL.md) — editorial在`{#latest}`下傳遞新的`###`
