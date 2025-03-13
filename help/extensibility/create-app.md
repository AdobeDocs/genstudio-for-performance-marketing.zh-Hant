---
title: 建立App Builder應用程式以擴充GenStudio for Performance Marketing
description: 開始建立應用程式或附加元件。
source-git-commit: cd53f566981a005b24ef1f1951aa2e55c6dd46c1
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 0%

---

# 開發App Builder應用程式

擴充GenStudio for Performance Marketing原生功能的開發人員使用[Adobe App Builder](https://developer.adobe.com/app-builder/)來建立、提交及部署其可擴充的應用程式或附加元件。

>[!BEGINSHADEBOX]

**必要條件**：

* Node.js （20.x版或更新版本）

* npm （與Node.js封裝）

* Adobe Developer命令列介面(CLI)。 若要安裝： `npm install -g @adobe/aio-cli`

>[!ENDSHADEBOX]

## 應用程式結構

GenStudio for Performance Marketing附加元件是App Builder應用程式，包含與其他App Builder應用程式相同的基本元件。

### 建置和組態檔

App Builder應用程式的關鍵元件包括這些組建和設定檔案。 此清單未包含所有組建和組態檔。

* `README.md`：包含應用程式的一般資訊。

* TS應用程式檔案：

   * `package.json`
   * `package-lock.json`
   * `eslint`
   * `tsconfig`
   * `jest test up`

* App Builder設定檔案：

   * `app.config.yaml`
   * `ext.config.yaml`：附加元件的組態檔
   * `app.config.yaml`：附加元件的設定檔(包括將您的應用程式定義為GenStudio for Performance Marketing附加元件)
   * `.aio`
   * `.env`：不要將`.env`檔案認可到原始檔控制

### Source程式碼

```
- src/
    - genstudiopem/
        - web-src/
            - src/
                - components/
                - utils/
                - Constants.ts
                - index.tsx
                - index.css
                - utils.ts
        - index.html
```

### Source程式碼元件

* `ExtensionRegistration.tsx`：定義主機應用程式(GenStudio for Performance Marketing)需要載入及顯示附加元件的必要API。

* `App.tsx`：定義路由傳送至其他元件的主要應用程式元件。

* `AdditionalContextDialog.tsx`：用於顯示其他內容附加元件的對話方塊元件。

* `RightPanel.tsx`：驗證附加元件的對話方塊元件。

* `Helper`元件：包含`ClaimsChecker`。

## 從現有應用程式建立App Builder應用程式

您可以使用範例應用程式來開始建立附加元件。

**若要從現有應用程式建立App Builder應用程式**：

1. 從[GenStudio UIX範例](https://github.com/adobe/genstudio-uix-examples)存放庫下載範例應用程式。

1. 從[Adobe Developer Console](https://developer.adobe.com/console/)上的App Builder專案工作區中，選取「**[!UICONTROL 全部下載]**」以下載專案詳細資料。

1. 在您偏好的整合式開發環境(IDE)中，在本機開啟範例應用程式。

1. 使用Adobe Developer命令列介面進行驗證：

   ```bash
   aio login
   ```

1. 下載您的JSON檔案，然後建立您的應用程式：

   ```bash
   aio app use '/path/to/your/downloaded/app-builder/project/details/config.json'
   ```

## 新增自訂程式碼到您的附加元件

您在`AdditionalContextDialog.tsx`和`RightPanel.tsx`檔案中定義您的附加元件程式碼。 這兩個檔案定義使用者存取附加元件時的快顯視窗外觀和行為。

* `AdditionalContextDialog.tsx`：如果您打算使用&#x200B;_新增內容_&#x200B;附加元件，請定義此元件。 使用者在[!DNL Create]的提示抽屜中按一下&#x200B;_附加元件_&#x200B;時，與此元件互動。

* `RightPanel.tsx`：如果您打算使用&#x200B;_Right Panel_&#x200B;附加元件（體驗驗證），請定義此元件。 使用者在[!DNL Create]體驗草稿中按一下右側面板中的驗證附加元件，與此元件互動。

您現在已準備好[部署您的應用程式](deploy-app.md)

## 應用程式開發的最佳作法

維護開發環境可協助您避免應用程式開發和部署錯誤：

* 如果您使用舊版範例應用程式，請重新安裝以升級相依性：

  ```bash
  rm -rf node_modules package-lock.json && npm i
  ```

* 升級GenStudio UIX SDK。 確認您使用的是最新版本的[GenStudio UIX SDK](https://github.com/adobe/genstudio-uix-sdk)。 請參閱[GenStudio UIX範例存放庫](https://github.com/adobe/genstudio-uix-examples)以瞭解如何使用最新的SDK變更。
