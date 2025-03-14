---
title: 電子郵件體驗
description: 瞭解Adobe GenStudio for Performance Marketing中的電子郵件體驗。
feature: Experiences, Content Generation, Create, Generative AI, Variant Generation
role: User
level: Beginner
exl-id: e2bddd02-914e-43a8-92b6-fdcbced94a6a
source-git-commit: e4f552016fe17d2d7eb61792b62859475f107094
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# 電子郵件體驗

透過Adobe GenStudio for Performance Marketing，您可以使用創作AI來簡化[建立高影響力的電子郵件體驗](/help/user-guide/create/create-email-experience.md)。

[!DNL Create]可讓現代行銷人員使用[指南](/help/user-guide/guidelines/overview.md)、影像資產和[精心打造的提示](/help/user-guide/effective-prompts.md)，快速[建立符合品牌的電子郵件體驗](/help/user-guide/create/create-email-experience.md)。

產生中繼體驗時，四個變數會建立並顯示在畫布中。

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

請參閱[使用區段自訂範本](/help/user-guide/content/customize-template.md#sections-or-groups)，瞭解如何建立多區段範本。

## 漸進式載入

內容產生程式開始時，電子郵件變體所產生內容的每個區段都會逐步載入畫布。 體驗、資產以及體驗中的欄位和區段會在產生時分別顯示在畫布中。

當您按一下&#x200B;**[!UICONTROL 產生]**&#x200B;時，畫布底部會顯示載入指示器，用於更新您的產生進度。

電子郵件體驗的每個欄位和區段都會依照此順序逐步載入：

1. 變體名稱
1. 所有變數的主旨列
1. 前置標題
1. 標題、電子郵件內文（適用於單一區段電子郵件）和行動號召
1. 後續章節的電子郵件內文（適用於多節電子郵件）
1. 品牌驗證

   品牌驗證與內容檢查程式會進行，且每個變體會填入&#x200B;[_內容檢查_&#x200B;摘要](/help/user-guide/guidelines/brand-validation.md#content-check-summary)。

## 字元數

產生一組電子郵件變體後，您可以看到每個區段顯示的字元數。 將游標停留在產生的區段上或按一下該區段，例如主旨行或內文，然後檢視該區段的區段名稱和字元計數。

![字元計數](/help/assets/character-count.png){width="500" zoomable="yes"}
