---
title: 管理Assets和体验
description: 简化并增强对品牌认可资产的管理，以在您的数字营销历程中使用和重复使用。
feature: Content Management, Content Attributes
exl-id: e2ce8797-6d3b-46d4-b12f-f5f80e26c669
source-git-commit: 6880aadb104aac6b3282980760406168df3da5fe
workflow-type: tm+mt
source-wordcount: '1514'
ht-degree: 1%

---

# 管理资源和体验

Adobe GenStudio for Performance Marketing [!DNL Content]简化并增强了对品牌批准资源的管理，以便在您的数字营销历程中使用和重复使用。

## [!DNL Content]图库

图库会根据所选视图显示已批准资产、体验或模板的清单。 表格左上方的筛选器（漏斗）切换可打开&#x200B;**[!UICONTROL 筛选器]**&#x200B;菜单，您可以从多个类别中进行选择，以筛选图库中显示的内容。 在&#x200B;_[!UICONTROL Assets]_&#x200B;视图中，单击搜索（放大镜）图标以使用关键字查找资源。

下面显示了`space`Assets[!UICONTROL 图库中搜索词]的搜索：

![搜索空间的Assets视图](/help/assets/content-assets-filter.png "搜索具有空间属性的资源")

### 搜索内容

过滤器和搜索界面快速且响应迅速，提供了高效的搜索优先体验。 每个[!DNL Content]视图都提供筛选选项，以缩小搜索范围，从而缩小搜索范围，以找到理想的资产、体验或模板。 对于资源和体验，您可以选择营销活动和特定准则，例如为特定产品制作的内容。

存在基于[准则](/help/user-guide/guidelines/overview.md)、[关键字](asset-details.md#user-defined-metadata)和[属性类别](/help/user-guide/insights/attributes.md#categories)的筛选器以缩小搜索结果范围。 例如，您可能希望查找特定文件类型或主题的资产，以帮助您为营销策划构建新的体验。 或者，您也可以根据用户名或团队成员姓名来筛选内容：

- **[!UICONTROL 上传者]**：将&#x200B;_[!UICONTROL Assets]_&#x200B;列表限制为仅显示您或特定人员上传的资源。
- **[!UICONTROL 创建者]**：限制&#x200B;_[!UICONTROL 体验]_&#x200B;列表以仅显示您或特定人员创建的体验。
- **[!UICONTROL 模板]**：将&#x200B;_[!UICONTROL 体验]_&#x200B;列表限制为仅显示使用所选模板创建的体验。

如果某些过滤器选项不可见，则表示存储库中没有符合相应元数据条件的模板。 确保使用元数据正确标记模板，以使这些模板可通过这些过滤器发现。

**要搜索要重复使用的内容，请执行以下操作：**

1. 在&#x200B;_[!DNL Content]_中，选择&#x200B;**[!UICONTROL Assets]**部分。

1. 从&#x200B;**[!UICONTROL 位置]**&#x200B;列表中选择一个资源存储库，或验证您所查看的资源存储库是否正确。 `GenStudio assets`是默认存储库。

   >[!IMPORTANT]
   >
   >_位置_&#x200B;列表仅在您[连接到AEM存储库](connect-aem-repo.md)时可用。

1. 单击&#x200B;**[!UICONTROL 搜索]**（放大镜）以输入关键字或说明。

1. 通过从&#x200B;_[!UICONTROL 筛选器]_&#x200B;列表中选择一个类别来缩小搜索范围。 例如，如果要查找PNG文件，请单击&#x200B;**[!UICONTROL 文件格式]**，然后选择&#x200B;**PNG**。

   缩小搜索范围越多，可用的过滤器选项就越少。 单击&#x200B;**[!UICONTROL 全部清除]**&#x200B;可删除所有筛选器。

1. 选择资源以获取完整视图和详细信息列表。

   单击&#x200B;**[!UICONTROL 下载]**（向下箭头）以在本地工作站中使用资产。

### 位置

默认情况下，您通过[!DNL Content]进程或通过上载添加到[!DNL Create]的资源存储在`GenStudio assets`存储库中。 `GenStudio assets`存储库是GenStudio for Performance Marketing中的读写存储库。 这意味着您可以保存、编辑和删除`GenStudio assets`存储库中的资源。

位于右侧&#x200B;**[!UICONTROL Assets]**&#x200B;图库上方的&#x200B;_[!UICONTROL 位置]_&#x200B;列表允许您从连接的Adobe Experience Manager (AEM) [!DNL Assets Content Hub]存储库中进行选择。

![存储库的位置列表](/help/assets/content-location-selection.png "选择内容存储库"){width="350"}

选择AEM存储库后，图库会显示该存储库中的资源清单，这样您就可以将这些存储库中已批准的资源用作内容创建的输入。 筛选器选项会更改以反映[!DNL AEM Assets Content Hub]中配置的类别。

有关将[存储库添加到GenStudio for Performance Marketing的指导，请参阅](connect-aem-repo.md)连接AEM存储库[!DNL AEM Assets Content Hub]。

AEM存储库为只读，这意味着您可以访问内容，但无法将草稿、新资源或元数据保存到AEM存储库。 资产、体验和模板的所有草稿和最终更新都将使用新的`GenStudio assets`系统元数据[保存到](asset-details.md#system-metadata)存储库。

{{note-aem-assets}}

AEM存储库可能会强制实施某些许可要求，如资源过期。 这些资产可能无法在[!DNL Create]工作流中使用。 可能需要续订或替换过期的资产，以保持项目的连续性。 请咨询您的[!DNL AEM Assets Content Hub]管理员以获得这些资源的帮助。

## Assets管理

在[!UICONTROL Content]中，您可以轻松地存储、检索和管理数字资源。 通过利用`GenStudio assets`存储库和AEM存储库，您可以确保您的资源有条理并且可供各种营销活动访问。 这种多存储库方法提供了跨环境使用资产的灵活性和控制力，确保在营销工作中仅使用经批准和最新的资产。

下表列出了资产、体验和模板可用的管理任务：

| 任务 | 资源 | 体验 | 模板 |
| --------------------------------------------------------- | :----: | :---------: | :-------: |
| [查看详细信息](/help/user-guide/content/asset-details.md) | ✓ | ✓ | ✓ |
| [创建体验](/help/user-guide/create/overview.md) |        |             | ✓ |
| 在Adobe Express中[编辑](#edit-in-express) | ✓ |             |           |
| [导出体验](#export-experiences) |        | ✓ |           |
| [刷新](/help/user-guide/content/use-templates.md#refresh-template) |   |      | ✓ |
| [下载](#download-assets) | ✓ |             | ✓ |
| [删除](#delete-assets) | ✓ | ✓ | ✓ |

### 添加资源

将资源添加到[!DNL Content]时，默认情况下存储在`GenStudio assets`存储库中。 仅当&#x200B;_[!UICONTROL 位置]_&#x200B;是&#x200B;_[!UICONTROL 存储库时，]_&#x200B;添加资源`GenStudio assets`按钮才可用。

![位置字段](/help/assets/content-location.png "位置字段"){width="350"}

**要添加一个或多个资源**：

1. 在&#x200B;_[!DNL Content]_中，单击&#x200B;**[!UICONTROL 添加资源]**。

2. 在&#x200B;_添加批准的资产_&#x200B;视图中，将一个或多个文件拖放到放置空间中。 或者，您也可以使用&#x200B;**[!UICONTROL 浏览]**&#x200B;从本地文件中选择，或者从Dropbox或Microsoft OneDrive导入文件。

3. 在&#x200B;_添加详细信息_&#x200B;部分中，选择&#x200B;**[!UICONTROL 促销活动名称]**&#x200B;或输入新名称。

4. 为便于发现，请在&#x200B;_更多详细信息_&#x200B;部分中添加可选详细信息，如&#x200B;_品牌名称_、_角色_、_区域_&#x200B;和&#x200B;**关键字**。

   您提供的详细信息越多，就越能体验GenStudio for Performance Marketing的强大功能。 从列表中选择一个或多个详细信息，或在适用的情况下输入新详细信息，例如使用关键字。 您添加的每个详细信息都显示在列表下方。 单击&#x200B;**`x`**&#x200B;可删除详细信息。

   您添加的任何详细信息都适用于在此操作中添加的所有资源。

   查看[元数据详细信息](/help/user-guide/content/asset-details.md#system-metadata)。

5. 单击&#x200B;**[!UICONTROL 添加资源]**。

6. 完成资产上传后，单击&#x200B;**完成**。

7. 要查看您上传的新资源，请在画布底部的&#x200B;**[!UICONTROL 可用新资源]**&#x200B;通知中单击&#x200B;_刷新_。

### 下载资源

**要下载资源**：

1. 在&#x200B;_[!DNL Content]_中，选择一个资源或模板。 单击资产可打开资产的集中视图。

1. 在资源视图中，单击右上角的&#x200B;**[!UICONTROL 下载]**&#x200B;图标（向下箭头）。

1. 下载操作将开始将资产副本放置到默认下载位置。

### 删除资源

**要删除资源**：

1. 在&#x200B;_[!DNL Content]_中，选择资产、体验或模板。 单击资产可打开资产的集中视图。

1. 在资源视图中，单击右上角的&#x200B;**[!UICONTROL 删除]** （垃圾桶）。

1. 在&#x200B;_删除资产_&#x200B;弹出窗口中，验证该资产并单击&#x200B;**[!UICONTROL 删除]**。

## 导出体验

您可以选择一个或多个已批准的体验，以使用与目标渠道兼容的格式下载。 使用导出日期命名下载的文件： `2025-06-15-export.zip`。 解压缩文件时，每个渠道类型都会有一个文件夹，其中包含以所选格式导出的资产。 每个导出的资源都会保留其原始资源名称作为文件名。

>[!WARNING]
>
>检索到的资产不安全，未经清理便无法显示。 所有用户都必须在其终端使用输入清理技术处理来自模板的跨站点脚本(XSS)。

**要导出或下载体验**：

1. 在&#x200B;_[!DNL Content]_中，选择一个或多个体验。

   此时将显示一个横幅，左侧显示所选体验数量，右侧显示用于[!UICONTROL 激活]、[!UICONTROL 下载]或[!UICONTROL 删除]的选项。

2. （可选）如果您选择激活，系统可能会要求您选择一个平台，然后继续执行[!DNL Activate]工作流。 请参阅[激活](/help/user-guide/activation/overview.md)。

3. 单击&#x200B;**[!UICONTROL “下载”。]**

4. 在&#x200B;_下载_&#x200B;弹出窗口中，从可用格式中选择。

   如果您从不同的渠道中选择了多个体验，则有机会为每个渠道类型选择格式。

   - 电子邮件，LinkedIn： `HTML`，`CSV`
   - 元、横幅和显示广告： `HTML`、`JPEG`、`PNG`

   ![下载体验](/help/assets/content-bulk-export.png "下载多个体验"){width=350}

## 在Express中编辑

您可以使用Adobe Express直接在GenStudio for Performance Marketing中编辑图像资源(JPG或PNG)。 由Adobe Express支持的&#x200B;_[!UICONTROL 画布]_&#x200B;提供了方便的功能，可在不离开GenStudio应用程序的情况下增强您的图像。 可以轻松删除背景、应用创成填充、调整效果和裁切图像。

>[!BEGINSHADEBOX]

使用[!DNL Edit in Adobe Express]功能增强图像的条件：

- 支持的MIME类型包括`image/png`和`image/jpeg`
- 最小图像尺寸为50x50像素
- 图像最大尺寸为8000x8000像素
- 最大大小为40MB（40,000,000字节）

>[!ENDSHADEBOX]

**使用Express**&#x200B;编辑资源：

1. 在&#x200B;_[!DNL Content]_中，选择一个图像资源。 单击资产可打开资产的集中视图。

1. 在资源视图中，单击右上角的&#x200B;**[!UICONTROL 在Adobe Express中编辑]**&#x200B;图标。

1. 在&#x200B;_[!UICONTROL Powered by Adobe Express]_&#x200B;画布中，使用左侧面板上的Express控件来增强图像。

1. 如果对更新的图像满意，请单击右上角的&#x200B;**[!UICONTROL 保存副本]**。

1. 选择文件格式 — JPG或PNG — 并单击&#x200B;**[!UICONTROL 保存副本]**。

1. 在&#x200B;_[!UICONTROL 保存资产]_&#x200B;的副本弹出窗口中，更新&#x200B;**[!UICONTROL 资产名称]**。

   - 选择&#x200B;**[!UICONTROL 与原始资产相同的详细信息]**&#x200B;以将资产详细信息结转到新图像。

   - 展开&#x200B;**[!UICONTROL 更多详细信息]**&#x200B;部分以更新准则和其他元数据。

   >[!TIP]
   >
   >您提供的详细信息越多，就越能体验GenStudio for Performance Marketing的强大功能。 从列表中选择一个或多个详细信息，或在适用的情况下输入新详细信息，例如使用关键字。 您添加的每个详细信息都显示在列表下方。 单击&#x200B;**`x`**&#x200B;可删除详细信息。

1. 单击&#x200B;**[!UICONTROL 保存]**。
