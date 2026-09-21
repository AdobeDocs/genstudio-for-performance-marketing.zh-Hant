---
title: 連線AI助理
description: 瞭解如何將支援的AI助理連線到[!DNL GenStudio for Performance Marketing]並驗證對可用工具的存取權。
role: User
source-git-commit: 6fb7ddb7549ea6bcd66b6139fbde9ebe12ddaa22
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 0%
---

# 連線AI助理

在您查詢效能資料、組合草稿或發佈核准的廣告之前，請將支援的AI助理連線到[!DNL GenStudio for Performance Marketing]。 連線選項因AI助理和組織而異。

## 先決條件

連線之前，請確認您擁有：

- 可存取[!DNL GenStudio for Performance Marketing]的有效Adobe帳戶。
- 支援的計畫，可在您使用Claude、ChatGPT或Microsoft Copilot時允許遠端MCP連線。 請參閱AI助理檔案，以取得手動設定MCP連線的具體指示。

## 連線Adobe CX Enterprise Coworker

在Adobe CX Enterprise Coworker中將[!DNL GenStudio for Performance Marketing]工具管理為原生連線。 您的組織控制可用性，因此您不需要輸入直接MCP伺服器URL。

開始新的交談，並[驗證連線](#verify-the-connection)。 如果工具未出現，請聯絡貴組織的管理員或Adobe代表。

## 連結Claude

Claude需要Pro、Max、Team或Enterprise計畫。 相同的遠端聯結器可在網頁和案頭應用程式的Claude中運作。

1. 在Claude中，選取左側邊欄中的&#x200B;**[!UICONTROL 自訂]**。
1. 選取&#x200B;**[!UICONTROL 聯結器]**，然後選取新增圖示。
1. 選取&#x200B;**[!UICONTROL 新增自訂聯結器]**。
1. 輸入`https://genstudio-services.adobe.io/mcp`作為MCP伺服器URL。
1. 使用您的Adobe ID登入。
1. 選取可存取[!DNL GenStudio for Performance Marketing]的IMS組織。

&#x200B;> [!NOTE]
&#x200B;> 在團隊或企業計畫中，組織所有者可能需要先新增聯結器。 如果聯結器已經可用，請改為選取&#x200B;**[!UICONTROL 連線]**。

## 連線ChatGPT

ChatGPT需要Plus、Pro、Business、Enterprise或Education帳戶。 自訂MCP連線可在網頁上透過開發人員模式取得。

1. 在網頁瀏覽器中登入[ChatGPT](https://chatgpt.com)。
1. 開啟&#x200B;**[!UICONTROL 設定]**，然後啟用&#x200B;**[!UICONTROL 開發人員模式]**。
1. 在&#x200B;**[!UICONTROL 設定]**&#x200B;中，開啟應用程式或聯結器的區域。
1. 新增名為`GenStudio`的自訂MCP連線。
1. 輸入`https://genstudio-services.adobe.io/mcp`作為MCP伺服器URL。
1. 保留&#x200B;**[!UICONTROL OAuth]**&#x200B;作為驗證方法。
1. 使用您的Adobe ID登入。
1. 選取可存取[!DNL GenStudio for Performance Marketing]的IMS組織。

&#x200B;> [!NOTE]
> ChatGPT可以變更開發人員和聯結器設定的位置。 如果帳戶中的這些標籤不同，請依照目前的OpenAI指示新增遠端MCP聯結器。

## 連線字典

Codex需要Codex命令列介面和已驗證的Codex帳戶。

1. 為所有專案開啟`~/.codex/config.toml`，或為一個專案開啟`.codex/config.toml`。
1. 新增此設定：

   ```toml
   [mcp_servers.genstudio]
   url = "https://genstudio-services.adobe.io/mcp"
   auth = "oauth"
   ```

1. 執行`codex mcp login genstudio`。
1. 在開啟的瀏覽器視窗中使用您的Adobe ID登入。
1. 選取可存取[!DNL GenStudio for Performance Marketing]的IMS組織。

## 連線寫入器

Writer需要存取AI Studio。

1. 在Writer中，開啟&#x200B;**[!UICONTROL AI Studio]**。
1. 選取&#x200B;**[!UICONTROL 聯結器和工具]**。
1. 選取&#x200B;**[!UICONTROL 建立自訂聯結器]**。
1. 選取&#x200B;**[!UICONTROL MCP伺服器]**&#x200B;作為聯結器型別。
1. 輸入聯結器的名稱和描述。
1. 輸入`https://genstudio-services.adobe.io/mcp`作為MCP伺服器URL。
1. 設定聯結器的群組存取權。
1. 選取&#x200B;**[!UICONTROL OAuth 2.0 （使用者層級）]**&#x200B;做為驗證方法。
1. 使用您的Adobe ID登入。
1. 選取&#x200B;**[!UICONTROL 「儲存」]**。

[!DNL GenStudio for Performance Marketing]工具出現在AI Studio工具庫中。 每個Writer使用者都會使用個別Adobe ID登入。

## 連線Microsoft Copilot

Microsoft可控制Copilot中自訂MCP連線的設定流程。 依照目前的[Microsoft Copilot檔案](https://learn.microsoft.com/en-us/copilot/)新增遠端MCP伺服器，然後使用`https://genstudio-services.adobe.io/mcp`做為伺服器URL。

出現提示時，請使用您的Adobe ID登入，並選取有權存取[!DNL GenStudio for Performance Marketing]的IMS組織。

## 驗證連線

設定後，確認工具可供使用。

1. 在您的AI助理中開始新交談。
1. 詢問助理可以存取哪些[!DNL GenStudio for Performance Marketing]工具。
1. 確認回應中列出了「見解」、「建立」和「啟動」的工具。
1. 要求連線付費媒體頻道的效能摘要。

助理會傳回可用的效能資料，或說明為何沒有資料符合要求。

&#x200B;> [!TIP]
&#x200B;> 如果驗證失敗，請重新連線，並確認您選取正確的IMS組織。 如果未顯示工具，請確認您的帳戶可以存取[!DNL GenStudio for Performance Marketing]。

## 相關功能

- [AI助理概述](overview.md)
- [使用AI助理](use-ai-assistants.md)
- [AI助理工具參考](tools-reference.md)
