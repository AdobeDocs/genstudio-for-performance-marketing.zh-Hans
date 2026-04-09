---
title: 适用于GenStudio的Marketo
description: 安装和配置适用于GenStudio Adobe Exchange的Marketo应用程序，以便您的组织可以在GenStudio for Performance Marketing中使用Marketo Engage模板。
feature: Extensibility
source-git-commit: 4118624b479905cd2f2193d542c000678daaf4b8
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 0%

---

# 适用于GenStudio的Marketo

在同一[!DNL IMS]组织中使用[!DNL Marketo Engage]和[!DNL GenStudio for Performance Marketing]的组织可以从[!DNL Adobe Exchange]安装GenStudio的&#x200B;**Marketo**&#x200B;应用程序。 系统管理员批准应用程序并完成部署后，作者可以在GenStudio中创建电子邮件体验时选择Marketo模板，并选择直接上传到[!DNL Content]的模板旁边。

本主题适用于安装应用程序、从Marketo收集凭据并在Exchange中部署应用程序的&#x200B;**管理员**。 有关AJO和Marketo模板语法如何与GenStudio配合使用的信息，请参阅[AJO和Marketo中的模板](/help/user-guide/templates/use-templates.md#templates-from-ajo-and-marketo)。

## 先决条件

* 必须在部署扩展的组织中配置[!DNL Marketo Engage]。
* 部署该应用程序的用户需要&#x200B;**Marketo凭据**。 若要创建和检索这些凭据，您必须具有&#x200B;**Marketo产品管理员**&#x200B;访问权限（打开Marketo时，**[!UICONTROL 管理员]**&#x200B;区域必须可用）。

## 从Adobe Exchange安装应用程序

>[!VIDEO](https://video.tv.adobe.com/v/3483299?learn=on)

1. 打开[Adobe Exchange](https://exchange.adobe.com)并转到&#x200B;**[!UICONTROL Experience Cloud]**。
1. 打开[Marketo for GenStudio](https://exchange.adobe.com/apps/ec/ab6p21vo8r/marketo-for-genstudio)列表。
   Adobe Exchange上的![Marketo for GenStudio列表](/help/extensibility/marketo-adobe-exchange.png){width="75%"}
1. 选择&#x200B;**[!UICONTROL 免费]**&#x200B;为您的组织请求应用。
1. 在您的组织&#x200B;**审核并批准**&#x200B;请求后，继续[获取Marketo凭据](#get-marketo-credentials)和[从Exchange部署应用程序](#deploy-the-application-from-exchange)。

## 获取Marketo凭据

您使用的是来自&#x200B;**Marketo**&#x200B;实例（而非Adobe Developer Console）的凭据。 在Exchange中部署之前，请收集以下信息。

### 创建仅限API的用户（如果重用现有API用户，则可选）

1. 在Marketo中，转到&#x200B;**[!UICONTROL 管理员]**。
1. 在&#x200B;**[!UICONTROL 安全性]**&#x200B;下，打开&#x200B;**[!UICONTROL 用户和角色]**。
1. 对于新API用户，单击&#x200B;**[!UICONTROL 创建仅API用户]** （对每个API用户使用唯一的电子邮件）。 分配&#x200B;**[!UICONTROL API角色（所有工作区）]**&#x200B;角色（或您的组织所需的角色）。 如果您已有要使用的API用户，请跳至[创建或选择LaunchPoint服务](#create-or-select-a-launchpoint-service)。

![用户和角色具有仅API用户和API角色](/help/extensibility/marketo-users-roles-api-user.png){width="80%"}

### 创建或选择LaunchPoint服务

1. 在&#x200B;**[!UICONTROL 管理员]**&#x200B;中，在&#x200B;**[!UICONTROL 集成]**&#x200B;下，打开&#x200B;**[!UICONTROL LaunchPoint]**。
1. 单击&#x200B;**[!UICONTROL 创建]**以创建新服务（或使用现有的自定义服务）。
   ![LaunchPoint自定义服务](/help/extensibility/marketo-launchpoint-custom-service.png){width="80%"}
1. 对于您的服务，请单击&#x200B;**[!UICONTROL 查看详细信息]**&#x200B;并复制&#x200B;**[!UICONTROL 客户端ID]**&#x200B;和&#x200B;**[!UICONTROL 客户端密钥]**。 您将在Adobe Exchange **[!UICONTROL 配置]**&#x200B;中输入这些内容。

### 记下Marketo REST API基本URL

1. 在&#x200B;**[!UICONTROL 管理员]**&#x200B;中，在&#x200B;**[!UICONTROL 集成]**&#x200B;下，打开&#x200B;**[!UICONTROL Web服务]**。
1. 找到&#x200B;**[!UICONTROL REST API]**&#x200B;终结点。 仅复制&#x200B;**基本URL** （主机），格式为`https://###-XXX-###.mktorest.com`。 请&#x200B;**不**&#x200B;包含路径区段，如`/rest`或`/identity`。 此值在每个Marketo实例中是唯一的。

![Web服务REST API终结点基本URL](/help/extensibility/marketo-web-services-rest-endpoint.png){width="80%"}

您还将需要Exchange部署屏幕请求的&#x200B;**[!UICONTROL Marketo Engage标识URL]**，以及REST基本URL和LaunchPoint的客户端ID和客户端密钥。

## 从Exchange部署应用程序

要使扩展在GenStudio中可用，请从Adobe Exchange部署应用程序。

1. 返回至[Adobe Exchange](https://exchange.adobe.com)。
1. 选择&#x200B;**[!UICONTROL 管理]**，然后打开适用于GenStudio **应用程序的** Marketo（例如，在&#x200B;**[!UICONTROL App Builder应用程序]**&#x200B;下或您组织的托管应用程序下）。
1. 在&#x200B;**[!UICONTROL 环境]**&#x200B;下，从下拉列表中选择一个现有环境，或选择&#x200B;**[!UICONTROL 添加环境]**&#x200B;以创建环境。
1. 为所选环境打开&#x200B;**[!UICONTROL 配置]**。
1. 输入来自[LaunchPoint](#create-or-select-a-launchpoint-service)的&#x200B;**[!UICONTROL 客户端ID]**&#x200B;和&#x200B;**[!UICONTROL 客户端密钥]**、**[!UICONTROL Marketo Engage标识URL]**&#x200B;和&#x200B;**[!UICONTROL Marketo Engage REST API基本URL]**（来自[Web服务](#note-your-marketo-rest-api-base-url)的基本主机）。
1. 单击&#x200B;**[!UICONTROL 部署]**。 部署成功后，操作将更改为&#x200B;**[!UICONTROL 取消部署]**。

### 更新配置

要更改环境的配置值，请先&#x200B;**[!UICONTROL 取消部署]**，更新字段，然后重新&#x200B;**[!UICONTROL 部署]**。

## 访问GenStudio中的Marketo模板

安装和配置Marketo for GenStudio后，当您在GenStudio中创建&#x200B;**电子邮件**&#x200B;体验时，会显示&#x200B;**[!UICONTROL Marketo模板]**&#x200B;选项卡。 使用该选项卡浏览Marketo Engage中的模板。

>[!IMPORTANT]
>
>在GenStudio for Performance Marketing中的&#x200B;**标准电子邮件**&#x200B;体验流下创建电子邮件。 此集成不支持使用新电子邮件编辑器体验创建的电子邮件。

使用Marketo凭据的![Exchange配置](/help/extensibility/marketo-exchange-configuration.png){width="80%"}

## 故障排除

### Marketo“模板”选项卡不可见

* 确认该应用在Exchange中是&#x200B;**已批准**，并且环境是&#x200B;**已部署**，具有有效的客户端ID、客户端密钥和Marketo基本URL。
* 请要求您的管理员验证在创建凭据时是否使用了&#x200B;**Marketo产品管理员**&#x200B;访问权限。

### 未加载模板

* 重新加载页面或注销并重新登录到GenStudio。
* 在浏览器开发人员工具&#x200B;**[!UICONTROL 网络]**&#x200B;面板中，查找对您的Marketo实例的失败API调用，并验证REST基本URL是否与Marketo中的&#x200B;**[!UICONTROL Web服务]**&#x200B;匹配（主机后面没有额外路径）。
