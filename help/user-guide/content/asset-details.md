---
title: 资源详细信息
description: Adobe GenStudio for Performance Marketing使用丰富的元数据存储经批准的内容，以便进行可搜索性和性能跟踪。
feature: Generative AI, Content Attributes, Content Management
exl-id: 2be5cfee-f315-4ad6-8cf0-a8d3929b9ba3
source-git-commit: c0f45fb0ffc61d20611693498f1b12d3946ca6ca
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 1%

---

# 资源详细信息

Adobe GenStudio for Performance Marketing使用丰富的元数据存储经批准的内容，以便进行可发现性和性能跟踪。

每个资源（包括体验和模板）都关联了&#x200B;_详细信息_（元数据），可帮助识别、跟踪、使用和学习内容性能。

**要查看资源详细信息**：

1. 在&#x200B;_[!DNL Content]_&#x200B;中，选择资产、体验或模板。 单击资产可打开资产的集中视图。

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

有关图像、视频和文本功能的详细列表，请参阅[!DNL Insights] [属性类别](/help/user-guide/insights/attributes.md#categories)。

### 生成的内容元数据

用于生成新资源或体验的信息将成为元数据，例如所使用的提示。 内容获得批准后，您无法编辑提示，但可以将其用作生成新内容的起点。

## 用户定义的元数据

用户定义的元数据将营销上下文添加到资产的内容，使营销人员能够了解如何使用及参与资产。

在[上传资源](/help/user-guide/content/manage-assets.md#add-assets)时，您可以将GenStudio for Performance Marketing中存在的一组可选资源详细信息定义为元数据。 包含更多详细信息可以改进搜索和筛选中的资产识别。

**要编辑用户定义的元数据**：

1. 在&#x200B;_[!DNL Content]_&#x200B;中，选择资产、体验或模板。 单击资产可打开资产的集中视图。

1. 在资源视图中，查看右侧的&#x200B;_[!UICONTROL 详细信息]_&#x200B;部分。

1. 单击&#x200B;**[!UICONTROL 编辑详细信息]** （铅笔）可编辑资源、体验或模板元数据。

   您提供的详细信息越多，就越能体验GenStudio for Performance Marketing的强大功能。 从列表中选择一个或多个详细信息，或在适用的情况下输入新详细信息，例如使用关键字。 您添加的每个详细信息都显示在列表下方。 单击&#x200B;**`x`**&#x200B;可删除详细信息。

### 元数据详细信息

下表详细列出了在创建资源时可以定义的元数据（资源详细信息）。

| 字段 | 描述 |
| -------------- | ----------- |
| 标题 | 资源的名称；默认标题可能是原始文件名 |
| [!DNL Campaigns] | [[!DNL Campaigns]](/help/user-guide/campaigns/overview.md)包含具有一致消息传递的促销内容，以实现业务目标<br>单击促销活动链接将会转到促销活动的概述页面 |
| [!DNL Brands] | [[!DNL Brands]](/help/user-guide/guidelines/brands.md)已添加到GenStudio for Performance Marketing并发布以供使用 |
| [!DNL Products] | [[!DNL Products]](/help/user-guide/guidelines/products.md)已添加到GenStudio for Performance Marketing以供使用 |
| [!DNL Personas] | [[!DNL Personas]](/help/user-guide/guidelines/personas.md)已添加到GenStudio for Performance Marketing以供使用 |
| 渠道 | 用于分发特定内容类型（如电子邮件、横幅和显示广告）的平台 |
| [!UICONTROL 时间范围] | 使用资产的时间范围，如季度、季度、年份等。 示例：`Winter 2023` |
| 区域 | 使用资产的区域。 示例： `North America`，`APAC`，`Italy` |
| 语言 | 资源使用的语言。 示例：`Spanish` |
| 关键字 | 用户定义的关键字用于进一步标识资源特征和用途 |

>[!TIP]
>
>单击&#x200B;**[!UICONTROL 编辑详细信息]** （铅笔）以编辑资源元数据。 例如，您可以更改资源名称或添加或删除关键字。

## 生成上下文

[!UICONTROL 生成上下文]部分显示用于生成体验的信息，例如`Prompt`进程期间使用的[!DNL Create]。 此insight可以帮助您构建更加成功的变体。

信息可能包括：

- 在`Brand`进程期间选择的`Product`、`Persona`和[!DNL Create]参数
- 电子邮件体验的`Subject line`和`Preheader`
- 用于Meta广告的`Headline`和`Body`

## 历史记录

展开体验中的&#x200B;_[!UICONTROL 历史记录]_&#x200B;部分以查看审批和活动的时间表。 例如，已批准的体验将显示批准日期、时间和批准者：

```
Approved

December 10, 2024 at 6:00 PM by Username
```
