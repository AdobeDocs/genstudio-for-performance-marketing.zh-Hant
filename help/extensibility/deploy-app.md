---
title: 部署您的App Builder應用程式
description: 部署適用於GenStudio for Performance Marketing的App Builder應用程式或附加元件。
feature: Extensibility
exl-id: 51888ab7-7772-4ac8-838d-26db3019e9b0
TQID: https://experienceleague.adobe.com/7Z4Fb-jPi4FHrTeOgHxxO4fl982sqri-7uEDoylFF-s
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: ad3738c7-91ac-48ed-a914-fd0b03f89396id: bfaa655b-e017-428d-80d0-09de2183b296id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: da3860b0-d637-47df-bef0-273751180266
source-git-commit: ca8bfb11a301697c92e97bad41ea3ba8aa359847
workflow-type: tm+mt
source-wordcount: 622
ht-degree: 0%

---

# 部署您的應用程式

執行應用程式可提供附加元件在部署前的初步行為快照。 這有助於偵錯。

## 執行應用程式

在`https://localhost:9080`中執行應用程式：

```bash
aio app run
```

## 部署應用程式

1. 導覽至您的部署工作區：

   ```bash
   aio app use -w [deployment_workspace]
   ```

2. 部署應用程式：

   ```bash
   aio app deploy
   ```

## 強制重新部署

您可以強制建立及部署應用程式，而不需重新提交以進行核准。

>[!NOTE]
>
>強制建置和部署會覆寫您現有的部署。 **請先在測試環境中完整測試您的應用程式**。

```bash
aio app build --force-build
```

```bash
aio app deploy --force-deploy
```

## 同時建置和部署

```bash
aio app deploy --force-build --force-deploy
```

## 尋找您的新應用程式

部署後，您可以在GenStudio for Performance Marketing中檢視新的應用程式。

### 使用URL檢視

將`query`引數新增至GenStudio for Performance Marketing URL以檢視新應用程式：

```txt
https://experience.adobe.com/?ext=https://<my-deployed-add-on>.adobeio-static.net/index.html#/@<ims-org>/genstudio/create
```

### 在使用者介面中檢視

根據您部署的擴充功能型別，可在UI中的不同位置找到新擴充功能。 目前可用的擴充功能點包括：

* 合規性擴充功能，包括：
   * [*提示延伸點*](#find-prompt-extensions)，可讓客戶新增其他內容至LLM產生，以及
   * [*驗證延伸點*](#find-validation-extensions)，可讓客戶驗證LLM產生的內容。 驗證通常會與「提示」延伸功能搭配使用，以確保以延伸提示產生的內容符合客戶要求（例如，醫療藥品索賠或法律）
* [數位資產管理(DAM)擴充功能](#find-dam-extensions)
* [範本副檔名](#find-template-extensions)
* [翻譯擴充功能](#find-translation-extensions)
* [內容片段延伸](#find-content-fragment-extension)

### 尋找提示副檔名

在範本的&#x200B;**引數區段**&#x200B;的&#x200B;**附加元件**&#x200B;下拉式清單中找到提示副檔名。

![提示副檔名](./select-prompt-ext.png){width="600" zoomable="yes"}

附加元件對話方塊將會開啟，讓您選取要為LLM產生新增的其他前後關聯。

![提示延伸功能下拉式清單](./select-prompt-dropdown.png){width="600" zoomable="yes"}

### 尋找驗證擴充功能

產生提示後，可在與結果一起顯示的右側找到驗證延伸模組。

![驗證延伸模組](./validation-ext.png){width="600" zoomable="yes"}

執行您選取的擴充功能以驗證產生的內容。

![有效驗證](./validation-valid.png){width="600" zoomable="yes"}

發生錯誤時，您可以使用擴充功能以程式設計方式更新體驗副本。 按一下「**[!UICONTROL 複製]**」按鈕會將建議的文字複製到剪貼簿。 按一下&#x200B;**[!UICONTROL 套用]**&#x200B;按鈕會將文字套用至所產生體驗中的特定文字方塊。

![顯示複製和套用按鈕的驗證錯誤](./validation-copy-apply.png){width="600" zoomable="yes"}

### 尋找DAM擴充功能

在範本的&#x200B;**引數區段**&#x200B;中選取內容時，找到數位資產管理(DAM)擴充功能。 檢視&#x200B;**選取位置**&#x200B;下拉式清單的底部以檢視任何附加元件。

![DAM延伸模組](./dam-ext.png){width="600" zoomable="yes"}

### 尋找範本擴充功能

選取範本時，可在&#x200B;**外部範本應用程式**&#x200B;索引標籤中找到範本擴充功能。 只有在有可選取的範本應用程式時，才會顯示此索引標籤。

![範本延伸模組](./template-ext.png){width="600" zoomable="yes"}

### 尋找翻譯擴充功能

使用翻譯擴充功能點，透過Proxy提供您自己的翻譯服務，而不使用GenStudio預設翻譯。
這些擴充功能沒有使用者介面位置。

如果已註冊擴充功能，則會使用提供的翻譯服務。 否則會使用預設的GenStudio翻譯服務。

### 尋找內容片段延伸模組

[!DNL GenStudio for Performance Marketing]中的內容片段延伸以來自連線第三方(3P)存放庫的專案，取代[!DNL Create]畫布上產生的電子郵件體驗中的文字。 設定並部署擴充功能後，您無需離開工作流程即可從畫布交換副本。

>[!NOTE]
>
>內容片段延伸功能交換現在可用於畫布上的&#x200B;**電子郵件**&#x200B;體驗。 即將提供&#x200B;**Horizon**&#x200B;管道支援。

**若要使用內容片段延伸**&#x200B;交換文字：

1. 在畫布上，按一下所產生電子郵件變體中的可編輯文字欄位。
1. 按一下&#x200B;**[!UICONTROL 交換]**。
   ![交換文字](./subject-line-swap.png){width="400" zoomable="yes"}
1. 選取您的第三方存放庫。 您的組織可以控制要顯示哪些存放庫以及存放庫UI的行為。
1. 選取要用來取代欄位文字的索賠。

如果您對您的附加元件感到滿意，您就可以不使用`query`引數來分配它。

您現在可以[散發您的應用程式](distribute-app.md)。
