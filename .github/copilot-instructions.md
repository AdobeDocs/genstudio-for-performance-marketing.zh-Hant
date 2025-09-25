---
source-git-commit: 8ed1e6853c9f844c72431dc692b556ece9c215a8
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---
## 用途

協助AI編碼助理對GenStudio for Performance Marketing檔案存放庫進行安全的小幅編輯。

## 高階架構（簡短）
- 此存放庫是檔案網站，由`help/`底下的Markdown所組成，`help/_includes/`底下的共用包含專案和`help/_includes/assets/`底下的組織影像。
- 發行說明、使用手冊及擴充性內容都在`help/`下提供。 大型內容變更應保留前置內容和現有標題結構。
- 此網站是使用Jekyll建立並託管在GitHub頁面上。 建置程式使用標準Jekyll慣例與一些自訂外掛程式。

## 專案特定慣例
- 游標規則：自訂自動化和指引存在於`.cursor/rules/*.mdc`中。 範例： `.cursor/rules/docs-lint.mdc` （lint程式）、`.cursor/rules/generate-release-notes.mdc` （發行說明格式）。 請遵循這些步驟以自動執行工作。
- 檔案名稱和前置內容：
   - 發行說明需要特定的frontmatter （請參閱`.cursor/rules/generate-release-notes.mdc`）。
   - 規則檔和`.mdc`副檔名使用索引鍵大小寫。
- 格式慣例：檔案使用GitHub風格的Markdown。 標題通常遵循句子大小寫和簡短段落。 偏好使用`*`專案符號來取得發行說明中的清單，偏好使用`###`專案符號來取得功能區段。

## 說明檔案風格指南
- 如需技術檔案最佳實務，請遵循[Microsoft撰寫風格指南](https://learn.microsoft.com/en-us/style-guide/)：
   - 撰寫以使用者動作為中心的簡潔明瞭的句子
   - 使用主動語態和現在時態
   - 將文字分成短的、可掃描的區塊
   - 保持溫暖的直接語調，同時保持技術準確性
- Markdown製作：
   - 標題使用句子大小寫（僅第一字大寫）
   - 將段落保持簡短（2-3個句子）以提高可讀性
   - 在標題和清單前後新增空白行
   - 對UI元素、檔案路徑和程式碼使用反引號
   - 包含所有影像的替代文字
   - 使用描述性文字連結至特定區段

## 編輯的安全性規則（AI應該做什麼）
- 切勿將Jira ID、內部連結或僅限公司的參照新增至公開檔案。 請參閱`generate-release-notes.mdc`「問題追蹤」區段。
- 編輯包含前端YAML的檔案時，請完全保留前端YAML。 許多範本和發行說明都依賴固定索引鍵（標題、說明、角色、exl-id）。
- 對於Lint修正，偏好從`.cursor/rules/docs-lint.mdc`自動的等冪編輯（移除尾端空格，確保最後是新行）。 人類使用的命令範例：

```sh
sed -i '' 's/ $//' <file>
sed -i '' '$ { /^$/d; }' <file> && echo "" >> <file>
```

## 範例（變更專案及方式）
- 小復本修正：更新`help/` Markdown檔案中的文字，保持標題和錨點不變。
- 影像更新： `help/_includes/assets/`下的參考影像。 請勿在未更新所有參照的情況下移動或重新命名影像。

## 首先要看的位置
- `help/_includes/` — 共用的片段和影像。
- `.cursor/rules/` — 自動化和連結指引；使用這些作為格式化和程式的權威規則。
- `markdownlint_custom.json` — 本機markdownlint覆寫。
- `.github/pull_request_template.md` — PR期望。

## 何時詢問人員
- 如果變更需要執行或修改基於Docker的工具（lint規則提及Docker）或影響站點構建管道。
- 如果檔案參考未知的外部設定（例如`markdownlint.json`遺失） — 詢問是否要建立或忽略。

## 最簡單的人類命令

```sh
# Install linter (if not present)
npm install -g markdownlint-cli

# Run lint locally using project config
markdownlint --config markdownlint_custom.json "help/**/*.md"

# Project lint via yarn (preferred if available in environment)
yarn lint
```

---
如果您想要的話，我可以將此合併到存放庫中的`.github/copilot-instructions.md`中（或調整用詞/長度）。 我應該變更或新增哪些專案？
