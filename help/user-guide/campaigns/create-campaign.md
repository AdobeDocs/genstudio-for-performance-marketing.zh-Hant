---
title: Adobe GenStudio for Performance Marketing行銷活動
description: 瞭解如何建立和管理運用創作AI資產和體驗的數位行銷活動。
feature: Campaign Planning, Campaign Brief
badgeBeta: label="Beta" tooltip="此功能目前在Beta中，因此某些功能可能會受到限制或有所變更。"
source-git-commit: edbeb7f0d08e2215a23f15cfeff77a5217cd264b
workflow-type: tm+mt
source-wordcount: '859'
ht-degree: 0%

---

# 建立行銷活動

GenStudio for Performance Marketing行銷活動會定義關鍵數位行銷活動特徵，並隨著階段的部署和評估而發展。 GenStudio for Performance Marketing支援動態程式，包括啟動行銷活動、追蹤個別行銷活動元件的效能，以及根據效能指標重新調整廣告體驗的焦點。

行銷活動的主要元素儲存在行銷活動物件中，這會為所有使用相同唯一行銷活動名稱標籤的資產和體驗建立共用內容。 此標籤可識別整個GenStudio for Performance Marketing中的行銷活動。

GenStudio系統管理員和Genstudio編輯人員可以建立行銷活動。

## 定義行銷活動詳細資料

{{$include /help/_includes/campaign-details.md}}


**若要輸入行銷活動詳細資料**：

1. 從[!DNL Campaigns]，按一下&#x200B;**[!UICONTROL 新增行銷活動]**。 _建立行銷活動_&#x200B;檢視隨即開啟。

   詳細資料包含定義行銷活動的選用和必填欄位。 這些詳細資料會儲存於[!DNL Campaigns]，作為行銷活動的中繼資料屬性。

1. 連按兩下&#x200B;_新行銷活動_&#x200B;標題並輸入資訊豐富的唯一名稱。

   此名稱會成為GenStudio for Performance Marketing中的&#x200B;_行銷活動標籤_，可讓您在上傳和建立期間將資產或體驗與行銷活動建立關聯。

1. 在描述行銷活動的&#x200B;_詳細資料_&#x200B;欄位中輸入值。 請參閱&#x200B;_促銷活動詳細資料_&#x200B;表格，瞭解這些促銷活動功能的定義。

## 指派管道和區域

管道和區域設定會決定行銷活動的部署位置及其發佈管道。

GenStudio for Performance Marketing使用名為「_記錄_」的預定義範本來代表重要的行銷活動元件，例如管道、地區、角色和產品。 建立行銷活動時，您會將其與每個元件的相關記錄建立關聯。

* **管道設定** — 定義行銷活動的公開發佈管道，包括付費媒體帳戶、電子郵件行銷服務和顯示廣告網路。 有關這些管道中行銷活動、資產和體驗的績效資料會饋送到[[!DNL Insights]](/help/user-guide/insights/overview.md)，以進行特定管道的分析。

* **區域設定** — 指定您部署行銷活動的地理區域。 透過連線到地區資料來源，GenStudio for Performance Marketing可以根據當地受眾偏好量身打造內容和策略。 如此一來，即可根據地區量度，進行更精確的目標定位和效能分析。

**若要選取行銷活動的發佈管道**：

1. 按一下&#x200B;**[!UICONTROL 管道]**&#x200B;旁的+符號（**[!UICONTROL 連線記錄+]**）。

   _選取頻道_&#x200B;快顯視窗隨即開啟。

1. 選取行銷活動部署所在的管道。 有效值包括`Email`、`Paid media`、`Web`和`Display ads`。

   可選擇性地選擇&#x200B;**[!UICONTROL 檢視全部]**&#x200B;以開啟所有支援頻道的檢視。

**若要指派區域給行銷活動**：

1. 按一下&#x200B;**[!UICONTROL 區域]**&#x200B;旁的+符號（**[!UICONTROL 連線記錄+]**）。

   _選取區域_&#x200B;快顯視窗開啟。 您可以搜尋特定的支援區域。

1. 選取地區：行銷活動的一或多個目標地區。 有效區域包括`AMER`、`LATAM`、`EMEA`、`APAC`和`Japan`。

   可選擇性地選擇&#x200B;**[!UICONTROL 檢視全部]**，以開啟所有支援區域的檢視。

## 指派角色和產品

[角色](/help/user-guide/guidelines/personas.md)和[產品](/help/user-guide/guidelines/products.md)已儲存為記錄。 個人記錄會定義特定客戶區段的特徵，即所產生內容的目標對象。 其中可能包含人口統計細節，以及客戶互動的歷史。

產品記錄會根據您的品牌指導方針定義關鍵產品規格和屬性。 屬性可包含您品牌內的功能、相關影像和產品定位。

_角色_&#x200B;和&#x200B;_產品_&#x200B;下拉式功能表中的選項是在組織層級定義的。 建立行銷活動時，您可從這些預先定義的記錄中進行選取，以確保一致的產品表示方式，並支援準確定位、傳送訊息和效能追蹤。

**若要指派角色給行銷活動**：

1. 按一下&#x200B;**[!UICONTROL 角色]**&#x200B;旁的+符號（**[!UICONTROL 連線記錄+]**）。

   _選取角色_&#x200B;快顯視窗隨即開啟。 您可以搜尋特定的受支援角色。

1. 選取您的行銷活動鎖定的角色。 有效角色由您的組織在[准則建立](/help/user-guide/guidelines/personas.md)期間定義。

   選擇性地選擇&#x200B;**[!UICONTROL 檢視全部]**&#x200B;以開啟所有可用角色的檢視。

**若要指派產品給行銷活動**：

1. 按一下&#x200B;**[!UICONTROL 產品]**&#x200B;旁的+符號（**[!UICONTROL 連線記錄+]**）。

   _選取產品_&#x200B;快顯視窗隨即開啟。 您可以搜尋特定的支援產品。

1. 選取一或多個產品。 產品是由您的組織在[准則建立](/help/user-guide/guidelines/products.md)期間所定義。

   可選擇性地選擇&#x200B;**[!UICONTROL 檢視全部]**，以開啟所有可用產品的檢視。

## 完成行銷活動建立

按一下&#x200B;**[!UICONTROL 建立]**&#x200B;以儲存輸入的值並建立行銷活動。

新的行銷活動名稱現在可在[!DNL Content]和[!DNL Create]中作為行銷活動標籤使用。 您可以透過[!DNL Content]將已核准的資產和體驗新增至行銷活動，或在內容建立期間將資產和體驗指派至行銷活動。

## 將內容新增至行銷活動

GenStudio for Performance Marketing使用儲存在[!DNL Content]中繼資料中的行銷活動標籤，將內容連結至行銷活動。 單一內容可與多個行銷活動相關聯。

行銷活動標籤會識別行銷活動及其屬性。 為資產或體驗指派標籤，可將其連結至對應的促銷活動。

**若要從[!DNL Content]**&#x200B;新增資產和體驗：

1. 從[!DNL Content] _體驗_&#x200B;或&#x200B;_Assets_&#x200B;收藏館，選擇核准的體驗或資產。

1. 從&#x200B;_詳細資料_&#x200B;檢視，從&#x200B;_行銷活動_&#x200B;下拉式功能表選取行銷活動名稱。

**若要在內容建立期間新增資產和體驗**：

在內容建立期間，您可以將新建立的資產或體驗發佈到[!DNL Content]。

1. 從&#x200B;_確認核准內容的詳細資料_&#x200B;快顯視窗，從&#x200B;_行銷活動_&#x200B;下拉式功能表選取行銷活動。

1. 點擊&#x200B;**[!UICONTROL 發佈]**。

此行銷活動現在可在&#x200B;_行銷活動_&#x200B;儀表板中使用。
