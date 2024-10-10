---
title: 资源详细信息
description: Adobe GenStudio for Performance Marketing使用丰富的元数据存储经批准的内容，以便进行可搜索性和性能跟踪。
feature: Attributes, Assets
exl-id: 2be5cfee-f315-4ad6-8cf0-a8d3929b9ba3
source-git-commit: ce08231cb723bec3d80a732837b72a435d3b552d
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 0%

---

# 资源详细信息

Adobe GenStudio for Performance Marketing使用丰富的元数据存储经批准的内容，以便进行可发现性和性能跟踪。

每个资源（包括体验和模板）都关联了&#x200B;_详细信息_（元数据），可帮助识别、跟踪、使用和学习内容性能。

**要查看资源详细信息**：

1. 在&#x200B;_[!DNL Content]_中，选择资产、体验或模板。 单击资产可打开资产的集中视图。

1. 在资源视图中，查看右侧的&#x200B;_[!UICONTROL 详细信息]_&#x200B;部分。

   >[!TIP]
   >
   >如果&#x200B;_[!UICONTROL 详细信息]_&#x200B;部分不可见，请单击&#x200B;**[!UICONTROL 信息]** (i)图标。

   资源详细信息包括在创建或上传过程中应用的元数据。 资源元数据类型包括[系统元数据](#system-metadata)和[用户定义的元数据](#user-defined-metadata)。

>[!NOTE]
>
>AEM存储库中的Assets显示不同的元数据。 请参阅[配置资源可见性](connect-aem-repo.md#step-4-configure-asset-visibility)以了解如何配置[!DNL AEM Assets Content Hub]资源详细信息。

## 在Express中编辑

您可以使用Adobe Express直接在GenStudio for Performance Marketing中编辑图像资源(JPG或PNG)。 _[!UICONTROL Powered byAdobe Express]_&#x200B;画布提供了方便的功能，无需离开GenStudio应用程序即可增强图像。 可以轻松删除背景、应用创成填充、调整效果和裁切图像。

1. 在&#x200B;_[!DNL Content]_中，选择一个图像资源。 单击资产可打开资产的集中视图。

1. 在资源视图中，单击右上角的&#x200B;**[!UICONTROL 在Adobe Express中编辑]**&#x200B;图标。

1. 在&#x200B;_[!UICONTROL Powered byAdobe Express]_&#x200B;画布中，使用左侧面板上的Express控件增强图像。

1. 如果对更新的图像满意，请单击右上角的&#x200B;**[!UICONTROL 保存副本]**。

1. 选择文件格式(JPG或PNG)，然后单击&#x200B;**[!UICONTROL 保存副本]**。

1. 在&#x200B;_[!UICONTROL 保存资产]_&#x200B;的副本弹出窗口中，更新&#x200B;**[!UICONTROL 资产名称]**。

   - 选择&#x200B;**[!UICONTROL 与原始资产相同的详细信息]**&#x200B;以将资产详细信息结转到新图像。

   - 展开&#x200B;**[!UICONTROL 更多详细信息]**&#x200B;部分以更新营销活动、准则和其他元数据。

   >[!TIP]
   >
   >您提供的详细信息越多，就越能体验GenStudio for Performance Marketing的强大功能。 从列表中选择一个或多个详细信息，或在适用的情况下输入新详细信息，例如使用关键字。 您添加的每个详细信息都显示在列表下方。 单击&#x200B;**`x`**&#x200B;可删除详细信息。

1. 单击&#x200B;**[!UICONTROL 保存]**。

## 系统元数据

上传资源时，会自动收集某些资源元数据。 无法编辑默认的系统元数据。

为资源存储和捕获的默认元数据包括文件名、维度、源等。

### 生成的标记

当您在[!DNL Content]中存储批准的资源时，GenStudio for Performance Marketing会使用Adobe的AI和机器学习功能来研究该资源并根据资源功能应用标记。 例如，猫的图片可能会产生诸如`pet photography`或`cat`之类的属性标记，以及标识图片中主要颜色的颜色标记。 无法编辑标记。

请参阅[分析属性](/help/user-guide/insights/attributes.md)。

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
| 时间范围 | 资产使用的时间范围，如季度、季度、年份等。 示例： `Winter 2023` |
| 区域 | 使用资产的区域。 示例： `North America`，`APAC`，`Italy` |
| 语言 | 资源使用的语言。 示例： `Spanish` |
| 关键字 | 用于进一步标识资产特征和用途的关键字 |

<!-- ## History

Expand the _[!UICONTROL History]_ section to view a timeline of approvals and activity.

list other activity, show screenshot?
-->
