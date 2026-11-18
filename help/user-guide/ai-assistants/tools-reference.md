---
title: AI助手工具参考
description: 了解AI助手可以与[!DNL GenStudio for Performance Marketing]一起使用的见解、创建、计划、激活和反馈工具。
role: User
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 244293cf4f83acbc252f1d5f3495db403ed4a9bb
workflow-type: tm+mt
source-wordcount: '2265'
ht-degree: 13%
---

# AI助手工具参考

此参考描述了连接的AI助理可以与[!DNL GenStudio for Performance Marketing]一起使用的工具。 可用的工具列表取决于贵组织的配置。

在启动工作流之前，询问您的AI助手可以访问的工具。

## 功能区域

| 面积 | 用途 | 行为 |
|---|---|---|
| 洞察 | 查询付费媒体和电子邮件性能并检索创意推荐。 | 只读。 |
| 创建 | 查找资源，从快速模板或见解推荐中汇编草稿，然后管理审核。 | 读取和写入。 在Creative Cloud中创建文档。 |
| 规划 | 从简报中提取营销活动详细信息，并将其保存到Workfront Planning。 | 提取是只读的。 保存操作会在Workfront Planning中创建记录，并且无法自动回滚。 |
| 激活 | 解决发布目标并将批准的体验发送到平台。 | 写入。 广告会发送到平台，并以关闭状态发布。 分别打开它们。 无法通过这些工具进行还原。 |
| 反馈 | 将产品反馈发送到[!DNL GenStudio for Performance Marketing]团队。 | 写入。 |

大多数分析工具涵盖`meta`、`linkedin`和`innovid`。 量度值工具涵盖`meta`和`linkedin`。 电子邮件营销活动报告涵盖Adobe Journey Optimizer (`ajo`)和Adobe Campaign (`acc`)。

创建支持`meta`、`linkedin`、`display`、`tiktok`和`youtube`。 激活支持`META`、`LINKEDIN`和`GOOGLECM360`。

## 分析工具

### get_insights_capabilities

返回为您的组织启用的分析渠道和报表操作。 当可用性不明确时，请首先使用此工具。 支持的渠道为`meta`、`linkedin`、`innovid`、`ajo`和`acc`。

此工具返回功能元数据，而不是营销活动、广告或量度值。 要查找贵组织的自定义量度键，请使用`list_connected_channels_and_metrics`。

### list_connected_channels_and_metrics

返回贵组织的活动Meta、LinkedIn和Google Campaign Manager 360连接、支持的分析渠道和操作以及配置的自定义转化量度。 在调用`get_insights_metric_values`之前使用它查找量度键。

此工具返回量度键、标签和格式，而不是量度值。 连接并不保证历史报表数据可用。

| 参数 | 必需 | 描述 |
|---|---|---|
| `limit`, `offset` | 否 | 页面大小和分页偏移。 省略两者以返回完整的目录。 |

### get_insights_summary

返回选定日期范围内某个渠道的标题性能指标和趋势。

| 参数 | 必需 | 描述 |
|---|---|---|
| `channel` | 是 | `meta`、`linkedin`或`innovid`。 |
| `startDate` | 否 | 开始日期为`YYYY-MM-DD`格式。 默认值为30天前。 |
| `endDate` | 否 | 结束日期为`YYYY-MM-DD`格式。 默认为今天。 |
| `metrics` | 否 | 要用于图表的量度： `spend`、`ctr`、`cpc`、`cpm`、`cpa`、`impressions`、`clicks`、`conversions`、`videoPlays`、`engagement`、`likes`、`comments`或`shares`。 默认值为`spend`、`ctr`、`cpc`和`cpm`。 |

### list_insights_campaigns

返回促销活动绩效指标的可排序表和总计行。

| 参数 | 必需 | 描述 |
|---|---|---|
| `channel` | 是 | `meta`、`linkedin`或`innovid`。 |
| `startDate`, `endDate` | 否 | 日期范围`YYYY-MM-DD`格式。 默认值为过去30天。 |
| `search` | 否 | 营销活动名称过滤器。 |
| `sortBy` | 否 | 排序字段： `spend`、`impressions`、`clicks`、`ctr`、`cpc`、`cpm`或`name`。 默认为 `spend`。 结果始终按降序排序。 |
| `limit`, `offset` | 否 | 页面大小和分页偏移。 默认页面大小为20。 |

### list_insights_email_campaigns

返回包含Adobe Journey Optimizer和Adobe Campaign的交付和参与量度的电子邮件营销活动的可排序表。 对于广告营销活动，请使用`list_insights_campaigns`。

| 参数 | 必需 | 描述 |
|---|---|---|
| `channel` | 是 | `ajo`或`acc`。 |
| `startDate`, `endDate` | 否 | 日期范围`YYYY-MM-DD`格式。 默认值为结束日期之前的最近30天。 |
| `search` | 否 | 营销活动名称过滤器。 |
| `sortBy` | 否 | 排序字段： `campaignName`、`emailsNumber`、`emailsDelivered`、`totalClicks`、`openRate`、`ctr`、`ctor`、`bounceRate`、`unsubscribeRate`或`spamComplaintRate`。 默认为 `emailsDelivered`。 结果始终按降序排序。 |
| `limit`, `offset` | 否 | 页面大小和分页偏移。 |

### list_insights_ads

返回广告级别的性能。 对可排序表使用默认浏览模式，对高性能广告和低性能广告使用层模式。

| 参数 | 必需 | 描述 |
|---|---|---|
| `channel` | 是 | `meta`、`linkedin`或`innovid`。 |
| `tier` | 否 | `all`、`high`或`low`。 默认为 `all`。 |
| `mainMetric` | 否 | `high`或`low`层模式的排名量度：`ctr`、`cpc`、`cpm`、`cpa`、`spend`、`impressions`或`clicks`。 在浏览模式下被忽略。 |
| `metrics` | 否 | 要在层模式下为每个广告报告的其他量度。 |
| `campaigns` | 否 | 用于限制结果的营销活动，最多为50个。 每个营销活动都包含`channel`、`accountId`和`campaignId`。 |
| `search` | 否 | 广告名称过滤器。 |
| `sortBy` | 否 | 浏览模式排序字段： `spend`、`impressions`、`clicks`、`ctr`、`cpc`、`cpm`或`name`。 默认为 `spend`。 结果始终按降序排序。 |
| `spendMin`, `spendMax` | 否 | 每个广告的总支出范围。 仅限层模式。 |
| `includeUnsupported` | 否 | 包含其创意无法呈现的广告。 默认为 `false`。 |
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
| `ads` | 是 | 一到200个广告需要解释。 每个广告都包含`channel`、`accountId`、`campaignId`和`adId`，以及可选的`adGroupId`和`performanceTier` （`high`或`low`）。 在层模式下使用`list_insights_ads`返回的标识符。 |
| `mainMetric` | 是 | 用于为广告排名的量度： `ctr`、`cpc`、`cpm`、`cpa`、`spend`、`impressions`或`clicks`。 |
| `campaigns` | 否 | 用于定义最多50个比较群体的营销活动。 每个营销活动都包含`channel`、`accountId`和`campaignId`。 |
| `spendMin`, `spendMax` | 否 | 比较群体的支出范围。 |
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
| `tagSource` | 否 | `ad_tags`或`campaign_tags`。 默认为 `ad_tags`。 |
| `sortBy` | 否 | 排序字段： `adsCount`、`spend`、`impressions`、`clicks`、`conversionCount`、`ctr`、`cpc`、`cpm`或`cpa`。 默认为 `adsCount`。 |
| `search` | 否 | 标记值过滤器。 |
| `startDate`, `endDate` | 否 | 日期范围`YYYY-MM-DD`格式。 |
| `limit`, `offset` | 否 | 页面大小和分页偏移。 |

### get_insights_metric_values

返回贵组织跟踪量度的值和趋势，例如Meta和LinkedIn的潜在客户、注册或广告支出回报率。

| 参数 | 必需 | 描述 |
|---|---|---|
| `channels` | 否 | `meta`、`linkedin`或两者。 |
| `metrics` | 否 | `list_connected_channels_and_metrics`最多返回20个量度键。 默认设置是您组织的默认可见设置。 |
| `campaigns` | 否 | 用于限制结果的营销活动，最多为50个。 每个营销活动都包含`channel`、`accountId`和`campaignId`。 |
| `startDate`, `endDate` | 否 | 日期范围`YYYY-MM-DD`格式。 默认值为过去30天。 |

### get_insights_recommendations

根据贵组织的性能数据返回建议的创意更改。 当所选范围不包含符合条件的广告时，请求无法返回任何推荐。

| 参数 | 必需 | 描述 |
|---|---|---|
| `channels` | 是 | `meta`、`linkedin`或`innovid`中的一个或多个。 |
| `campaigns` | 否 | 用于限制结果的营销活动，最多为50个。 每个营销活动都包含`channel`、`accountId`和`campaignId`。 |
| `search` | 否 | 营销活动名称过滤器。 |
| `recommendationId` | 否 | 一个推荐的`adUid`，用于检索该推荐的详细信息。 |
| `onlyWithPreview` | 否 | 不包括没有示例创意预览的建议。 默认为 `true`。 |
| `limit`, `offset` | 否 | 页面大小和分页偏移。 |

## 创建工具

在体验准备好激活之前，创建工具以查找资源、从Adobe Express模板收集草稿和管理审核。

### list_express_templates

列出具有筛选条件和Facet计数的可用快速模板。

| 参数 | 必需 | 描述 |
|---|---|---|
| `channel` | 否 | `meta`、`display`、`linkedin`、`tiktok`、`youtube`或`__unspecified__`。 |
| `query` | 否 | 模板的搜索词。 |
| `activatableMimeType`, `aspectRatios`, `externalTemplateSource`, `isHTML5Template`, `keywords`, `languages`, `mediaFormat`, `regions`, `timeframes` | 否 | 模板Facet筛选器。 |
| `sortBy` | 否 | `modified`或`created`。 默认为 `modified`。 |
| `order` | 否 | `asc`或`desc`。 默认为 `desc`。 |
| `limit`, `offset` | 否 | 页面大小和分页偏移。 |

### describe_express_template

返回模板中可编辑的文本字段和图像投放位置。

| 参数 | 必需 | 描述 |
|---|---|---|
| `templateId` | 是 | 快速模板标识符。 |

### list_cta_options

返回某个渠道允许的call-to-action值。 显示区返回空列表，因为它接受自由格式文本。

| 参数 | 必需 | 描述 |
|---|---|---|
| `channel` | 是 | `linkedin`、`meta`、`display`、`tiktok`或`youtube`。 |
| `limit`, `offset` | 否 | 页面大小和分页偏移。 省略两者以返回每个选项。 |

### search_assets

搜索GenStudio内容中的图像和视频。 使用它可以为草稿选择现有资源。 派生、外部和过期的资产将被排除在外。 此工具不会上传、编辑、删除或生成资源，并且需要GenStudio内容权限。

| 参数 | 必需 | 描述 |
|---|---|---|
| `query` | 否 | 跨资产元数据的关键字或自然语言搜索。 |
| `mediaTypes` | 否 | `image`、`video`或两者。 缺省值包括两者。 |
| `aspectRatios` | 否 | 宽高比，如`1:1`或`16:9`。 如果比率不可用，则该工具将返回可用选项。 |
| `brands`, `campaigns`, `products`, `personas`, `channels` | 否 | 按名称过滤。 |
| `customMetadata` | 否 | 最多5个元数据字段，每个字段具有一个或多个值。 |
| `uploadedBy` | 否 | `me`或Uploader电子邮件地址。 |
| `createdAtFrom`, `createdAtTo` | 否 | ISO 8601格式的创建时间范围。 |
| `aiGenerated` | 否 | 按AI生成状态过滤。 |
| `contentCredentials` | 否 | 按Content Credentials状态筛选。 |
| `limit`, `offset` | 否 | 页面大小和分页偏移。 |

结果包括`create_draft`的稳定资产引用和短期签名URL。

### create_draft

从具有一个或多个体验的Express模板创建可编辑的草稿。 每次调用都会创建一个新草稿。

| 参数 | 必需 | 描述 |
|---|---|---|
| `templateId` | 是 | 快速模板标识符。 |
| `prompt` | 是 | Creative摘要并复制与草稿一起存储的说明。 |
| `experiences` | 是 | 一个或多个体验。 请参阅下表。 |
| `name` | 否 | 文档名称。 |
| `allowAssetReuse` | 否 | 允许跨多个体验重用一个选定的资产。 默认为 `false`。 |

每个体验都支持以下字段：

| 字段 | 必需 | 描述 |
|---|---|---|
| `channel` | 是 | `linkedin`、`meta`、`display`、`tiktok`或`youtube`。 |
| `title` | 否 | 体验标题。 默认值为“概念&#x200B;*n*”。 |
| `headline` | Meta和LinkedIn | 主要标题。 |
| `body` | Meta、LinkedIn和TikTok | 正文副本。 对于LinkedIn，这是介绍性文本。 对于TikTok，这是主文本。 |
| `description` | YouTube | 广告描述。 对于Meta和LinkedIn而言，它是可选项。 |
| `display_url` | Meta和LinkedIn | 在广告中显示URL。 |
| `destination_url` | 否 | 广告链接到的URL。 |
| `cta` | 否 | 来自`list_cta_options`的Call-to-action文本。 |
| `templateFields` | 否 | 覆盖`describe_express_template`中的命名模板元素。 每个覆盖设置文本、带尺寸的图像URL或视频URL。 |
| `assetTemplateFields` | 否 | 模板中图像或视频字段来自`search_assets`的内容资源。 |

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
| `emails` | 是 | 1到20个协作者电子邮件地址。 |
| `role` | 是 | `editor`或`viewer`。 |
| `message` | 否 | 邀请消息。 |

### request_draft_approval

向一个或多个人员发送草稿以供审批。

| 参数 | 必需 | 描述 |
|---|---|---|
| `draftId` | 是 | 草稿资产标识符。 |
| `emails` | 是 | 1到20个审阅人电子邮件地址。 |

### list_experiences

返回已批准、已发布、准备激活的体验。 不包含草稿。

| 参数 | 必需 | 描述 |
|---|---|---|
| `channel` | 否 | `email`、`meta`、`meta_organic`、`display`、`ctv`、`linkedin`、`linkedin_organic`、`tiktok`、`chatgpt`或`youtube`。 |
| `createdByMe` | 否 | 将结果限制为当前用户创建的体验。 |
| `campaignNames` | 否 | 最多5个准确的促销活动名称过滤器。 |
| `creatorEmail` | 否 | 创建者电子邮件过滤器。 |
| `createdAtFrom`, `createdAtTo` | 否 | 创建日期范围。 |
| `language` | 否 | BCP 47语言标记。 |
| `limit`, `cursor` | 否 | 页面大小（1-50，默认为20）和分页光标。 |

## 计划工具

规划工具可将营销活动摘要转换为可审核的营销活动草稿，并将其保存到Workfront规划中。

### extract_campaign_from_brief

从粘贴的营销简报中提取可审核的营销活动草稿。 此工具不保存任何记录。 无法推断缺少的事实和日期。

| 参数 | 必需 | 描述 |
|---|---|---|
| `briefText` | 是 | 一个营销活动简报的全纯文本，最多100,000个字符。 不支持文件和链接。 |

结果包括活动草稿、包含支持引号的调查结果、建议的受众和警告。

### create_workfront_campaign

根据您审查和批准的草稿，创建一个带有链接产品和角色的Workfront Planning营销活动。 此工具不是幂等，并且无法自动回滚记录。 在重试可能已成功的写入操作之前检查Workfront。

| 参数 | 必需 | 描述 |
|---|---|---|
| `campaignDraft` | 是 | 核准的草稿。 需要`name`。 可选字段为`description`、`objective`、`keyMessaging`、`startDate`、`endDate` (`YYYY-MM-DD`)、`status`、`channels`、`products`和`personas`。 |
| `channelSelections` | 否 | 已批准不明确的渠道名称选项。 |
| `entitySelections` | 否 | 已批准现有产品和角色记录。 使用`null`请求新记录。 |
| `createMissingEntities` | 否 | 创建您选择作为新的产品和角色。 默认为 `false`。 |

如果产品、角色或渠道不明确，则该工具会返回确认选项且不做更改。

## 激活工具

激活工具可解决付费媒体目标并将已批准的体验发送到平台。 广告发布时处于关闭状态（Meta已暂停、LinkedIn草稿、促销活动管理器360未激活），因此您必须先单独打开这些广告，然后才能投放它们。 向平台发送广告无法通过这些工具进行还原。

### configure_activation_target

必要时解析并验证付费媒体帐户、营销活动、广告集和Facebook页面。

| 参数 | 必需 | 描述 |
|---|---|---|
| `platform` | 是 | `META`、`LINKEDIN`或`GOOGLECM360`。 |
| `platformAccountId` | 否 | 付费媒体帐户标识符。 省略它以发现帐户。 |
| `campaignId` | 否 | Meta或LinkedIn的营销活动标识符。 不用于Campaign Manager 360。 |
| `adsetId` | 否 | Meta广告集或LinkedIn营销活动标识符。 不用于Campaign Manager 360。 |
| `pageId` | 否 | Meta的Facebook页面标识符。 |

对于Campaign Manager 360，只需要广告帐户。

### create_activation

使用验证的目标将批准的体验作为广告发送到平台。 广告以关闭状态发布。 Meta会为每个纵横比创建一个带有第一个图像的广告。 LinkedIn和Campaign Manager 360会为每个已解析的图像创建一个广告。

| 参数 | 必需 | 描述 |
|---|---|---|
| `platform` | 是 | `META`、`LINKEDIN`或`GOOGLECM360`。 |
| `targetId` | 是 | 由`configure_activation_target`返回的已验证目标。 |
| `experienceId` | 是 | `list_experiences`返回的已批准体验标识符。 |
| `name` | 否 | 广告投放显示名称。 默认是体验的广告标题。 |

结果会列出已创建、已排队和已跳过的广告数量，每个广告的初始状态及其链接均位于[!DNL GenStudio for Performance Marketing]中。 状态`PENDING`表示作业已排队，而不是广告正在投放。

调用`create_activation`两次会创建其他广告，而不是更新第一个广告。

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
- **查看跟踪的指标：**&#x200B;调用`list_connected_channels_and_metrics`，然后使用返回的指标键调用`get_insights_metric_values`。
- **将推荐转换为草稿：**&#x200B;调用`get_insights_recommendations`，然后调用`create_draft_from_recommendation`。
- **从模板生成：**&#x200B;调用`list_express_templates`、`describe_express_template`和`list_cta_options`，然后调用`create_draft`。
- **从现有资源生成：**&#x200B;调用`search_assets`，然后在`assetTemplateFields`中将返回的资源引用传递给`create_draft`。
- **将营销活动简报保存到Workfront：**&#x200B;致电`extract_campaign_from_brief`，查看草稿，然后致电`create_workfront_campaign`。
- **将批准的体验发送到平台：**&#x200B;调用`list_experiences`，然后调用`configure_activation_target`和`create_activation`。

## 相关功能

- [AI助理概述](overview.md)
- [连接AI助手](connect-ai-assistants.md)
- [使用AI助理](use-ai-assistants.md)
