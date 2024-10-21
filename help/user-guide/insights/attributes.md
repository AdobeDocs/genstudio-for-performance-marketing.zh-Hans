---
title: 属性概述
description: 了解如何评估Adobe GenStudio for Performance Marketing中特定属性的性能。
feature: Insights, Assets
source-git-commit: 87a8833549569aaeaa60f5760b4e9a8b710a6033
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 0%

---

# 属性概述

[!DNL Insights] _[!UICONTROL 属性]_&#x200B;视图显示所选渠道帐户在广告营销活动中使用的属性列表。

_[!UICONTROL 属性]_&#x200B;表是使用[!UICONTROL 属性]名称组织的。 您可以使用&#x200B;**[!UICONTROL 图像]**&#x200B;按钮和&#x200B;**[!UICONTROL 视频]**&#x200B;按钮在列表类型之间切换。 单击表格右侧上方的设置(cog)图标可切换可查看列。

表左上方的筛选器（漏斗）图标打开&#x200B;**[!UICONTROL 筛选器]**&#x200B;菜单，您可以从中从[!UICONTROL 帐户]和[!UICONTROL 属性类别]中选择以筛选表中的属性。 以下示例显示了`Lighting Condition`类别中的属性列表。

![属性筛选器和表](/help/assets/insights-attributes-filter.png){zoomable="yes"}

## 属性详细信息

属性有助于通过资产的内在详细信息（如颜色、构成、可视元素和其他属性）来识别资产。

在属性详细信息视图中，您可以看到哪些体验使用了所选属性。 详细信息包括总属性性能和与每个体验相关的性能量度细分。

![属性绩效指标](/help/assets/insights-attribute-details.png){zoomable="yes"}

GenStudio for Performance Marketing会检测某些功能，并将相应的属性作为标记应用于资源或体验。 请参阅[类别](#categories)以查看这些标记的示例。 要查看与体验关联的所有属性，请单击表右上方的设置(cog)图标以选择&#x200B;**[!UICONTROL 属性]**&#x200B;列。

## 类别

GenStudio for Performance Marketing可识别图像、视频和文本的某些功能，并将功能标记应用于资源。 _类别_&#x200B;是共享特定特征的一组功能。 _图像方向_&#x200B;的示例值为`landscape`。

无法编辑检测和自动应用的属性。

<!--
Select any of the following to open a detailed list of feature categories:

+++**Image features**

| Category               | Values                              |
| ---------------------- | ----------------------------------- |
| Background Colors      | 14 colors |
| Camera Position        | - `low angle`, `high angle`, `dutch angle`<br>- `overhead view`, `eye level`,`bird's eye view` |
| Camera Proximity       | `close up`, `mid shot`, `long shot` |
| Camera Setting         | - `fast shutter speed`, `long exposure`, `double exposure`<br>- `normal mode`, `flash`, `macro`, `wide-angle`<br>- `black and white`, `surreal`<br>- `bokeh blur`, `motion blur`, `tilt-shift blur` |
| Foreground Colors      | 14 colors |
| Image Type             | `photograph`, `sketch`, `painting`, `digital cartoon`, `infographics`, `graphic design`, `collage`, `screenshot` |
| Lighting Condition     | golden hour, blue hour, midday, overcast, night, high-key, low-key, daylight, incandescent, fluorescent, colorful, studio |
| Objects                | The items, entities, and elements that are visible, such as `lighthouse`, `orchid`, or `tunnel`. |
| Orientation            | Examples: `landscape`, `portrait`, `square` |
| Overall Tone           | `warm`, `cool`, `neutral` |
| People Categories      | Examples: `person`, `social group`, `people`, `kid` |
| Photography Styles     | `aerial photography`, `aerial photography`, `architectural photography`, `astrophotography`, `black and white photography`, `business photography`, `cityscape photography`, `commercial photography`, `composite photography`, `creative photography`, `editorial photography`, `event photography`, `family photography`, `fashion photography`, `fine art photography`, `food photography`, `holiday photography`, `indoor photography`, `landscape photography`, `lifestyle photography`, `macro photography`, `minimalist photography`, `night photography`, `outdoor photography`, `pet photography`, `portrait photography`, `product photography`, `real estate photography`, `seascape photography`, `sports photography`, `still-life photography`, `street photography`, `travel photography`, `underwater photography`, `wildlife photography` |
| Scenes                 | Examples: `city`, `island`, `living room` |
| Tags                   | Examples: `gaming`, `law`, `yoga` |
| Visual Attention Spread| The level of viewer attention spread across an image: `high`, `low` |
| Visual Content Density | The amount of information or detail in an image: `high`, `low` |

+++

+++**Video features**

| Category               | Values                              |
| ---------------------- | ----------------------------------- |
| Audio Genre  | |
| Audio Genre Category  | |
| Audio Mood  | |
| Audio Types| |
| Objects  | |
| Orientation  | |
| People Categories  | |
| Scenes  | |
| Styles  | |
| Tags   | |
| Video Category  | |
| Video Type  | |

+++

+++**Text features**

| Category               | Values                              |
| ---------------------- | ----------------------------------- |
| Emojis Count  | |
| HashTags Count  | |
| Keywords  | |
| Marketing Emotions  | |
| Narratives  |  |
| Persuasion Strategies  |  |
| Readability  | |
| Sentences Count  | |
| Stop Words Ratio  | |
| Text Quotes Count  | |
| Tones  | |
| Words Count  | |
| Words Count Per Sentence  | |

+++

-->

## 属性量度

分析量度可以帮助您评估哪些属性能激发更多的客户参与。

### 量度详细信息

下表提供了[!UICONTROL 属性]表视图中关键数字营销指标的定义和见解。 每个量度都包括与资产相关的简短定义、量度的计算方式以及一个或多个见解，以帮助了解其重要性及其对广告促销活动的影响。

| 量度 | 定义 | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL 属性]** | 属性名称。 | 单击任何关键量度的列标题可对表进行排序。 |
| **[!UICONTROL 类别]** | 表示属性的固有质量的[类别](#categories)。 |  |
| **[!UICONTROL #个图像]** | 具有此属性的图像的计数。 |  |
| **[!UICONTROL #个视频]** | 具有此属性的视频计数。 |  |
| **[!UICONTROL 展示次数]** | 每次在渠道中加载具有此属性的图像或视频时的计数，而不考虑交互或查看。 | 高展示次数计数可能表示广泛的可见性，但为了获得真正的性能洞察，请考虑其他参与量度。 |
| **[!UICONTROL 次点击]** | 用户与此属性相关的图像或视频交互的次数。 | 高点击数表示对内容非常感兴趣并参与其中，这可能有效并影响合适的受众。 |
| **[!UICONTROL CTR ]**<br>_点进率_ | 导致点击具有此属性的图像或视频的展示次数百分比(%)。<br>**计算**：`clicks`除以`impressions` | 高点进率表明，内容在消息传递和设计中与受众高度相关且具有激励性，能够有效地定位受众的兴趣。 |
| **[!UICONTROL CPM ]**<br>_每千成本_ | 具有此属性的图像或视频的每1,000次广告展示的费用($)。<br>**计算**：总金额`spent`除以范围，然后乘以1000 | 低值可能表示可视性具有成本效益，尤其是与高点进率配对时。 |
| **[!UICONTROL CPA ]**<br>_每个操作的成本_ | 完成特定客户操作（如购买或订阅）所花费的平均成本($)。<br>**计算**：总金额`spent`除以已完成的客户操作数 | 帮助确定可导致客户采取重要行动的属性。 |
| **[!UICONTROL CPC ]**<br>_每次点击成本_ | 与此属性相关的每次图像或视频点击的平均成本($)。<br>**计算**：总金额`spent`除以`clicks` | 平均成本降低可能表明广告支出具有成本效益，尤其是与转化率提高相比。 |
| **[!UICONTROL 支出]** | 与指定时间段内的属性相关的预算支出金额($)。 | 在短时间内高支出量可能表示使用迅速，这可能导致资源提前耗尽。 根据关键绩效指标跟踪支出金额，以帮助监控总体投资回报。 |
