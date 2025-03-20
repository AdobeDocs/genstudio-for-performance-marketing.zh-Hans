---
title: 属性概述
description: 了解如何评估Adobe GenStudio for Performance Marketing中特定属性的性能。
feature: Reporting and Insights, Content Attributes, Content Performance
exl-id: 9d05c128-50d5-415a-ae60-7023c36c06ad
source-git-commit: 3448392bc3f1496dafdbed2995f40bdba9c91c31
workflow-type: tm+mt
source-wordcount: '840'
ht-degree: 0%

---

# 属性概述

[!DNL Insights] _[!UICONTROL 属性]_&#x200B;视图显示所选渠道帐户在广告营销活动中使用的属性列表。

{{connect-insights}}

_[!UICONTROL 属性]_&#x200B;表是使用[!UICONTROL 属性]名称组织的。 您可以使用&#x200B;**[!UICONTROL 图像]**&#x200B;按钮和&#x200B;**[!UICONTROL 视频]**&#x200B;按钮在列表类型之间切换。 单击表格右侧上方的设置(cog)图标可切换可查看列。

表格左上方的筛选器（漏斗）图标会打开&#x200B;**[!UICONTROL 筛选器]**&#x200B;菜单，您可以从多个列表中进行选择。 选择表上方的&#x200B;**[!UICONTROL 全部清除]**&#x200B;可删除所有筛选器。

![属性筛选器和表](/help/assets/insights-attributes-filter.png){zoomable="yes"}

{{$include /help/_includes/download-insights.md}}

## 属性详细信息

属性通过固有详细信息（如颜色、合成、视觉元素和其他属性）帮助识别[媒体](media.md#media-details)。

在属性详细信息视图中，您可以看到哪些广告使用了所选属性。 详细信息包括总属性性能和与每个广告相关的性能量度细分。

![属性绩效指标](/help/assets/insights-attribute-details.png){zoomable="yes"}

GenStudio for Performance Marketing会检测某些功能，并将相应的属性作为标记应用于媒体内容或广告。 有关这些标记的示例，请参阅[类别](#categories)。 要查看与广告关联的所有属性，请单击表格右侧上方的设置(cog)图标以选择&#x200B;**[!UICONTROL 属性]**&#x200B;列。

## 类别

属性&#x200B;_category_&#x200B;是一个分类组，它组织具有共同特征的相关属性。 这些类别通过提供更丰富的上下文并方便其应用和使用，有助于简化对特定属性的发现、识别和理解。

GenStudio for Performance Marketing使用Adobe的AI和机器学习功能来研究[图像](image-features.md)、[视频](video-features.md)和文本并根据正确概率应用[!UICONTROL 媒体属性]。

检测到的媒体内容属性列表并不完整。 包含丰富功能的媒体可能仅限于AI确定的三个最主要的特征。 例如，下图包含多个检测到的图像属性，包括多个对象、前景色和背景色。

![图像属性](/help/assets/category/asset-attributes.png "Toucan图像包含多个检测到的属性"){width="300" zoomable="yes"}

>[!INFO]
>
>您无法编辑已检测并自动应用的标记。

## 属性性能

分析量度可以帮助您评估哪些属性能激发更多的客户参与。

下表提供了[!UICONTROL 属性]表视图中关键数字营销指标的定义和见解。 每个量度都包含一个与属性相关的简短定义、量度的计算方式以及一个或多个见解，以帮助了解其重要性及其对广告促销活动的影响。

| 量度 | 定义 | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL 属性]** | 属性名称。 | 单击任何关键量度的列标题可对表进行排序。 |
| **[!UICONTROL 类别]** | 表示属性的固有质量的[类别](#categories)。 |  |
| **[!UICONTROL #个图像]** | 具有此属性的图像数。 | “属性”表中的计数可能与“属性详细信息”视图中的计数不同。 如果渠道源(如Meta和GenStudio)使用的摘要计算略有不同，则会出现这种差异。 |
| **[!UICONTROL #个视频]** | 具有此属性的视频数。 | “属性”表中的计数可能与“属性详细信息”视图中的计数不同。 如果渠道源(如Meta和GenStudio)使用的摘要计算略有不同，则会出现这种差异。 |
| **[!UICONTROL 展示次数]** | 每次在渠道中加载具有此属性的图像或视频时的计数，而不考虑交互或查看。 | 高展示次数计数可能表示广泛的可见性，但为了深入了解真实性能，请考虑将其与其他参与量度关联起来。 |
| **[!UICONTROL 次点击]** | 用户与此属性对应的图像或视频交互的次数。 | 高点击数表示对内容非常感兴趣并参与其中，这可能有效并影响合适的受众。 |
| **[!UICONTROL CTR ]**<br>_点进率_ | 导致点击具有此属性的图像或视频的展示次数百分比(%)。<br>**计算**：`clicks`除以`impressions` | 高点进率表明，内容在消息传递和设计中与受众高度相关且具有激励性，能够有效地定位受众的兴趣。 |
| **[!UICONTROL CPM ]**<br>_每千成本_ | 具有此属性的图像或视频的每1,000次广告展示次数成本。<br>**计算**：总金额`spent`除以范围，然后乘以1000 | 低值可能表示可视性具有成本效益，尤其是与高点进率配对时。 |
| **[!UICONTROL CPA ]**<br>_每个操作的成本_ | 完成特定客户操作（如购买或订阅）所花费的平均成本。<br>**计算**：总金额`spent`除以已完成的客户操作数 | 帮助确定可导致客户采取重要行动的属性。 |
| **[!UICONTROL CPC ]**<br>_每次点击成本_ | 与此属性相关的每次点击图像或视频的平均成本。<br>**计算**：总金额`spent`除以`clicks` | 平均成本降低可能表明广告支出具有成本效益，尤其是与转化率提高相比。 |
| **[!UICONTROL 支出]** | 与指定时间段内的属性相关的预算支出金额。 | 在短时间内高支出量可能表示使用迅速，这可能导致资源提前耗尽。 根据关键绩效指标跟踪支出金额，以帮助监控总体投资回报。 |
