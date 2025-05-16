---
title: 自訂範本
description: 瞭解如何使用Adobe GenStudio for Performance Marketing generative AI辨識的內容預留位置來自訂HTML範本。
level: Intermediate
role: Developer
feature: Media Templates, Content Generation, Generative AI
exl-id: 292c1689-1b12-405d-951e-14ee6aebc75a
source-git-commit: 04bb7adcc9ce7eaeca2ea1f3ef39882f8e43ff6d
workflow-type: tm+mt
source-wordcount: '1480'
ht-degree: 0%

---

# 自訂範本

您可以透過插入內容預留位置或產生AI用來插入內容的欄位，自訂要在GenStudio for Performance Marketing中使用的範本。

以下幾節將說明如何使用&#x200B;_[!DNL Handlebars]_&#x200B;範本化語言來調整您的HTML範本以適用於GenStudio for Performance Marketing。 [!DNL Handlebars]語法使用具有雙大括弧的規則文字做為內容預留位置。 請參閱_ Handlebars語言指南&#x200B;_中的[什麼是 [!DNL Handlebars]](https://handlebarsjs.com/guide/#what-is-handlebars)，瞭解如何準備您的範本。

您的範本準備就緒後，您可以[將其上傳到GenStudio for Performance Marketing](use-templates.md#upload-a-template)，並開始根據您的自訂範本產生個人化電子郵件。

>[!TIP]
>
>遵循[協助工具准則](accessibility-for-templates.md)和[最佳實務](/help/user-guide/content/best-practices-for-templates.md)，以便您可以觸及更多對象並提供最佳體驗。

## 內容預留位置

GenStudio for Performance Marketing可辨識範本中的某些[元素](use-templates.md#template-elements)，但前提是您使用[可辨識的欄位名稱](#recognized-field-names)來識別它們。

在HTML範本的head或body中，您可以使用[!DNL Handlebars]語法來插入內容預留位置，以要求GenStudio for Performance Marketing將實際內容填入範本。 GenStudio for Performance Marketing會根據[可辨識的&#x200B;_欄位_&#x200B;名稱](#recognized-field-names)來辨識及解譯內容預留位置。

例如，您可以使用`{{headline}}`搭配[!DNL Handlebars]語法來指示電子郵件標題的放置位置。 GenStudio可辨識此欄位，根據您的指引和提示條件產生相關標題，並將標題插入此位置：

```handlebars
<div>{{headline}}</div>
```

### 可辨識的欄位名稱

下表列出GenStudio for Performance Marketing將預留位置新增至範本時識別的欄位名稱。 使用[!DNL Handlebars]語法新增這些欄位名稱至您的範本，其中您需要GenStudio for Performance Marketing產生特定型別的內容。

| 欄位 | 角色 | 頻道範本 |
| ----------------------- | ------------------------- | ------------------------------------------------ |
| `{{pre_header}}` | 預覽文字 | 電子郵件 |
| `{{headline}}` | 標題 | 電子郵件<br>中繼廣告<br>橫幅和顯示廣告<br>LinkedIn廣告 |
| `{{sub_headline}}` | 副標題 | 電子郵件<br>橫幅和顯示廣告 |
| `{{introductory_text}}` | 簡介文字 | LinkedIn廣告 |
| `{{body}}` | 內文 | 電子郵件<br>中繼廣告<br>橫幅和顯示廣告 |
| `{{cta}}` | call to action<br>檢視[行動號召](#calls-to-action) | 電子郵件<br>中繼廣告<br>橫幅和顯示廣告<br>LinkedIn廣告 |
| `{{image}}` | 影像 — 從[!DNL Content]中選取 | 電子郵件<br>中繼廣告<br>橫幅和顯示廣告<br>LinkedIn廣告 |
| `{{on_image_text}}` | 在影像文字上<br>請參閱[在影像文字上](#on-image-text)。 | 中繼廣告<br>LinkedIn廣告 |
| `{{link}}` | 影像上的呼叫動作<br>請參閱影像[&#128279;](#link-on-image)上的連結。 | 電子郵件 |

<!-- | `{{brand_logo}}`        | Logo of selected brand<br>See [Brand logo field name](#brand-logo-field-name). | email<br>Meta ad <br>LinkedIn ad | -->

GenStudio for Performance Marketing會在下列範本中自動產生特定欄位：

- **電子郵件範本**&#x200B;不需要您識別`subject`欄位
- **中繼廣告範本**&#x200B;不需要您識別`headline`、`body`和`CTA`欄位
- **橫幅和顯示廣告範本**&#x200B;不需要您識別`CTA`欄位
- **LinkedIn廣告範本**&#x200B;不需要您識別`headline`、`introductory_text`和`CTA`欄位

>[!WARNING]
>
>如果是Instagram廣告，產生的標題不會出現在最終體驗中。

上傳範本到GenStudio for Performance Marketing時有20個欄位的限制。 由於`subject`欄位會在電子郵件中自動產生，因此會計為一個欄位。 這表示電子郵件範本中允許19個欄位。

>[!TIP]
>
>您可以使用GenStudio for Performance Marketing中的[範本預覽](#template-preview)來驗證範本。

### 呼叫動作

call to action (CTA)包含片語和連結。 若要讓&#x200B;_[!UICONTROL 重述]_&#x200B;和&#x200B;_[!UICONTROL 新增連結]_&#x200B;功能在變體產生過程中正常運作，您必須在範本中包含連結和片語的預留位置。

使用下列指引設定CTA預留位置：

- CTA重新片語可供使用，且連結可供編輯

  ```html
  <a class="button" href="{{pod1_link}}" >{{cta}}</a>
  ```

- CTA重新短語可使用，但連結&#x200B;**無法**&#x200B;編輯，因為範本中提供實際連結

  ```html
  <a align="center" href="https://link">{{cta}}</a>
  ```

- CTA連結可編輯，但重新片語是&#x200B;**無法使用**，因為範本中提供片語

  ```html
  <a class="button" href="{{pod1_link}}" >Register now</a>
  ```

GenStudio for Performance Marketing也可以提供各種行動號召短語。 請參閱[修訂Call to action](/help/user-guide/create/manage-variants.md#revise-call-to-action)。

### 影像上的連結

您可以自訂電子郵件範本，讓創意人員新增連結至影像。 與CTA連結類似，使用下列指引將`link`預留位置套用至影像標籤：

```html
<a href="{{link}}"><img src="image-source.jpg" alt="{{imageDescription}}"></a>
```

在此範例中：

- `{{link}}`是實際URL的預留位置。
- `src="image-source.jpg"`應該取代為實際的影像來源URL。
- `{{imageDescription}}`是使用者定義的欄位名稱，提供影像替代文字的預留位置，對於協助工具和SEO很有用。

### 替代文字

使用使用者定義的欄位名稱做為預留位置，以產生影像的替代文字(HTML `alt="text"`屬性)說明。 下列`{{imageDescription}}`預留位置與相同`<img>`標籤內的`{{image}}`欄位搭配使用，確保影像與其描述之間的關係持續存在。

```html
<img src="{{image}}" alt="{{imageDescription}}">
```

在此範例中：

- `{{image}}`是影像來源URL的預留位置。
- `{{imageDescription}}`是替代文字的預留位置，它提供影像的說明，以供協助工具及SEO使用。

### 在影像文字上

`{{on_image_text}}`預留位置是用來指定直接放置在體驗影像上且具影響力之短訊息的文字覆蓋。

```html
<div class="image-text">{{on_image_text}}</div>
```

<!-- this field does not work in Create canvas 2025/03

### Brand logo field name

At this time, you cannot select the brand logo for the template upload. The following examples demonstrate two methods that conditionally render the brand logo. Each method verifies the source, provides a default or alternative image in case the brand logo is not available, and applies a style:

**Example 1**: Using [!DNL Handlebars] Built-in Helpers condition directly in the HTML `img src` attribute:

```html
<img src="{{#if brand_logo}}{{brand_logo}}{{else}}<default-image>{{/if}}" alt="img alt text" style="max-width: 88px; margin: 10px auto; display: block;">
```

**Example 2**: Using [!DNL Handlebars] Built-in condition statement to wrap the HTML `img` tag:

```html
{{#if brand_logo}}
    <img src="{{brand_logo}}" alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
    {{else}}
    <img src="data:image/png;base64,iVBORw0KGgo..." alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
{{/if}}
```

-->

### 手動欄位名稱

所有其他欄位名稱由使用者定義，並視為手動填入的欄位。 例如，您可能想要為頁尾內容保留區段。

若要建立可編輯的區段，請在區段名稱兩側加上雙括弧：

```html
<tbody>
    <tr>
        <td>
            <p><span class="footer-text">{{footerLegal}}</span></p>
        </td>
    </tr>
</tbody>
```

## 區段或群組

_區段_&#x200B;通知GenStudio for Performance Marketing此區段中的欄位需要高度一致性。 建立此關係可協助AI產生符合區段中創意元素的內容。

在欄位名稱中使用您選擇的前置詞來指示欄位是區段或群組的一部分。 在底線(`_`)之後使用欄位名稱（例如`headline`、`body`、`image`或`cta`）。

- _正確_ (👍)： `pod1_body`
- _不正確_ (❌)： `pod1body`

每個區段只能使用每個欄位型別中的一個。 例如，下列欄位屬於`pod1`區段：

- `pod1_headline`
- `pod1_body`
- `pod1_image`
- `pod1_cta`

因為此規則，區段無法巢狀化。

每種範本型別（例如電子郵件或中繼廣告）在區段的使用上都有通道特定的限制。 請參閱&#x200B;_使用範本的最佳實務_&#x200B;主題中的[頻道特定准則](https://experienceleague.adobe.com/zh-hant/docs/genstudio-for-performance-marketing/user-guide/content/templates/best-practices-for-templates#follow-channel-specific-template-guidelines)。

例如，電子郵件範本最多可包含三個區段；因此，您可以有三個標題和正文區段：


- `pre_header`
- `pod1_headline`
- `pod1_body`
- `pod2_headline`
- `pod2_body`
- `pod3_headline`
- `pod3_body`
- `cta`

GenStudio for Performance Marketing瞭解`pod1_headline`與`pod1_body`的關聯性比`pod2_body`更密切。

>[!TIP]
>
>請參閱[結構化提示](/help/user-guide/effective-prompts.md#structured-prompts)，瞭解如何製作提示，為多節電子郵件中的每個節產生不同的內容。

## 範本預覽

當您[上傳範本](use-templates.md#upload-a-template)時，GenStudio for Performance Marketing會掃描HTML檔案以找出可辨識的欄位。 使用預覽檢閱您的[範本元素](use-templates.md#template-elements)，並確認您以[可辨識的欄位名稱](#recognized-field-names)正確識別它們。

電子郵件範本的範例預覽：

![偵測到預覽欄位](/help/assets/template-detected-fields.png "檢查偵測到的欄位"){zoomable="yes"}

請參閱[範本程式碼編輯器](/help/user-guide/content/code-editor.md)。

### 控制項預覽

您可以使用內建協助程式（可執行特定動作的[!DNL Handlebars]範本語言中的特殊運算式）來控制特殊內容的可見度。 例如，您可以新增條件陳述式，在匯出的範本中新增追蹤引數至連結，同時保持預覽連結整齊。

呈現範本時會設定`_genStudio.browser`值，匯出範本時會設定`genStudio.export`值。 例如，當範本用於匯出時，您可使用條件包裝函式，決定在電子郵件頂端包含特定內容：

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

另一個範例可能是為了防止在GenStudio for Performance Marketing中預覽範本時使用追蹤程式碼。 下列範例說明如何在匯出的範本中將追蹤引數新增至連結，同時保持預覽連結整齊：

```html
<a class="button" {{#if _genStudio.browser }}
   href="{{link}}"{{/if}}{{#if _genStudio.export }}
   href="{{link}}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{cta}}</a>
```

## 靜態內容

電子郵件和中繼範本通常會連結到託管在其他網域上的影像和CSS檔案。 GenStudio for Performance Marketing產生範本預覽或從中衍生的體驗的縮圖時，會驗證內容來源並嵌入復本以供預覽。

外部檔案暫時內嵌只是為了建立範本預覽，可確保預覽精確地反映建立時顯示的內容。 這些外部檔案&#x200B;**不是**&#x200B;永久儲存在GenStudio for Performance Marketing中。 建立範本預覽後，GenStudio for Performance Marketing會繼續參照範本中提供的原始來源連結。

### 重新整理內容

如果來源在建立初始預覽後變更，請使用[重新整理](/help/user-guide/content/use-templates.md#refresh-template)函式，以外部來源的最新內容版本更新範本預覽。

## 範本範例

+++範例：電子郵件範本包含一個區段

以下是包含一節之電子郵件的HTML範本基本範例。 標題包含用於樣式的簡單、內嵌CSS。 內文包含`pre_header`、`headline`和`image` [預留位置](#content-placeholders)，供GenStudio for Performance Marketing在電子郵件產生程式期間用來插入內容。

```html {line-numbers="true" highlight="13"}
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
    <body>{{pre_header}}
        <div class="container">
            <h1>{{headline}}</h1>
            <p><a href="{{link}}">
            <img alt="{{headline}}"
                    src="{{image}}"
                    width="600" height="600"
                    border="0"/></a></p>
            <p>{{body}}</p>
        </div>
    </body>
</html>
```

+++

+++範例：具有多個區段的電子郵件範本

以下是上述範例中的相同HTML範本，但包含另外兩個區段。 標題包含用於設定群組樣式的內嵌CSS。 本文使用兩個群組，其中的[內容預留位置](#content-placeholders)使用前置詞。

```html
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
    <body>{{pre_header}}
        <div class="container">
            <h1>{{headline}}</h1>
            <p>{{body}}</p>
            <!-- Pod1 -->
            <div class="pod">
                <h2>{{pod1_headline}}</h2>
                <p><img alt="{{ headline }}" src="{{pod1_image}}" width="200" height="200" border="0"></p>
                <p>{{pod1_body}}</p>
            </div>
            <!-- End of Pod1 -->
            <!-- Pod2 -->
            <div class="pod">
                <h2>{{pod2_headline}}</h2>
                <p><img alt="{{headline}}" src="{{pod2_image}}" width="200" height="200" border="0"></p>
                <p>{{pod2_body}}</p>
            </div>
            <!-- End of Pod2 -->
        </div>
    </body>
</html>
```

+++

+++範例：中繼廣告範本

以下是中繼廣告範本的基本範例。 標題包含用於樣式的內嵌CSS。 本文使用[內容預留位置](#content-placeholders) （例如`image`和`on_image_text`）來指示GenStudio for Performance Marketing可以在何處產生內容。

```html {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Adobe</title>
        <style>
            .ad-container {
            font-family: Helvetica, sans-serif;
            position: relative;
            text-align: center;
            height: 100%;
            }
            .ad-image {
            width: 100%;
            height: 100%;
            object-fit: cover;
            }
            .ad-text {
            position: absolute;
            top: 0;
            left: 0;
            margin: 1em;
            background-color: rgba(0, 0, 0, 0.5);
            color: white;
            padding: 1em;
            font-size: 75px;
            }
        </style>
    </head>
    <body>
        <div class="ad-container">
            <img src="{{image}}" alt="Ad Image" class="ad-image" />
            <div class="ad-text">{{on_image_text}}</div>
        </div>
    </body>
</html>
```

+++
