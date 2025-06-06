---
title: 媒体概述
description: 了解如何在Adobe GenStudio for Performance Marketing中评估媒体效果。
level: Intermediate
feature: Reporting and Insights, Media Performance, Content Attributes
exl-id: 1e93422b-2645-4e29-a216-fc1008afbfc7
source-git-commit: facc38b8afe8104e27a89ac3d9ec40d1209229a9
workflow-type: tm+mt
source-wordcount: '645'
ht-degree: 0%

---

# 媒体概述

[!DNL Insights] _[!UICONTROL 媒体]_&#x200B;视图显示选定帐户在广告和广告营销活动中使用的媒体列表。 _媒体_&#x200B;表示已批准用于营销计划的图像、视频、文本或其他创意内容。

{{connect-insights}}

_[!UICONTROL 媒体]_&#x200B;表是使用&#x200B;**[!UICONTROL 媒体ID]**&#x200B;组织的。 您可以使用视图列表（表格）图标和图库视图（网格）图标在视图之间切换。 单击表格右侧上方的设置(cog)图标可切换可查看列。

![媒体筛选器和表](/help/assets/insights-media-filter.png){zoomable="yes"}

_[!UICONTROL 媒体]_&#x200B;图库视图显示媒体预览拼贴和量度，如点进率。 单击图库右上方的设置(cog)图标以打开&#x200B;**[!UICONTROL 卡片设置]**&#x200B;并切换三个可查看的量度之一：

- CPA（每次操作的成本）
- CTR（点进率）
- CPC（每次点击成本）
- 支出

{{filter-table}}

## 媒体详细信息

在&#x200B;_媒体详细信息_&#x200B;视图中，您可以看到哪些广告使用了所选媒体。 详细信息包括总媒体性能、使用媒体的广告、用户定义的属性，以及与媒体关联的AI检测功能。

![媒体详细信息](/help/assets/insights-media-details.png){zoomable="yes"}

### 媒体属性

{{$include /help/_includes/generated-attributes.md}}

## 媒体效果

分析量度可以帮助您评估哪些媒体对活动取得成功做出了贡献以及哪些媒体属性最有效。

下表提供了[!UICONTROL 媒体]表视图中关键数字营销量度的定义和见解。 每个量度都包括与媒体相关的简短定义、量度的计算方式以及一个或多个洞察，以帮助了解其重要性和影响。

| 量度 | 定义 | insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL 媒体ID]** | 与图像、视频、文本或其他创意内容关联的名称。 | 单击任何关键量度的列标题可对表进行排序。 |
| **[!UICONTROL 展示次数]** | 每次媒体加载到频道中的计数，无论交互或观看情况如何。 | 高展示次数计数可能表示广泛的可见性，但为了深入了解真实性能，请考虑将其与其他参与量度关联起来。 |
| **[!UICONTROL 次点击]** | 用户与媒体上可点击元素（例如链接）交互的次数。 | 高点击数表示对内容非常感兴趣并参与其中，这可能有效并影响合适的受众。 |
| **[!UICONTROL CTR &#x200B;]**<br>_点进率_ | 在广告中导致媒体点击的展示次数百分比(%)。<br>**计算**：`clicks`除以`impressions` | 高点进率表明媒体与受众高度相关且富有吸引力。 这表明，信息传递和设计有效地抓住了观众的兴趣，促使他们采取行动。 此外，高CTR可能意味着媒体具有针对性并与目标受众产生共鸣，从而带来更好的整体营销活动效果。 |
| **[!UICONTROL CPM &#x200B;]**<br>_每千成本_ | 每1000次媒体印象的平均成本。<br>**计算**：总金额`spent`除以展示次数，然后乘以1000 | CPM值较低可能表示介质性能具有成本效益，尤其是与高点进率配对时。 |
| **[!UICONTROL CPA &#x200B;]**<br>_每个操作的成本_ | 完成特定客户操作（如购买或订阅）所花费的平均成本。<br>**计算**：总金额`spent`除以已完成的客户操作数 | 帮助识别导致客户采取重要行动的媒体。 |
| **[!UICONTROL CPC &#x200B;]**<br>_每次点击成本_ | 每次点击介质时产生的平均成本。<br>**计算**：总金额`spent`除以`clicks` | 平均成本降低可能表明广告支出具有成本效益，尤其是与转化率提高相比。 |
| **[!UICONTROL 支出]** | 在指定时间段内与单个媒体相关的预算支出金额。 | 在短时间内高支出量可能表示使用迅速，这可能导致资源提前耗尽。 根据关键绩效指标跟踪支出金额，以帮助监控总体投资回报。 |
| **[!UICONTROL 用于这些广告]** | 使用此媒体的广告数量。 | |
| **属性** | 此媒体中存在的固有功能列表。 | 属性有助于识别与受众产生最多共鸣的创意元素。 |
