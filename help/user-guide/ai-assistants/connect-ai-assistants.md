---
title: 连接AI助手
description: 了解如何将受支持的AI助手连接到[!DNL GenStudio for Performance Marketing]并验证对可用工具的访问权限。
role: User
source-git-commit: 6fb7ddb7549ea6bcd66b6139fbde9ebe12ddaa22
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 0%
---

# 连接AI助手

在查询性能数据、汇编草稿或发布批准的广告之前，将受支持的AI助手连接到[!DNL GenStudio for Performance Marketing]。 连接选项因AI助手和组织而异。

## 先决条件

在连接之前，请确认您拥有：

- 有权访问[!DNL GenStudio for Performance Marketing]的有效Adobe帐户。
- 一种受支持的计划，当您使用Claude、ChatGPT或Microsoft Copilot时，该计划允许远程MCP连接。 有关手动配置MCP连接的特定说明，请参阅AI助手文档。

## 连接Adobe CX Enterprise Coworker

在Adobe CX Enterprise Coworker中将[!DNL GenStudio for Performance Marketing]工具作为本机连接进行管理。 贵组织控制可用性，因此请勿输入直接MCP服务器URL。

开始新对话并[验证连接](#verify-the-connection)。 如果未显示这些工具，请联系贵组织的管理员或Adobe代表。

## 连接克劳德

Claude需要Pro 、 Max 、 Team或Enterprise计划。 相同的远程连接器在Web和桌面应用程序的Claude中工作。

1. 在Claude的左侧边栏中选择&#x200B;**[!UICONTROL 自定义]**。
1. 选择&#x200B;**[!UICONTROL 连接器]**，然后选择添加图标。
1. 选择&#x200B;**[!UICONTROL 添加自定义连接器]**。
1. 输入`https://genstudio-services.adobe.io/mcp`作为MCP服务器URL。
1. 使用您的Adobe ID登录。
1. 选择有权访问[!DNL GenStudio for Performance Marketing]的IMS组织。

> [!NOTE]
> 在团队或企业计划中，组织所有者可能需要先添加连接器。 如果连接器已经可用，请改为选择&#x200B;**[!UICONTROL 连接]**。

## 连接ChatGPT

ChatGPT需要Plus 、 Pro 、 Business 、 Enterprise或Education帐户。 可通过开发人员模式在Web上访问自定义MCP连接。

1. 在Web浏览器中登录到[ChatGPT](https://chatgpt.com)。
1. 打开&#x200B;**[!UICONTROL 设置]**，然后启用&#x200B;**[!UICONTROL 开发人员模式]**。
1. 在&#x200B;**[!UICONTROL 设置]**&#x200B;中，打开应用程序或连接器的区域。
1. 添加名为`GenStudio`的自定义MCP连接。
1. 输入`https://genstudio-services.adobe.io/mcp`作为MCP服务器URL。
1. 保留&#x200B;**[!UICONTROL OAuth]**&#x200B;作为身份验证方法。
1. 使用您的Adobe ID登录。
1. 选择有权访问[!DNL GenStudio for Performance Marketing]的IMS组织。

> [!NOTE]
> ChatGPT可以更改开发人员和连接器设置的位置。 如果帐户中的这些标签不同，请按照当前的OpenAI说明添加远程MCP连接器。

## 连接代码

Codex需要Codex命令行界面和经过身份验证的Codex帐户。

1. 为所有项目打开`~/.codex/config.toml`或为一个项目打开`.codex/config.toml`。
1. 添加此配置：

   ```toml
   [mcp_servers.genstudio]
   url = "https://genstudio-services.adobe.io/mcp"
   auth = "oauth"
   ```

1. 运行`codex mcp login genstudio`。
1. 在打开的浏览器窗口中使用Adobe ID登录。
1. 选择有权访问[!DNL GenStudio for Performance Marketing]的IMS组织。

## 连接编写器

Writer需要访问AI Studio。

1. 在Writer中，打开&#x200B;**[!UICONTROL AI Studio]**。
1. 选择&#x200B;**[!UICONTROL 连接器和工具]**。
1. 选择&#x200B;**[!UICONTROL 创建自定义连接器]**。
1. 选择&#x200B;**[!UICONTROL MCP服务器]**&#x200B;作为连接器类型。
1. 输入连接器的名称和说明。
1. 输入`https://genstudio-services.adobe.io/mcp`作为MCP服务器URL。
1. 设置连接器的组访问权限。
1. 选择&#x200B;**[!UICONTROL OAuth 2.0（用户级别）]**&#x200B;作为身份验证方法。
1. 使用您的Adobe ID登录。
1. 选择&#x200B;**[!UICONTROL 保存]**。

[!DNL GenStudio for Performance Marketing]工具显示在AI Studio工具库中。 每个Writer用户都使用单独的Adobe ID登录。

## 连接Microsoft Copilot

Microsoft控制Copilot中自定义MCP连接的设置流程。 按照当前[Microsoft Copilot文档](https://learn.microsoft.com/en-us/copilot/)添加远程MCP服务器，然后使用`https://genstudio-services.adobe.io/mcp`作为服务器URL。

出现提示时，请使用您的Adobe ID登录并选择有权访问[!DNL GenStudio for Performance Marketing]的IMS组织。

## 验证连接

安装后，确认工具可用。

1. 在AI助手中开始新对话。
1. 询问助理可以访问哪些[!DNL GenStudio for Performance Marketing]工具。
1. 确认响应中列出了分析、创建和激活中的工具。
1. 询问连接的付费媒体渠道的性能摘要。

该助理会返回可用的性能数据，或解释为何没有数据与请求匹配。

> [!TIP]
> 如果身份验证失败，请重新连接，并确认您选择了正确的IMS组织。 如果未显示工具，请确认您的帐户有权访问[!DNL GenStudio for Performance Marketing]。

## 相关功能

- [AI助理概述](overview.md)
- [使用AI助理](use-ai-assistants.md)
- [AI助手工具参考](tools-reference.md)
