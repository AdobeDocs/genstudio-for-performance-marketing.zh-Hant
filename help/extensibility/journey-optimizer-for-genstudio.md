---
title: 適用於GenStudio的Journey Optimizer
description: 安裝和設定適用於GenStudio Adobe Exchange應用程式的Journey Optimizer ，讓您的組織可以在GenStudio for Performance Marketing中使用Adobe Journey Optimizer範本。
feature: Extensibility
source-git-commit: fbec4567d960a6e3607c5e5e43057e2f22e9f6ea
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 0%

---

# 適用於GenStudio的Journey Optimizer

在同一[!DNL IMS]組織中使用[!DNL Adobe Journey Optimizer] (AJO)和[!DNL GenStudio for Performance Marketing]的組織可以從[!DNL Adobe Exchange]安裝適用於GenStudio **應用程式的** Journey Optimizer。 系統管理員核准應用程式並完成部署後，作者可以在GenStudio中建立電子郵件體驗時，於直接上傳至[!DNL Content]的範本旁選擇AJO內容範本。

此主題適用於安裝應用程式、在[!DNL Adobe Developer Console]中建立OAuth認證，以及在[!DNL Adobe Experience Platform]中對應技術帳戶許可權的&#x200B;**管理員和開發人員**。 如需AJO和Marketo範本語法如何搭配GenStudio使用的資訊，請參閱[AJO和Marketo的範本](/help/user-guide/templates/use-templates.md#templates-from-ajo-and-marketo)。

## 先決條件

* AJO必須布建在您部署擴充功能的組織中。
* 在AJO中製作範本的使用者需要許可權，才能按照您組織的定義，在Journey Optimizer中&#x200B;**建立和編輯**&#x200B;內容範本。
* AJO中的電子郵件範本必須包含產生內容應該出現的欄位預留位置（把手列）。 可以在沒有這些欄位的情況下選取範本，但如果遺漏預留位置[!DNL GenStudio for Performance Marketing]預期的&#x200B;**體驗產生失敗**。 請參閱[自訂範本](/help/user-guide/templates/customize-template.md)和[可辨識的欄位名稱](/help/user-guide/templates/customize-template.md#recognized-field-names)。

## 從Adobe Exchange安裝應用程式

>[!VIDEO](https://video.tv.adobe.com/v/3483287?learn=on)

1. 開啟[Adobe Exchange](https://exchange.adobe.com)並移至&#x200B;**[!UICONTROL Experience Cloud]**。
1. 開啟GenStudio [&#128279;](https://exchange.adobe.com/apps/ec/abpopqqr1q/journey-optimizer-for-genstudio)適用的Journey Optimizer清單。
   Adobe Exchange上適用於GenStudio的![Journey Optimizer清單，包括需求和免費安裝](/help/extensibility/ajo-adobe-exchange.png){width="75%"}
1. 選取&#x200B;**[!UICONTROL 免費]**&#x200B;為您的組織請求應用程式。
1. 在您的組織&#x200B;**檢閱並核准**&#x200B;要求後，繼續執行[在Adobe Developer Console中建立OAuth認證](#create-oauth-credentials-in-adobe-developer-console)以及[從Exchange部署應用程式](#deploy-the-application-from-exchange)。

## 在Adobe Developer Console中建立OAuth認證

在[Adobe Developer Console](https://developer.adobe.com/console/)中建立提供Journey Optimizer API的OAuth認證的&#x200B;**專案**。 當您在Exchange中設定應用程式時，將需要&#x200B;**使用者端識別碼**、**使用者端密碼**、**組織識別碼**&#x200B;和&#x200B;**領域**&#x200B;之類的值。

1. 登入Adobe Developer Console並建立&#x200B;**新專案**。
1. 按一下「**[!UICONTROL 新增API]**」並從&#x200B;**[!DNL Experience Cloud]**&#x200B;產品API清單中選取「**[!UICONTROL Adobe Journey Optimizer (AJO) API]**」，將&#x200B;**Adobe Journey Optimizer () API**&#x200B;新增至專案。
1. 在專案工作區中產生認證，並複製&#x200B;**使用者端識別碼**、**使用者端密碼**、**組織識別碼**、**領域**&#x200B;以及部署流程要求的任何其他值。 安全地儲存它們以供下一節使用。

>[!NOTE]
>
>當您從Exchange安裝時，如果同時顯示OAuth使用者端ID和技術帳戶ID，請使用&#x200B;**OAuth使用者端ID**。

## 從Exchange部署應用程式

### 在「管理」中開啟應用程式並新增環境

1. 返回[Adobe Exchange](https://exchange.adobe.com)。
1. 選取「**[!UICONTROL 管理]**」並開啟&#x200B;**[!UICONTROL App Builder應用程式]** （或貴組織到受管理應用程式的路徑）。
1. 選取GenStudio的&#x200B;**Journey Optimizer**，並確認應用程式為&#x200B;**已核准**。
1. 在&#x200B;**[!UICONTROL 環境]**&#x200B;下，從&#x200B;**環境：**&#x200B;下拉式清單中選擇現有環境，或選取&#x200B;**[!UICONTROL 新增環境]**&#x200B;以建立環境。
   ![狀態為已核准並新增環境的應用程式詳細資料](/help/extensibility/ajo-config-002.png){width="50%"}
1. 在選取的環境中，選取&#x200B;**[!UICONTROL 組態]**。
1. 在&#x200B;**[!UICONTROL 組態]**&#x200B;索引標籤上，尋找&#x200B;**[!UICONTROL AJO認證]**。
   ![部署前使用AJO認證進行設定（草稿）](/help/extensibility/ajo-config-004.png){width="80%"}
1. 輸入已新增Journey Optimizer API之Developer Console專案的認證（例如，**[!UICONTROL AJO使用者端識別碼]**、**[!UICONTROL AJO使用者端密碼]**&#x200B;和&#x200B;**[!UICONTROL AJO權杖端點]**，以及任何其他必要欄位）。
1. 請以全部小寫輸入&#x200B;**沙箱名稱** （例如，`prod`）。
1. 按一下&#x200B;**[!UICONTROL 部署]**。 部署完成後，狀態將顯示為已部署。 按鈕文字將變更為&#x200B;**[!UICONTROL 取消部署]**。
   在App Builder應用程式檢視上可使用![已部署的應用程式與取消部署](/help/extensibility/ajo-config-005.png){width="80%"}

部署後，Adobe Developer Console包含一個名為&#x200B;**Journey Optimizer的新自動產生專案，此專案適用於GenStudio &lt;Your_Environment_Name>**&#x200B;搭配AJO和Adobe Runtime API。 此專案是唯讀的，無法編輯或刪除。
部署後![唯讀自動產生的Developer Console專案](/help/extensibility/ajo-auto-project.png){width="100%"}

### 更新設定

若要變更環境的設定變數，請先取消部署&#x200B;**，更新值，然後再重新部署**&#x200B;以讓變更生效。**&#x200B;**

您可以在Exchange中建立&#x200B;**多個環境** （例如，每個沙箱一個）。 當您的組織使用多個沙箱時，每個部署都可以在GenStudio中顯示為個別的體驗。

## 對應技術帳戶的許可權

使用者可以在GenStudio中看到AJO擴充功能，但沒有完整[!DNL Adobe Experience Platform]存取權。 對於API呼叫（例如載入範本），繫結至OAuth認證的技術帳戶必須在&#x200B;**[!DNL Adobe Experience Platform]** > **[!UICONTROL 許可權]**&#x200B;中授與Journey Optimizer許可權。 確切的角色名稱和許可權集取決於您的組織。

在AJO **[!UICONTROL 許可權]** > **[!UICONTROL 角色]**&#x200B;中，檢視&#x200B;**[!UICONTROL 歷程管理員]**&#x200B;底下的擴充功能，並從Developer Console專案新增&#x200B;**API認證**，與您從Exchange部署時所使用的認證相同。

![在Adobe Experience Platform許可權中指派給AJO架構者角色的API認證](/help/extensibility/ajo-map-permissions.png){width="80%"}

**另請參閱** （Journey Optimizer存取控制）：

* [存取控制](https://experienceleague.adobe.com/zh-hant/docs/journey-optimizer/using/access-control/access-control-landing-page)
* [Journey Optimizer中的許可權](https://experienceleague.adobe.com/zh-hant/docs/journey-optimizer/using/access-control/permissions)
* [系統管理員快速入門](https://experienceleague.adobe.com/zh-hant/docs/journey-optimizer/using/get-started/quick-start/administrator)

## 存取GenStudio中的AJO範本

部署和許可權對應之後：
1. 在GenStudio for Performance Marketing中開啟&#x200B;**[!UICONTROL 建立]**，並啟動&#x200B;**電子郵件**&#x200B;體驗。
1. 在&#x200B;**[!UICONTROL 選取範本]**&#x200B;中，開啟&#x200B;**[!UICONTROL 已上傳範本]**&#x200B;旁的&#x200B;**[!UICONTROL AJO範本]**&#x200B;索引標籤，以從Journey Optimizer瀏覽範本。

![使用AJO範本索引標籤和範本相簿選取範本](/help/extensibility/ajo-template-tab.png){width="80%"}

## 疑難排解

### AJO範本索引標籤不可見

* 確認在Exchange **[!UICONTROL 組態]**&#x200B;中輸入的值正確，包括&#x200B;**使用者端識別碼**、**使用者端密碼**、**領域**&#x200B;以及&#x200B;**沙箱**。
* 請確定&#x200B;**沙箱名稱為小寫** （例如`prod`）。
* 從Exchange安裝時，請使用&#x200B;**使用者端識別碼**，如[建立OAuth認證](#create-oauth-credentials-in-adobe-developer-console)中所述。

### 「AJO範本」標籤會出現，但未出現範本

* 重新載入頁面或再次開啟&#x200B;**[!UICONTROL AJO範本]**&#x200B;索引標籤。
* 在瀏覽器&#x200B;**[!UICONTROL 網路]**&#x200B;工具中，檢查&#x200B;**`get-templates`**&#x200B;要求。 如果它傳回&#x200B;**403 Forbidden**，則技術帳戶未指派給具有必要Journey Optimizer許可權的角色或群組。 依您的組織需求，更新[!DNL Adobe Experience Platform] **[!UICONTROL 許可權]**&#x200B;和AJO **[!UICONTROL 許可權]**&#x200B;中的對應。
