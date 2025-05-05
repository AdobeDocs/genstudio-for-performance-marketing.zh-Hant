---
title: 影像功能
description: 瞭解GenStudio for Performance Marketing中使用的屬性類別的影像功能。
level: Intermediate
feature: Reporting and Insights, Image Attributes, Generative AI
exl-id: b7e3d202-4085-48a4-a6ba-c950dfd52233
source-git-commit: 0092458ae4f7e5ca5015a5b768ecfd70f8fcd7d8
workflow-type: tm+mt
source-wordcount: '1044'
ht-degree: 0%

---

# 影像功能

影像功能代表影像中用於[!DNL Insights]分析的不同資訊元素或模式。 這些功能有助於分類和瞭解視覺內容，實現更準確和詳細的深入分析。 藉由識別各種屬性，例如樣式、顏色和物件，AI可以提供影像的全面分析，以協助進行更好的決策和策略制定。

## 樣式偵測

判斷&#x200B;_影像樣式_&#x200B;可作為識別其他影像特性的基礎。 AI可套用適當的分析技術並辨識相關功能，進而對影像有更全面的瞭解。 每種風格都有獨特的視覺特性，會影響影像的感知和分析方式。

如果影像樣式識別為`photograph`，AI會分析`camera settings`、`camera proximity`和`Photography genres`的其他特徵。 這些特徵只適用於像片，可讓您更深入地瞭解影像的構成和品質。 檢視Adobe的&#x200B;_學習攝影_&#x200B;中的[28種攝影樣式](https://www.adobe.com/creativecloud/photography/discover/types-of-photography.html)，並了解熱門攝影型別和基本術語。

如果影像樣式被識別為`sketch`或`digital cartoon`，則可能會使用不同的特徵集。 這種階層式方法可確保分析在內容上準確，並根據所檢查的特定影像型別量身打造。

## 搜尋影像功能

**若要檢視特定屬性類別中的影像**：

1. 在&#x200B;_[!DNL Insights]_&#x200B;中，選取&#x200B;**[!UICONTROL 屬性]**&#x200B;檢視。

1. 選取&#x200B;**[!UICONTROL 影像]**&#x200B;以變更表格檢視。

1. 從&#x200B;**[!UICONTROL 屬性類別]**&#x200B;清單中選取影像功能，例如`Scenes`。

1. 選取屬性，以檢視共用該類別之影像的詳細資訊。

   例如，`Scenes`類別可以有`restaurant`做為屬性。

1. _屬性詳細資料_&#x200B;頁面列出具有此屬性的所有影像。

下表列出GenStudio for Performance Marketing AI識別的影像功能類別。 偵測到的媒體內容屬性清單並非詳盡無遺。 包含一組豐富功能的媒體，可能限於AI所識別的三個最主要功能。

<!-- For the writer: turn off word wrap to work with these tables. Option + Z -->

| 類別 | 說明 | 範例 |
| ----------------------- | ----------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 注意分佈 | 檢視者在影像上分散的注意力等級，表示影像不同區域可能獲得的焦點程度。 分佈越高表示沒有單一區域可主導檢視者的焦點，而分佈越低則表示一或兩個焦點可吸引檢視者的注意。 | `high`, `medium`, `low`<p>左側`low`分配與右側`high`分配的範例：<p>![低分佈和高分佈球賽](/help/assets/category/image-attn-lowhigh.png "低分佈和高分佈差異"){width="200" zoomable="yes"} |
| 攝影機角度 | 相機用來擷取主旨的角度，這會影響檢視者對影像的感知和詮釋。 如果影像樣式為`photograph`，則會識別此特徵。 | `Low angle`，`High angle`，`Eye level`，`Neutral angle`，`Bird's eye view`<p>`eye level`的範例：<p>![眼睛水準](/help/assets/category/image-camera-angle.png "不同角度坐著的人"){width="200" zoomable="yes"} |
| 相機設定 | 相機控制項的特定調整和組態會影響影像的最終外觀和品質。 如果影像樣式為`photograph`，則會識別此特徵。 | `Fast shutter speed`、`Long exposure`、`Bokeh blur`、`Motion blur`、`Tilt-shift blur`、`Flash`、`Wide-angle`、`Black and white`、`Double-exposure`、`Macro`、`Normal mode`<p>`macro`設定的範例：<p>![巨集特寫鏡頭](/help/assets/category/image-subject-distance.png "特寫花和珠寶蜜蜂的巨集設定"){width="200" zoomable="yes"} |
| 色彩和色調 | 影像中的顏色和色調品質。 在不同影像圖層中，從預先定義的40種顏色集合中識別最多三種顏色：<p>**[!UICONTROL 前景色彩]** — 影像正面圖層的色彩<br>**[!UICONTROL 背景色彩&#x200B;]**— 影像背面圖層的色彩 | 色彩值： `Red`、`Dark Red`、`Green`、`Bright Green`、`Dark Green`、`Light Green`、`Mud Green`、`Blue`、`Dark Blue`、`Light Blue`、`Royal Blue`、`Black`、`White`、`Off White`、`Gray`、`Dark Gray`、`Silver`、`Cream`、`Magenta`、`Cyan`、`Yellow`、`Mustard`、`Khaki`、`Brown`、`Dark Brown`、`Violet`、`Pink`、`Dark Pink`、`Maroon` `Tan`、`Purple`、`Lavender`、`Turquoise`、`Plum`、`Gold`、`Emerald`、`Orange`、`Beige`、`Lilac`、`Olive` |
| 色溫 | 說明影像中顏色的一般溫暖或冷度。 | 色調或溫度值： `warm`、`cool`、`neutral`<br>![色彩和冷色調](/help/assets/category/image-color-temp.png "色溫搭配冷色背景和多種色彩物件"){width="200" zoomable="yes"} |
| 內容密度 | 影像中視覺元素和細節的集中程度，表示有多少資訊封裝在視覺空間中。<p>不同於注意力分佈可測量檢視者焦點在影像不同區域的分佈情形，內容密度會專注於視覺資訊呈現的數量。 較高的內容密度表示有更多元素。 | `high`, `medium`, `low`<p>左側`low`密度和右側`high`密度的範例：<p>![低密度和高密度球賽](/help/assets/category/image-attn-lowhigh.png "低密度和高內容密度的差異"){width="200" zoomable="yes"} |
| 影像樣式 | 影像的視覺化處理，例如像片或素描。 一旦AI判斷出影像樣式，其他特徵即會被識別。 例如，如果影像是像片，則可能適用相機設定、相機鄰近度和照明條件。 | `Photograph`、`Photograph with text overlay`、`Sketch`、`Painting`、`Digital cartoon`、`Infographics`、`Graphic design`、`Collage`、`Software screenshot`<p>`digital cartoon`影像樣式範例![卡通影像樣式](/help/assets/category/image-style.png "貓的影像樣式卡通"){width="200" zoomable="yes"} |
| 照明條件 | 描述影像中光的品質和特性，影響其情緒、色調和可見度。 | `Golden hour`、`Blue hour`、`Midday`、`Overcast`、`Night`、`Daylighting`、`Incandescent`、`Fluorescent`、`Colorful`、`Studio`<p>`daylighting`條件的範例：<p>![在日光下的人行道上](/help/assets/category/image-lighting.png "日光下條件"){width="200" zoomable="yes"} |
| 物件 | 識別構成影像的一或多個專案、圖元和元素。 | 值太多，但某些範例包括： `backpack`、`book`、`hawk`、`glasses`、`fish`、`pencil`、`mountain bike`、`soap`<p>`toucan`和`bird`物件的範例：<p>![Bird， toucan物件](/help/assets/category/image-objects-bird.png "Toucan鳥物件的圖形設計"){width="200" zoomable="yes"} |
| 方向 | 相對於其寬度和高度的影像對齊方式。 偵測它是否比高（橫向）寬、比寬（縱向）高，或寬度和高度相等（正方形）。 | `landscape`, `portrait`, `square`<p>`square`方向的範例：<p>![方形草圖](/help/assets/category/image-orientation-square.png "方形定向花草圖"){width="200" zoomable="yes"} |
| 人員 | 當至少有一個人在場時，一個或多個屬性可以描述影像中的一個或多個人。 | `person`、`woman`、`man`、`girl`、`boy`、`social group`、`kid`、`crowd`、`people`<p>人員`woman`與`person`類別的範例：<p>![有攝影機的女性](/help/assets/category/image-people.png "管理攝影機的人員"){width="200" zoomable="yes"} |
| 攝影流派 | 偵測用於擷取影像的主旨和技術，例如`abstract`或`landscape` （與橫向不同）。 | `Architecture`、`Astro`、`Landscape`、`Pet`、`Interior`、`Wildlife`、`Night`、`Cityscape`、`Seascape`、`Underwater`、`Storm`、`Adventure sports`、`Fashion`、`Portrait`、`Sports`、`Food`、`Street`、`Event`、`Lifestyle`、`Commercial`、`Group`、`Abstract`、`Minimalist`、`Composite`、`Surreal` <p>檢視[攝影型別](https://www.adobe.com/creativecloud/photography/discover/types-of-photography.html)。 |
| 場景 | 識別影像中的設定或環境，提供有關影像擷取位置或描繪位置型別的內容。 | 值太多，但某些範例包括： `lake`、`underwater`、`highway`、`hill`、`log cabin`、`island`、`beach`、`lounge`<p>反映在頭盔上的範例`snow`、`sky`、`winter`和`mountain`場景：<p>![冬季雪景](/help/assets/category/image-scenes.png "冬天、雪天、天空和山地景物反射"){width="200" zoomable="yes"} |
| 主題距離 | 相機與影像主體之間的距離。 | `close up`, `mid shot`, `long shot`<p>`closeup shot`的範例：<p>![特寫鏡頭](/help/assets/category/image-subject-distance.png "特寫花和珠寶蜜蜂"){width="200" zoomable="yes"} |
| 樣式 | 偵測套用至影像元素的視覺化處理，例如Lightroom或Photoshop中使用的視覺化處理。 | `design`，`illustration`，`logo`，`square`，`cartoon`，`art`，`circle`，`circular`<p>`circular`樣式的範例：<p>![珊瑚礁的圓形閘道](/help/assets/category/image-styles-circular.png "珊瑚礁的圓形入口網站"){width="200" zoomable="yes"} |
| 標記 | 偵測不屬於特定分類的其他影像特性。 標籤提供有關影像的其他內容和中繼資料。 例如，AI可能偵測到影像中的`helmet`和`motorobike`物件，並將`riding`加入為標籤。 | 值太多，但某些範例包括： `construction`、`gothic`、`healing`、`military`、`selfie`、`football`、`typing`、`dancer`、`dancing`<p>`dancer`和`dancing`標籤的範例：<p>跳舞者和跳舞者的![標籤](/help/assets/category/image-tags.png "跳舞者"){width="200" zoomable="yes"} |
