---
title: 範本程式碼編輯器
description: 瞭解如何在GenStudio for Performance Marketing中使用範本程式碼編輯器。
level: Intermediate
role: Developer
feature: Media Templates, Content Generation
exl-id: b46fc7a9-88c1-474a-9d7b-1df7740d8f5a
source-git-commit: 9e51e853542d20f0b90b10071f4f26aaae1d6aad
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 0%

---

# 範本程式碼編輯器

範本程式碼編輯器可協助您驗證並調整範本，以便在使用GenStudio for Performance Marketing產生新體驗時最佳使用。 編輯器支援Handlebars語法，此語法使用範本中的預留位置來指示GenStudio for Performance Marketing應在何處為您產生內容。

>[!TIP]
>
>在[!DNL Content] _範本_&#x200B;檢視中上傳範本HTML程式碼之前，請先插入[自訂範本](customize-template.md)指南中定義的內容預留位置以準備範本。

## 檢查偵測到的欄位

_[!UICONTROL 檢查偵測到的欄位]_&#x200B;窗格會顯示GenStudio for Performance Marketing在您的範本中辨識的欄位清單。 檢閱清單，然後您可以捲動HTML程式碼以檢視範本的形式。

![程式碼編輯器檢視](/help/assets/template-detected-fields.png "檢查偵測到的欄位"){width="600"}

如果您發現清單中缺少欄位，請搜尋範本程式碼並尋找缺少欄位的位置。 使用Handlebars語法和[可辨識的欄位名稱](/help/user-guide/templates/customize-template.md#recognized-field-names)插入正確的預留位置。 使用程式碼編輯器底部的「尋找和取代」表單，搜尋程式碼中的特定字串。 (Windows `CTRL`+`F`或macOS `CMD`+`F`)

## 調整變數的角色

您可以在範本結構檢查期間使用下拉式清單選取和變更文字型欄位角色（例如，`headline`、`sub_headline`、`body`、`cta`、`on_image_text`、`custom`）的欄位角色。 在範本編輯期間會保留欄位角色選擇，這樣自訂就不會遺失，進而提高工作流程效率。

>[!NOTE]
>
>影像變數的角色無法調整。

![多重角色欄位選擇](/help/assets/multirole-dropdown-field.png "多重角色欄位選擇"){width="600"}

若要將角色指派給變數：

1. 在&#x200B;_[!UICONTROL 檢查偵測到的欄位]_&#x200B;窗格中找到變數。 系統會自動探索這些變數。
2. 檢閱指派給每個變數的角色。 角色會自動指派，但可使用範本中任何變數的下拉式清單進行調整。
3. 從下拉式選單中選取新角色，即可調整角色。
4. 按一下[下一步]****&#x200B;繼續。

## 進行更正

如果您的範本中有錯誤，您可能會看到`Template is invalid`訊息，其中包含問題的簡短說明。 在下列範例中，訊息指出`_image`欄位不符合在多重面板範本中建立的欄位命名慣例。 該訊息進一步建議您需要使用正確的前置詞更新欄位名稱。 在範本程式碼編輯器中尋找`_image`欄位，並依建議更新名稱。

![更正無效的範本](/help/assets/animation/template-code-editor.gif){width="600"}

_[!UICONTROL 檢查偵測到的欄位]_&#x200B;窗格會更新以反映您所做的變更。 在您滿意欄位正確且完成之後，請按[下一步] ****&#x200B;繼續[上傳您的範本](/help/user-guide/templates/use-templates.md#add-a-template)。

## 常見範本問題和解決方案

| **錯誤** | **說明** | **解決方案** |
|-----------------------------|---------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|
| 剖析失敗 | 無法將範本內容剖析為有效的Handlebars。 | 檢查範本中是否有HTML和Handlebars語法錯誤，並更正這些錯誤，以確保[內容預留位置](/help/user-guide/templates/customize-template.md#content-placeholders)的格式有效。 |
| 未指派群組 | 多群組電子郵件範本中的影像欄位未指派給任何群組。 | 檢查是否一致使用區段首碼。 每個[區段](/help/user-guide/templates/customize-template.md#sections-or-groups)只能使用每個欄位型別(`headline`、`body`、`image`、`cta`)中的一個。 將`image`欄位指派給範本中的有效群組。 |
| 影像遺失 | 缺少必要的影像欄位。 | 特定範本型別(例如Meta、顯示或橫幅廣告)只需要一個`image`欄位。 將必要的`image`欄位新增至您的範本。 |
| 無效的單一群組 | 電子郵件範本只包含一個群組，這是無效的。 | 基本電子郵件範本包含單一範本元素集，這些元素不需要[區段或群組](/help/user-guide/templates/customize-template.md#sections-or-groups)中定義的群組命名慣例。 移除任何群組命名語法，將範本調整為零區段。 |
| 無欄位 | 範本不包含任何欄位。 | 使用Handlebars語法新增[可辨識的欄位名稱](/help/user-guide/templates/customize-template.md#recognized-field-names)至您的範本，在其中您需要GenStudio for Performance Marketing產生特定型別的內容。 |
| 缺少必要屬性 | 缺少部分必要的中繼資料屬性。 | 每個範本型別都有根據通道指引的需求和限制。 例如，Meta需要外觀比例，而顯示廣告則需要尺寸。 [遵循特定管道的範本准則](/help/user-guide/templates/best-practices-for-templates.md#follow-channel-specific-template-guidelines)。 |
| 使用的保留名稱 | 正在使用禁止或保留的欄位名稱。 | 某些[欄位名稱](/help/user-guide/templates/customize-template.md#recognized-field-names) （例如`subject`或`introductory_text`）已保留。 重新命名使用保留或禁止名稱的欄位。 |
| 太多欄位 | 欄位數超過全域限制20。 | 移除不必要的欄位，確保總計不超過20個。 |
| 太多群組 | 群組數量超過頻道允許的最大值。 | Meta、display和LinkedIn範本不允許有多個區段。 定義兩個或三個區段時，電子郵件需要群組命名。 減少範本中的群組數量以符合[管道的需求](/help/user-guide/templates/best-practices-for-templates.md#follow-channel-specific-template-guidelines)。 |
| 不支援的欄位 | 範本使用管道不支援的欄位。 | 根據[可辨識的欄位名稱](/help/user-guide/templates/customize-template.md#recognized-field-names)取代或移除不支援的欄位。 |
