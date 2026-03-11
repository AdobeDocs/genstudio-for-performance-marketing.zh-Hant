---
title: Adobe GenStudio for Performance Marketing概念
description: 瞭解Adobe GenStudio for Performance Marketing概念和術語。
feature: Generative AI
role: User
exl-id: 7dd00b4c-f429-499b-851d-3606c82c09dc
TQID: https://experienceleague.adobe.com/i3VF7S-ndAMDoF1akF3l20tStW-IPS--MSysxD-MArc
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7id: c5a86ad9-9158-4ab1-a7ea-9e29985087b8id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12id: c95c94c1-727b-457a-9184-a4dda4c95ab2id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: f71bd2fc-e9ca-4cb6-8088-82e250211e32id: f912fa8d-7beb-4468-9ea7-1c0f198b59ef
subfeature_v2: id: a98e0185-3180-4e8c-8f31-f72af4cc21a2id: be495d08-ecd1-455f-951e-c22de504e667id: dd48f9df-f2e2-49fe-a918-332a8e240ffeid: e3878dde-4b87-4290-9e81-ed7ee6eb83feid: ec92a2bc-afe3-4ff0-a985-0c8ef22b4da0id: f54ee13b-9545-4d68-9842-a12026e60aaf
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: c7d04a2c-412a-4c9d-9d7a-4456eaa5adebid: cdd65e7e-8839-44a2-bc21-0e03623b5dd1id: e1e0219c-f879-479f-8427-888ed2a6e9c2id: eb30f47f-d87a-400f-8f78-63ce7979ff56
source-git-commit: 242ab858144fd152fd55645143f869fddf7b6fe0
workflow-type: tm+mt
source-wordcount: 754
ht-degree: 0%

---

# 概念

GenStudio for Performance Marketing是獨立企業產品，其中包含Adobe的內容supply chain，可簡化行銷活動。 大規模建立個人化、品牌核准的內容、監控成效，以及快速適應不斷變化的市場，這些都是極具挑戰性的工作。 GenStudio for Performance Marketing將Creative Cloud和Experience Cloud整合在一個應用程式中，該應用程式利用創作AI作為企業行銷團隊的效能倍增器。

透過GenStudio for Performance Marketing，您可以：

* 針對您最優先的數位頻道，使用自然語言提示來建立品牌內內容，例如付費媒體、電子郵件和顯示廣告

* 與利害關係人共同作業，檢閱及核准產生的內容
* 儲存產生和核准的內容，以存取未來的行銷活動
* 透過分析資產績效和識別績效最佳內容的關鍵屬性來評估內容有效性

## Generative AI技術

GenStudio for Performance Marketing運用創作AI的強大功能，加速內容建立流程，並確保產生高品質的內容。 創意資產的反複生命週期會產生日益準確且符合品牌標準的內容，以便與目標受眾產生共鳴。

透過強大的品牌指南功能，從擷取您組織的品牌、客戶角色和產品說明開始。 請參閱[指引概述](../user-guide/guidelines/overview.md)，瞭解如何準備並上傳這些指引。

{{in-academy}}

### 大型語言模型

GenStudio for Performance Marketing運用Adobe的創作AI平台，該平台提供基礎AI和機器學習(ML)服務。 此平台可簡化大型語言模型(LLM)的使用，讓Adobe的GenAI功能能夠建立吸引人的體驗。

GenStudio for Performance Marketing透過Azure OpenAI使用GPT系列的協力廠商LLM。<!-- Claude, and Gemini models. -->

## [!DNL Generative Actions]

_[!DNL Generative Actions]_(如[Adobe GenStudio for Performance Marketing產品說明](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html)中所定義)是量化GenStudio for Performance Marketing內產生式AI功能之使用的單位。

<!-- 
Add example about usage mode?
Where users check how many generative actions they have left
How they re-up their genactions
If genactions roll over month to month or not 
-->

### 費率

您會收到[GenStudio for Performance Marketing產品說明](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html)中所述的[!DNL Generative Actions]預設配額。

>[!NOTE]
>
>使用率可能有所不同。 計畫可能會有變動。 如需更新的費率資訊，請參閱[Adobe GenStudio for Performance Marketing產品說明](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html)。

下列函式以指定的速率使用[!DNL Generative Actions]。

| 函數 | 產生式動作率 |
| -----------------------  | ------------------ |
| 建立電子郵件 | 每代5個 |
| 建立付費媒體廣告 | 每代5個 |
| 建立顯示廣告 | 每代5個 |
| 重新產生截面 | 每代1個 |

<!-- 
| Generate on-brand images | 1 per prompt  |
| Translation              | 1 per prompt  |
| Video: ADLS              | 1 per prompt  |
| Video: TTS + Avatar      | 1 per prompt  | 
-->

[!DNL Generative Actions] _未在下列情況下使用_：

* 在產生變體期間使用[品牌驗證](/help/user-guide/guidelines/brand-validation.md)
* 正在從[上傳的准則](/help/user-guide/guidelines/add-guidelines.md)擷取資訊
* 手動[重新檢查變體](/help/user-guide/guidelines/brand-validation.md#improve-brand-alignment)
* 數位資產會自動使用屬性([[!DNL Insights]](/help/user-guide/insights/overview.md))標籤

>[!TIP]
>
>如果您超過[!DNL Generative Actions]的權益，您可以直接向帳戶代表購買更多產品。

## 資料控管

使用AI產生內容時，必須確保輸出安全且包容所有使用者。 這需要評估內容中潛在的有害偏見、仇恨言論、冒犯性材料或褻瀆行為。 Adobe從多個角度徹底測試內容產生技術、執行全面的道德審查，並實施有效的緩解計畫，以防止有害內容出現在輸出中。

此方法可強化社會責任、降低聲譽風險，並確保遵守[Adobe的信任與安全及道德政策](https://www.adobe.com/content/dam/cc/en/ai-ethics/pdfs/Adobe-AI-Ethics-Principles.pdf)。

GenStudio for Performance Marketing納入緩解計畫，以防止根據Adobe資料治理標準和政策使用已識別的有害或偏見內容。 偵測到這類內容時，系統會使用「無法產生」訊息封鎖資產產生作業。

出現此訊息時，您可以編輯提示，並再試一次&#x200B;_或_&#x200B;標示提示內容以供GenStudio for Performance Marketing檢閱。 系統會收集標示為要複查之內容的提示資料，以供內部複查之用。

## 內容生命週期

對於以更快的速度在多個管道提供高品質體驗的需求很高。 GenStudio for Performance Marketing為行銷人員將內容supply chain簡化為妥善組織的工作流程。 GenStudio for Performance Marketing在生命週期的每個階段都運用Adobe技術。

<table style="table-layout:auto">

<tr style="border: 0;">

    <td>

       <p><strong>工作流程與規劃</strong></p>

    </td>

    <td>

        <p>集思廣益、定義指引，並圍繞內容建立策略以吸引受眾。</p>

    </td>

</tr>

<tr style="border: 0;">

    <td>

        <p><strong>建立與生產</strong></p>

    </td>

    <td>

        <p>根據計畫產生內容。 即時共同作業、接收意見回饋、進行編輯並核准內容。</p>

    </td>

</tr>

<tr style="border: 0;">

    <td>

        <p><strong>內容管理</strong></p>

    </td>

    <td>

        <p>在集中式存放庫中儲存、共用和尋找創意資產。 根據效能重新使用和振興內容。</p>

    </td>

</tr>

<tr style="border: 0;">

    <td>

        <p><strong>傳遞與啟用</strong></p>

    </td>

    <td>

        <p>啟用內容並跨多個行銷管道發佈。</P>

    </td>

</tr>

<tr style="border: 0;">

    <td>

        <p><strong>報告與深入分析</strong></p>

    </td>

    <td>

        <p>收集資料並取得資產效能最佳化的深入分析。</p>

    </td>

</tr>

</table>
