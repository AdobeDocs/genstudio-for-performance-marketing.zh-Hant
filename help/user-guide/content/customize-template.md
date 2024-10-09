---
title: 自訂範本
description: 瞭解如何針對Adobe GenStudio for Performance Marketing個人化和最佳化您的範本。
level: Intermediate
feature: Templates, Content
exl-id: 292c1689-1b12-405d-951e-14ee6aebc75a
source-git-commit: ce08231cb723bec3d80a732837b72a435d3b552d
workflow-type: tm+mt
source-wordcount: '1032'
ht-degree: 0%

---

# 自訂範本

使用&#x200B;_Handlebars_&#x200B;範本語言，調整您的HTML範本以適應Adobe GenStudio for Performance Marketing。 [!DNL Handlebars]語法使用具有雙大括弧的規則文字做為內容預留位置。 請參閱&#x200B;_Handlebars語言指南_&#x200B;中的[`What is [!DNL Handlebars]?`](https://handlebarsjs.com/guide/#what-is-handlebars)，瞭解如何準備您的範本。

以下幾節將說明如何新增內容預留位置、在預覽中隱藏不必要的元素以及管理靜態內容的連結。 您的範本準備就緒後，您可以[將其上傳到GenStudio for Performance Marketing](use-templates.md#upload-a-template)，並開始根據您的自訂範本產生個人化電子郵件。

## 內容預留位置

GenStudio for Performance Marketing可辨識範本中的某些[元素](use-templates.md#template-elements)，但前提是您使用可辨識的欄位名稱來識別它們。

在範本的head或body中，您可以使用[!DNL Handlebars]語法作為內容預留位置，其中您要求GenStudio for Performance Marketing將實際內容填入範本。 GenStudio for Performance Marketing會根據[可辨識的&#x200B;_欄位_&#x200B;名稱](#recognized-field-names)來辨識及解譯內容預留位置。

例如，您可以使用`{{ headline }}`搭配[!DNL Handlebars]語法來指示電子郵件標題的放置位置：

```handlebars
<div>{{headline}}</div>
```

### 可辨識的欄位名稱

下表列出GenStudio for Performance Marketing識別的欄位名稱，以填入範本。 在需要GenStudio for Performance Marketing產生內容的範本中，使用[!DNL Handlebars]語法新增這些欄位名稱。

| 欄位 | 角色 | 頻道範本 |
| -------------- | ---------------------- | ------------------------------ |
| `pre_header` | 前置標題 | 電子郵件 |
| `headline` | 標題 | 電子郵件<br>中繼廣告 |
| `body` | 內文 | 電子郵件<br>中繼廣告 |
| `cta` | 行動號召 | 電子郵件<br>中繼廣告 |
| `on_image_text` | 在影像文字上 | 中繼廣告 |
| `image` | 影像 | 電子郵件<br>中繼廣告 |
| `brand_logo` | 選取品牌的標誌<br>如需建議使用方式，請參閱[品牌標誌欄位名稱](#brand-logo-field-name)。 | 電子郵件<br>中繼廣告 |

GenStudio for Performance Marketing會自動填入下列範本中的特定欄位：

- **電子郵件範本**&#x200B;不需要您識別`subject`欄位
- **中繼廣告範本**&#x200B;不需要您識別`headline`、`body`和`CTA`欄位

<!--
- **Display Ads template** does not require you to idenitify the `CTA` field
-->

>[!WARNING]
>
>針對Instagram廣告，產生的標題不會出現在最終體驗中。

上傳範本到GenStudio for Performance Marketing時有20個欄位的限制。 由於`subject`欄位會在電子郵件中自動產生，因此會計為一個欄位。 這表示電子郵件範本中允許19個欄位。

>[!TIP]
>
>您可以使用GenStudio for Performance Marketing中的[範本預覽](#template-preview)來驗證範本。

#### 品牌標誌欄位名稱

此時，您無法選取範本上傳的品牌標誌。 下列範例示範兩種有條件地呈現品牌標誌的方法。 每種方法都會驗證來源、提供預設或替代影像（若沒有品牌標誌可用）並套用樣式：

**範例1**：直接在HTML`img src`屬性中使用[!DNL Handlebars]內建Helpers條件：

```html
<img src="{{#if brand_logo}}{{brand_logo}}{{else}}<default-image>{{/if}}" alt="img alt text" style="max-width: 88px; margin: 10px auto; display: block;">
```

**範例2**：使用[!DNL Handlebars]內建條件陳述式來包裝HTML`img`標籤：

```handlebars
{{#if brand_logo}}
    <img src="{{brand_logo}}" alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
    {{else}}
    <img src="data:image/png;base64,iVBORw0KGgo..." alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
{{/if}}
```

#### 手動欄位名稱

所有其他欄位名稱會視為手動填入的欄位。

若要建立可編輯的區段，請在區段名稱兩側加上雙括弧：

```handlebars
{{customVariable}}
```

### 區段或群組

_區段_&#x200B;通知GenStudio for Performance Marketing此區段中的欄位需要高度一致性。 建立此關係可協助AI產生符合區段中創意元素的內容。

在欄位名稱中使用您選擇的前置詞來指示欄位是區段或群組的一部分。 例如，您可能想要將焦點放在反白區域中出現的內容：

- `pod1_headline`
- `pod1_body`

每個區段只能使用每個欄位型別中的一個。 在上述範例中，`pod1`區段只能使用一個`pod1_headline`欄位。

範本最多可包含三個區段：

- `headline`
- `body`
- `pod1_headline`
- `pod1_body`
- `pod2_headline`
- `pod2_body`

GenStudio for Performance Marketing瞭解`pod1_headline`與`pod1_body`的關聯性比`pod2_body`更密切。

## 範本預覽

當您[上傳範本](use-templates.md#upload-a-template)時，GenStudio for Performance Marketing會掃描HTML檔案以找出可辨識的欄位。 使用預覽檢閱您的[範本元素](use-templates.md#template-elements)，並確認您以[可辨識的欄位名稱](#recognized-field-names)正確識別它們。

電子郵件範本的範例預覽：

![偵測到預覽欄位](../../assets/template-detected-fields.png){width="650"}

### 控制項預覽

您可以使用內建協助程式（可執行特定動作的[!DNL Handlebars]範本語言中的特殊運算式）來控制特殊內容的可見度。 例如，您可以新增條件陳述式，在匯出的範本中新增追蹤引數至連結，同時保持預覽連結整齊。

呈現範本時會設定`_genStudio.browser`值，匯出範本時會設定`genStudio.export`值。 例如，當範本用於匯出時，您可使用條件包裝函式，決定在電子郵件頂端包含特定內容：

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

另一個範例可能是為了防止在GenStudio for Performance Marketing中預覽範本時使用追蹤程式碼。 下列範例說明如何在匯出的範本中將追蹤引數新增至連結，同時保持預覽連結整齊：

```handlebars
<a class="button" {{#if _genStudio.browser }}
   href="{{ link }}"{{/if}}{{#if _genStudio.export }}
   href="{{ link }}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{ cta }}</a>
```

## 靜態內容

電子郵件和中繼範本通常會連結至GenStudio for Performance Marketing外部託管的影像和CSS檔案。 當GenStudio for Performance Marketing為這些範本或衍生自這些範本的體驗產生縮圖時，如果這些外部資源沒有正確的跨原始資源共用(CORS)標題，則可能會忽略這些外部資源。

為了確保這些資源在縮圖產生程式期間可供使用，請考慮兩個選項：

1. **使用CORS標頭**：主機伺服器必須傳送回應，且生產環境的`Access-Control-Allow-Origin`標頭設為`https://experience.adobe.com`值。 此方法可讓GenStudio for Performance Marketing存取並包含資源。

1. **使用資料URL**：使用資料URL將外部資源直接內嵌到範本中。 此方法會繞過CORS限制，並確保資源在產生縮圖期間可供使用。

## 範本範例

+++範例：電子郵件範本包含一個區段

以下是包含一節之電子郵件的HTML範本基本範例。 標題包含用於樣式的簡單、內嵌CSS。 內文包含`pre-header`、`headline`和`image` [預留位置](#content-placeholders)，供GenStudio for Performance Marketing在電子郵件產生程式期間用來插入內容。

```handlebars {line-numbers="true" highlight="13"}
<!DOCTYPE html>
<html>
<head>
    <title>Adobe</title>
    <style>
        .container {
            width: 100%;
            padding: 20px;
            font-family: Arial, sans-serif;
        }
    </style>
</head>
<body>{{ pre_header }}
    <div class="container">
        <h1>{{ headline }}</h1>
        <p><img alt="{{ headline }}"
                src="{{ image }}"
                width="600" height="600"
                border="0"/></p>
        <p>{{ body }}</p>
    </div>
</body>
</html>
```

+++

+++範例：具有多個區段的電子郵件範本

以下是上述範例中的相同HTML範本，但包含另外兩個區段。 標題包含用於設定群組樣式的內嵌CSS。 本文使用兩個群組，其中的[內容預留位置](#content-placeholders)使用前置詞。

```handlebars {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
<head>
    <title>Adobe</title>
    <style>
        .container {
            width: 100%;
            padding: 20px;
            font-family: Arial, sans-serif;
        }
        .pod {
            background-color: #f8f8f8;
            margin: 10px;
            padding: 20px;
            border-radius: 5px;
        }
        .pod h2 {
            color: #333;
        }
        .pod p {
            color: #666;
        }
    </style>
</head>
<body>{{ pre_header }}
    <div class="container">
        <h1>{{ headline }}</h1>
        <p><img alt="{{ headline }}"
                src="{{ image }}"
                width="600" height="600"
                border="0"/></p>
        <p>{{ body }}</p>
    <!-- Pod1 -->
        <div class="pod">
            <h2>{{ pod1_header }}</h2>
            <p>{{ pod1_body }}</p>
        </div>
        <!-- End of Pod1 -->
    <!-- Pod2 -->
        <div class="pod">
            <h2>{{ pod2_header }}</h2>
            <p>{{ pod2_body }}</p>
        </div>
        <!-- End of Pod2 -->
    </div>
</body>
</html>
```

+++

+++範例：中繼廣告範本

以下是中繼廣告範本的基本範例。 標題包含用於樣式的內嵌CSS。 本文使用前置詞的[內容預留位置](#content-placeholders)。

```handlebars {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Adobe</title>
    <style>
        .ad-container {
            width: 300px;
            border: 1px solid #ddd;
            padding: 16px;
            font-family: Arial, sans-serif;
        }
        .ad-image {
            width: 100%;
            height: auto;
        }
        .ad-headline {
            font-size: 18px;
            font-weight: bold;
            margin: 12px 0;
        }
        .ad-body {
            font-size: 14px;
            margin: 12px 0;
        }
        .ad-cta {
            display: inline-block;
            padding: 10px 20px;
            background-color: #007bff;
            color: #fff;
            text-decoration: none;
            border-radius: 4px;
            text-align: center;
        }
    </style>
</head>
<body>
<div class="ad-container">
    <img src="{{ image }}" alt="Ad Image" class="ad-image">
    <div class="ad-headline">"{{ headline }}"</div>
    <div class="ad-body">"{{ body }}"</div>
    <a href="(https://example.com)" class="ad-cta">"{{ CTA }}"</a>
</div>
</body>
</html>
```

+++
