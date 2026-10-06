---
title: 產生和調整內容並產生可設定狀態
description: 瞭解如何產生品牌內內容，並在[!DNL GenStudio for Performance Marketing]中透過語音列印和視覺提示開啟對話來調整內容。
feature: Create Prompt, Generative AI, Content Generation
role: User
level: Beginner
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12
    internal-label: Generative AI
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
subfeature_v2:
  - id: de1f9646-abd3-4e21-9de2-df62ce55c8dc
    internal-label: Create prompt
  - id: be495d08-ecd1-455f-951e-c22de504e667
    internal-label: Content generation
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
source-git-commit: 4d35c796d2968255c3e1f525215cfe71434f8e23
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%
---
# 使用可產生狀態的專案來產生和調整內容

[!DNL GenStudio for Performance Marketing]使用狀態產生來協助您建立品牌內內容，然後在對話中輪流調整內容，而不是每次都以新的提示重新開始。 當您調整時，層代會記住您之前的指示和您保留的變體，然後僅套用您要求的變更。

可設定狀態的產生會新增三種上下文至您的世代：聲紋會保留品牌聲音的復本、影像或視訊中的視覺提示地面復本，以及網頁URL會新增您所選頁面的參考上下文。

## 產生和調整內容

1. 在[!DNL GenStudio for Performance Marketing]中，開始產生您的頻道與格式。 請參閱[[!DNL Create] 總覽](/help/user-guide/create/overview.md)，開始產生每個管道的內容。
1. _選擇性_：若要將復本移植到您自己的創意中，請選取&#x200B;**[!UICONTROL 從[內容]中選取]**，然後選擇要用作[視覺提示](#ground-content-in-an-image-or-video)的影像或視訊。
1. 選取&#x200B;**[!UICONTROL 產生]**。 [!DNL GenStudio for Performance Marketing]會建立一組變體，並在支援的頻道上自動套用您的[品牌語音](#keep-copy-in-your-brand-voice)。
1. 調整提示抽屜中的結果。 輸入您想要的變更，例如`shorten the headline`、`make variant 2 punchier`或`change the headline`。 產生僅會套用變更，並保留您先前的指示。
1. 若要保留變體，同時繼續調整，請在提示抽屜中輸入指示，例如`keep variant 2`。
1. 內容準備就緒後，請匯出或傳送以供檢閱。

## 影像或視訊中的背景內容

視覺提示可讓層代讀取您附加的影像或視訊，然後撰寫反映該創意的復本。 **[!UICONTROL Creative選項]**&#x200B;切換可控制視覺提示，預設為開啟。

若要使用視覺提示，請選取&#x200B;**[!UICONTROL 從[內容]選取]**，然後在產生影像或視訊之前選擇影像或視訊。 若要在沒有視覺提示的情況下產生，請關閉&#x200B;**[!UICONTROL Creative選項]**。

>[!NOTE]
>多框架顯示廣告或輪播廣告無法使用視覺提示。

## 讓您的品牌語調保持文案風格

聲紋功能會將您品牌所學的聲音套用到產生的文案中，因此不需要額外的提示，就能在品牌上發出音效。 具有[Insights](/help/user-guide/insights/overview.md)的管道預設為啟用，例如LinkedIn和Meta。

## 使用網頁作為內容

您可以將產生的結果指向網頁，並使用其內容作為上下文。 在提示抽屜中，輸入包含URL的指示，例如`Use this URL to generate an ad for this channel: https://www.example.com`。

>[!NOTE]
>在提示中輸入URL。 不要透過&#x200B;_引數_&#x200B;新增它。

## 相關功能

- [管理變體](/help/user-guide/create/manage-variants.md)：直接在畫布上編輯和微調產生的變體。
- [撰寫有效提示](/help/user-guide/effective-prompts.md)：製作產生較佳結果的提示。
