---
title: 资源详细信息
description: Adobe GenStudio for Performance Marketing使用丰富的元数据存储经批准的内容，以便进行可搜索性和性能跟踪。
feature: Attributes, Assets
exl-id: 2be5cfee-f315-4ad6-8cf0-a8d3929b9ba3
source-git-commit: 5e1702b26d34f519c4ab321b2adc04754fa1fcb6
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 资源详细信息

Adobe GenStudio for Performance Marketing使用丰富的元数据存储经批准的内容，以便进行可发现性和性能跟踪。

每个资源（包括体验和模板）都关联了&#x200B;_详细信息_（元数据），可帮助识别、跟踪、使用和学习内容性能。

**要查看资源详细信息**：

1. 在&#x200B;_[!DNL Content]_中，选择资产、体验或模板。 单击资产可打开资产的集中视图。

1. 在资源视图中，查看右侧的&#x200B;_[!UICONTROL 详细信息]_&#x200B;部分。

1. 如果&#x200B;_[!UICONTROL 详细信息]_&#x200B;部分不可见，请单击&#x200B;**[!UICONTROL 信息]** (i)图标。

资源详细信息包括在创建或上传过程中应用的元数据。 资源元数据类型包括[系统元数据](#system-metadata)和[用户定义的元数据](#user-defined-metadata)。

以下图像资产包含描述文件类型、大小和其他特征的系统元数据、一个用户定义的关键字以及多个AI检测到的属性和颜色。

具有多个标记的资源的![详细信息](/help/assets/content-asset-details.png)

>[!NOTE]
>
>AEM存储库中的Assets显示不同的元数据。 请参阅[配置资源可见性](connect-aem-repo.md#step-4-configure-asset-visibility)以了解如何配置[!DNL AEM Assets Content Hub]资源详细信息。

## 系统元数据

上传资源时，会自动收集某些资源元数据，例如文件类型、大小、维度、源等。 除文件名外，您无法编辑默认的系统元数据。

### 生成的标记

当您在[!DNL Content]中存储批准的资源时，GenStudio for Performance Marketing会使用Adobe的AI和机器学习功能来研究该资源并根据资源功能应用标记。 例如，猫的图片可能会产生诸如`pet photography`或`cat`之类的属性标记，以及标识图片中主要颜色的颜色标记。 您无法编辑已检测并自动应用的标记。

有关图像、视频和文本功能的详细列表，请参阅[!DNL Insights] [属性类别](/help/user-guide/insights/attribute-category.md)。

### 生成的内容元数据

用于生成新资源或体验的信息将成为元数据，例如所使用的提示。 内容获得批准后，您无法编辑提示，但可以将其用作生成新内容的起点。

## 用户定义的元数据

用户定义的元数据将营销上下文添加到资产的内容，使营销人员能够了解如何使用及参与资产。

在[上传资源](/help/user-guide/content/manage-assets.md#add-assets)时，您可以将GenStudio for Performance Marketing中存在的一组可选资源详细信息定义为元数据。 包含更多详细信息可以改进搜索和筛选中的资产识别。

### 元数据详细信息

下表详细列出了在创建资源时可以定义的元数据（资源详细信息）。

| 字段 | 描述 |
| ------------- | ----------- |
| 营销活动（项目名称） | 捕获并随资产一起存储的默认元数据 |
| [!DNL Brands] | [[!DNL Brands]](/help/user-guide/guidelines/brands.md)已添加到GenStudio for Performance Marketing并发布以供使用 |
| [!DNL Products] | [[!DNL Products]](/help/user-guide/guidelines/products.md)已添加到GenStudio for Performance Marketing以供使用 |
| [!DNL Personas] | [[!DNL Personas]](/help/user-guide/guidelines/personas.md)已添加到GenStudio for Performance Marketing以供使用 |
| 渠道 | GenStudio for Performance Marketing中用于资源的内容类型，如电子邮件和元广告 |
| [!UICONTROL 时间范围] | 使用资产的时间范围，如季度、季度、年份等。 示例： `Winter 2023` |
| 区域 | 使用资产的区域。 示例： `North America`，`APAC`，`Italy` |
| 语言 | 资源使用的语言。 示例： `Spanish` |
| 关键字 | 用于进一步标识资产特征和用途的用户定义关键字 |

<!-- ## History

Expand the _[!UICONTROL History]_ section to view a timeline of approvals and activity.

list other activity, show screenshot?
-->
