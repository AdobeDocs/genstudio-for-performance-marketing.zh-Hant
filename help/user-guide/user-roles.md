---
title: Adobe GenStudio for Performance Marketing使用者角色和許可權
description: 瞭解GenStudio for Performance Marketing使用者角色和許可權。
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
exl-id: 33ebcf9c-e5f8-4011-b449-5f73d151f221
source-git-commit: 8f8aa9b92a97d528e1dec6e183d0e4ea1e3a5bdc
workflow-type: tm+mt
source-wordcount: '1115'
ht-degree: 1%

---

# 使用者角色和許可權

建立和部署現代行銷活動需要具有不同責任和技能的利害關係人之間的合作。 _使用者角色_&#x200B;可控制利害關係人對GenStudio for Performance Marketing許多功能的存取權。 您指派的使用者角色會決定您可以使用此平台執行的工作。 Adobe系統管理員會將您指派給Adobe Admin Console中GenStudio產品設定檔的角色。 您的歡迎電子郵件會識別您指派的角色。

>[!NOTE]
>
>在將任何使用者布建到這些角色之前，必須在Adobe Admin Console中指定Adobe系統管理員以執行一次性設定任務。 此Adobe管理員角色僅能在Adobe Admin Console的環境中運作。 它在GenStudio for Performance Marketing平台介面中沒有任何角色。 需要系統管理員許可權的Adobe系統管理員必須在Adobe Admin Console中將自己布建為GenStudio系統管理員。 請參閱[布建GenStudio for Performance Marketing](product-provisioning.md)。

## Adobe系統管理員與GenStudio系統管理員

這些使用者角色標題看起來可能類似，但它們可識別在不同環境中提供許可權的唯一角色。

**Adobe系統管理員**&#x200B;在Adobe Admin Console中擁有超級使用者許可權，並執行所有使用者管理工作，例如新增或刪除使用者。 此系統管理員角色未提供GenStudio for Performance Marketing應用程式中的許可權，這說明了為何Adobe系統管理員不需要GenStudio的授權。 Adobe系統管理員通常會使用Admin Console在GenStudio部署中新增和刪除使用者帳戶，並從個別使用者或使用者群組中指派或移除權益或許可權。

**GenStudio系統管理員**&#x200B;是GenStudio for Performance Marketing中的超級使用者，但沒有在Adobe Admin Console中執行工作的許可權。 此系統管理員角色需要Genstudio產品授權，而且它對應至[Adobe GenStudio for Performance Marketing產品說明](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html)中的超級使用者。 GenStudio系統管理員擁有GenStudio for Performance Marketing功能的完整權利，包括[!DNL Brands]、[!DNL Persona]以及[!DNL Product]建立、刪除、更新和發佈。 [Adobe GenStudio for Performance Marketing產品說明](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html)說明GenStudio使用者角色與產品授權的關係。

請參閱&#x200B;_企業和團隊管理指南_&#x200B;中的[管理角色](https://helpx.adobe.com/enterprise/using/admin-roles.html#enterprise)。

## 權益

_權益_&#x200B;授予執行特定工作及存取受保護資源的許可權。 權利或許可權在產品設定檔中的使用者角色中定義，使用者在指派給該角色時會收到這些權利。

>[!IMPORTANT]
>
>請勿新增、編輯或刪除現有的產品設定檔。 變更預設產品設定檔可能會嚴重干擾您的GenStudio for Performance Marketing部署。

## 使用者角色

三種GenStudio for Performance Marketing使用者角色型別可支援這種組織角色的多樣性。 權益會針對這些使用者型別量身打造，並支援行銷組織中每個使用者的責任。 這三種使用者角色型別為：

* **GenStudio編輯器**&#x200B;使用GenStudio for Performance Marketing的創作AI功能來建立行銷活動資產、要求內容稽核和核准，以及發佈此內容的已核准草稿。 當資產的編輯者將資產儲存至[!DNL Content]後，所有GenStudio for Performance Marketing使用者都可以存取及使用資產。 GenStudio編輯器是GenStudio for Performance Marketing的超級使用者。

* **GenStudio共同作業人員**&#x200B;是範圍最廣的GenStudio for Performance Marketing使用者。 共同作業人員可以檢視及核准內容，並且是工作流程的重要一環，可確保您產生的內容符合組織的需求和標準。 GenStudio共同作業人員是GenStudio for Performance Marketing中的&#x200B;_共同作業人員使用者_。

* **GenStudio系統管理員**&#x200B;在GenStudio for Performance Marketing中擁有最廣泛的權益或許可權集。 系統管理員執行基本入門任務，為行銷活動資產建立和部署建立基本護欄。 系統管理員透過上傳品牌和組織特定資訊（例如[品牌准則](./guidelines/overview.md)）來實作這些護欄。 系統管理員擁有建立和發佈[!DNL Brands]的許可權，但沒有使用者管理許可權。 GenStudio系統管理員是GenStudio for Performance Marketing的超級使用者。

### GenStudio編輯器

_編輯器_&#x200B;或內容建立者擁有建立GenStudio for Performance Marketing [!DNL Brands]、[!DNL Campaigns]和[!DNL Content]資產所需的核心許可權。 這些進階使用者也可以編輯和刪除已建立的資產。 GenStudio for Performance Marketing支援快速建立數百個內容。 這些使用者可以產生內容片段或完整體驗，以協調核准內容的分散片段，以滿足特定行銷活動的需求。

編輯人員透過&#x200B;_提示_&#x200B;與GenStudio for Performance Marketing產生AI技術互動。 「畫布」中的提示抽屜提供工具，可在特定行銷活動指引的內容中放置提示。 因此，產生內容的品質和成功部分取決於貴組織上傳的品牌指引品質和提示的特定性。 請參閱[撰寫有效的提示](effective-prompts.md)。

下表顯示預設的編輯器許可權：

| 功能 | 建立 | 更新 | 刪除 | 檢視 |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | 否 | 否 | 否 | 是 |
| [!DNL Campaigns] | 是 | 是 | 是 | 是 |
| [!DNL Content] | 是 | 是 | 是 | 是 |
| [!DNL Create] | 是 | 是 | 是 | 是 |
| [!DNL Insights] | 只能設定聯結器 |    |     | 是 |
| [!DNL Personas] | 是 | 是* | 是* | 是 |
| [!DNL Products] | 是 | 是* | 是* | 是 |
| [!DNL Reviews and approvals] | 是 | 是 | 是 | 是 |
| [!DNL Templates] | 否 | 否 | 否 | 是 |

編輯人員可以編輯和刪除他們建立的[!DNL Personas]和[!DNL Products]。

GenStudio系統管理員可授予編輯者編輯及刪除[!DNL Brand]的許可權。

### GenStudio共同作業人員

_共同作業人員_&#x200B;可以在GenStudio for Performance Marketing中檢視資產，但無法建立、編輯或刪除這些資產。 共同作業人員包括對內容的稽核和核准流程成功至關重要的利害關係人，但他們不需要建立或直接編輯內容。 法律專家與創意人員經理是潛在共同作業人員的範例。 GenStudio for Performance Marketing共同作業人員可能擁有在其他Creative Cloud產品中建立和檢視資產的許可權。

下表顯示預設的Collaborator許可權：

| 功能 | 建立 | 更新 | 刪除 | 檢視 |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | 否 | 否 | 否 | 是 |
| [!DNL Campaigns] | 否 | 否 | 否 | 是 |
| [!DNL Content] | 否 | 否 | 否 | 是 |
| [!DNL Create] | 否 | 否 | 否 | 是 |
| [!DNL Insights] | 否 | 否 | 否 | 是 |
| [!DNL Personas] | 否 | 否 | 否 | 是 |
| [!DNL Products] | 否 | 否 | 否 | 是 |
| [!DNL Reviews and approvals] | 否 | 否 | 否 | 是 |
| [!DNL Templates] | 否 | 否 | 否 | 是 |

### GenStudio系統管理員

_GenStudio系統管理員_&#x200B;在GenStudio for Performance Marketing中有最強大的許可權集。 這些進階使用者會執行重要的入門任務，建立行銷活動資產建立和部署的基本護欄。 系統管理員透過上傳品牌和組織特定資訊（例如[品牌准則](./guidelines/overview.md)）來實作這些護欄。 系統管理員擁有建立和發佈[!DNL Brands]的許可權，但沒有使用者管理許可權。

下表顯示預設的系統管理員許可權：

| 功能 | 建立 | 更新 | 刪除 | 檢視 |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | 是 | 是 | 是 | 是 |
| [!DNL Campaigns] | 是 | 是 | 是 | 是 |
| [!DNL Content] | 是 | 是 | 是 | 是 |
| [!DNL Insights] | 是 | 是 | 是 | 是 |
| [!DNL Personas] | 是 | 是 | 是 | 是 |
| [!DNL Products] | 是 | 是 | 是 | 是 |
| [!DNL Reviews and approvals] | 是 | 是 | 是 | 是 |
| [!DNL Templates] | 是 | 是 | 是 | 是 |

系統管理員也可以上傳範本。

請參閱[開始使用Adobe GenStudio for Performance Marketing](get-started.md)，以取得初步設定工作的概觀。
