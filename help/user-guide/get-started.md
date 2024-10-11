---
title: 開始使用Adobe GenStudio for Performance Marketing
description: 瞭解如何設定GenStudio for Performance Marketing以產生新的品牌一致行銷內容。
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
exl-id: bcb03198-bbcb-45ae-af01-25c1e834b563
source-git-commit: 449c212ab167a6c126492e9becedf9318bfe08ee
workflow-type: tm+mt
source-wordcount: '1128'
ht-degree: 1%

---

# 開始使用Adobe GenStudio for Performance Marketing

Adobe GenStudio for Performance Marketing是建立、評估及管理行銷體驗的綜合平台，可反映並遵循您的品牌識別。

利害關係人對其許多功能的存取權由指派的&#x200B;_使用者角色_&#x200B;控制。 您指派的使用者角色會決定您可以在GenStudio for Performance Marketing中執行的工作。 Adobe系統管理員會在Adobe Admin Console的GenStudio for Performance Marketing產品設定檔中指派您的許可權。 您的歡迎電子郵件會識別您指派的角色。

如果您是創作AI型工具的新手，或只是對GenStudio for Performance Marketing核心原則有好奇，請參閱[概念](concepts.md)和[撰寫有效提示](effective-prompts.md)。

## 使用者角色

建立和部署現代行銷活動需要具有不同責任和技能的利害關係人之間的合作。

三種GenStudio for Performance Marketing使用者角色型別可支援這種組織角色的多樣性。 許可權會針對每個使用者型別量身打造，並支援行銷組織中每個使用者的職責。

**三種使用者角色型別為**：

* **編輯器**&#x200B;使用GenStudio for Performance Marketing generative AI功能來建立行銷活動資產、要求內容稽核和核准，以及發佈此內容的已核准草稿。 當資產的建立者將資產儲存至內容後，所有GenStudio for Performance Marketing使用者都可存取和使用資產。

* **共同作業人員**&#x200B;是GenStudio for Performance Marketing使用者最廣泛的範圍。 共同作業人員可以檢視及核准內容，並且是工作流程的重要一環，可確保您產生的內容符合組織的需求和標準。

* **系統管理員**&#x200B;在GenStudio for Performance Marketing中擁有最廣泛的許可權集。 系統管理員執行基本入門任務，為行銷活動資產建立和部署建立基本護欄。 系統管理員透過上傳品牌和組織特定資訊（例如[品牌准則](/help/user-guide/guidelines/overview.md)）來實作這些護欄。 GenStudio for Performance Marketing系統管理員擁有建立和發佈品牌的許可權，但沒有使用者管理許可權。

>[!NOTE]
>在將任何使用者布建到這些角色之前，必須在Adobe Admin Console中指定Adobe系統管理員以執行一次性設定任務。 此Adobe管理員角色僅能在Adobe Admin Console的環境中運作。 它在GenStudio for Performance Marketing平台介面中沒有任何角色。

### GenStudio for Performance Marketing編輯器

**編輯器**&#x200B;具有建立GenStudio for Performance Marketing [!DNL Brands]、[!DNL Campaigns]和[!DNL Content]資產所需的核心許可權。 他們也可以編輯和刪除已建立的資產。 GenStudio for Performance Marketing支援快速建立數百個內容。 這些使用者可以產生內容區段或完整體驗，以協調核准內容的分散片段，以滿足特定行銷活動的需求。

編輯人員透過&#x200B;_提示_&#x200B;與GenStudio for Performance Marketing產生AI技術互動。 「畫布」中的提示抽屜提供工具，可在特定行銷活動指引的內容中放置提示。 因此，產生內容的品質和成功部分取決於貴組織上傳的品牌指引品質和提示的特定性。

請參閱[撰寫有效的提示](effective-prompts.md)。

下表顯示預設的編輯器許可權：

| 功能 | 建立 | 更新 | 刪除 | 檢視 |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | 否 | 否 | 否 | 是 |
| [!DNL Campaigns] | 是 | 是 | 是 | 是 |
| [!DNL Content] | 是 | 是 | 是 | 是 |
| [!DNL Insights] | 僅可設定廣告聯結器 |    |     | 是 |
| [!DNL Personas] | 是 | 是 | 是 | 是 |
| [!DNL Products] | 是 | 是 | 是 | 是 |
| [!DNL Reviews and approvals] | 是 | 是 | 是 | 是 |

### GenStudio for Performance Marketing共同作業人員

**共同作業人員**&#x200B;可以在GenStudio for Performance Marketing中檢視資產，但無法建立、編輯或刪除這些資產。 共同作業人員包括對內容的稽核和核准流程成功至關重要的利害關係人，但他們不需要建立或直接編輯內容。 潛在共同作業人員的範例包括法律專家與創作者的經理。 GenStudio for Performance Marketing共同作業人員可能有權在其他Creative Cloud產品中建立和檢視資產。

下表顯示預設的Collaborator許可權：

| 功能 | 建立 | 更新 | 刪除 | 檢視 |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | 否 | 否 | 否 | 是 |
| [!DNL Campaigns] | 否 | 否 | 否 | 是 |
| [!DNL Content] | 否 | 否 | 否 | 是 |
| [!DNL Insights] | 否 | 否 | 否 | 是 |
| [!DNL Personas] | 否 | 否 | 否 | 是 |
| [!DNL Products] | 否 | 否 | 否 | 是 |
| [!DNL Reviews and approvals] | 否 | 否 | 否 | 是 |

### GenStudio for Performance Marketing系統管理員

**GenStudio系統管理員**&#x200B;會完成初始工作，讓您的組織準備好部署GenStudio for Performance Marketing。

下表顯示預設的GenStudio for Performance Marketing系統管理員許可權：

| 功能 | 建立 | 更新 | 刪除 | 檢視 |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | 是 | 是 | 是 | 是 |
| [!DNL Campaigns] | 是 | 是 | 是 | 是 |
| [!DNL Content] | 是 | 是 | 是 | 是 |
| [!DNL Insights] | 是 | 是 | 是 | 是 |
| [!DNL Personas] | 是 | 是 | 是 | 是 |
| [!DNL Products] | 是 | 是 | 是 | 是 |
| [!DNL Reviews and approvals] | 是 | 是 | 是 | 是 |


## 準備GenStudio for Performance Marketing以產生內容

GenStudio for Performance Marketing系統管理員準備組織的GenStudio for Performance Marketing環境，以供編輯和共同作業人員建立行銷活動資產。 這些初步設定工作包括：

1. [為[!DNL Brands]、[!DNL Products]和[!DNL Personas]新增准則](./guidelines/overview.md)。 設定組織品牌識別的重要建置組塊，是建立者和共同作業人員工作的必要先決條件。 您可以上傳品牌指引檔案或手動輸入品牌資訊。
   * **準備您的指引檔案**。 品牌指引的描述性越強、內容越全面，輸出效果就越好。 加入您視為品牌重要功能的簡短範例，並新增要從內容建立中排除的行為說明。 GenStudio for Performance Marketing會從這些上傳的檔案中擷取資訊，並開始建立您的品牌。 品牌聲音、管道和影像指引等資訊會填入，因為GenStudio for Performance Marketing會從您上傳的檔案中組合每個指引。
   * **視需要編輯或完成品牌指引欄位**。 完整的品牌指引是GenStudio for Performance Marketing瞭解您組織品牌的基礎。 GenStudio for Performance Marketing從品牌指引檔案中擷取所需的資訊後，系統會提示您手動編輯或完成擷取資訊的欄位。 新增[!DNL Product]，指定內容建立的個別產品焦點區域。 [!DNL Personas]指引可協助針對已定義的客戶區段量身打造內容建立。

   雖然設定組織的品牌指引可能是一次性動作，但您可能需要根據組織的波動、成長和不斷變化的市場環境修訂和增強這些指引。

1. **[上傳範本](./content/use-templates.md)**。 範本提供捷徑並加速內容建立。 範本包含核准的功能（例如頁首和頁尾），並建立內容建立的護欄。 系統管理員通常會上傳和管理其組織的範本。 建立者使用範本，在組織品牌的既定界限內快速啟動內容建立流程。

1. **[上傳已核准的資產](./content/manage-assets.md)**。 [!DNL Content]中已核准的資產可供所有GenStudio for Performance Marketing建立者使用。 您可以用建立者可用來建立新體驗或資產的資產來植入[!DNL Content]。

1. **[連線至中繼(Facebook)帳戶](./insights/connect-channel.md)**。 設定GenStudio for Performance Marketing與貴組織社交帳戶之間的連線，以接收來自作用中行銷活動、資產和體驗的資料。 [[!DNL Insights]](./insights/overview.md)提供工具來分析管道衍生的資料。
