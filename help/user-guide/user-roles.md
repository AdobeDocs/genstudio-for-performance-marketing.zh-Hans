---
title: Adobe GenStudio for Performance Marketing用户角色和权限
description: 了解GenStudio for Performance Marketing用户角色和权限。
level: Beginner
feature: Generative AI, Guidelines
role: Admin
exl-id: 33ebcf9c-e5f8-4011-b449-5f73d151f221
source-git-commit: 4bef680734ee3369c13b10088fd39f22995a5f0f
workflow-type: tm+mt
source-wordcount: '1123'
ht-degree: 10%

---

# 用户角色和权限

创建和部署现代营销活动需要具有不同责任和技能的利益相关者之间的协作。 _用户角色_&#x200B;控制利益相关者对GenStudio for Performance Marketing众多功能的访问。 您分配的用户角色决定了您可以使用此平台执行的任务。 Adobe系统管理员将您分配给Adobe Admin Console中GenStudio产品配置文件中的一个角色。 您的欢迎电子邮件将标识您分配的角色。

>[!NOTE]
>
>在将任何用户配置为这些角色之前，必须在Adobe Admin Console中指定Adobe系统管理员以执行一次性设置任务。 此Adobe管理员角色仅在Adobe Admin Console的上下文中运行。 它在GenStudio for Performance Marketing平台界面中没有角色。 需要系统管理员权限的Adobe系统管理员必须在Adobe Admin Console中将自己配置为GenStudio系统管理员。 请参阅[配置GenStudio for Performance Marketing](product-provisioning.md)。

## Adobe系统管理员与GenStudio系统管理员

这些用户角色标题可能看起来类似，但它们标识了在不同环境中提供权利的独特角色。

**Adobe系统管理员**&#x200B;在Adobe Admin Console中拥有超级用户权限并执行所有用户管理任务，例如添加或删除用户。 此系统管理员角色不提供GenStudio for Performance Marketing应用程序中的权限，因此解释了为何Adobe系统管理员不需要GenStudio的许可证。 Adobe系统管理员通常使用Admin Console在GenStudio部署中添加和删除用户帐户，并从单个用户或用户组分配或删除权利或权限。

**GenStudio系统管理员**&#x200B;是GenStudio for Performance Marketing中的超级用户，但没有在Adobe Admin Console中执行任务的权限。 此系统管理员角色需要GenStudio产品许可证，并且它对应于[Adobe GenStudio for Performance Marketing产品描述](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html)中的超级用户。 GenStudio系统管理员完全有权使用GenStudio for Performance Marketing功能，包括[!DNL Brands]、[!DNL Persona]和[!DNL Product]创建、删除、更新和发布。 [Adobe GenStudio for Performance Marketing产品说明](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html)介绍GenStudio用户角色与产品许可证的关系。

请参阅[企业和团队管理指南](https://helpx.adobe.com/enterprise/using/admin-roles.html#enterprise)中的&#x200B;_管理角色_。

## 权利

_授权_&#x200B;授予执行特定任务以及访问受保护资源的权限。 权利或权限在产品配置文件的用户角色中定义，用户会在分配给该角色时收到这些权利。

>[!IMPORTANT]
>
>请勿添加新产品配置文件，也不编辑或删除现有产品配置文件。 更改默认产品配置文件可能会严重干扰GenStudio for Performance Marketing部署。

## 用户角色

三种类型的GenStudio for Performance Marketing用户角色支持这种多样化的组织角色。 权利针对每种用户类型量身定制，并支持每个用户在营销组织中的职责。 这三种用户角色类型为：

* **GenStudio编辑器**&#x200B;使用GenStudio for Performance Marketing的创作AI功能创建营销活动资源、请求内容审查和批准以及发布此内容的已批准草稿。 在编辑者将资产保存到[!DNL Content]后，所有GenStudio for Performance Marketing用户都可以访问和使用资产。 GenStudio编辑器是GenStudio for Performance Marketing中的高级用户。

* **GenStudio协作者**&#x200B;是范围最广的GenStudio for Performance Marketing用户。 协作者可以查看和批准内容，并且是工作流的重要组成部分，可确保生成的内容符合贵组织的需求和标准。 GenStudio协作者是GenStudio for Performance Marketing中的&#x200B;_协作者用户_。

* **GenStudio系统管理员**&#x200B;在GenStudio for Performance Marketing中拥有最广泛的权限集。 系统管理员执行基本入门任务，为营销活动资产的创建和部署建立基本保障。 系统管理员通过上传品牌和组织特定的信息（如[品牌准则](./guidelines/overview.md)）来实施这些护栏。 系统管理员有权创建和发布[!DNL Brands]，但没有用户管理权限。 GenStudio系统管理员是GenStudio for Performance Marketing中的超级用户。

### GenStudio编辑器

_编辑者_&#x200B;或内容创建者具有创建GenStudio for Performance Marketing [!DNL Brands]、[!DNL Campaigns]和[!DNL Content]资源所需的核心权限。 这些高级用户还可以编辑和删除他们创建的资产。 GenStudio for Performance Marketing支持快速创建数百个内容。 这些用户可以生成内容片段或整个体验，这些片段或体验可以编排已批准内容的离散片段，以满足特定营销活动的需求。

编辑者通过&#x200B;_提示_&#x200B;与GenStudio for Performance Marketing创作AI技术交互。 Canvas中的提示抽屉提供了一些工具，用于在特定营销活动准则的上下文中放置提示。 因此，生成的内容的质量和成功部分取决于贵组织上传的品牌指南的质量以及提示的特定性。 请参阅[编写有效的提示](effective-prompts.md)。

下表显示了默认编辑器权限：

| 功能 | 创建 | 更新 | 删除 | 视图 |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | 否 | 否 | 否 | 是 |
| [!DNL Campaigns] | 是 | 是 | 是 | 是 |
| [!DNL Content] | 是 | 是 | 是 | 是 |
| [!DNL Create] | 是 | 是 | 是 | 是 |
| [!DNL Insights] | 只能配置连接器 |    |     | 是 |
| [!DNL Personas] | 是 | 是 | 是 | 是 |
| [!DNL Products] | 是 | 是 | 是 | 是 |
| [!DNL Reviews and approvals] | 是 | 是 | 是 | 是 |
| [!DNL Templates] | 否 | 否 | 否 | 是 |

GenStudio系统管理员可以向编辑者提供编辑和删除[!DNL Brand]的权限。

### GenStudio协作者

_协作者_&#x200B;可以在GenStudio for Performance Marketing中查看资源，但不能创建、编辑或删除这些资源。 例如，协作者在尝试访问&#x200B;*时看到“*&#x200B;您无权访问此内容[[!DNL Create]](/help/user-guide/create/overview.md)”消息。

协作者包括对内容的审阅和批准流程取得成功至关重要的利益相关者，但他们不需要创建或直接编辑内容。 法律专家和创意人员管理人员就是潜在合作者的例子。 GenStudio for Performance Marketing协作者可能有权在其他Creative Cloud产品中创建和查看资源。

下表显示默认的Collaborator权限：

| 功能 | 创建 | 更新 | 删除 | 视图 |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | 否 | 否 | 否 | 是 |
| [!DNL Campaigns] | 是 | 是 | 是 | 是 |
| [!DNL Content] | 否 | 否 | 否 | 是 |
| [!DNL Create] | 否 | 否 | 否 | 是 |
| [!DNL Insights] | 否 | 否 | 否 | 是 |
| [!DNL Personas] | 是 | 是 | 是 | 是 |
| [!DNL Products] | 是 | 是 | 是 | 是 |
| [!DNL Reviews and approvals] | 否 | 否 | 否 | 是 |
| [!DNL Templates] | 否 | 否 | 否 | 是 |

### GenStudio系统管理员

_GenStudio系统管理员_&#x200B;在GenStudio for Performance Marketing中具有最强大的权限集。 这些高级用户执行重要的入门任务，为营销活动资产的创建和部署建立基本保障。 系统管理员通过上传品牌和组织特定的信息（如[品牌准则](./guidelines/overview.md)）来实施这些护栏。 系统管理员有权创建和发布[!DNL Brands]，但没有用户管理权限。

下表显示默认的系统管理员权限：

| 功能 | 创建 | 更新 | 删除 | 视图 |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | 是 | 是 | 是 | 是 |
| [!DNL Campaigns] | 是 | 是 | 是 | 是 |
| [!DNL Content] | 是 | 是 | 是 | 是 |
| [!DNL Insights] | 是 | 是 | 是 | 是 |
| [!DNL Personas] | 是 | 是 | 是 | 是 |
| [!DNL Products] | 是 | 是 | 是 | 是 |
| [!DNL Reviews and approvals] | 是 | 是 | 是 | 是 |
| [!DNL Templates] | 是 | 是 | 是 | 是 |

系统管理员也可以上传模板。

有关初步设置任务的概述，请参阅[Adobe GenStudio for Performance Marketing入门](get-started.md)。
