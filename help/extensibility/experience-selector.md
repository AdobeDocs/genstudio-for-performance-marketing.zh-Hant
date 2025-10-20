---
title: GenStudio Experience Selector MFE
description: 瞭解如何為您的GenStudio應用程式和附加元件實作Experience Selector Micro FrontEnd。
feature: Extensibility, Extensions, Experiences
source-git-commit: 2d6453274d1bfeb35df2821e7e31eec1ca87b013
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 6%

---

# GenStudio Experience Selector MFE

Experience Selector是Micro Frontend (MFE)，提供用於選取GenStudio體驗的`ExperienceSelectorDialog`元件。 從獨立的JavaScript套件組合匯入`renderExperienceSelectorWithSUSI`函式，在您的應用程式中使用元件，這會自動載入最新部署的Micro Frontend，並顯示一個天然元件介面。

GenStudio Experience Selector MFE允許使用者：

- 瀏覽並選取GenStudio體驗
- 依各種條件篩選體驗
- 支援單一和多重選取模式
- 透過SUSI （註冊登入）整合處理驗證
- 在不同的架構中提供一致的UI

## 整合選項

可使用兩種不同方法來整合MFE：

### ESM （ES模組） — 建議

```javascript
import { renderExperienceSelectorWithSUSI } from 'https://experience.adobe.com/solutions/GenStudio-experience-selector-mfe/static-assets/resources/@genstudio/experience-selector/esm/standalone.js';
```

### UMD （通用模組定義）

```html
<script src="https://experience.adobe.com/solutions/GenStudio-experience-selector-mfe/static-assets/resources/@genstudio/experience-selector/umd/standalone.js"></script>
```

## 設定屬性

`renderExperienceSelectorWithSUSI`函式接受具有下列屬性的組態物件：

| 屬性 | 類型 | 必要 | 說明 |
|----------|------|----------|-------------|
| `apiKey` | 字串 | 是 | GenStudio服務的API金鑰 |
| `imsOrg` | 字串 | 是 | IMS組織ID |
| `env` | 字串 | 是 | 環境(`stage`， `prod`) |
| `susiConfig` | 物件 | 是 | [SUSI驗證組態](#susi-configuration) |
| `onSelectionConfirmed` | 函式 | 是 | 確認選取時回撥 |
| `onDismiss` | 函式 | 是 | 對話方塊關閉時回呼 |
| `locale` | 字串 | 否 | 語言地區設定（例如，`en-US`） |
| `isOpen` | 布林值 | 否 | 初始對話方塊狀態 |
| `selectionType` | 字串 | 否 | 選擇模式（`single`或`multiple`） |
| `customFilters` | 陣列 | 否 | 自訂篩選條件 |
| `dialogTitle` | 字串 | 否 | 自訂對話方塊標題 |

### SUSI設定

`susiConfig`物件可能包括：

```javascript
{
  clientId: 'genstudio',
  environment: 'stg1', // or 'prod'
  scope: 'additional_info.projectedProductContext,additional_info.ownerOrg,AdobeID,openid,session,read_organizations,ab.manage',
  locale: 'en_US',
  modalSettings: {
    width: 500,
    height: 700
  }
}
```

## 快速入門

1. **從下列可用範例中選擇您的架構**
1. **瀏覽至範例目錄**
1. **安裝相依性** （適用於React/Vue範例）
1. **使用您的API金鑰和IMS組織更新設定**：

   ```javascript
   const experienceSelectorProps = {
     locale: 'en-US',
     apiKey: 'exc_app',           
     imsOrg: 'your-ims-org@AdobeOrg',  // Replace with your IMS Org
     env: 'stage', // or 'prod'
     susiConfig: {
        clientId: 'genstudio',
        environment: 'stg1', // or 'prod'
        scope: 'additional_info.projectedProductContext,additional_info.ownerOrg,AdobeID,openid,session,read_organizations,ab.manage',
        locale: 'en_US',
        modalSettings: {
          width: 500,
          height: 700,
        },
     },
     customFilters: ['genstudio-channel:email'],
     selectionType: 'single', // or 'multiple'
     dialogTitle: 'Select Email Templates'
   };
   ```

1. **執行開發伺服器**

### 實作範例

此存放庫包含不同架構的工作範例：

- [一個&#x200B;**完整的React應用程式**，展示與Vite組建系統](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/react-js)的整合。

- [具有組合API整合的&#x200B;**Vue 3應用程式**](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vue-js)。

- [兩個&#x200B;**Vanilla JavaScript實作**](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vanilla-js)：

   - [此&#x200B;**Vanilla ESM**&#x200B;版本使用ES6模組和現代JavaScript](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vanilla-js/vanilla-esm)。

   - [此&#x200B;**Vanilla UMD**&#x200B;版本使用透過指令碼標籤](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vanilla-js/vanilla-umd-global-var)載入的UMD組合。

## 驗證流程

Experience Selector會透過SUSI自動處理驗證：

1. 對話方塊開啟時，會檢查是否有現有的驗證。
1. 如果未驗證，則會開啟SUSI登入流程。
1. 成功驗證後，體驗選擇器會顯示。
1. 使用者可以瀏覽及選取體驗。
1. 選取的體驗會透過`onSelectionConfirmed`回呼傳回。
