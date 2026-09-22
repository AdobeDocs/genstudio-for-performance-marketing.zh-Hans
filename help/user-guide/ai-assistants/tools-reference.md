---
title: AI助手工具参考
description: 了解AI助手可以与[!DNL GenStudio for Performance Marketing]一起使用的分析、创建、激活和反馈工具。
role: User
source-git-commit: 6fb7ddb7549ea6bcd66b6139fbde9ebe12ddaa22
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 15%
---

# AI助手工具参考

此参考描述了连接的AI助理可以与[!DNL GenStudio for Performance Marketing]一起使用的工具。 可用的工具列表取决于贵组织的配置。

在启动工作流之前，询问您的AI助手可以访问的工具。

## 功能区域

| 面积 | 用途 | 行为 |
|---|---|---|
| 洞察 | 查询付费媒体性能并检索创意推荐。 | 只读。 |
| 创建 | 从快速模板或见解推荐中收集草稿，然后管理审核。 | 读取和写入。 在Creative Cloud中创建文档。 |
| 激活 | 解决发布目标并发布已批准的体验。 | 写和破坏性。 可以发布实时广告并产生广告支出。 |
| 反馈 | 将产品反馈发送到[!DNL GenStudio for Performance Marketing]团队。 | 写入。 |

大多数分析工具涵盖`meta`、`linkedin`和`innovid`。 转化量度工具涵盖`meta`和`linkedin`。

创建支持`meta`、`linkedin`、`display`、`tiktok`和`youtube`。 激活支持`META`、`LINKEDIN`和`GOOGLECM360`。

## 分析工具

### get_insights_capabilities

返回为您的组织启用的分析渠道、操作和自定义转化量度。 当可用性不明确时，请首先使用此工具。

此工具返回功能元数据，而不是营销活动、广告或量度值。

### get_insights_summary

返回选定日期范围内某个渠道的标题性能指标和趋势。

| 参数 | 必需 | 描述 |
|---|---|---|
| `channel` | 是 | `meta`、`linkedin`或`innovid`。 |
| `startDate` | 否 | 开始日期为`YYYY-MM-DD`格式。 默认值为30天前。 |
| `endDate` | 否 | 结束日期为`YYYY-MM-DD`格式。 默认为今天。 |
| `metrics` | 否 | 要绘制图表的量度，如`spend`、`ctr`、`cpc`、`cpm`、`impressions`、`clicks`或`conversions`。 |

### list_insights_campaigns

返回促销活动绩效指标的可排序表和总计行。

| 参数 | 必需 | 描述 |
|---|---|---|
| `channel` | 是 | `meta`、`linkedin`或`innovid`。 |
| `startDate`, `endDate` | 否 | 日期范围`YYYY-MM-DD`格式。 默认值为过去30天。 |
| `search` | 否 | 营销活动名称过滤器。 |
| `sortBy` | 否 | 排序字段，如`spend`、`impressions`、`clicks`、`ctr`、`cpc`、`cpm`或`name`。 |
| `limit`, `offset` | 否 | 页面大小和分页偏移。 |

### list_insights_ads

返回广告级别的性能。 对可排序表使用默认浏览模式，对高性能广告和低性能广告使用层模式。

| 参数 | 必需 | 描述 |
|---|---|---|
| `channel` | 是 | `meta`、`linkedin`或`innovid`。 |
| `tier` | 否 | `all`、`high`或`low`。 默认为 `all`。 |
| `mainMetric` | 条件 | `high`或`low`层模式所需的排名量度。 |
| `campaigns` | 否 | 用于限制结果的营销活动标识符。 |
| `search` | 否 | 广告名称过滤器。 |
| `startDate`, `endDate` | 否 | 日期范围`YYYY-MM-DD`格式。 |
| `limit`, `offset` | 否 | 页面大小和分页偏移。 |

层模式返回`get_insights_ad_attributes`所需的广告标识符。

### get_insights_ad_details

返回一个广告的创意元数据，包括副本、call to action、资源和投放。 它不会返回性能量度。

| 参数 | 必需 | 描述 |
|---|---|---|
| `channel` | 是 | `meta`、`linkedin`或`innovid`。 |
| `accountId` | 是 | 付费媒体帐户标识符。 |
| `campaignId` | 是 | 营销活动标识符。 |
| `adId` | 是 | 广告标识符。 |
| `adgroupId` | 否 | 渠道使用广告组时的广告组标识符。 |

### get_insights_ad_attributes

将所选广告的创意特征与渠道平均值进行比较。 在`list_insights_ads`识别高性能或低性能广告之后使用它。

| 参数 | 必需 | 描述 |
|---|---|---|
| `ads` | 是 | 要说明的广告，包括`list_insights_ads`返回的标识符。 |
| `mainMetric` | 是 | 用于对广告进行排名的量度。 |
| `campaigns` | 否 | 用于定义比较群体的营销活动标识符。 |
| `startDate`, `endDate` | 否 | 日期范围`YYYY-MM-DD`格式。 |

### get_insights_tag_categories

返回在请求期间可用于贵组织的标记类别。 它返回类别名称，而不是性能量度。

| 参数 | 必需 | 描述 |
|---|---|---|
| `channels` | 是 | 一个或多个受支持的渠道。 |
| `startDate`, `endDate` | 否 | 日期范围`YYYY-MM-DD`格式。 |

### get_insights_ad_tags

返回一个类别（如产品、区域或创意主题）中按标记值的性能。

| 参数 | 必需 | 描述 |
|---|---|---|
| `channel` | 是 | `meta`、`linkedin`或`innovid`。 |
| `tagCategory` | 是 | `get_insights_tag_categories`返回的类别。 |
| `tagSource` | 否 | `ad_tags`或`campaign_tags`。 |
| `sortBy` | 否 | 用于对结果进行排序的量度。 |
| `search` | 否 | 标记值过滤器。 |
| `startDate`, `endDate` | 否 | 日期范围`YYYY-MM-DD`格式。 |

### get_insights_custom_metrics

返回为您的组织配置的自定义转化量度。 在`get_insights_conversion_metrics`之前使用它。

此工具返回量度标识符，而不是量度值。

### get_insights_conversion_metrics

返回Meta和LinkedIn的配置转化量度值和趋势。

| 参数 | 必需 | 描述 |
|---|---|---|
| `channels` | 否 | 支持的转换渠道。 默认为 `meta`。 |
| `metrics` | 否 | 由`get_insights_custom_metrics`返回的量度标识符。 |
| `campaigns` | 否 | 用于限制结果的营销活动标识符。 |
| `startDate`, `endDate` | 否 | 日期范围`YYYY-MM-DD`格式。 |

### get_insights_recommendations

根据贵组织的性能数据返回建议的创意更改。 当所选范围不包含符合条件的广告时，请求无法返回任何推荐。

| 参数 | 必需 | 描述 |
|---|---|---|
| `channels` | 是 | 一个或多个受支持的渠道。 |
| `campaigns` | 否 | 用于限制结果的营销活动标识符。 |
| `search` | 否 | 营销活动名称过滤器。 |
| `recommendationId` | 否 | 用于详细检索一个推荐的标识符。 |
| `limit`, `offset` | 否 | 页面大小和分页偏移。 |

## 创建工具

在体验准备好激活之前，创建工具以从Adobe Express模板收集草稿并管理审核。

### list_express_templates

列出具有筛选条件和Facet计数的可用快速模板。

| 参数 | 必需 | 描述 |
|---|---|---|
| `channel` | 否 | `meta`、`display`、`linkedin`、`tiktok`、`youtube`或`__unspecified__`。 |
| `query` | 否 | 模板的搜索词。 |
| `aspectRatios`, `keywords`, `languages`, `mediaFormat`, `regions`, `timeframes` | 否 | 模板Facet筛选器。 |
| `sortBy`, `order` | 否 | 对字段和顺序进行排序。 |
| `limit`, `offset` | 否 | 页面大小和分页偏移。 |

### describe_express_template

返回模板中可编辑的文本字段和图像投放位置。

| 参数 | 必需 | 描述 |
|---|---|---|
| `templateId` | 是 | 快速模板标识符。 |

### list_cta_options

返回某个渠道允许的call-to-action值。

| 参数 | 必需 | 描述 |
|---|---|---|
| `channel` | 是 | `linkedin`、`meta`、`display`、`tiktok`或`youtube`。 |

### create_draft

从具有一个或多个体验的Express模板创建可编辑的草稿。

| 参数 | 必需 | 描述 |
|---|---|---|
| `templateId` | 是 | 快速模板标识符。 |
| `prompt` | 是 | Creative摘要并复制与草稿一起存储的说明。 |
| `experiences` | 是 | 每个体验的渠道、内容字段和可选模板字段覆盖。 |
| `name` | 否 | 文档名称。 |

在为具有固定call-to-action值的渠道创建草稿之前，请使用`list_cta_options`。

### create_draft_from_recommendation

根据特定的分析推荐创建可编辑的草稿。

| 参数 | 必需 | 描述 |
|---|---|---|
| `channel` | 是 | `meta`或`linkedin`。 |
| `adUid` | 是 | 由`get_insights_recommendations`返回的推荐标识符。 |
| `prompt` | 是 | Creative根据建议编写摘要。 |
| `name` | 否 | 文档名称。 |

### list_recent_drafts

列出最近的Express模板草稿及其状态和链接。

| 参数 | 必需 | 描述 |
|---|---|---|
| `limit`, `offset` | 否 | 页面大小和分页偏移。 |

### get_draft_metadata

返回草稿的名称、渠道、审批状态、审核者结果和协作者访问权限。

| 参数 | 必需 | 描述 |
|---|---|---|
| `draftId` | 是 | 草稿资产标识符。 |

### share_draft

为协作者提供对草稿的查看或编辑权限，而无需请求审批。

| 参数 | 必需 | 描述 |
|---|---|---|
| `draftId` | 是 | 草稿资产标识符。 |
| `emails` | 是 | 一个或多个协作者电子邮件地址。 |
| `role` | 是 | `editor`或`viewer`。 |
| `message` | 否 | 邀请消息。 |

### request_draft_approval

向一个或多个人员发送草稿以供审批。

| 参数 | 必需 | 描述 |
|---|---|---|
| `draftId` | 是 | 草稿资产标识符。 |
| `emails` | 是 | 一个或多个审阅人电子邮件地址。 |

### list_experiences

返回已批准、已发布、准备激活的体验。 不包含草稿。

| 参数 | 必需 | 描述 |
|---|---|---|
| `channel` | 否 | 体验渠道过滤器。 |
| `createdByMe` | 否 | 将结果限制为当前用户创建的体验。 |
| `campaignNames` | 否 | 准确的营销活动名称过滤器。 |
| `creatorEmail` | 否 | 创建者电子邮件过滤器。 |
| `createdAtFrom`, `createdAtTo` | 否 | 创建日期范围。 |
| `language` | 否 | BCP 47语言标记。 |
| `limit`, `cursor` | 否 | 页面大小和分页光标。 |

## 激活工具

激活工具解决付费媒体目标并发布已批准的体验。 发布功能无法通过这些工具进行恢复，并且可能会产生广告支出。

### configure_activation_target

必要时解析并验证付费媒体帐户、营销活动、广告集和Facebook页面。

| 参数 | 必需 | 描述 |
|---|---|---|
| `platform` | 是 | `META`、`LINKEDIN`或`GOOGLECM360`。 |
| `platformAccountId` | 否 | 付费媒体帐户标识符。 省略它以发现帐户。 |
| `campaignId` | 否 | Meta或LinkedIn的营销活动标识符。 |
| `adsetId` | 否 | Meta广告集或LinkedIn营销活动标识符。 |
| `pageId` | 否 | Meta的Facebook页面标识符。 |

### create_activation

根据批准的体验和验证的目标发布单图像实时广告。

| 参数 | 必需 | 描述 |
|---|---|---|
| `platform` | 是 | `META`、`LINKEDIN`或`GOOGLECM360`。 |
| `targetId` | 是 | 由`configure_activation_target`返回的已验证目标。 |
| `experienceId` | 是 | `list_experiences`返回的已批准体验标识符。 |
| `assetId` | 否 | 具有多个合格变体的体验的变体标识符。 |
| `name` | 否 | 广告投放显示名称。 |

调用`create_activation`两次会创建两个单独的广告，而不是更新第一个广告。

## 反馈工具

### submit_mcp_feedback

向[!DNL GenStudio for Performance Marketing]团队发送有关工具或工作流的反馈。

| 参数 | 必需 | 描述 |
|---|---|---|
| `category` | 是 | `bug`、`feature_request`或`workflow_friction`。 |
| `comment` | 是 | 反馈的简要说明。 |
| `tags` | 否 | 用于对反馈进行分类的标记。 |
| `tool_name` | 否 | 与反馈关联的工具。 |

## 常见工作流

当一个工具为另一个工具提供标识符或配置时，请使用以下顺序：

- **在`high`或`low`层模式下诊断广告：**&#x200B;调用`list_insights_ads`，然后使用相同的排名量度调用`get_insights_ad_attributes`。
- **按标记分析：**&#x200B;调用`get_insights_tag_categories`，然后使用返回的类别调用`get_insights_ad_tags`。
- **查看转化指标：**&#x200B;调用`get_insights_custom_metrics`，然后使用返回的指标标识符调用`get_insights_conversion_metrics`。
- **将推荐转换为草稿：**&#x200B;调用`get_insights_recommendations`，然后调用`create_draft_from_recommendation`。
- **从模板生成：**&#x200B;调用`list_express_templates`、`describe_express_template`和`list_cta_options`，然后调用`create_draft`。
- **发布已批准的体验：**&#x200B;调用`list_experiences`，然后调用`configure_activation_target`和`create_activation`。

## 相关功能

- [AI助理概述](overview.md)
- [连接AI助手](connect-ai-assistants.md)
- [使用AI助理](use-ai-assistants.md)
