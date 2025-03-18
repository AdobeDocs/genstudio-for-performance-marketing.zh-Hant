---
title: 範本程式碼編輯器
description: 瞭解如何在GenStudio for Performance Marketing中使用範本程式碼編輯器。
level: Intermediate
feature: Media Templates, Content Generation
exl-id: b46fc7a9-88c1-474a-9d7b-1df7740d8f5a
source-git-commit: 19d0b8b929e293179a091cc7b5a6a1268b0abbbd
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 0%

---

# 範本程式碼編輯器

範本程式碼編輯器可協助您驗證並調整範本，以便在使用GenStudio for Performance Marketing產生新體驗時最佳使用。 編輯器支援Handlebars語法，此語法使用範本中的預留位置來指示GenStudio for Performance Marketing應在何處為您產生內容。

>[!TIP]
>
>在[!DNL Content] _範本_&#x200B;檢視中上傳範本HTML程式碼之前，請先插入[自訂範本](customize-template.md)指南中定義的內容預留位置以準備範本。

## 檢查偵測到的欄位

_[!UICONTROL 檢查偵測到的欄位]_&#x200B;窗格會顯示GenStudio for Performance Marketing在您的範本中辨識的欄位清單。 檢閱清單，然後您可以捲動HTML程式碼以檢視範本的形式。

![程式碼編輯器檢視](/help/assets/template-detected-fields.png "檢查偵測到的欄位"){width="600" zoomable="yes"}

如果您發現清單中缺少欄位，請搜尋範本程式碼並尋找缺少欄位的位置。 使用Handlebars語法和[可辨識的欄位名稱](/help/user-guide/content/customize-template.md#recognized-field-names)插入正確的預留位置。 使用程式碼編輯器底部的「尋找和取代」表單，搜尋程式碼中的特定字串。 (Windows `CTRL`+`F`或macOS `CMD`+`F`)

### 進行更正

如果您的範本中有錯誤，您可能會看到`Template is invalid`訊息，其中包含問題的簡短說明。 在下列範例中，訊息指出`_image`欄位不符合在多重面板範本中建立的欄位命名慣例。 該訊息進一步建議您需要使用正確的前置詞更新欄位名稱。 在範本程式碼編輯器中尋找`_image`欄位，並依建議更新名稱。

![更正無效的範本](/help/assets/animation/template-code-editor.gif){width="600" zoomable="yes"}

_[!UICONTROL 檢查偵測到的欄位]_&#x200B;窗格會更新以反映您所做的變更。 在您滿意欄位正確且完成之後，請按[下一步] ****&#x200B;繼續[上傳您的範本](/help/user-guide/content/use-templates.md#add-a-template)。
