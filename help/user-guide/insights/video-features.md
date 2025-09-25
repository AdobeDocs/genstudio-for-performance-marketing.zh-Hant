---
title: 視訊功能
description: 瞭解GenStudio for Performance Marketing中所使用屬性類別的影片功能。
level: Intermediate
feature: Reporting and Insights, Video Attributes, Generative AI
exl-id: 0dfdd735-b365-4a15-a6fd-e981697442cb
source-git-commit: 72cd93d9d6fdd99d5a524d05cba923e9c0191960
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 1%

---

# 視訊功能

視訊功能代表視訊中不同的資訊元素、聲音或模式，以透過[!DNL Insights]進行分析。 這些功能有助於分類和瞭解視訊內容，進而啟用更準確且詳細的深入分析。 藉由識別各種屬性，例如音訊氣氛、音樂流派和物件，AI可提供視訊的完整分析，以協助做出更好的決策和策略制定。

## 音訊偵測

GenStudio for Performance Marketing中的音訊偵測涉及分析視訊的音訊軌跡以識別各種屬性。 此偵測程式會識別呈現的音訊型別、標籤特定型別或音樂類別，並從語音中擷取關鍵字，以決定音訊的整體情緒。 透過瞭解這些音訊元素，AI可針對視訊內容和內容提供更深入的見解，從而增強整體分析和分類流程。

## 搜尋視訊功能

**若要預覽視訊並聆聽音訊範例**：

1. 在&#x200B;_[!DNL Insights]_中，選取&#x200B;**[!UICONTROL 屬性]**檢視。

1. 選取&#x200B;**[!UICONTROL 影片]**&#x200B;以變更資料表檢視。

1. 從&#x200B;**[!UICONTROL 屬性類別]**&#x200B;清單中選取功能。 如需音訊範例，請選取&#x200B;**音樂型別**。

1. 選取屬性，以檢視共用該類別的視訊。

   例如，`Music genre`類別可以有`electronic`做為屬性。

1. _屬性詳細資料_&#x200B;頁面列出具有此屬性的所有視訊。 將滑鼠指標放在清單中的任何視訊上，即可開始視訊預覽。

1. 切換&#x200B;**取消靜音** （位於視訊預覽的左下角）按鈕，並聆聽視訊預覽的音訊。

下表列出GenStudio for Performance Marketing AI識別的視訊功能類別。 偵測到的媒體內容屬性清單並非詳盡無遺。 包含一組豐富功能的媒體，可能限於AI所識別的三個最主要功能。

<!-- For the writer: turn off word wrap to work with these tables. Option + Z -->

| 類別 | 說明 | 範例 |
| ------------------- | ------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------- |
| 音訊心情 | 決定音軌的整體情緒音調或氣氛，例如`calm`、`upbeat`或`tense`。 | `Energetic`、`Happy`、`Emotional Ambient/atmospheric`、`Relaxing`、`Dramatic`、`Expressive/characterful`、`Intense`、`Slow`、`Neutral` |
| 音訊型別 | 標籤視訊有一或多個音訊內容型別，例如`music`或`speech`。 | `Music`，`Speech`，`Silence`，`Special effects`，`Ambience` |
| 類別 | 將視訊分類為一或多個廣泛的內容類別。 | `Entertainment`、`Sports`、`Music`、`Gaming`、`Howto tutorials`、`Fashion and style`、`Film and animation`、`Science and technology`、`Autos and vehicles`、`Pets and animals`、`People and blogs`、`News and politics`、`Social causes and activism`、`Travel and events`、`Education`、`Sales and offers` |
| 音樂類別 | 當影片中有音樂出現時，音樂型別的廣泛分類。 型別有助於識別音樂的一般型別，例如`contemporary`或`traditional`樣式。 | `Contemporary/pop music`，`Traditional/folk-based music`，`Instrumental/orchestral music`，`Rock music`，`Acoustic/unplugged music`，`Specialised/occasional music`，`Experimental/unique music` |
| 音樂型別 | 視訊中存在音樂時音樂風格的特定分類，可提供更詳細的音樂識別，例如`electronic`或`jazz`。 | `electronic`、`hip-hop`、`dance`、`novelty`、`rock`、`world`、`reggae`、`pop`、`film`、`jazz`、`background`、`latin` |
| 物件 | 識別視訊中顯示的一或多個專案、實體和元素。 | 值太多，但某些範例包括： `backpack`、`book`、`hawk`、`glasses`、`fish`、`pencil`、`mountain bike`、`soap` |
| 方向 | 視訊相對於其寬度和高度的對齊方式。 偵測它是否比高（橫向）寬、比寬（縱向）高，或寬度和高度相等（正方形）。 | `landscape`、`portrait`、`square` |
| 人員 | 當至少有一個人在場時，一個或多個屬性可以描述影片中的人或在場的人。 | `person`、`woman`、`man`、`girl`、`boy`、`social group`、`kid`、`crowd`、`people` |
| 場景 | 識別視訊中的設定或環境，提供製作視訊的位置或描繪位置型別的相關內容。 | 值太多，但某些範例包括： `lake`、`underwater`、`highway`、`hill`、`log cabin`、`island`、`beach`、`lounge` |
| 樣式 | 偵測套用至視訊元素的視覺化處理，例如After Effects或Lightroom中使用的視覺化處理。 | `design`，`illustration`，`logo`，`square`，`cartoon`，`art`，`matte`，`neon` |
| 標記 | 偵測不屬於特定分類的其他視訊特性。 標籤提供有關視訊的其他內容和中繼資料。 | 值太多，但某些範例包括： `construction`、`gothic`、`healing`、`military`、`selfie`、`football`、`typing`、`dancer`、`dancing` |
