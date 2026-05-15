---
title: 範本的最佳實務
description: 搭配Adobe GenStudio for Performance Marketing使用範本時，請遵循最佳實務作法。
level: Intermediate
role: Developer, User
feature: Media Templates, Content Generation, Brand Personalization
exl-id: 3ff24fec-e836-4202-80f8-ba165e173b75
TQID: https://experienceleague.adobe.com/fiKHSZ-YFZ2gSD5iZ-aKaZtsC49Mrj1dqHpHqtbXZVM
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: f71bd2fc-e9ca-4cb6-8088-82e250211e32
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: cc72dcf1-72e1-48cc-b434-e7c27d62d67cid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 3322f783cd49ddcb897942e5e91590d53b554bdd
workflow-type: tm+mt
source-wordcount: 1347
ht-degree: 0%

---

# 使用範本的最佳實務

範本提供包括預先設定版面和設計元素的起點，大幅減少產生新內容所需的時間和精力。

將範本與GenStudio for Performance Marketing搭配使用時，請遵循下列建議：

1. 瞭解[範本元素](#know-about-template-elements)
1. 設定[頻道准則](#configure-channel-guidelines)，以有效個人化內容
1. 使用[協助工具標準](accessibility-for-templates.md)進行設計，以獲得最佳體驗
1. 遵循[特定管道的範本准則](#follow-channel-specific-template-guidelines)
1. 使用[Express範本](/help/user-guide/templates/express-templates.md)時，請考慮[Express to GenStudio範本最佳實務](#express-to-genstudio-template-best-practices)下的特定提示。
>>
瞭解[使用範本](use-templates.md)中範本元素和程式的基本知識。 深入探討[自訂範本](customize-template.md)，以取得下次行銷活動使用的特定指示。

## 使用正確的範本元素

每種範本型別使用不同元素來建立通道特定內容建立的結構。 [熟悉範本的各個部分](use-templates.md#template-elements)，並包含內容與範本型別的最佳元素。

自訂範本時，請使用欄位名稱來取代這些元素，因為您需要GenStudio for Performance Marketing產生內容。

請參閱[範本元素](use-templates.md#template-elements)。

## 在範本中使用預留位置文字

預留位置文字可協助定義語法或結構，讓使用者稍後在範本中填入內容。 例如，{first_name}.{last_name}@email.等，以定義電子郵件地址。 不過，有些常見分隔字元已保留給GenStudio for Performance Marketing中的其他含義：

❌ `< >` — 正用於HTML標籤。
❌ `{{ }}` — 用於Handlebar運算式。

使用單括弧（直括弧或大括弧）來表示預留位置文字，以避免與現有標籤混淆。

✅ `{first_name}` — 名字的預留位置。

## 設定頻道准則

定義明確的管道指引是確保產生的內容符合品牌需求和目標的關鍵。 色版指導方針可讓您指定範本中所使用元素的規則，例如色調、長度和樣式。 例如，您可以設定內文的字元數上限，或需要特定的call-to-action樣式。 透過預先設定這些准則，您就不需要在每個AI提示中寫出詳細指示，簡化內容產生流程並確保電子郵件的一致性。

檢閱並定義範本中所有主要欄位之品牌的[頻道指導方針](/help/user-guide/guidelines/brands.md#channel-guidelines)。 如果您未定義准則，則會套用[預設管道准則](/help/user-guide/guidelines/brands.md#default-channel-guidelines)，這可能無法完全反映您的品牌需求。

![主體規格](/help/assets/channel-email-body.png)

瞭解[品牌、產品和角色准則](/help/user-guide/guidelines/overview.md)如何影響產生的內容，以及如何根據您的行銷目標量身打造內容。

## 正在上傳範本的影像

範本中使用的影像應來自內容存放庫，且必須正確上傳以確保影像正確顯示。

當範本具有邊緣對邊緣（完整出血）影像時，選取的影像會自動調整大小以符合完整範本尺寸。 不過，如果影像不符合範本外觀比例，則會裁切影像以符合範本尺寸，且可能無法如預期顯示。

範本中包含的影像沒有「自動調整」功能。

若要解決影像裁切問題，使用者必須定義將影像上傳至內容存放庫時，範本中要使用的影像外觀比例。 上傳已核准的範本時：

1. [繼續範本上傳程式](/help/user-guide/templates/use-templates.md#add-a-template)，直到您到達&#x200B;**[!UICONTROL 新增詳細資料]**&#x200B;頁面。

2. 以&#x200B;**[!UICONTROL 廣告寬度(px)]**&#x200B;和&#x200B;**[!UICONTROL 廣告高度(px)]**&#x200B;定義範本中要使用的影像外觀比例。 這會為顯示影像的範本區段定義影像視窗。

3. 在&#x200B;**[!UICONTROL 更多詳細資料]**&#x200B;區段中，選取&#x200B;**[!UICONTROL 影像大小]**&#x200B;下拉式清單，並選擇&#x200B;_裁切成固定大小_。
   ![裁切為固定大小](images/crop-to-fixed-size.png "裁切為固定大小"){width="80%"}

若要在瀏覽器中決定影像的大小與外觀比例：

1. 檢查影像。
   - 在Windows/Linux上：
      - 按F12。
   - 在macOS上：
      - 按下Command + Option + I。

1. 將滑鼠停留在影像上。

1. 請注意外觀比例。 使用此專案來定義範本中影像的外觀比例。

上傳期間未套用這些詳細資料時，系統假設影像是範本的整個外觀比例，若影像與該外觀比例不完全相符，系統就會裁切該影像。

![在顯示廣告中裁切的影像](images/cropped-display.png "影像裁切"){width="60%"}

顯示廣告範本中的&#x200B;**❌已裁切的影像**

![顯示在顯示廣告中的影像](images/full-fit.png "顯示在顯示廣告中的影像"){width="60%"}

**✅影像已完整顯示**

## 遵循特定頻道的範本准則

建立範本時，請確保它們符合預期通道的特定需求。 建立可容納每個管道的版面和視覺需求的範本。 有些一般准則適用於任何範本，例如：

- 使用簡潔且回應式的HTML和內嵌CSS
- 使用Adobe或Google字型
- 請&#x200B;**不**&#x200B;使用JavaScript

{{note-css-effects}}

使用每種範本型別時，請參閱進一步的提示和限制以確保最佳效能：

- [電子郵件](/help/user-guide/templates/email-template.md)
- [顯示廣告和橫幅廣告](/help/user-guide/templates/display-template.md)
- [LinkedIn](/help/user-guide/templates/linkedin-template.md)
- [Meta廣告](/help/user-guide/templates/meta-template.md)

## Express to GenStudio範本最佳作法

下列秘訣可協助您將[!DNL Adobe Express]的設計轉換為[!DNL GenStudio for Performance Marketing]的範本時，取得可靠的結果。

### 使用多變數範本

在[!DNL Adobe Express]中，頁面可以在一個範本檔案中呈現多個大小或外觀比例變化。
當您在[!DNL GenStudio for Performance Marketing]中選取範本時，所有變數都會出現在畫布中。

此行為可改善HTML範本，其僅支援每個檔案一個變數。

### 鎖定欄位以控制行銷人員可以編輯的內容

使用鎖定來傳達意圖。 例如，鎖定法律免責宣告，使其絕不會由人工智慧產生，但為世代保留標題彈性。

在[!DNL Adobe Express]中的任何元素上按一下滑鼠右鍵以設定鎖定行為：

- **[!UICONTROL 完全鎖定]** — 元素是靜態的，而且AI不會為其產生內容。
- **[!UICONTROL 鎖定，允許影像取代]** — 鎖定大小和位置，但允許使用者交換影像。 此選項非常適用於圖志。
- **[!UICONTROL 鎖定，允許文字取代]** — 鎖定大小和位置，但允許使用者編輯文字。 AI不會自動為其產生內容。
- **完全彈性** （已解鎖） — 使用者可以移動元素並調整其大小，AI會將其視為要產生的內容。

### 為圖層命名，以更好的AI對應

當您將設計轉換為範本時，AI會掃描設計並對應欄位，例如標題、CTA和正文。 AI對應簡單範本的頻率高於高度複雜的版面。

**最佳實務：**&#x200B;在預留位置副本中，包含預期的欄位型別（例如，`headline`、`sub-headline`或`CTA`）以協助AI對應欄位正確無誤。 此方法可減少對應錯誤。

### 轉換為範本

1. 在[!DNL Adobe Express]中，按一下&#x200B;**[!UICONTROL 共用]** > **[!UICONTROL 轉換成範本]**。
1. 只有&#x200B;**[!UICONTROL 資訊]**&#x200B;索引標籤和&#x200B;**[!UICONTROL 鎖定]**&#x200B;索引標籤會移轉到[!DNL GenStudio for Performance Marketing]。
1. 在轉換時，選擇解鎖的運作方式：
   - **[!UICONTROL 允許使用者解除鎖定]**
   - **[!UICONTROL 防止所有解除鎖定]**
   - **[!UICONTROL 設定複雜密碼]** — 中間地帶，不鼓勵不永久封鎖存取的隨意變更。

### 保留原始設計檔案的復本

轉換會建立單獨的[!DNL Adobe Express]範本檔案，但原始設計檔案仍可編輯。

**秘訣：**&#x200B;保留原稿，以便日後修改設計、建立變化及產生新範本。

### 共用以提升可見度

轉換後，預設只有您能看見範本。 您可以與個人或整個組織共用。

**需求：** [!DNL Adobe Express]和[!DNL GenStudio for Performance Marketing]必須使用相同的IMS組織才能同步處理範本。 範本通常會在轉換後立即出現在[!DNL GenStudio for Performance Marketing]中。

### 控制人工智慧欄位對應

在您選取範本後，AI會為每個範本對應欄位一次，指派標籤，例如&#x200B;**[!UICONTROL 主要媒體]**、**[!UICONTROL 已產生]**&#x200B;或&#x200B;**[!UICONTROL 已鎖定]**。 當AI指派欄位不正確時，您可以手動調整對應。

使用&#x200B;**[!UICONTROL 啟用產生]**&#x200B;切換功能，在您產生之前開啟或關閉每個欄位。 當AI指派欄位不正確時，您可以手動調整對應。 已計畫在未來版本中永久更正範本對應。

### 設計於[!DNL Adobe Express]，組合於[!DNL GenStudio for Performance Marketing]

請考量這些設計工作流程，以便充份運用各項服務：

- 在[!DNL Adobe Express]中完成設計工作，例如色彩、版面配置及圖形。
- 使用[!DNL GenStudio for Performance Marketing]從這些範本組合併產生內容。
- 使用[!DNL Adobe Express]品牌（顏色、標誌、字型和圖形）進行設計管理。
- 使用[!DNL GenStudio for Performance Marketing]品牌在產生後變更字型顏色。

### 電子郵件限制

在[!DNL Adobe Express]範本工作流程的Horizon畫布上，**不支援**&#x200B;電子郵件。 電子郵件會繼續使用傳統的HTML範本程式。

### 善用自訂字型

團隊經常詢問自訂字型如何搭配[!DNL Adobe Express]範本使用。 管理員可能需要在Admin Console中接受自訂字型合格選件，這些字型才能使用；請參閱[使用 [!DNL Adobe Express] 範本](express-templates.md)。
