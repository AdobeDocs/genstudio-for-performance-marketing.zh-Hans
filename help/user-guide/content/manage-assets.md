---
title: 管理资源和体验
description: 简化并增强对品牌认可资产的管理，以在您的数字营销历程中使用和重复使用。
feature: Content, Assets, Experiences
exl-id: e2ce8797-6d3b-46d4-b12f-f5f80e26c669
source-git-commit: 82ac164cb852305fce206845d15f04c4b4395387
workflow-type: tm+mt
source-wordcount: '786'
ht-degree: 0%

---

# 管理资源和体验

Adobe GenStudio for Performance Marketing [!DNL Content]简化并增强了对品牌批准资源的管理，以便在您的数字营销历程中使用和重复使用。

## Assets图库

[!UICONTROL Assets]图库显示已批准资源的清单。 表格左上方的筛选器（漏斗）图标会打开&#x200B;**[!UICONTROL 筛选器]**&#x200B;菜单，您可以从多个类别中进行选择，以筛选图库中显示的资产。 单击搜索（放大镜）图标可使用关键字查找资产。

下面显示了[!UICONTROL Assets]图库中搜索词`dog`的搜索：

![Assets视图（包含对狗的搜索）](../../assets/content-assets.png)

### Assets位置

默认情况下，您通过[!DNL Create]进程或通过上载添加到[!DNL Content]的资源存储在`GenStudio assets`存储库中。 `GenStudio assets`存储库是GenStudio for Performance Marketing中的读写存储库。 这意味着您可以保存、编辑和删除`GenStudio assets`存储库中的资源。

右侧图库上方的&#x200B;**[!UICONTROL 位置]**&#x200B;列表允许您从连接的Adobe Experience Manager (AEM) [!DNL Assets Content Hub]存储库中进行选择。 选择AEM存储库时，库会显示该存储库中的资源清单，这样您就可以利用这些存储库中已批准的资源作为内容创建的输入。 筛选器选项会更改以反映[!DNL AEM Assets Content Hub]中配置的类别。

有关将[!DNL AEM Assets Content Hub]存储库添加到GenStudio for Performance Marketing的指导，请参阅[连接AEM存储库](connect-aem-repo.md)。

AEM存储库是只读的，这意味着您不能将草稿、新资源或元数据保存到AEM存储库。 资产、体验和模板的所有草稿和最终更新都将使用新的[系统元数据](asset-details.md#system-metadata)保存到`GenStudio assets`存储库。

{{note-aem-assets}}

## Assets管理

在[!UICONTROL Content]中，性能营销人员可以轻松地存储、检索和管理其数字资产。 通过同时利用`GenStudio assets`存储库和AEM存储库，用户可以确保其资源组织良好并可访问各种营销活动。 这种多存储库方法提供了跨环境使用资产的灵活性和控制力，确保在营销工作中仅使用经批准和最新的资产。

### 添加资源

将资源添加到[!DNL Content]时，默认存储在`GenStudio assets`存储库中。 仅当&#x200B;_[!UICONTROL 位置]_&#x200B;是`GenStudio assets`存储库时，_[!UICONTROL 添加资源]_&#x200B;按钮才可用。

![位置字段](../../assets/content-location.png){width="350" align="center"}

**要添加一个或多个资源**：

1. 在&#x200B;_[!DNL Content]_中，单击&#x200B;**[!UICONTROL 添加资源]**。

1. 在&#x200B;_添加批准的资产_&#x200B;视图中，将一个或多个文件拖放到放置空间中。 或者，您可以使用&#x200B;**[!UICONTROL 浏览]**&#x200B;从本地文件中选择，或者从Dropbox或Microsoft OneDrive导入文件。

1. 在&#x200B;_添加详细信息_&#x200B;部分中，选择&#x200B;**[!UICONTROL 促销活动名称]**&#x200B;或输入新名称。

1. 为了提高可发现性，请在&#x200B;**更多详细信息**&#x200B;部分中添加可选详细信息，如&#x200B;_品牌名称_、_角色_、_区域_&#x200B;和&#x200B;_关键字_。

   您提供的详细信息越多，就越能体验GenStudio for Performance Marketing的强大功能。 从列表中选择一个或多个详细信息，或在适用的情况下输入新详细信息，例如使用关键字。 您添加的每个详细信息都显示在列表下方。 单击&#x200B;**`x`**&#x200B;可删除详细信息。

   您添加的任何详细信息都适用于在此操作中添加的所有资源。

   查看[元数据详细信息](/help/user-guide/content/asset-details.md#system-metadata)。

1. 单击&#x200B;**[!UICONTROL 添加资源]**。

1. 完成资产上传后，单击&#x200B;**完成**。

1. 要查看您上传的新资源，请在画布底部的&#x200B;_可用新资源_&#x200B;通知中单击&#x200B;**[!UICONTROL 刷新]**。

<!-- 
In the future, need guidance on template upload errors. For now, the UI just says error.
-->

### 搜索内容

过滤器和搜索界面快速且响应迅速，提供了高效的搜索优先体验。 每个[!DNL Content]视图都提供筛选器选项，以缩小搜索范围，从而缩小搜索范围，以找到理想的资产、体验或模板。 对于资源和体验，您可以选择营销活动和特定准则，例如为特定产品制作的内容。

存在基于[关键字](asset-details.md#user-defined-metadata)和[属性](/help/user-guide/insights/attributes.md)的筛选器以缩小搜索结果范围。 例如，您可能希望查找特定文件类型或主题的资产，以帮助您为营销策划构建新的体验。

在搜索&#x200B;_体验_&#x200B;时，您可以使用&#x200B;**[!UICONTROL 创建者]**&#x200B;筛选器将列表限制为仅显示您或特定人员创建的体验。

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
