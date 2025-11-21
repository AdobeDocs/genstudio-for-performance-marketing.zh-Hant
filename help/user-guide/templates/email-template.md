---
title: 電子郵件範本准則
description: 搭配Adobe GenStudio for Performance Marketing使用電子郵件範本時，請遵循最佳實務作法。
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 8b1e8d32-5a23-45ce-a2d4-ae6de3698c45
source-git-commit: 3251d81a6bfb0c1f7d2bf3c5bd319ad4e2237699
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 0%

---

# 電子郵件範本准則

行銷電子郵件範本是進行視覺化互動和回應式電子郵件行銷活動的基礎。 一般而言，HTML範本可讓您控制版面、印刷樣式、顏色和影像，以符合您的品牌方針。 準備要在GenStudio for Performance Marketing中使用的範本時，請使用語意HTML和內嵌CSS來設定樣式，並避免指令碼或外部相依性。 結構良好的HTML範本可增強收件者的體驗，並改善傳遞能力及參與率。

自訂電子郵件範本以搭配GenStudio for Performance Marketing使用時，請遵循下列設計最佳實務：

- 使用Adobe或Google字型
- 使用簡潔且回應式的HTML和內嵌CSS
- 請&#x200B;**不**&#x200B;使用JavaScript
- 請&#x200B;**不**&#x200B;在主體或容器中使用固定寬度
- 請&#x200B;**不**&#x200B;使用base64編碼處理影像，因為它會大幅增加範本大小
- HTML檔案大小上限為102 KB

## 可辨識的欄位名稱

自訂電子郵件範本時，請在下列必填欄位中使用內容預留位置：

- `headline`
- `sub_headline`
- `body`
- `cta`
- `image` (從JPEG、PNG或GIF內容中選取)

GenStudio for Performance Marketing會自動產生下列欄位。 未啟用RTF文字。 您不需要為下列專案套用內容預留位置：

- `pre_header`
- `subject`

範本中允許的最大欄位為20。 請參閱[內容預留位置](/help/user-guide/templates/customize-template.md#content-placeholders)，進一步瞭解如何在範本中使用欄位名稱。

## 多節電子郵件

_區段_&#x200B;可讓您將內容組織成不同的群組，以支援更複雜的版面配置。 在GenStudio for Performance Marketing中，您可以使用群組命名慣例來定義每個區段。 請參閱[自訂範本區段](/help/user-guide/templates/customize-template.md#sections-or-groups)。

多區段範本可以有0、2或3個區段：

- 基本範本（零個區段）可以產生一組不需要群組命名慣例的單一範本元素。
- 複雜範本（多個區段）最多可以產生三組範本元素，這需要您遵循群組命名慣例： `<groupname_fieldname>`。
- 使用多個區段時，不會填入區段外任何保持獨立的元素。

以下是兩個區段使用群組命名慣例的欄位名稱範例：

- 在區段1：`pod1_headline`， `pod1_body`， `pod1_cta`
- 在區段2：`pod2_headline`， `pod2_body`， `pod2_cta`

## 範本範例

+++範例：電子郵件範本包含一個區段

以下是具有一個區段的HTML電子郵件範本的基本範例。 `<head>`包含用於樣式的簡單內嵌CSS，而`<body>`使用內容預留位置，例如`pre_header`、`headline`、`sub_headline`、`body`、`cta`和`image`等具有連結和。 這些預留位置可讓GenStudio for Performance Marketing在電子郵件產生期間插入動態內容。

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Marketing Email</title>
        <style>
            .container {
                width: 100%;
                padding: 20px;
                font-family: Arial, sans-serif;
            }
            .cta-button {
                display: inline-block;
                background-color: #fff;
                color: #000;
                border: 2px solid #000;
                padding: 10px 20px;
                text-decoration: none;
                font-family: 'Source Sans Pro', Arial, sans-serif;
                font-weight: 600;
                font-size: 14px;
                margin-top: 20px;
                text-align: center;
            }
        </style>
    </head>
    <body>
        <div class="container">
            {{pre_header}}
            <h1>{{headline}}</h1>
            <p>
                <a href="{{link}}">
                    <img alt="banner headline" src="{{image}}" width="600" height="600">
                </a>
            </p>
            <h2>{{sub_headline}}</h2>
            <p>{{body}}</p>
            <a href="#" class="cta-button">{{cta}}</a>
        </div>
    </body>
</html>
```

+++

+++範例：具有多個區段的電子郵件範本

以下是上述範例中的相同HTML範本，但另有兩個區段。 標題包含用於設定群組樣式的內嵌CSS。 本文使用兩個群組，其中的[內容預留位置](#content-placeholders)使用前置詞。

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
            .cta-button {
            display: inline-block;
            background-color: #fff; /* Background color to white */
            color: #000; /* Text color to black */
            border: 2px solid #000; /* Border color to black */
            padding: 10px 20px;
            text-decoration: none;            
            font-family: 'Source Sans Pro', Arial, sans-serif;
            font-weight: 600; /* Semibold */
            font-size: 14px;
            margin-top: 20px;
            text-align: center;
            }
        </style>
    </head>
    <body>{{pre_header}}
        <div class="container">
            <!-- Pod1 -->
            <div class="pod">
                <h2>{{pod1_headline}}</h2>
                <p><img alt="pic1" src="{{pod1_image}}" width="200" height="200" border="0"></p>
                <p>{{pod1_body}}</p>
            </div>
            <!-- End of Pod1 -->
            <!-- Pod2 -->
            <div class="pod">
                <h2>{{pod2_headline}}</h2>
                <p><img alt="pic2" src="{{pod2_image}}" width="200" height="200" border="0"></p>
                <p>{{pod2_body}}</p>
            </div>
            <!-- End of Pod2 -->
            <a href="#" class="cta-button">{{cta}}</a>
        </div>
    </body>
</html>
```

+++
