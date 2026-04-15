---
source-git-commit: f6a305c6a4e700525b570bbe280e5d1049d06537
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 6%

---
# 參考資料：發行說明製作

## Frontmatter

即時頁面[help/user-guide/release-notes.md](../../help/user-guide/release-notes.md)包含超過最小集合的Experience League中繼資料（例如`TQID`、`product_v2`、`feature_v2`、分類識別碼）。

**規則：**

- 編輯發行說明&#x200B;**內文**&#x200B;內容時，**會保留現有的frontmatter**&#x200B;索引鍵和值，除非工作明確要求變更中繼資料。
- 請勿移除分類法或產品中繼資料以符合較短的範本。
- ExL頁面的必要概念通常包含`title`、`description`和`role`；請遵循[Experience League中繼資料指引](https://experienceleague.adobe.com/en/docs/authoring-guide/using/authoring/using-metadata)以取得新頁面。

## 內部來源（KT和發行Wiki）

僅於起草&#x200B;**時使用這些欄位**；已發佈的發行說明不得參考內部檔案。

### 知識轉移(KT)檔案

擷取自：

| 欄位 | 使用 |
|-------|-----|
| 說明 | 核心功能說明 |
| 電梯間推介 | 價值主張 |
| 已提供的功能 | 具體行為 |
| 問題陳述 | 使用者痛點 |
| 發行型別和日期 | 定時 |

### 發行Wiki頁面

分組和範圍依據：

| 欄位 | 使用 |
|-------|-----|
| 發行日期（修正版本） | 相同日期→相同發行說明批次 |
| 行動方案 | 僅限內容；請勿在公開文字中於內部連結 |
| PM會使用KT呈現功能 | 代表可能存在更深入的KT細節 |

**範圍規則：**&#x200B;共用相同發行日期（修正版本）的專案屬於相同的每月發行區塊。

## 檔案連結

- 連結至&#x200B;**最相關的**&#x200B;片語（例如，將「不支援的影像和視訊資產」連結至廣告格式區段）。
- 偏好`#anchor`個連結放入右側子區段。
- 沒有更深入的錨點時，可使用概觀頁面。

## 通用檔案路徑

| 區域圖 | 路徑前置詞 |
|------|-------------|
| 建立 | `/help/user-guide/create/` |
| 內容 | `/help/user-guide/content/` |
| 啟用 | `/help/user-guide/activation/` |
| 核准 | `/help/user-guide/approvals/` |
| Insights | `/help/user-guide/insights/` |
| 准則 | `/help/user-guide/guidelines/` |
| 範本 | `/help/user-guide/templates/` |
| 行銷活動 | `/help/user-guide/campaigns/` |
| 擴展性 | `/help/extensibility/` |
