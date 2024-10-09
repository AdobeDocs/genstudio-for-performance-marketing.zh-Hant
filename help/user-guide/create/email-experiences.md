---
title: 電子郵件體驗
description: 瞭解Adobe GenStudio for Performance Marketing中的電子郵件體驗。
feature: Experiences, Content Generation, Create, Generative AI, Variant Generation
role: User
level: Beginner
source-git-commit: 157aee296304c9aa1b8b86dc8905fe103fe4f83c
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---


# 電子郵件體驗

透過Adobe GenStudio for Performance Marketing，您可以使用創作AI來簡化[建立高影響力的電子郵件體驗](/help/user-guide/create/create-email-experience.md)。

[!DNL Create]可讓現代行銷人員使用[指南](/help/user-guide/guidelines/overview.md)、影像資產和[精心打造的提示](/help/user-guide/effective-prompts.md)，快速[建立符合品牌的電子郵件體驗](/help/user-guide/create/create-email-experience.md)。

電子郵件體驗的可編輯區段包括：

* 前置標題
* 標題
* 內文
* 行動號召(CTA)
* 影像
* 品牌標誌

請參閱[範本元素](/help/user-guide/content/use-templates.md#template-elements)。

<!-- ## Email capabilities

Content creators and marketers can produce brand-consistent email experiences in GenStudio for Performance Marketing. -->

## 多節電子郵件

電子郵件體驗可以包含多個區段，允許完全自訂以符合您的品牌和目標。 [為每個區段](/help/user-guide/create/create-email-experience.md#add-parameters)選取 [!DNL Products] 和視覺資產，並使用[結構化提示](/help/user-guide/effective-prompts.md#structured-prompts)製作獨特的內容。 每個區段支援一個視覺資產。

請參閱[準備電子郵件範本](/help/user-guide/content/email-template.md)以瞭解如何建立多節範本。

## 漸進式載入

內容產生程式開始時，電子郵件變體所產生內容的每個區段都會逐步載入畫布。 體驗、資產以及體驗中的欄位和區段會在產生時分別顯示在畫布中。

當您按一下&#x200B;**[!UICONTROL 產生]**&#x200B;時，畫布底部會顯示載入指示器，用於更新您的產生進度。

電子郵件體驗的每個欄位和區段都會依照此順序逐步載入：

1. 變體名稱
1. 所有變數的主旨列
1. 前置標題
1. 標題、電子郵件內文（適用於單一區段電子郵件）和行動號召
1. 後續章節的電子郵件內文（適用於多節電子郵件）
1. 進行品牌驗證程式，且&#x200B;[_品牌指引檢查_](/help/user-guide/guidelines/brand-validation.md#brand-guidelines-check)&#x200B;會針對每個變體填入。
