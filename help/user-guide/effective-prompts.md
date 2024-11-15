---
title: 撰寫有效的提示
description: 了解如何為 Adobe GenStudio for Performance Marketing 編寫有效提示。
feature: Prompt, Generative AI, Brands Service, Personas Service, Products Service, Guidelines
exl-id: 0cd4db4f-d031-4c1f-a4e7-adc220f947fc
source-git-commit: e3745e1eed08512f9f2c7d62a2f3af6812e2019f
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 2%

---

# 撰寫有效的提示

與創作AI溝通對於Adobe GenStudio for Performance Marketing中的有效運作至關重要。

GenStudio for Performance Marketing會在每次有機會修改資產時提供產生式AI提示。 有效提示的元件應包括描述性語言、範例，以及未透過您設定的准則提供的資訊。

最佳實務是使用[指南](/help/user-guide/guidelines/overview.md)為GenStudio for Performance Marketing提供您的品牌資訊，然後您就可以完全運用創作AI來產生與品牌一致的內容體驗。

## 描述性語言

您可以使用自然語言來表達您的想法以建立體驗。 您的提示會引導AI產生個人化的頻道內容以及補充您視覺效果的影像。 您提供的詳細資訊越多，產生符合您需求的影像或體驗的機會就越大。 使用清楚的描述性語言，儘可能提供詳細資訊：

- 對於&#x200B;**影像**，請使用描述氣氛、情緒、色彩、作文和樣式的文字。
- 針對&#x200B;**副本**，請使用描述對象、用途、新功能說明、範例和動作的文字。

以下是範例提示，詳述有關您的意圖、目標對象和樣式的資訊。

```bash
Write an email to motivate infrequent users of Photoshop to follow an in-app tutorial that teaches them to combine elements of two photos into a beautiful work of art. Highlight the generative AI capabilities of Photoshop and use references to natural imagery.
```

+++檢視範例結果

![三個產生的電子郵件](/help/assets/sample-email.png)

+++

## 提示條件

在GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md)中，您可以在提示抽屜中使用&#x200B;**[!UICONTROL 提示條件]** （[_引數_](/help/user-guide/create/overview.md#parameters)&#x200B;和提示），透過選取來新增詳細資料，以改善AI解譯。

對於[電子郵件](/help/user-guide/create/email-experiences.md)，提示條件可能包括在&#x200B;_引數_&#x200B;中新增[指南](/help/user-guide/guidelines/overview.md)、上傳要在電子郵件變體中使用的資產，以及描述性提示。 對於[中繼廣告](/help/user-guide/create/create-meta-ad.md)，提示條件可能包括&#x200B;_引數_&#x200B;中的品牌指引、選取或上傳現有資產、影像或資產（例如外觀比例）的相關設定以及提示。 實際效能始於[設定准則](/help/user-guide/guidelines/add-guidelines.md)。

>[!NOTE]
>
>如果在提示抽屜的&#x200B;_引數_&#x200B;中新增准則，您就不需要在提示中包含這些准則的參照。 GenStudio for Performance Marketing在內容產生中會運用這些[!DNL Brands]、[!DNL Products]和[!DNL Personas]。

### 准則

GenStudio for Performance Marketing指南可協助創作AI個人化您的資產構成。 出現提示條件時，您可以從已設定的准則中選擇[[!DNL Brand]](/help/user-guide/guidelines/brands.md)、[[!DNL Persona]](/help/user-guide/guidelines/personas.md)和[[!DNL Product]](/help/user-guide/guidelines/products.md)。

>[!TIP]
>
>您可以控制GenStudio for Performance Marketing使用您[!DNL Brand]指引的方式和時間。 請參閱[准則](/help/user-guide/guidelines/overview.md)以瞭解如何設定和管理您的品牌准則。

### 結構化提示

對於多節電子郵件，您可以建構提示以提供特定節的指示，以產生[電子郵件](/help/user-guide/create/email-experiences.md)中每個節的不同內容。 結構化提示應直接參照電子郵件範本](/help/user-guide/content/email-template.md#multi-section-emails)中的[節名稱，以便將產生的內容插入對應的內容預留位置。

例如，您可以指示GenStudio for Performance Marketing產生在電子郵件第一區段中推廣新產品的內容，並產生在第二電子郵件區段中詳細說明產品成本節省效益的內容。

結構化提示應：

- 在電子郵件範本中對區段名稱使用以下其中一個參照：
   - Pod
   - 群組
   - 區段
   - 模組

  例如，如果您的範本使用`moduleA`或`Group-3`作為區段名稱，則您可以在提示中參照這些區段名稱。

- 遵循建議的規則/結構。 如果提示結構不符合提供的格式，提示會套用到&#x200B;*所有*&#x200B;電子郵件區段，並且仍然會方便內容產生。
- 使用區段名稱作為電子郵件範本](/help/user-guide/content/email-template.md#code-an-email-template)中定義的[。 提示參考必須符合電子郵件範本中編碼的區段名稱。
- 不區分大小寫。 例如，您可以在電子郵件範本和結構化提示中使用`Pod`或`pod`。
- 先參考一般使用者提示，然後參考區段特定指示。
- 使用冒號、連字型大小、逗號或其他分隔(`,:;#$!~|@=-%&*^_`)作為區段名稱參考和指示詞之間的分隔。 例如，您可以使用下列作為特定區段提示指令： `Pod1; Describe how to easily edit text and swap images.`

下列是範例提示，可清楚說明建議的提示結構，並運用電子郵件範本，使用識別字詞`Pod`，如`Pod1`、`Pod2`和`Pod3`中所示。

```properties
Create an exciting multi-pod email focusing on Creative Cloud and its powerful generative AI capabilities.

Encourage customers to convert to Photoshop or use a free Photoshop trial. We want to better educate them about app features.

Pod1: Focus on Adobe Photoshop and its new generative AI tools that enable creators to bring images to life in minutes.

Pod2: Focus on Adobe Illustrator and its new generative AI tools, such as Generative Shape Fill, which allows you to quickly fill your vector outline and explore a variety of options that match the look and feel of your own artwork.

Pod3: Focus on Adobe Acrobat Pro. Make users aware that with Acrobat Pro they can edit images and text inside a PDF.
```

請參閱[準備電子郵件範本](/help/user-guide/content/email-template.md#code-an-email-template)。

## 再試一次

提示是一個反複的過程。 如果結果不符合您的預期，請檢視您的提示並進行一些變更或新增更多詳細資訊。 或者，您也可以貼上行銷活動簡報的區段。 您甚至可以要求GenStudio for Performance Marketing避免使用某些字詞、元素或主題。

## 最佳做法

製作有效提示的一些簡單最佳實務：

- 做到具體，並提供該做什麼和不該做什麼的詳細資訊。
- 使用外部參照提供內容。
- 運用GenStudio for Performance Marketing指引。
- 定期檢閱和調整指引。
- 反複和調整。
- 透過實驗瞭解。

{{in-academy}}
