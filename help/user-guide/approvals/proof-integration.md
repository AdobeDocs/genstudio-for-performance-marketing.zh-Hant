---
title: Workfront Proof與檢閱和核准整合
description: Workfront Proof與Adobe GenStudio for Performance Marketing整合。
feature: Content Review, Content Management
exl-id: 149db773-4787-4cfb-b29e-c49f13abf39a
source-git-commit: 47195c08f500e50a01db127c6badc461c10afaf9
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# Workfront Proof與GenStudio for Performance Marketing整合

與Workfront Proof的整合透過進階功能（包括核准範本、多階段工作流程，以及[比較校訂版本](https://experienceleague.adobe.com/zh-hant/docs/workfront/using/workfront-proof/work-with-proofs-in-wf-proof/review-proofs-web-proofing-viewer/compare-proofs)的功能）增強了GenStudio for Performance Marketing檢閱和核准生命週期。 此結構化版本設定可確保透明度、責任感，並在整個內容檢閱生命週期中簡化共同作業。

>[!BEGINSHADEBOX]

**必要條件**：

安裝[Adobe Workfront Web Viewer擴充功能](https://experienceleague.adobe.com/zh-hant/docs/workfront/using/review-and-approve-work/proofing/review-proofs-in-workfront/review-a-proof/review-proof-in-web-viewer-extension)

>[!ENDSHADEBOX]

Workfront Proof的[!DNL Proofing Viewer]是供檢視、評論和比較校訂的豐富工作區。 從[!DNL Proofing Viewer]，您可以

* 比較不同版本的內容
* 在校訂中新增註解與繪圖示示
* 核准證明

當您在核准要求電子郵件或產品內通知中按一下校訂URL時，[!DNL Proofing Viewer]會載入。 [!DNL Proofing Viewer] _我的新核准_&#x200B;檢視開啟。 從這個檢視中，您可以使用核心[!DNL Proofing Viewer]註解工具檢閱內容並提供註解。

若要結束[!DNL Proofing Viewer]，請按一下&#x200B;**[!UICONTROL 返回GenStudio]**。

## Genstudio for Performance Marketing和Workfront Proof：功能比較

下表比較了GenStudio for Performance Marketing的標準稽核與核准功能，以及透過Workfront Proof整合提供的更進階功能。

| 功能        | GenStudio for Performance Marketing                                                                 | Workfront Proof                                                                 |
|-------------------------------|------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|
| **草稿/校訂生命週期**        | 草稿內容在發佈時過期。 | 具有時間戳記的永久性記錄的多階段角色型核准鏈。<br>所有版本都會無限期保留。 |
| **個註解**                | 評論會繫結至草稿ID，並在發佈後捨棄。                                           | 持續性註釋和註解會保留以供稽核和法規遵循。     |
| **版本**           | 會將草稿視為不重複例項。<br>沒有並排比較。                                      | 完整版本控制，提供並排和覆蓋比較工具。        |
| **專案管理** | 基本行銷活動管理。 | 完整的行銷活動生命週期管理，包括自訂、範本、報告和詳細稽核。 |

### 授權和使用者角色

授權可識別產品中的一組使用者權益。 Workfront Proof比GenStudio for Performance Marketing提供更多的授權型別或使用者角色。 [校訂角色概觀](https://experienceleague.adobe.com/zh-hant/docs/workfront/using/review-and-approve-work/proofing/proofing-overview/proof-roles)介紹與Workfront Proof檢閱及核准工作流程相關的使用者角色。

| GenStudio for Performance Marketing授權       | Workfront授權                 | 說明                                                                                                                                                      |
|---------------------------------------------------|-----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| GenStudio系統管理員                          | Workfront管理員/超級使用者 | 完整存取GenStudio效能行銷功能，例如品牌、角色和產品管理。 管理工作流程與設定。 建立核准範本。 |
| 內容建立者和編輯者（超級使用者授權）   | 校訂建立者（標準授權）  | 產生並提交內容草稿。 在校訂檢視器中，上傳資產和起始校訂。 需要Workfront Proof授權。                              |
| 檢閱者/核准者（Collaborator授權）        | 檢閱者/核准者                 | 參與多階段稽核、新增註解，以及核准或拒絕內容。                                                                             |

Adobe系統管理員在Adobe Admin Console中管理這兩種產品的使用者布建和權益。

>[!NOTE]
>
> Workfront Proof提供[個額外的使用者角色](https://experienceleague.adobe.com/zh-hant/docs/workfront/using/review-and-approve-work/proofing/proofing-overview/proof-roles)。 並非所有角色都可見於效能行銷內部。 不過，系統會遵循Workfront Proof範本中設定的任何角色。

### 草稿和校樣

Workfront [!DNL Proofing Viewer]利用更結構化的檢閱和核准功能，延伸GenStudio for Performance Marketing的基本檢閱和核准流程。 在此整合中檢閱的校訂限於GenStudio for Performance Marketing支援的格式。

### 版本控制

GenStudio for Performance Marketing不支援核准範本，但Workfront Proof支援。 Proof的版本設定功能大幅增強了GenStudio的內容檢閱和核准程式。 校訂工作流程中的每個提交都會被視為內容草稿或&#x200B;_校訂_&#x200B;的不同版本。 校訂會自動儲存，並可和先前的版序並排比較。 利害關係人可以追蹤變更、提供精確意見回饋，並在整個稽核週期中維持一致性。 校訂會保留所有評論、決定和版本的完整歷史記錄，支援稽核整備和合規性要求。 每個版本也支援以角色為基礎的多階段核准工作流程，每個動作（核准、拒絕或評論）都有明確記錄和時間戳記。

### 核准範本

Workfront Proof核准範本提供預先格式化的步驟，可簡化校訂核准工作流程。 這些範本包括選定的稽核者和核准者、校訂角色和截止日期，以確保一致性和效率。 啟動稽核的內容建立者可以從一組預先定義的範本中選取單一階段和多階段核准工作流程。

工作流程範本的每個階段都會識別指派的稽核者。 來自Workfront Proof工作流程的所有狀態更新和註解都會顯示在校訂檢視器中，增加透明度和共同作業。

核准範本支援多階段核准，可協調不同利害關係人群組的審閱。

### 評論

檢閱者可以直接按一下校樣的特定區域，以留下精確的情境式評論。 所有註解都會加上時間戳記，並儲存為校樣版本歷史記錄的一部分。 GenStudio for Performance Marketing中沒有評論歷程記錄。

您可以[比較兩個版本的校訂](https://experienceleague.adobe.com/zh-hant/docs/workfront/using/workfront-proof/work-with-proofs-in-wf-proof/review-proofs-web-proofing-viewer/compare-proofs)，以評估稽核評論和內容。

## 通知和提醒

當新校訂可供檢閱或當進行中的檢閱已變更狀態時，檢閱者和核准者會收到電子郵件通知。
[校訂通知和提醒](https://experienceleague.adobe.com/zh-hant/docs/workfront/using/workfront-proof/proof-notifications-and-reminders/proof-notifications-and-reminders/proof-notifications-and-reminders)包含校訂的個人化連結、有關校訂及其通過核准程式進度的詳細資訊，以及版本設定資訊。
