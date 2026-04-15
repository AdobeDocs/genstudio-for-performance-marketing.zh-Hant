---
name: generate-release-notes
description: ""
source-git-commit: 1a33b08048233c5f9a82b5f428082aa5c71b0052
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---


# 產生GenStudio發行說明

**標準目標檔案：** [help/user-guide/release-notes.md](help/user-guide/release-notes.md)

**完整範例：** [範例.md](examples.md)

**KT/wiki欄位對應和檔案路徑：** [reference.md](reference.md)

## 工作流程檢查清單

以此順序工作。 複製檢查清單並追蹤多步驟編輯的進度。

1. [ ]開啟`help/user-guide/release-notes.md`並讀取目前的`## YYYY.MM {#latest}`區塊和&#x200B;**舊版發行說明**&#x200B;區域。
2. [ ]如果新增&#x200B;**新的**&#x200B;每月發行：封存目前的最新版本（請參閱[封存先前的最新](#archive-previous-latest)）。
3. [ ]新增或編輯前`## YYYY.MM {#latest}`個區段（最新月份在發行清單頂端）。
4. [ ]針對每個專案，套用[決定規則](#decision-rules) （功能`###`與&#x200B;**修正和增強功能**、Beta徽章或不是）。
5. [ ]新增或驗證最相關片語的檔案連結（請參閱[reference.md](reference.md#documentation-linking)）。
6. [ ]在完成前執行[品質檢查](#quality-checks)。
7. [ ]在頁面上保留[frontmatter](reference.md#frontmatter)，除非工作明確更新中繼資料。

## 決定規則

使用這些if/then規則，讓內容登陸正確的位置：

| 若 | 則 |
|----|------|
| Beta提供全新功能 | 在`###`標題下方直接新增Beta徽章行（請參閱[examples.md](examples.md)）。 |
| Source資料明確標示專案為&#x200B;**fix**&#x200B;或&#x200B;**增強功能** | 只用`*`專案符號放在`### Fixes and enhancements`下面。 |
| 該專案是全新功能或功能劇本 | 使用包含1-3個句子的`###`功能區段（不是修正清單）。 |
| 您不確定某件事是修正還是特徵 | 預設為`###`功能區段，除非來源明確指出修正/增強功能。 |

**修正區段規則：**&#x200B;請勿將專案符號新增至&#x200B;**修正和增強功能**，除非來源明確標示為修正或增強功能。

## 封存上一個最新的

匯入新`## YYYY.MM {#latest}`時：

1. 剪下整個`## YYYY.MM {#latest}`區段（從標題到發行內容結尾，在下一個`##`或&#x200B;**舊版發行說明**&#x200B;之前）。
2. 將其貼到可收合區塊內的&#x200B;**舊版發行說明**&#x200B;中。
3. 將舊標題取代為： `+++Notes from YYYY.MM.DD+++` （使用實際的發行日期；如檔案中現有附註的格式）。
4. 從封存的標題中移除`{#latest}`；新的頂端區段是唯一具有`{#latest}`的區段。
5. 在&#x200B;**舊版發行說明**&#x200B;內保持時間順序（除非檔案已使用不同的順序 — **符合現有的檔案**，否則最新的封存區塊會朝頂端對齊）。

## 必要的結構

### 頁面標題和簡介

在frontmatter之後，使用：

```markdown
# GenStudio for Performance Marketing release notes

This release information details the latest updates to the GenStudio for Performance Marketing application.
```

如果檔案已使用稍微不同的介紹句子（例如「提供」而非「詳細資訊」），請和頁面的其餘部分保持一致。

### 最新發行標題

- 格式：最新發行區塊的`## YYYY.MM {#latest}`。
- 頁面上只有一個`{#latest}`錨點。

### 功能區段

- 主要功能類別請使用`###`。
- 呈現時態，1-3個句子，清楚什麼/為什麼，以及有幫助的使用者動作。
- 產品名稱： `[!DNL Create]`、`[!DNL Content]`、`[!DNL Insights]`等
- UI： `[!UICONTROL Control Name]`適當時。
- 強調： UI區域/區段為`_italics_`；關鍵詞請謹慎使用`**bold**`。

### Beta徽章

完全使用：

```markdown
[!BADGE Beta]{type=Informative tooltip="This feature is currently in Beta, so some functionality may be limited or subject to change."}
```

### 檔案連結

- 模式： `[link text](/help/user-guide/section/page.md#anchor)`
- 偏好錨點；連結使用者關心的片語，而不是「按一下這裡」。

### 修正和增強功能

- 專案符號行使用`*`。
- 僅限在原始材料中明確標示為修復/增強的專案。
- 與功能相同的連結和術語慣例。

## 禁止的內容

- **不**&#x200B;在發佈的發行說明中包含Jira金鑰、內部問題編號、僅限內部的URL或公司Wiki連結。
- 請&#x200B;**不**&#x200B;引用知識轉移檔案、票證或內部工具作為證明 — 僅摘要使用者面對的結果。
- 請&#x200B;**不**&#x200B;在多個區段上複製`{#latest}`。

## 品質檢查

完成工作之前：

- [ ]所有新連結或已變更的相對連結儘可能解析為`help/`下的真實路徑。
- [ ]個Beta功能包含必要的Beta徽章片段。
- [ ]術語符合現有的版本注意事項(`[!DNL …]`， `[!UICONTROL …]`)。
- [ ]掃描草稿是否有意外的內部ID (`[A-Z]+-\d+`)、Wiki URL或「參閱Jira」語言；請移除它們。
- [ ] **修正和增強功能**&#x200B;僅包含明確標籤的修正/增強功能。
- [ ]新增新月份時，上一個最新區段已正確封存。

## 內容來源（摘要）

從內部提取知識轉移檔案或發行Wiki時，依照[reference.md](reference.md#internal-sources-kt-and-release-wikis)中的說明對應欄位。 出貨頁面必須讀取為獨立使用者檔案。

## 可選：拋光新子區段

在`{#latest}`下新增新的`###`內容後，針對複製編輯器式的傳遞執行[Polish發行說明](../polish-release-notes/SKILL.md) （權益轉寄語氣，每個段落&#x200B;**2-3個句子**，沒有程式說明） **僅限**&#x200B;這些&#x200B;**新**&#x200B;子區段 — **非**&#x200B;舊版發行說明或預先存在的文字，除非明確要求。

## 其他資源

- [examples.md](examples.md) — 可貼上的範例（功能、修正、封存區塊）。
- [reference.md](reference.md) — frontmatter附註、檔案路徑、連結策略。
- [波蘭文發行說明](../polish-release-notes/SKILL.md) — 在`{#latest}`下新增`###`的可選編輯傳遞。
