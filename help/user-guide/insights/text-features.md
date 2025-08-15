---
title: 文字功能
description: 瞭解GenStudio for Performance Marketing中使用的屬性類別的文字功能。
feature: Reporting and Insights, Text Attributes, Generative AI
exl-id: 7b81b0ae-0c62-468f-965c-fd8070644fb3
source-git-commit: 3ccc6313a7c559f1c0846c144d23b783da0aecfa
workflow-type: tm+mt
source-wordcount: '1290'
ht-degree: 1%

---

# 文字功能

文字功能包括某些文字元素的計數，例如文字、句子、表情符號，以及使用[!DNL Insights]進行分析時所使用的語意、情緒和語調的分類。 文字也可能收到可讀性分數。

GenStudio for Performance Marketing使用Adobe的AI和機器學習功能來學習文字，並根據關聯的文字音調和行銷敘述套用[!UICONTROL 媒體屬性]。 程式會驗證輸入文字，確保文字包含英數字元、移除多餘的空格和無法列印的字元，並將文字截斷至允許的1500個字詞上限。 在套用偵測到的屬性標籤之前，AI會預測普遍的色調。

## 語調

色調代表透過語言展現的一般角色、態度或氣氛。 只要選擇字詞和標點符號、句子結構和樣式，就能改變訊息的語調。 例如，請考量下列使用三個基本音階的緊急訊息：

| 色調 | 說明 | 範例 |
| -------------- | ----------------------------------- | --------------------------------------------------------- |
| 正式 | 精緻專業的語言。 | `Take advantage of this distinctive and exceptional opportunity!` |
| 對話 | 友善的非正式語言。 | `Don't miss out on this great opportunity!` |
| 直接 | 簡單明瞭，切中要害。 | `Don't miss the chance!` |

音調的其他次要值可讓您更清楚地區分訊息的字元和態度。 為了與先前緊急訊息的範例保持一致，GenAI可能會在這個異想天開的範例中偵測到&#x200B;_詩意_&#x200B;音調： `Embrace the moment, without delay, for this occasion won't always stay.`

下表列出GenStudio for Performance Marketing AI識別的色調值。

| 色調 | 說明 | 範例 |
| -------------- | ------------------------------------------------ | --------------------------------------------------------- |
| 主觀 | 自信而有力的表達方式。 | `You need to act now to secure this deal!` |
| 直接 | 簡單明瞭，切中要害。 | `Don't miss the chance!` |
| 同理心 | 顯示理解和敏感度。 | `We understand your needs, and this is perfect for you.` |
| 熱心 | 顯示強烈且急切的享受、興趣或認可。 | `This is an amazing opportunity you can't miss!` |
| 幽默/風趣 | 輕鬆又聰明。 | `Why wait? Grab this deal before it's gone!` |
| 勵志 | 鼓舞人心和令人振奮之處。 | `Believe in yourself and seize this opportunity!` |
| 詩意 | 藝術性和表現力。 | `Embrace the dawn of a new opportunity.` |
| 量化 | 根據數值資料。 | `99% of users loved this offer, and you will too.` |
| 感官 | 運用感官功能。 | `Feel the excitement with this incredible offer!` |
| 講故事 | 敘述故事以傳達訊息。 | `Once upon a time, there was an offer you couldn't refuse.` |

## 情感訴求

行銷人員運用人類情感的力量，在對象與品牌之間建立強大的連結。 透過利用快樂、恐懼、興奮或懷舊等感覺，行銷人員可以製作在更深層次上產生共鳴的訊息，以推動參與並影響消費者行為。 情感吸引力有助於提供更易傳達且令人難忘的內容，最終提升品牌忠誠度，並鼓勵所需行動。

說服策略、行銷情感和敘述樣式可共同作用來鎖定客戶區段。

- **敘事樣式**，例如真誠、慶祝和社群，有助於傳達與目標受眾產生共鳴的價值和身分，創造更吸引人且更可傳達的訊息。
- **勸說策略** （例如稀缺、社交證明和互惠）是設計來吸引消費者的情感和喜好以影響他們的行為。
- **行銷情感**&#x200B;旨在刺激情緒，增強參與度和與品牌的聯絡。

GenStudio for Performance Marketing AI會通過分析文字的情緒提示、語調和敘述風格來偵測和區分這些特徵。 AI使用自然語言處理(NLP)和機器學習演演算法來識別模式，並根據預先定義的情感和說服屬性來分類文字。

### 敘事風格

敘事或上訴因素屬性有助於識別可傳達可與目標受眾產生共鳴的值、目的或身份的媒體。 下表列出GenStudio for Performance Marketing AI識別的敘述樣式。

| 上訴因數 | 說明 | 範例 |
| ----------------- | --------------------------------------------------------------------- | ------------------------------------------ |
| 真實性 | 真實與真實，經常強調透明與誠實。 | `A behind-the-scenes look at how our products are made.` |
| 慶祝 | 以歡樂和節日來紀念特殊場合或成就。 | `Join us in celebrating our 10th anniversary with special offers!` |
| 社群 | 培養群組的歸屬感和凝聚感。 | `Our brand is built on the strength of our community.` |
| 便利性 | 強調易用性和省時的優點。 | `Get what you need with just one click.` |
| 賦權 | 鼓勵並使個人能夠掌控局面並做出決策。 | `Empower yourself with our latest tools and resources.` |
| 探索 | 邀請探索和冒險，通常與新體驗相關聯。 | `Discover new horizons with our travel packages.` |
| 未來主義 | 強調創新與前瞻性思維。 | `Experience the future of technology today.` |
| 炒作 | 圍繞產品或事件產生興奮和期待。 | `Don't miss out on the most anticipated event of the year!` |
| 放任 | 吸引幻想、慾望或快樂。 | `Treat yourself to the finest gourmet chocolates.` |
| 完全安心 | 提供安心和安全性感。 | `Rest easy knowing your data is safe with us.` |
| 個人化 | 根據個人偏好設定量身打造體驗或產品。 | `Get a custom-fit solution just for you.` |
| 威望 | 與高地位和專屬性建立關聯。 | `Join the elite with our premium membership.` |
| 無時間 | 強調經久不衰的品質和經典魅力。 | `Our designs are timeless and never go out of style.` |
| 多功能 | 強調適應性和多重用途。 | `Our product fits seamlessly into any lifestyle.` |
| 福利 | 促進健康、快樂和整體健康。 | `Enhance your well-being with our holistic approach.` |

### 勸說策略

勸說技巧是用來影響消費者行為並驅動所需的動作。 這些策略會鎖定特定的心理觸發器和客戶區段，以提升行銷訊息的有效性。 下表列出GenStudio for Performance Marketing AI識別的說服策略。

| 策略 | 說明 | 範例 |
| --------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------- |
| 擬人 | 將人的特性歸因於產品或品牌。 | `Our friendly chatbot is here to help you.` |
| 比較 | 醒目提示選項之間的差異以影響選擇。 | `See how we compare to the competition.` |
| 具體 | 提供具體細節，讓訊息更清晰可見。 | `Save 20% on your next purchase.` |
| 簽署 | 獲得可靠來源或影響者的核准。 | `Recommended by top industry experts.` |
| 踏進門 | 從小型請求開始，以增加同意大型請求的可能性。 | `Try our free trial today.` |
| 克服電抗 | 承認並解決異議以降低阻力。 | `We understand your concerns, and here's how we address them.` |
| 互惠 | 提供有價值的東西以鼓勵回報優惠。 | `Get a free gift with your purchase.` |
| 稀缺 | 強調有限可用性，營造緊迫感。 | `Only a few items left in stock!` |
| 社交身分 | 運用消費者對群組的歸屬感。 | `Join our community of innovators.` |
| 社交影響 | 強調對社會或環境的正面影響。 | `Your purchase helps plant a tree.` |
| 社交校訂 | 使用口碑或使用者產生的內容來建立信任。 | `See why thousands of users love our product.` |

### 行銷情感

情緒是行銷訊息的目標，可喚起觀眾的特定情感和回應，這可能會增強與品牌的參與度和聯絡。 下表列出GenStudio for Performance Marketing AI識別的情緒。

| 情緒 | 說明 | 範例 |
| ------------- | --------------------------------------------------------------------------- | --------------------------------------------------------- |
| 抱負 | 激發達成或獲得更高成就的慾望。 | `Imagine the possibilities with our premium service.` |
| 挑戰 | 鼓勵受眾克服障礙或接受新任務。 | `Are you ready to take the next step in your career?` |
| 好奇 | 激起進一步瞭解的興趣和渴望。 | `Discover the secrets behind our success.` |
| 排他性 | 建立屬於選取群組的感覺。 | `Join our exclusive club for members-only benefits.` |
| 迷戀 | 使用有趣或令人興奮的內容吸引受眾。 | `Be amazed by our latest innovations.` |
| 滿足感 | 提供使用產品或服務的滿意度和樂趣。 | `Enjoy the ultimate comfort with our luxury bedding.` |
| 認可 | 認可和評估受眾的成就或狀態。 | `Get the recognition you deserve with our award-winning service.` |
| 信任 | 在品牌中建立信心和可靠性。 | `Trust us to deliver quality and excellence every time.` |
| 急迫性 | 強調時效性高的機會以立即採取行動。 | `Act now before this limited-time offer expires!` |

## 可讀性分數

可讀性評分會評估一段文字閱讀和理解的難易程度。 這可協助確保您的內容適合您的目標對象。 分數取決於多種因素，包括句子長度和字詞複雜度。 下表列出GenStudio for Performance Marketing AI辨識的可讀性等級。

| 可讀性層級 | 說明 | 範例 |
| ------------------- | ------------------------------------------------------------------ | --------------------------------------------------------- |
| 5年級 | 非常簡單的語言，適合幼童使用。 | `The cat sat on the mat.` |
| 6年級 | 簡單清晰的語言，適合一般受眾。 | `You can find great deals on our website.` |
| 7年級 | 簡單易懂，辭彙和結構簡單明瞭。 | `Our new product is simple to use and very effective.` |
| 八年級和九年級 | 簡潔明瞭，適合青少年使用。 | `This guide will help you understand the basics of our service.` |
| 10至12年級 | 更複雜的語言，適用於較年長的青少年和成年人。 | `The comprehensive manual provides detailed instructions for setup.` |
| 大學 | 進階語言，適用於受過良好教育的對象。 | `The study explores the multifaceted implications of the new policy.` |
| 大學畢業生 | 高度進階的語言，適合專家和專家使用。 | `The dissertation delves into the intricacies of quantum mechanics.` |

## 計數

瞭解並利用主題標籤計數、字數、句子計數和停用字數等計數屬性，可大幅提升您的內容策略。 這些量度可讓您深入瞭解行銷工作的效益和觸及範圍。 下表列出GenStudio for Performance Marketing AI識別的計數類別。

| 類別 | 說明 | 範例 |
| --------------------- | --------------------------------------------------------------------------- | --------------------- |
| 表情符號計數 | 文字中出現的emoji數目。 表情符號可以提升參與度，並快速傳達情感。 | `😊`, `🚀`, `❤️` |
| 雜湊標籤計數 | 文字中使用的雜湊標籤數量。 雜湊標籤有助於分類內容並提高在社群媒體上的可發現性。 | `#Marketing`、`#Sale` |
| 每句字數計數 | 文字中每句的平均字數。 較短的句子通常更容易閱讀和理解。 | `10` |
| 字數 | 文字中的字數總計。 較高的字數可提供較詳細的資訊，但可能需要較多的努力才能閱讀。 | `1500 words` |
| 停用字比率 | 停用字與文字中有意義字的比率。 搜尋查詢和結果中通常會忽略停用詞（例如「a」、「an」、「the」）。 停用詞比率高可能會讓內容變得不那麼吸引人且不易閱讀。 | `0.375` |
| 句數計數 | 文字中的句子總數。 更多的句子可以表示更詳細的內容，但過長的文字可能會失去讀者的興趣。 | `75 sentences` |
