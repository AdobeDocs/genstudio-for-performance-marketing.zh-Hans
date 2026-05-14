---
title: Salesforce中的Experience Selector MFE
description: 了解如何在Salesforce Lightning中部署和配置Experience Selector MFE，包括CSP、Adobe身份验证、Apex电子邮件模板和验证。
feature: Extensibility, Extensions, Experiences
source-git-commit: 4cac970f46ab08bcec2f23fd882c552af088c4ea
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 0%

---

# Salesforce中的Experience Selector MFE

本主题介绍客户和实施人员如何在Salesforce组织中部署和运行[!DNL GenStudio for Performance Marketing] Experience Selector微前端(MFE)。 它涵盖了管理员步骤（无代码）、开发人员步骤（部署和配置）以及与安全相关的设置，例如内容安全策略(CSP)。

有关通用MFE集成选项、配置属性和框架示例，请参阅[GenStudio Experience Selector MFE](experience-selector.md)。

## 此集成的用途

>[!VIDEO](https://video.tv.adobe.com/v/3491089?captions=chi_hans&learn=on)

Lightning Web Component (LWC) `sfgsmfe`加载Adobe的Experience Selector UMD捆绑包并在`<dialog>`中呈现它，以便用户能够从[!DNL GenStudio for Performance Marketing]中选取体验。

该集成还可以：

* **预览和解码：**&#x200B;将所选有效负载显示为JSON、解码后的HTML以及LWC中经过清理的HTML预览。
* **电子邮件模板（可选）：** Salesforce中的&#x200B;**[!UICONTROL 创建电子邮件模板]**&#x200B;流程可以调用Apex (`EmailTemplateController.createEmailTemplate`)来插入`EmailTemplate`记录（HTML、主题和文件夹）。
* **运行时加载：** GenStudio脚本是从`experience.adobe.com`上的Adobe托管URL加载，而不是从典型实施中的Salesforce静态资源加载。

## 先决条件

* **Salesforce组织：**&#x200B;可在其中部署元数据和使用&#x200B;**[!UICONTROL Lightning App Builder]**&#x200B;的沙盒或生产组织。
* **Salesforce CLI：** Salesforce CLI (`sf`)已安装和验证，例如：

  ```bash
  sf org login web --alias <your-org-alias>
  ```

* **权限：**&#x200B;创建电子邮件模板的用户需要访问目标电子邮件模板文件夹，并有权根据您的组织策略创建模板。 Apex运行`with sharing`。
* **Adobe / GenStudio：**&#x200B;您的Adobe IMS组织ID和SUSI `clientId`必须与您的Adobe配置匹配（请参阅[配置集成值](#configure-integration-values-developer--implementation)）。
* **浏览器/CSP：** Salesforce必须允许从`https://experience.adobe.com`加载脚本（请参阅[配置内容安全策略和Adobe URL](#configure-content-security-policy-and-adobe-url)）。

## 部署包（开发人员）

集成遵循Salesforce DX样式布局。 Salesforce DX项目中的默认包目录通常为`force-app`。

1. 从项目根目录，将源部署到目标组织：

   ```bash
   sf project deploy start --source-dir force-app --target-org <your-org-alias>
   ```

2. 确认部署已完成且没有错误。

项目中的典型元数据包括：

* 一个名为`sfgsmfe`的LWC包（HTML、JavaScript、CSS和元XML），它承载选择器UI和脚本加载。
* Apex类（例如`EmailTemplateController`），在您使用该可选流程时创建电子邮件模板。

您的项目也可以定义静态资源。 如果LWC加载器使用`standalone.js`的Adobe CDN URL，则该加载路径不需要这些资源，除非您更改实现。

## 将组件添加到Lightning页面（管理员）

`sfgsmfe`组件已公开：

* 闪电般的应用程序页面
* 主页
* 记录页面
* 选项卡（通过将组件放在从自定义选项卡打开的Lightning页面上）

要添加组件，请执行以下操作：

1. 在&#x200B;**[!UICONTROL 设置]**&#x200B;中，打开&#x200B;**[!UICONTROL 应用程序管理器]**。
1. 创建&#x200B;**[!UICONTROL 新的Lightning应用程序]**（或打开要扩展的现有应用程序）。
   ![新的Lightning应用程序模式](./mfe-new-lighting-app.png){width="80%" zoomable="yes"}
1. 打开应用，然后选择&#x200B;**[!UICONTROL 编辑]**。
   ![The Edit Lightning App模式](./mfe-lightning-edit.png){width="80%" zoomable="yes"}
1. 创建&#x200B;**[!UICONTROL 新页面]**（或编辑现有的Lightning页面）。
   ![新页面模式](./mfe-lightning-new-page.png){width="60%" zoomable="yes"}
1. 在&#x200B;**[!UICONTROL 闪电App Builder]**&#x200B;中，将&#x200B;**sfgsmfe**&#x200B;组件拖动到布局上。
1. **[!UICONTROL 保存]**、**[!UICONTROL 激活]**，并将页面分配给正确的Lightning应用程序、配置文件和应用程序可见性，以便目标用户可以打开它。

## 配置内容安全策略和Adobe URL

LWC注入一个`<script>`标记，该标记的`src`指向Adobe的UMD捆绑包，例如：

`https://experience.adobe.com/solutions/GenStudio-experience-selector-mfe/static-assets/resources/@genstudio/experience-selector/umd/standalone.js`

您必须配置Salesforce，以便根据组织的CSP和Lightning安全设置，允许使用此源进行脚本加载。

如果脚本加载失败：

1. 打开浏览器开发人员工具。
1. 检查&#x200B;**[!UICONTROL Console]**&#x200B;和&#x200B;**[!UICONTROL Network]**&#x200B;选项卡中是否有阻止的请求或CSP违规。
1. 按照最新的Salesforce闪电文档，添加或调整`https://experience.adobe.com`的&#x200B;**[!UICONTROL CSP受信任站点]**（以及您的Salesforce版本的任何相关设置）。

## 配置集成值（开发人员/实施）

在LWC JavaScript中为`sfgsmfe`设置了多个值。 客户通常会根据环境替换这些参数。

| 价值 | 描述 |
| --- | --- |
| `folderId` | 用于创建新模板的电子邮件模板的Salesforce文件夹ID (`00l...`)。 对于Apex是必需的；文件夹必须存在并且可供运行的用户访问。 |
| `imsOrg` | Adobe IMS组织标识符传递到`GenStudioExperienceSelector.renderExperienceSelectorWithSUSI`。 |
| `susiConfig.clientId` | 用于Experience Selector应用程序注册的Adobe SUSI客户端ID。 |
| GenStudio `script.src` | UMD `standalone.js`包的URL；如果Adobe发布新路径，则更新。 |

电子邮件模板创建将GenStudio字段映射到模板（例如，来自`experienceFields`的主题）。 如果内容模型不同，则调整LWC中的映射。

有关`renderExperienceSelectorWithSUSI`和相关选项的详细信息，请参阅Experience Selector MFE主题中的[配置属性](experience-selector.md#configuration-properties)。

## Apex： EmailTemplateController

`EmailTemplateController.createEmailTemplate`通常：

* 验证模板名称、文件夹ID以及非空的HTML。
* 创建具有`TemplateType = 'custom'`、`HtmlValue`、`Subject`、`Body`和文件夹分配的`EmailTemplate`。
* 通过`AuraHandledException`向LWC显示错误。

操作提示：

* 尊重组织中的DeveloperName唯一性和命名规则。
* 确认文件夹ID，并确认用户可在该文件夹中创建`EmailTemplate`记录。
* 当DML无法捕获确切错误时，请使用Salesforce调试日志。

## 验证核对清单

在部署和配置后使用此列表：

* [ ]部署完成，没有错误。
* [ ]用户可以打开包含`sfgsmfe`的Lightning页面。
* [ ]组件未显示加载错误；“网络”选项卡返回`standalone.js`的HTTP 200。
* [ ] **[!UICONTROL 选择GenStudio Experience]**&#x200B;将打开选择器并运行选择回调。
* [ 使用该流程时，] **[!UICONTROL 创建电子邮件模板]**&#x200B;成功，该模板显示在&#x200B;**[!UICONTROL 安装程序]**&#x200B;中已配置的文件夹下。

## 另请参阅

* [GenStudio体验选择器MFE](experience-selector.md)
