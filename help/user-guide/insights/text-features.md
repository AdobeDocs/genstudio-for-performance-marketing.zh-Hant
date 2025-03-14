---
title: 文字功能
description: 瞭解GenStudio for Performance Marketing中使用的屬性類別的文字功能。
feature: Insights, Attributes, Generative AI
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: 7b81b0ae-0c62-468f-965c-fd8070644fb3
source-git-commit: 808ffdb7f55f7ff938e9346b8513fab46f86df7c
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 1%

---

# 文字功能

文字功能包括某些文字元素的計數，例如文字、句子、表情符號，以及使用[!DNL Insights]進行分析時所使用的語意、情緒和語調的分類。 文字也可能收到可讀性分數。

GenStudio for Performance Marketing使用Adobe的AI和機器學習功能來學習文字，並根據關聯的文字音調和行銷敘述套用[!UICONTROL 媒體屬性]。 程式會驗證輸入文字，確保文字包含英數字元、移除多餘的空格和無法列印的字元，並將文字截斷至允許的1500個字詞上限。 在套用偵測到的屬性標籤之前，AI會預測普遍的色調。

## 語調

色調代表透過語言展現的一般角色、態度或氣氛。 只要選擇字詞和標點符號、句子結構和樣式，就能改變訊息的語調。 例如，請考量下列使用三個基本音階的緊急訊息：

- `Formal`

  ```
  Take advantage of this distinctive and exceptional opportunity!
  ```

- `Conversational`

  ```
  Don't miss out on this great opportunity!
  ```

- `Direct`

  ```
  Don't miss the chance!
  ```

AI會進一步偵測到更細微的色調。 使用先前範例中的相同緊急陳述式，下列版本使用異想天開的`poetic`語調：

- `Poetic`

  ```
  Embrace the moment, without delay, for this occasion won't always stay.
  ```

音調的其他次要值包括： `Enthusiastic`、`Assertive`、`Humorous/Witty`、`Inspirational`、`Empathetic`、`Sensory`、`Storytelling`、`Poetic`、`Quantitative`、`Personal`

## 敘述

敘述屬性可協助您識別傳達可與目標受眾產生共鳴的值、目的或身分的媒體。

| 敘述 | 說明 | 範例 |
| ----------------- | ----------- | ------- |
| `Authenticity` |             |         |
| `Celebration` |             |         |
| `Community` |             |         |
| `Convenience` |             |         |
| `Empowerment` |             |         |
| `Exploration` |             |         |
| `Futuristic` |             |         |
| `Hype` |             |         |
| `Indulgence` |             |         |
| `Peace of mind` |             |         |
| `Personalization` |             |         |
| `Prestige` |             |         |
| `Timelessness` |             |         |
| `Versatility` |             |         |
| `Well-being` |             |         |

## 可讀性分數

可讀性評分會評估一段文字閱讀和理解的難易程度。 這可協助確保您的內容適合您的目標對象。 分數取決於多種因素，包括句子長度和字詞複雜度。

| 分數 | 學校等級 | 備註 |
| ----------- | ------------------ | ------------------------------------------------------------------------- |
| 100.00-90.00 | 5年級 | 非常容易閱讀。 一般的11歲學生都能輕鬆理解。 |
| 90.0 - 80.0 | 6年級 | 容易閱讀。 適用於消費者的對話式英文。 |
| 80.0 - 70.0 | 7年級 | 相當容易閱讀。 |
| 70.0 - 60.0 | 八年級和九年級 | 純英文。 13至15歲的學生容易理解。 |
| 60.0-50.0 | 10至12年級 | 相當難讀。 |
| 50.0-30.0 | 大學 | 難以閱讀。 |
| 30.0-0.0 | 大學畢業生 | 很難閱讀。 大學畢業生最容易理解。 |

## 字數

待定

下表列出GenStudio for Performance Marketing AI識別的影像功能類別。

| 類別 | 說明 | 範例 |
| -------------------- | ------------- | --------------------- |
| 表情符號計數 |             |        |
| 雜湊標籤計數 |             |        |
| 關鍵字 |             |        |
| 行銷情感 | 情緒是行銷訊息的目標，可喚起觀眾的特定情感和回應，這可能會增強與品牌的參與度和聯絡。 | `Aspiration`、`Challenge`、`Curiosity`、`Exclusivity`、`Fascination`、`Gratification`、`Recognition`、`Trust`、`Urgency` |
| 說服策略 | 用來影響消費者行為並推動所需動作的技術。 這些策略會鎖定特定的心理觸發器和客戶區段，以提升行銷訊息的有效性。 | `Social identity`、`Social proof`、`Endorsement`、`Concreteness`、`Foot in the door`、`Overcoming reactance`、`Reciprocity`、`Comparison`、`Social impact`、`Scarcity`、`Anthropomorphism` |
| 語調 | 行銷訊息中透過字詞選擇、標點符號、句子結構和樣式所傳達的一般字元、態度或氣氛。 | `Enthusiastic`、`Assertive`、`Humorous/Witty`、`Inspirational`、`Empathetic`、`Sensory`、`Storytelling`、`Poetic`、`Quantitative`、`Personal` |
