---
title: 顯示廣告範本指導方針
description: 搭配Adobe GenStudio for Performance Marketing使用顯示廣告和橫幅範本時，請遵循最佳實務作法。
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 076239b3-9444-48f9-bdd6-ef2b757bdf0d
source-git-commit: f4bc3442678e6366e185d0c7a91c784d43b8e455
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# 顯示廣告範本准則

顯示範本是預先設計的版面，用於建立吸引目光的橫幅和顯示廣告。 它們提供彈性的架構，整合影像、文字和call to action，確保在製作多個廣告變化時的一致性和效率。 準備要在GenStudio for Performance Marketing中使用的範本時，請確定所有資產已針對Web顯示最佳化，並符合必要的檔案格式和大小。

自訂橫幅和顯示廣告範本以搭配GenStudio for Performance Marketing使用時，請遵循下列設計最佳實務：

- 使用Adobe或Google字型
- 準備以超薄尺寸顯示的優異資產
- 僅需要一個影像欄位
- 請&#x200B;**不**&#x200B;使用內嵌或編碼的背景影像
- 使用已上傳至GenStudio for Performance Marketing內容存放庫的背景影像（`image`欄位）。 遵循[上傳顯示廣告的影像](#uploading-images-for-display-ads)中的准則，以獲得最佳結果
- 請&#x200B;**不**&#x200B;使用JavaScript
- 只能使用一個區段，以產生一組範本元素

## 可辨識的欄位名稱

自訂橫幅或顯示廣告範本時，請為下列必填欄位使用內容預留位置：

- `headline`
- `sub_headline`
- `body`
- `image` (必要，從JPEG、PNG或GIF內容中選取)

GenStudio for Performance Marketing會自動產生下列欄位。 您不需要為下列專案套用內容預留位置：

- `cta`

請參閱[內容預留位置](/help/user-guide/content/customize-template.md#content-placeholders)，進一步瞭解如何在範本中使用欄位名稱。

## 支援的維度

必須設定寬度x高度（畫素）。

| 方向 | 尺寸（畫素） | 備註 |
|--------------|-------------------------------------------------------------|------------------------------------------------------------------|
| 垂直 | 300 x 600<br>160 x 600 | 適用於摩天大樓和半頁橫幅。 |
| 水準 | 300 x 250<br>728 x 90<br>336 x 280<br>320 x 50<br>970 x 250 | 標準排行榜、中等矩形和橫幅大小。 |
| 自訂 | 50 x 50至2000 x 2000 | 用於非標準或唯一版位；檢查平台限制。 |

## 上傳顯示廣告的影像

顯示廣告使用的影像應來自內容存放庫，且必須正確上傳，以確保影像在範本中正確顯示。

當顯示範本具有邊緣對邊緣（完整出血）影像時，選取的影像會自動調整大小以符合完整範本尺寸。 不過，如果影像不符合範本外觀比例，則會裁切影像以符合範本尺寸，且可能無法如預期顯示。

顯示廣告範本中的影像沒有「自動調整」功能。

若要解決影像裁切問題，使用者必須定義將影像上傳至內容存放庫時，範本中影像的外觀比例。 上傳已核准的顯示廣告範本時：

1. [繼續範本上傳程式](/help/user-guide/content/use-templates.md#add-a-template)，直到您到達&#x200B;**[!UICONTROL 新增詳細資料]**&#x200B;頁面。

1. 以&#x200B;**[!UICONTROL 廣告寬度(px)]**&#x200B;和&#x200B;**[!UICONTROL 廣告高度(px)]**&#x200B;定義範本中要使用的影像外觀比例。 這會為顯示影像的範本區段定義影像視窗。

1. 在&#x200B;**[!UICONTROL 更多詳細資料]**&#x200B;區段中，選取&#x200B;**[!UICONTROL 影像大小]**&#x200B;下拉式清單，並選擇&#x200B;_裁切成固定大小_。
   ![裁切為固定大小](./crop-to-fixed-size.png "裁切為固定大小"){width="80%"}

若要在瀏覽器中決定影像的大小與外觀比例：

1. 檢查影像。
   - Windows/Linux：
      - 按F12。
   - macOS：
      - 按下Command + Option + I。

1. 將滑鼠停留在影像上。

1. 請注意外觀比例。 使用此專案來定義範本中影像的外觀比例。

上傳期間未套用這些詳細資料時，系統假設影像是範本的整個外觀比例，若影像與該外觀比例不完全相符，系統就會裁切該影像。

![在顯示廣告中裁切的影像](./cropped-display.png "影像裁切"){width="60%"}

顯示廣告範本中的&#x200B;**❌已裁切的影像**

![顯示在顯示廣告中的影像](./full-fit.png "顯示在顯示廣告中的影像"){width="60%"}

**✅影像已完整顯示**
