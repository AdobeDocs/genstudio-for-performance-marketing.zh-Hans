---
title: 适用于GenStudio的Journey Optimizer
description: 安装和配置适用于GenStudio Adobe Exchange的Journey Optimizer应用程序，以便您的组织可以在GenStudio for Performance Marketing中使用Adobe Journey Optimizer模板。
feature: Extensibility
source-git-commit: fbec4567d960a6e3607c5e5e43057e2f22e9f6ea
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 0%

---

# 适用于GenStudio的Journey Optimizer

在同一[!DNL IMS]组织中使用[!DNL Adobe Journey Optimizer] (AJO)和[!DNL GenStudio for Performance Marketing]的组织可以从[!DNL Adobe Exchange]安装适用于GenStudio **应用程序的** Journey Optimizer。 系统管理员批准应用程序并完成部署后，作者可以在GenStudio中创建电子邮件体验时选择AJO内容模板，并选择直接上传到[!DNL Content]的模板旁边。

本主题适用于安装应用程序、在[!DNL Adobe Developer Console]中创建OAuth凭据以及在[!DNL Adobe Experience Platform]中映射技术帐户权限的&#x200B;**管理员和开发人员**。 有关AJO和Marketo模板语法如何与GenStudio配合使用的信息，请参阅[AJO和Marketo中的模板](/help/user-guide/templates/use-templates.md#templates-from-ajo-and-marketo)。

## 先决条件

* 必须在部署扩展的组织中配置AJO。
* 在AJO中创作模板的用户需要拥有在Journey Optimizer中&#x200B;**创建和编辑**&#x200B;内容模板的权限，具体如您的组织所定义。
* AJO中的电子邮件模板必须包含所生成内容应显示的字段占位符（手柄栏）。 可以选择不包含这些字段的模板，但如果缺少占位符[!DNL GenStudio for Performance Marketing]所需的占位符，则&#x200B;**体验生成失败**。 请参阅[自定义模板](/help/user-guide/templates/customize-template.md)和[可识别的字段名称](/help/user-guide/templates/customize-template.md#recognized-field-names)。

## 从Adobe Exchange安装应用程序

>[!VIDEO](https://video.tv.adobe.com/v/3483287?learn=on)

1. 打开[Adobe Exchange](https://exchange.adobe.com)并转到&#x200B;**[!UICONTROL Experience Cloud]**。
1. 打开[Journey Optimizer for GenStudio](https://exchange.adobe.com/apps/ec/abpopqqr1q/journey-optimizer-for-genstudio)列表。
   Adobe Exchange上的![Journey Optimizer for GenStudio列表，包括要求和免费安装](/help/extensibility/ajo-adobe-exchange.png){width="75%"}
1. 选择&#x200B;**[!UICONTROL 免费]**&#x200B;为您的组织请求应用。
1. 在您的组织&#x200B;**审核并批准**&#x200B;请求后，继续[在Adobe Developer Console中创建OAuth凭据](#create-oauth-credentials-in-adobe-developer-console)和[从Exchange部署应用程序](#deploy-the-application-from-exchange)。

## 在Adobe Developer Console中创建OAuth凭据

在[Adobe Developer Console](https://developer.adobe.com/console/)中创建一个&#x200B;**项目**，以提供Journey Optimizer API的OAuth凭据。 在Exchange中配置应用程序时，您将需要&#x200B;**客户端ID**、**客户端密钥**、**组织ID**&#x200B;和&#x200B;**作用域**&#x200B;之类的值。

1. 登录到Adobe Developer Console并创建&#x200B;**新项目**。
1. 通过单击&#x200B;**[!UICONTROL 添加API]**&#x200B;并从&#x200B;**[!DNL Experience Cloud]**&#x200B;产品API列表中选择&#x200B;**[!UICONTROL Adobe Journey Optimizer]**，将&#x200B;**Adobe Journey Optimizer (AJO) API**&#x200B;添加到项目中。
1. 在项目工作区中生成凭据，并复制&#x200B;**客户端ID**、**客户端密钥**、**组织ID**、**作用域**&#x200B;以及部署流要求的任何其他值。 安全地保存它们以供下一节使用。

>[!NOTE]
>
>从Exchange安装时，如果同时显示了OAuth客户端ID和技术帐户ID，请使用&#x200B;**OAuth客户端ID**。

## 从Exchange部署应用程序

### 在管理中打开应用程序并添加环境

1. 返回至[Adobe Exchange](https://exchange.adobe.com)。
1. 选择&#x200B;**[!UICONTROL 管理]**&#x200B;并打开&#x200B;**[!UICONTROL App Builder应用程序]**（或您的组织到托管应用程序的路径）。
1. 为GenStudio **选择** Journey Optimizer，并确认该应用程序已获得&#x200B;**批准**。
1. 在&#x200B;**[!UICONTROL 环境]**&#x200B;下，从&#x200B;**环境：**&#x200B;下拉列表中选择一个现有环境，或选择&#x200B;**[!UICONTROL 添加环境]**以创建一个环境。
   ![具有“已批准”状态的应用程序详细信息并添加环境](/help/extensibility/ajo-config-002.png){width="50%"}
1. 在选定的环境中，选择&#x200B;**[!UICONTROL 配置]**。
1. 在&#x200B;**[!UICONTROL 配置]**&#x200B;选项卡上，查找&#x200B;**[!UICONTROL AJO凭据]**。
   ![部署前使用AJO凭据进行配置（草稿）](/help/extensibility/ajo-config-004.png){width="80%"}
1. 输入已添加Journey Optimizer API的Developer Console项目中的凭据（例如，**[!UICONTROL AJO客户端ID]**、**[!UICONTROL AJO客户端密钥]**&#x200B;和&#x200B;**[!UICONTROL AJO令牌端点]**&#x200B;以及任何其他必填字段）。
1. 输入&#x200B;**沙盒名称，全部小写**（例如，`prod`）。
1. 单击&#x200B;**[!UICONTROL 部署]**。 部署完成后，状态将显示为已部署。 按钮文本将更改为&#x200B;**[!UICONTROL 取消部署]**。
   在App Builder应用程序视图上提供了![已部署应用程序及其取消部署](/help/extensibility/ajo-config-005.png){width="80%"}

部署后，Adobe Developer Console包含一个名为&#x200B;**Journey Optimizer的新自动生成的项目，该项目适用于使用AJO和Adobe Runtime API的GenStudio &lt;Your_Environment_Name>**。 此项目为只读，无法编辑或删除。
部署后![只读的自动生成Developer Console项目](/help/extensibility/ajo-auto-project.png){width="100%"}

### 更新配置

若要更改环境的配置变量，请先&#x200B;**[!UICONTROL 取消部署]**，更新值，然后再次&#x200B;**[!UICONTROL 部署]**，以使更改生效。

您可以在Exchange中创建&#x200B;**多个环境**（例如，每个沙盒一个环境）。 当您的组织使用多个沙盒时，每个部署都可以在GenStudio中作为单独的体验显示。

## 映射技术帐户的权限

用户可以在GenStudio中看到AJO扩展，而无需具有完全[!DNL Adobe Experience Platform]访问权限。 对于API调用（例如，加载模板），必须在&#x200B;**[!DNL Adobe Experience Platform]** > **[!UICONTROL 权限]**&#x200B;中向与OAuth凭据关联的技术帐户授予Journey Optimizer权限。 确切的角色名称和权限集取决于您的组织。

在AJO **[!UICONTROL 权限]** > **[!UICONTROL 历程]**&#x200B;中查看&#x200B;**[!UICONTROL 角色管理员]**&#x200B;下的扩展，并从Developer Console项目添加&#x200B;**API凭据**，这与从Exchange进行部署时使用的凭据相同。

在Adobe Experience Platform权限中为AJO架构师角色分配了![API凭据](/help/extensibility/ajo-map-permissions.png){width="80%"}

**另请参阅** （Journey Optimizer访问控制）：

* [访问控制](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/access-control/access-control-landing-page)
* [Journey Optimizer中的权限](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/access-control/permissions)
* [系统管理员入门指南](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/quick-start/administrator)

## 访问GenStudio中的AJO模板

部署和权限映射后：
1. 在GenStudio for Performance Marketing中打开&#x200B;**[!UICONTROL 创建]**&#x200B;并启动&#x200B;**电子邮件**&#x200B;体验。
1. 在&#x200B;**[!UICONTROL 选择模板]**&#x200B;中，打开&#x200B;**[!UICONTROL 已上传模板]**&#x200B;旁边的&#x200B;**[!UICONTROL AJO模板]**&#x200B;选项卡，以从Journey Optimizer浏览模板。

![选择包含“AJO模板”选项卡和模板库的模板](/help/extensibility/ajo-template-tab.png){width="80%"}

## 故障排除

### AJO“模板”选项卡不可见

* 确认在Exchange **[!UICONTROL 配置]**&#x200B;中输入的值正确，包括&#x200B;**客户端ID**、**客户端密钥**、**作用域**&#x200B;和&#x200B;**沙盒**。
* 确保&#x200B;**沙盒名称为小写**（例如，`prod`）。
* 从Exchange进行安装时，请使用&#x200B;**客户端ID**，如[创建OAuth凭据](#create-oauth-credentials-in-adobe-developer-console)中所述。

### AJO“模板”选项卡可见，但不显示模板

* 重新加载页面或再次打开&#x200B;**[!UICONTROL AJO模板]**&#x200B;选项卡。
* 在浏览器&#x200B;**[!UICONTROL 网络]**&#x200B;工具中，检查&#x200B;**`get-templates`**&#x200B;请求。 如果返回&#x200B;**403 Forbidden**，则技术帐户未分配给具有所需Journey Optimizer权限的角色或组。 根据贵组织的需要，更新[!DNL Adobe Experience Platform] **[!UICONTROL 权限]**&#x200B;和AJO **[!UICONTROL 权限]**&#x200B;中的映射。
