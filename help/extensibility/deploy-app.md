---
title: 部署您的App Builder應用程式
description: 部署適用於GenStudio for Performance Marketing的App Builder應用程式或附加元件。
feature: Extensibility
exl-id: 51888ab7-7772-4ac8-838d-26db3019e9b0
source-git-commit: 52e8e078bc013fe686b5cc2105089f7098cce575
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---

# 部署您的應用程式

執行應用程式可提供附加元件行為的初步快照，然後再進行部署。 此資訊可促進偵錯。 您可以強制建置和部署已部署的應用程式，而不需重新提交以進行核准。


**若要執行應用程式**：

在`https://localhost:9080`中執行應用程式：

```bash
aio app run
```

**若要部署應用程式**：

1. 導覽至您的部署工作區。 例如，若要導覽至生產工作區：

   ```bash
   aio app use -w Production
   ```

1. 部署應用程式：

   ```bash
   aio app deploy
   ```

**強制重新部署**：

>[!NOTE]
>
>強制建置和部署會覆寫您現有的部署。 請先在測試環境中徹底測試您的應用程式。

```bash
aio app build --force-build
```

```bash
aio app deploy --force-deploy
```

**若要同時建置和部署**：

```bash
aio app deploy --force-build --force-deploy
```

**若要檢視應用程式**：

部署後，您可以在GenStudio for Performance Marketing中檢視應用程式，方法是將`query`引數新增至GenStudio for Performance Marketing URL：

`https://experience.adobe.com/?ext=https://<my-deployed-add-on>.adobeio-static.net/index.html#/@<ims-org>/genstudio/create`

如果您對您的附加元件感到滿意，您就可以不使用`query`引數來分配它。

您現在可以[散發您的應用程式](distribute-app.md)。
