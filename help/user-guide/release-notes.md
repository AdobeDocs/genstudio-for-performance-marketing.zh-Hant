---
title: Adobe GenStudio for Performance Marketing發行說明
description: 了解 Adobe GenStudio for Performance Marketing 的最新功能和增強功能。
recommendations: noDisplay
exl-id: 32f5104e-ae15-4092-8a34-642fc641baf9
source-git-commit: 958ad60d1d9a88e0dd4cba0decf8da8bc398d542
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 2%

---

# GenStudio for Performance Marketing發行說明

此版本資訊詳細說明GenStudio for Performance Marketing應用程式的最新更新。

## 2024.11.14 {#latest}

### 新功能

新增對多媒體範本的支援，讓客戶能夠重複使用已透過其自有受管內容頻道發佈的資產。<!-- GS-6107 -->

### 修正和增強功能

* 在用來產生初始內容的瀏覽器以外的瀏覽器中調整大小時，草稿現在會如預期般載入。<!-- GS-7204 -->

* 所有字元現在以匯出的HTML正確表示。<!-- GS-7246 -->

* 在某些語言中，[!DNL Content] _體驗_ **[!UICONTROL 匯出]**&#x200B;快顯視窗上的按鈕不再被截斷。<!-- GS-6873 -->

* 以大小為50x50的範本所建立的顯示廣告，現在會以預期的影像大小匯出。 以前，匯出的PNG檔案會以預期尺寸的兩倍匯出。<!-- GS-7192 -->

* 現在已解決調整顯示廣告大小時發生的範本錯誤。<!-- GS-7322 -->

### 本地化

此版本包含整個UI本地化的改良功能，包括：

* [!DNL Content] _上傳資產_&#x200B;快顯視窗的所有字串現在都已正確本地化。<!-- GS-6872 6770 -->
* [!DNL Content] _Assets_&#x200B;檢視&#x200B;**[!UICONTROL 搜尋]**&#x200B;欄位中的所有工具提示都已當地語系化。<!-- GS-6879 -->
* 取代[!DNL Create]畫布上電子郵件變體中的現有影像時，_從內容選取_&#x200B;檢視現已當地語系化。<!-- GS-6906 -->

## 2024.11.07

### 修正和增強功能

* 當使用者按一下&#x200B;**[!UICONTROL 上傳新影像]**，然後在上傳完成前取消作業時，_儲存進行中_&#x200B;旋轉圖示不再顯示。<!-- GS-6780 -->

* 體驗標題現在會在體驗重新產生期間正確建立。<!-- GS-7006 -->

* 已解決草稿載入期間卷軸閃爍的問題。<!-- GS-5587 -->

* [!DNL Content] _新增您核准的範本_&#x200B;快顯視窗中的`View documentation`連結現在可如預期運作。<!-- GS-6881 -->

* 在調整大小作業期間從提示抽屜中刪除影像不再導致錯誤。<!-- GS-7115 7009 -->

* 從[!DNL Create]動作功能表選取&#x200B;**[!UICONTROL 刪除]** (...)現在可如預期運作。<!-- GS-6871 -->

* 使用者現在可以單獨透過鍵盤控制所有中繼廣告範本互動元素。<!-- GS-4066 -->

* 新增從範本影像欄位提取影像尺寸至顯示廣告範本的功能。 智慧型裁切請求現在會針對影像的實際維度傳送，而非針對整個範本。 <!-- GS-6926 -->

* 已本地化產生的電子郵件和中繼廣告中的`Zoom to fit to screen`字串。<!-- GS-5063 -->

* 當使用者按一下離開時，[!DNL Create]提示抽屜現在會如預期關閉。<!-- GS-5254 -->

* 中繼廣告匯出現在會如預期包含所選的行動號召標籤。<!-- GS-6504 -->

* 品牌分數現在會更新並如預期保留再生體驗。<!-- GS-6535 -->

* 中繼廣告和顯示廣告的HTML匯出不再包含包裝函式`div`和`chrome`元素。<!-- GS-7116 -->

* 發佈期間電子郵件草稿呈現的問題現已解決。<!-- GS-6394 -->

* 未產生品牌分數時，畫布&#x200B;**[!UICONTROL 品牌]**&#x200B;按鈕現在會停用。<!-- GS-6429 -->

* 啟用`ReadOnly`畫佈設定時，「畫布」動作列上的Facebook/Instagram切換現在會依預期更新體驗呈現。<!-- GS-7039 -->

#### 影像重新產生

* 調整多個中繼廣告變體的大小現在可以如預期運作。 之前，「畫布」不會顯示重新產生的變體，但會保持空白。<!-- GS-7010 -->

* 片段重新產生現在對調整大小的體驗如預期般運作。<!-- GS-6836 -->

* 重新產生中繼廣告影像後，重新調整影像大小不會再產生錯誤。 先前，在重新產生之前調整影像大小會將頻道中繼資料從`meta`變更為`facebook`。<!-- GS-7042 -->

## 2024.10.31

### 新功能

* **[!DNL Content]**&#x200B;搜尋篩選器現在支援依顏色標籤搜尋。<!-- GS-5501 -->

* **[!DNL Create]**&#x200B;畫布現在會顯示電子郵件片段的字元計數。<!-- GS-5819 -->

### 修正和增強功能

* 已新增遺失的熒幕閱讀器標籤至行動裝置和案頭`view`元素。<!-- GS-5624 4729 -->

* **[!DNL Create]**&#x200B;畫布電子郵件主旨行和標題前文字區域的高度現在為動態的。<!-- GS-6258 -->

* 電子郵件框線的配置問題已解決。<!-- GS-6631 -->

* 鍵盤焦點現在在&#x200B;**[!DNL Content]** **[!UICONTROL 刪除]**&#x200B;按鈕上按預期運作。 之前，鍵盤無法連線或操作此按鈕。  <!-- GS-4065 -->

## 2024.10.14全面發佈

此發行版本介紹Adobe GenStudio for Performance Marketing，這是一個創作AI型應用程式，可加速行銷活動的規劃、開發和分析。 GenStudio for Performance Marketing可讓行銷團隊針對廣告、電子郵件和行銷活動建立品牌內多頻道內容，同時提供即時深入分析以最佳化內容效能。

### 功能

主要產品功能包括：

**[!DNL Create]**&#x200B;推出了Canvas，提供結構化的提示體驗，讓內容編輯人員快速產生內容和變體。 系統管理員會根據組織品牌指導方針來訓練產品。 [!DNL Create]可確保所有AI產生的內容都符合您的品牌准則（品牌、客戶角色和產品說明），並簡化產生高影響力、品牌一致的行銷內容。

**[!DNL Content]**&#x200B;個儲存已監管、符合品牌規範的核准資產和體驗。 GenStudio for Performance Marketing使用者可輕鬆尋找、編輯、重新調整用途和共用已核准資產，減少為每個行銷活動從頭開始重新建立內容的需求。

**[!DNL Reviews and Approvals]**&#x200B;建立了架構，讓利害關係人在儲存至&#x200B;**[!DNL Content]**&#x200B;或匯出之前，先檢閱及核准產生的變體。

**[!DNL Campaigns]**&#x200B;組織並管理行銷活動，確保簡化執行和追蹤。 共同作業人員可將行銷活動視覺化、規劃及追蹤，以有效管理多個方案並確保及時傳送。

**[!DNL Insights]**&#x200B;提供內容績效的即時評估，協助行銷人員最佳化其策略並做出資料導向式決策。

GenStudio for Performance Marketing與其他Adobe Experience Cloud產品整合，包括Adobe Express和AdobeAEM Assets。

### 其他資訊

請參閱下列實用資源：

* [Adobe GenStudio for Performance Marketing使用手冊](https://experienceleague.adobe.com/en/docs/genstudio/user-guide/home)

* [Adobe GenStudio Academy](https://learningmanager.adobe.com/genstudioacademy)，Adobe的線上學習平台，用於在創作過程中使用創作AI技術。
