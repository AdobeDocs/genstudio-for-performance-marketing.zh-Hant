---
title: 適用於GenStudio的Marketo
description: 安裝和設定適用於GenStudio Adobe Exchange應用程式的Marketo ，讓您的組織可以在GenStudio for Performance Marketing中使用Marketo Engage範本。
feature: Extensibility
source-git-commit: 4118624b479905cd2f2193d542c000678daaf4b8
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 0%

---

# 適用於GenStudio的Marketo

在相同[!DNL IMS]組織中使用[!DNL Marketo Engage]和[!DNL GenStudio for Performance Marketing]的組織可以從[!DNL Adobe Exchange]安裝適用於GenStudio **應用程式的** Marketo。 系統管理員核准應用程式並完成部署後，作者可以在GenStudio中建立電子郵件體驗時，於直接上傳至[!DNL Content]的範本旁選擇Marketo範本。

此主題適用於安裝應用程式、從Marketo收集認證，以及在Exchange中部署應用程式的&#x200B;**管理員**。 如需AJO和Marketo範本語法如何搭配GenStudio使用的資訊，請參閱[AJO和Marketo的範本](/help/user-guide/templates/use-templates.md#templates-from-ajo-and-marketo)。

## 先決條件

* [!DNL Marketo Engage]必須在您部署擴充功能的組織中布建。
* 部署應用程式的使用者需要&#x200B;**Marketo認證**。 若要建立並擷取這些認證，您必須擁有&#x200B;**Marketo產品管理員**&#x200B;存取權（開啟Marketo時，**[!UICONTROL 管理員]**&#x200B;區域必須可用）。

## 從Adobe Exchange安裝應用程式

>[!VIDEO](https://video.tv.adobe.com/v/3483299?learn=on)

1. 開啟[Adobe Exchange](https://exchange.adobe.com)並移至&#x200B;**[!UICONTROL Experience Cloud]**。
1. 開啟GenStudio ](https://exchange.adobe.com/apps/ec/ab6p21vo8r/marketo-for-genstudio)適用的[Marketo清單。
   在Adobe Exchange](/help/extensibility/marketo-adobe-exchange.png){width="75%"}上列出適用於GenStudio的![Marketo
1. 選取&#x200B;**[!UICONTROL 免費]**&#x200B;為您的組織請求應用程式。
1. 在您的組織&#x200B;**稽核並核准**&#x200B;要求之後，請繼續[取得Marketo認證](#get-marketo-credentials)以及[從Exchange部署應用程式](#deploy-the-application-from-exchange)。

## 取得Marketo認證

您使用的是來自&#x200B;**Marketo**&#x200B;執行個體（而非Adobe Developer Console）的認證。 在Exchange中部署之前，請先收集下列專案。

### 建立僅限API的使用者（如果您重複使用現有的API使用者，則為選用）

1. 在Marketo中，移至&#x200B;**[!UICONTROL 管理員]**。
1. 在&#x200B;**[!UICONTROL 安全性]**&#x200B;底下，開啟&#x200B;**[!UICONTROL 使用者與角色]**。
1. 若是新的API使用者，請按一下&#x200B;**[!UICONTROL 僅建立API使用者]** （針對每個API使用者使用唯一的電子郵件）。 指派&#x200B;**[!UICONTROL API角色（所有工作區）]**&#x200B;角色（或貴組織所需的角色）。 如果您已有要使用的API使用者，請跳至[建立或選取LaunchPoint服務](#create-or-select-a-launchpoint-service)。

![僅API使用者與API角色的使用者與角色](/help/extensibility/marketo-users-roles-api-user.png){width="80%"}

### 建立或選取LaunchPoint服務

1. 在&#x200B;**[!UICONTROL Admin]**&#x200B;中，在&#x200B;**[!UICONTROL Integration]**&#x200B;下，開啟&#x200B;**[!UICONTROL LaunchPoint]**。
1. 按一下「建立&#x200B;****」以建立新服務（或使用現有的自訂服務）。
   ![LaunchPoint自訂服務](/help/extensibility/marketo-launchpoint-custom-service.png){width="80%"}
1. 針對您的服務，按一下&#x200B;**[!UICONTROL 檢視詳細資料]**&#x200B;並複製&#x200B;**[!UICONTROL 使用者端識別碼]**&#x200B;和&#x200B;**[!UICONTROL 使用者端密碼]**。 您將在Adobe Exchange **[!UICONTROL 設定]**&#x200B;中輸入這些專案。

### 記下您的Marketo REST API基底URL

1. 在&#x200B;**[!UICONTROL Admin]**&#x200B;中，在&#x200B;**[!UICONTROL 整合]**&#x200B;下，開啟&#x200B;**[!UICONTROL 網頁服務]**。
1. 尋找&#x200B;**[!UICONTROL REST API]**&#x200B;端點。 僅複製&#x200B;**基底URL** （主機），格式為`https://###-XXX-###.mktorest.com`。 請&#x200B;**不**&#x200B;包含路徑區段，例如`/rest`或`/identity`。 此值在每個Marketo例項中都是唯一的。

![網站服務REST API端點基底URL](/help/extensibility/marketo-web-services-rest-endpoint.png){width="80%"}

您也需要Exchange部署畫面要求的&#x200B;**[!UICONTROL Marketo Engage身分URL]**，以及REST基底URL和LaunchPoint的使用者端ID與使用者端密碼。

## 從Exchange部署應用程式

若要在GenStudio中使用此擴充功能，請從Adobe Exchange部署應用程式。

1. 返回[Adobe Exchange](https://exchange.adobe.com)。
1. 選取「**[!UICONTROL 管理]**」並開啟GenStudio適用的&#x200B;**Marketo**&#x200B;應用程式（例如在&#x200B;**[!UICONTROL App Builder應用程式]**&#x200B;或您組織的Managed App下）。
1. 在&#x200B;**[!UICONTROL 環境]**&#x200B;下，從下拉式清單中選擇現有環境，或選取&#x200B;**[!UICONTROL 新增環境]**&#x200B;以建立環境。
1. 開啟所選環境的&#x200B;**[!UICONTROL 組態]**。
1. 輸入來自[LaunchPoint](#create-or-select-a-launchpoint-service)的&#x200B;**[!UICONTROL 使用者端識別碼]**&#x200B;和&#x200B;**[!UICONTROL 使用者端密碼]**、**[!UICONTROL Marketo Engage身分URL]**&#x200B;以及&#x200B;**[!UICONTROL Marketo Engage REST API基底URL]** （來自[Web服務](#note-your-marketo-rest-api-base-url)的基底主機）。
1. 按一下&#x200B;**[!UICONTROL 部署]**。 部署成功時，動作會變更為&#x200B;**[!UICONTROL 取消部署]**。

### 更新設定

若要變更環境的設定值，請先取消部署&#x200B;****，更新欄位，然後再次&#x200B;**[!UICONTROL 部署]**。

## 存取GenStudio中的Marketo範本

安裝及設定GenStudio適用的Marketo後，當您在GenStudio中建立&#x200B;**電子郵件**&#x200B;體驗時，會顯示&#x200B;**[!UICONTROL Marketo範本]**&#x200B;索引標籤。 使用該索引標籤從Marketo Engage瀏覽範本。

>[!IMPORTANT]
>
>在GenStudio for Performance Marketing中的&#x200B;**標準電子郵件**&#x200B;體驗流程下建立電子郵件。 此整合不支援使用新電子郵件編輯器體驗建立的電子郵件。

使用Marketo認證的![Exchange設定](/help/extensibility/marketo-exchange-configuration.png){width="80%"}

## 疑難排解

### Marketo範本索引標籤不可見

* 確認應用程式在Exchange中為&#x200B;**已核准**，且環境為&#x200B;**已部署**，具有有效的使用者端ID、使用者端密碼和Marketo基底URL。
* 請要求您的管理員確認在建立認證時使用了&#x200B;**Marketo產品管理員**&#x200B;存取權。

### 範本未載入

* 重新載入頁面或登出並重新登入GenStudio。
* 在瀏覽器開發人員工具&#x200B;**[!UICONTROL 網路]**&#x200B;面板中，尋找對您的Marketo執行個體發出失敗的API呼叫，並驗證REST基底URL是否符合Marketo中的&#x200B;**[!UICONTROL 網頁服務]** （主機後面沒有額外的路徑）。
