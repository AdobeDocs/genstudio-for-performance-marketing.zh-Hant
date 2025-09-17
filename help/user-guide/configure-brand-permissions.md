---
title: 指派 [!DNL Brand] 許可權
description: 瞭解如何為GenStudio for Performance Marketing [!DNL Brand] 建立者和編輯者指派權益。
level: Intermediate
feature: Brand Personalization, Generative AI
exl-id: fc33ecd3-4403-4045-87af-012a0377226c
source-git-commit: adb1d34eb76d7594933fe9951c4c1885e6d6369b
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 1%

---

# 指派[!DNL Brand]許可權

依預設，GenStudio系統管理員可以建立和編輯[!DNL Brands]。 內容編輯者和共同作業人員角色具有編輯和建立許可權，但可能不需要任何系統管理許可權。

若要授予內容編輯者和共同作業人員這些[!DNL Brand]相關權益，Adobe系統管理員必須在Adobe Admin Console中執行一些額外的設定工作。 請參閱[企業和團隊管理指南](https://helpx.adobe.com/enterprise/using/admin-console.html#Overview)中的&#x200B;_Adobe Admin Console_。

新增使用者和使用者群組是所有具有透過Admin Console管理之權益的Adobe產品所共有的基本工作。 請參閱[企業與團隊管理指南](https://helpx.adobe.com/tw/enterprise/using/users.html)中的&#x200B;_Adobe Admin Console使用者_，以取得新增使用者和使用者群組的使用者管理與程式的概觀。

觀看此影片逐步解說或遵循以下步驟。

>[!VIDEO](https://video.tv.adobe.com/v/3474996?learn=on&enablevpops)

## 步驟1：建立使用者群組

**若要建立使用者群組**：

1. 登入Admin Console並導覽至&#x200B;**[!UICONTROL 使用者]** > **[!UICONTROL 使用者群組]**。

1. 按一下&#x200B;**[!UICONTROL 新增使用者群組]**。 _建立新使用者群組_&#x200B;快顯視窗隨即開啟。

1. 將資訊型使用者群組名稱新增至&#x200B;**[!UICONTROL 使用者群組名稱]**&#x200B;欄位，以識別新群組的用途。 例如，「品牌管理員」。

1. 選擇性地新增群組及其用途的說明。

1. 按一下「**[!UICONTROL 儲存]**」。Admin Console會開啟&#x200B;_新群組_&#x200B;快顯視窗，其中包含新建立群組的名稱。

請參閱[企業和團隊管理指南](https://helpx.adobe.com/tw/enterprise/using/user-groups.html)中的&#x200B;_管理使用者群組_。

## 步驟2：將GenStudio系統管理員設定檔指派給使用者群組

建立新的使用者群組並新增使用者後，您可以將&#x200B;**Adobe GenStudio系統管理員**&#x200B;設定檔指派給此群組。 與指派的設定檔相關聯的權益為此群組中的所有使用者GenStudio [!DNL Brands]許可權（建立、更新和刪除品牌）。

**若要將設定檔指派給使用者群組**：

1. 導覽至新建立的使用者群組，然後按一下「_已指派的產品設定檔_」標籤。

1. 從&#x200B;_指派的產品設定檔_&#x200B;索引標籤，按一下&#x200B;**[!UICONTROL 指派設定檔]**。 _指派產品和設定檔_&#x200B;快顯視窗隨即開啟。

1. 從`Adobe GenStudio`選取產品&#x200B;_清單中選取_。

1. 按一下&#x200B;**[!UICONTROL 套用]**。 _選取產品設定檔_&#x200B;快顯視窗隨即開啟，顯示與Adobe GenStudio相關聯的產品設定檔。

1. 選取`Adobe GenStudio system manager`。

1. 按一下&#x200B;**[!UICONTROL 套用]**。 _指派產品和設定檔_&#x200B;快顯視窗隨即開啟，顯示新建立的使用者群組的產品設定檔。

1. 按一下「**[!UICONTROL 儲存]**」。

請參閱[企業和團隊管理指南](https://helpx.adobe.com/tw/enterprise/using/user-groups.html)中的&#x200B;_將產品設定檔指派給使用者群組_。

## 步驟3：將使用者新增至使用者群組

若要指派建立、編輯和發佈[!DNL Brands]的使用者許可權，請將他們新增至新建立的使用者群組。

>[!NOTE]
>
>您必須先將至少一個使用者新增至此使用者群組，才能將群組新增至專案。

**若要將使用者新增至使用者群組**：

1. 從&#x200B;_Admin Console_，瀏覽至&#x200B;**[!UICONTROL 使用者]** > **[!UICONTROL 使用者群組]**。

1. 選取您先前建立的使用者群組名稱。 _新增使用者到此使用者群組_&#x200B;快顯視窗開啟。

1. 透過使用者名稱或電子郵件地址新增新的或現有的使用者。 當您輸入現有使用者的名稱或電子郵件地址時，此欄位會自動填入屬於此IMS組織的已知使用者的相符名稱。 瞭解如何在[企業和團隊管理指南](https://helpx.adobe.com/tw/enterprise/using/user-groups.html)的&#x200B;_管理使用者群組_&#x200B;中管理使用者群組。

使用者新增至群組時，會獲得Adobe GenStudio系統管理員的[!DNL Brand]建立、編輯和發佈許可權。 使用者也會收到編輯Adobe GenStudio for Performance Marketing [!DNL Brands]專案的自動電子郵件邀請。

## 步驟4：建立[!DNL Brands]專案

_專案_&#x200B;提供儲存位置，讓選取的使用者可以儲存資產，在此案例中為[!DNL Brands]個資產。

**若要從[!DNL Brands]儲存體&#x200B;_標籤_建立**&#x200B;專案：

1. 導覽至Admin Console中的&#x200B;_儲存空間_&#x200B;索引標籤。

1. 按一下側面導覽中的&#x200B;**[!UICONTROL 專案]**。 _專案_&#x200B;索引標籤開啟。

1. 按一下&#x200B;**[!UICONTROL 建立專案]**。 _新專案_&#x200B;快顯視窗開啟。

1. 在專案名稱欄位中輸入`Adobe GenStudio Brands`。 輸入此專案名稱，與這裡顯示完全相同。 請勿包含額外的空格或變更字母大小寫。

1. 按一下 **[!UICONTROL 建立]**。_邀請加入專案_&#x200B;快顯視窗開啟。

請參閱[企業和團隊管理指南](https://helpx.adobe.com/enterprise/using/projects-in-business-storage.html)中的&#x200B;_管理專案_。

## 步驟5：邀請使用者群組加入專案

您現在已準備好將您剛才建立的使用者群組新增至`Adobe GenStudio [!DNL Brands]`專案。

**若要邀請使用者群組加入新建立的專案**：

1. 從&#x200B;_邀請加入專案_&#x200B;快顯視窗，將您剛建立的使用者群組新增至此專案。

1. 選擇&#x200B;**可以編輯**&#x200B;許可權選項。

1. 按一下&#x200B;**[!UICONTROL 邀請]**。
