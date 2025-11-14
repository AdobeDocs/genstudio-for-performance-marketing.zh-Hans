---
title: Adobe GenStudio for Performance Marketing发行说明
description: 了解 Adobe GenStudio for Performance Marketing 的最新功能和增强功能。
recommendations: noDisplay
role: User
exl-id: 32f5104e-ae15-4092-8a34-642fc641baf9
source-git-commit: f6dc843acc6d29b107f5165dfd2ee1d2c9e72f0f
workflow-type: tm+mt
source-wordcount: '4162'
ht-degree: 0%

---

# GenStudio for Performance Marketing发行说明

此发行信息提供了对GenStudio for Performance Marketing应用程序的最新更新。

## 2025.11.14 {#latest}

### Real-Time CDP受众集成

* GenStudio for Performance Marketing现在与Adobe Real-Time Customer Data Platform (RTCDP)集成，使营销人员能够直接在[!DNL Create]工作流中利用受众定义。
* 通过在内容生成期间选择[!DNL Audience]参数，营销人员可以根据客户上下文创建个性化的创意和电子邮件副本，包括消息传递偏好设置、购买者区段、历程阶段和行为数据。

### 展示广告的无痕见解

* [!DNL Insights]现在包括Innovid（以前称为Flashtalking）作为显示广告渠道，使营销人员能够在统一的平台上与Meta、LinkedIn和TikTok一起分析营销活动效果。
* 通过每天刷新数据并访问关键绩效指标（包括展示次数、点击次数和CTR），营销人员可以做出更快的优化决策，而无需在工具之间切换。

### 付费媒体和电子邮件的现成翻译

* 直接在GenStudio for Performance Marketing中将批准的付费媒体和电子邮件体验即时翻译为40多种语言。
* 使用Azure Open AI翻译服务，团队可以将内容同时批量翻译为多种目标语言。

### PDF导出体验

[!BADGE Beta]{type=Informative tooltip="此功能当前位于Beta中，因此某些功能可能会受到限制或发生更改。"}

* 营销人员现在可以[将体验导出为PDF格式](/help/user-guide/content/manage-assets.md#export-experiences)，以供审阅、批准和存档。

### Firefly Image Model 4上的自定义模型

* GenStudio for Performance Marketing现在支持在Adobe Firefly Image Model 4[上训练的](/help/user-guide/create/generate-assets.md)自定义模型，通过改进的照片真实感和细节提供增强的品牌上图像生成功能。

### Meta单个视频广告激活

* 营销人员现在可以直接从Meta将带有单个视频资源的GenStudio for Performance Marketing广告[激活](/help/user-guide/activation/activate-meta-ad.md)到Meta广告管理器。 这使媒体购买者、性能营销人员和创意团队能够无缝发布视频广告体验，并维护与静态广告激活相同的简化工作流程。
* 用户可以配置视频广告创意详细信息，预览视频的显示方式，并向Meta平台激活视频广告。

### 适用于Meta促销活动的按操作类型划分的CPA

* 针对Meta广告促销活动，通过灵活的转化跟踪[分析](/help/user-guide/insights/ads.md)每操作成本(CPA)。
* 从多种操作类型（如购买、添加到购物车的事件、商机、视频查看或自定义转化）中进行选择（而不是单个固定量度），以在[!DNL Insights]中跨促销活动、广告、资源和属性计算和查看CPA。

### 修复和增强功能

* 添加了SDK扩展，该扩展允许客户连接到其自己的DAM，而不是在内容生成期间使用AEM Assets作为资产的默认值。
* 用户现在可以应用[!DNL Brand]标记，以便按[!DNL Product]对[!DNL Persona]和[!DNL Brand]记录进行分组。
* [!DNL Experience Translations]流已随付费媒体和电子邮件的新翻译功能一起优化。


## 早期发行说明

+++2025.10.16版注释

### 适用于Photoshop和Figma的新GenStudio插件

* 使用适用于Adobe Photoshop的新GenStudio插件和Figma设计工具，直接创建品牌广告和个性化广告。

### 扩展的视频功能

* 营销人员现在可以轻松地将介绍剪辑和介绍剪辑添加到具有预生成的品牌或消息的视频广告中。
* 在整个视频长度中添加图像、文本和徽标叠加图

### LinkedIn、Meta和TikTok的扩展见解

* GenStudio Insights现在包括LinkedIn广告效果报表，使营销人员能够直接在平台中查看和分析其营销活动和广告的效果，以：
   * LinkedIn广告
   * Meta Ads
   * TikTok Ads

### Amazon Ads激活

* GenStudio现在支持直接在Amazon Ads平台中激活显示广告。

### Flashtalking激活

* GenStudio现在支持将显示广告直接激活到Flashtalking (Innovid)广告投放平台。
* 用户必须与激活工程团队协作，手动配置其Flashtalking API令牌。 未来版本中将添加自助令牌配置。

### 与Adobe Campaign V8集成

* GenStudio for Performance Marketing现在与Adobe Campaign V8集成，使营销人员能够无缝地利用AI支持的内容创建功能以及Campaign的高级编排功能。

### 视频自动播放

* 视频现在可以跨[!DNL Create]、[!DNL Content]和[!DNL Insights]模块自动播放，从而提供无缝的预览体验。

### 第三方电子邮件模板导入

* GenStudio for Performance Marketing现在支持通过可扩展性框架与第三方电子邮件设计系统无缝集成。 主要功能包括：

   * 在内容创建期间自动从第三方电子邮件设计系统导入模板
   * 将模板元数据与导入的模板一起引入
   * 通过直接连接到第三方系统维护单一真实来源
   * 为构建自定义集成提供的SDK和示例应用程序

+++



+++2025.09.11版注释

### 适用于付费媒体的创新型扩展AI功能

新的GenExpand功能可让营销人员动态调整其创意资源，以支持跨付费媒体渠道(如Meta、LinkedIn、显示广告和横幅)的不同宽高比。 当图像与预期纵横比不匹配时（如将窄图像添加到宽布局），可以使用GenExpand修改图像以适应。

此功能简化了直接在GenStudio for Performance Marketing中编辑图像和调整大小的过程。 有关详细信息，请参阅[生成扩展AI功能](/help/user-guide/create/manage-variants.md#use-generative-expand)。

+++

+++2025.08.15版注释

### 文本属性的分析

Adobe GenStudio中的“文本属性分析”可分析广告文案中使用的情绪色调、说服技术和叙述风格。 营销活动上线后，GenStudio会跟踪这些文本属性与CTR、CPA、CPC、展示次数和支出等关键绩效指标的关联情况。

这当前仅适用于英文广告。 有关详细信息，请参阅[文本功能](/help/user-guide/insights/text-features.md)。

### 分析模板改进

* 广告预览卡片现在包含用于文本的“查看更多”选项。
* 广告页面石砌卡的新模板。

### 通过品牌验证生成多语言内容

提示抽屉中新的语言选择器支持创建多语言内容，从而让区域营销人员能够为其本地受众开发品牌上内容。 此功能当前支持12种语言。

### 模板上的视频资产支持

* 可在Meta和LinkedIn模板中添加视频资源。

### 激活体验改进

* 用于保存激活草稿的新功能。
* 用于重试失败的激活的新功能。

### 在多个文本字段中使用相同的角色

对于复杂的客户模板，现在支持角色相同的多个文本字段（例如，“正文”、“cta”、“图像文本”等）。

在[有关模板代码编辑器的指南](/help/user-guide/content/code-editor.md)中浏览详细信息。

### 支持新的Firefly图像生成模型

[!BADGE Beta]{type=Informative tooltip="此功能当前位于Beta中，因此某些功能可能会受到限制或发生更改。"}

Adobe GenStudio for Performance Marketing现在支持最新的Firefly Image Model 4套件，其中包括两个强大的变体：

**Firefly图像4**：针对速度和简洁性进行了优化，非常适合生成插图、图标、基本对象照片和单主题肖像，满足90%的日常创意需求。

**Firefly Image 4 Ultra**：优先考虑照片真实感和精确度，在呈现人体肖像、中等大小的群组和复杂场景方面表现出色，适合高端创意任务。

有关使用这些新图像生成模型的详细信息，请参阅[生成资源](/help/user-guide/create/generate-assets.md)。

### 电子邮件的现成翻译

[!BADGE Beta]{type=Informative tooltip="此功能当前位于Beta中，因此某些功能可能会受到限制或发生更改。"}

Adobe GenStudio for Performance Marketing现在提供内置的电子邮件翻译功能，允许营销人员在全球范围内高效地扩展其电子邮件促销活动。 此功能允许您获取已获批准的电子邮件体验，并使用Azure Open AI翻译服务将其翻译为多种目标语言。

+++

+++2025.07.25版注释

### 兼容的资产过滤器

[!DNL Insights]模块中的新筛选器会自动从广告预览中隐藏[不受支持的图像和视频资源](/help/user-guide/insights/ads.md#ad-formats)，从而消除视觉混乱和磁贴损坏。 此增强功能可确保用户仅看到实际可用且准备使用的媒体，从而创造更干净和更可靠的体验。 该过滤器与现有兼容性广告过滤器配合使用。

### Meta的多资产激活

Meta广告的多纵横比图像激活允许广告商在单个广告创意下上传和激活多个不同纵横比的图像资源。 此功能使一个广告能够为各种元投放位置（如信息源、故事和胶卷）提供合适的创意内容。 广告商可以预览每个图像在投放位置之间的呈现方式，并在单个API调用中将所有版本发布到Meta。

### 变体中的富文本格式

[使用富文本格式编辑生成的变体中的文本字段](/help/user-guide/create/manage-variants.md#manually-edit-text)选项，包括粗体、斜体、下划线、文本对齐、列表、文本颜色、文本大小和链接。 这允许您优化受众的文本和短语，并应用格式以适应布局要求。

### 图像和链接的可访问性标签

向变体中的图像和call-to-action链接添加辅助功能标签(Aria-labels)，以提供有助于用户了解交互元素用途的辅助功能名称。 有关详细说明，请参阅[管理变体](/help/user-guide/create/manage-variants.md)。

### 非英语内容生成

[!BADGE Beta]{type=Informative tooltip="此功能当前位于Beta中，因此某些功能可能会受到限制或发生更改。"}

提示抽屉中新的语言选择器下拉菜单支持创建多语言内容，从而让区域营销人员能够为其本地受众开发品牌上内容。 此功能当前支持12种GA语言和5种Beta语言，语言列表为LLM提供定义的工作流和明确的语言指令，以实现更一致的输出。

### 适用于Meta广告的可选模板选择

[!BADGE Beta]{type=Informative tooltip="此功能当前位于Beta中，因此某些功能可能会受到限制或发生更改。"}

模板选择现在对于Meta广告是可选的，允许用户创建广告，而无需在媒体顶部使用文本和徽标。 此增强功能允许使用其他媒体类型，例如动画GIF和视频，这些媒体类型可能不需要文本叠加或徽标放置。

+++

+++2025.06.15版注释

### 可用的入门模板

[!BADGE Beta]{type=Informative tooltip="此功能当前位于Beta中，因此某些功能可能会受到限制或发生更改。"}

[入门模板](/help/user-guide/templates/starter-templates.md)提供了一种快速启动创意过程的方法。 您现在可以从Meta或LinkedIn广告启动模板中进行选择。

### 生成性扩展AI功能

[!BADGE Beta]{type=Informative tooltip="此功能当前位于Beta中，因此某些功能可能会受到限制或发生更改。"}

现在，在GenStudio for Performance Marketing [!DNL Create]中，您可以使用[生成扩展AI功能](/help/user-guide/create/manage-variants.md#use-generative-expand)来扩展图像的尺寸，并添加生成内容以适合付费媒体变体的广告模板。

### 将视频添加到广告

[!BADGE Beta]{type=Informative tooltip="此功能当前位于Beta中，因此某些功能可能会受到限制或发生更改。"}

除了图像内容之外，您现在还可以将视频添加到[LinkedIn](/help/user-guide/create/create-linkedin.md#manage-videos)和[Meta](/help/user-guide/create/create-meta-ad.md#manage-videos)广告。 选择并将视频添加到变体时，请直接在GenStudio for Performance Marketing中查看自动播放视频预览。

### 修复和增强功能

* 添加了对[将广告体验](/help/user-guide/activation/activate-linkedin-ad.md)从GenStudio for Performance Marketing发布到LinkedIn营销活动管理器的支持。 [!DNL Activate]在发布到LinkedIn营销活动管理器之前支持详细的LinkedIn广告预览。

* [Workfront Proof集成](/help/user-guide/approvals/overview.md)为GenStudio for Performance Marketing带来了校对的强大审核和审批功能。 在GenStudio for Performance Marketing中审阅的内容会同步到Workfront Proof，并且审阅评论和状态会保留。

* 添加了通过添加辅助功能标签(Aria-labels) [为您的变体中的图像和call-to-action链接](/help/user-guide/create/manage-variants.md#add-accessibility-labels)提供可访问名称的功能。

* 以非英语添加或修订[品牌指南](/help/user-guide/guidelines/brands.md)时，GenStudio for Performance Marketing会以相同的语言显示这些指南。

* 在手动添加[!DNL Brand]或通过手动提取文档创建[!DNL Brand]之后，您可以[更改或添加品牌缩略图图像](/help/user-guide/guidelines/add-guidelines.md#change-brand-thumbnail)，以确保每个品牌都可以轻松地在您的[!DNL Brands]列表中区分。

* 您现在可以在生成的变体中[对文本](/help/user-guide/create/manage-variants.md#manually-edit-text)使用富文本编辑格式。 尝试使用变体文本的各种格式选项，例如颜色、大小、列表等。

* 现在，您可以在平台设置期间通过克隆现有广告集来[创建新的广告集](/help/user-guide/activation/activate-meta-ad.md#create-a-new-ad-set)。 元广告集定义特定广告的时间、渠道详细信息和受众。 Meta营销活动可以包含多个广告集，但一个广告集仅与一个营销活动关联。

* 您现在可以导出营销活动详细信息，以便在Word或PDF中作为营销活动摘要从外部访问。 选择一个营销活动，然后单击&#x200B;**[!UICONTROL 导出]**（右上角）。

+++

+++2025.05.15版注释

### 修复和增强功能

* 启用了[将替代（替代）文本](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)添加到单个变体的图像的功能。
* 添加了[新的Meta宽高比](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) — 横向1.19:1（1080像素宽度）。
* 现在，您可以选择多个体验进行导出或下载。 请参阅[导出体验](/help/user-guide/content/manage-assets.md#export-experiences)。
<!-- * Added support for [publishing ad experiences](/help/user-guide/activation/activate-meta-ad.md) directly from _[!DNL Content]_ [into Google Campaign Manager 360 and Meta Ads Manager](/help/user-guide/activation/activate-cm360-ad.md). -->

+++

+++2025.04.15版注释

### 修复和增强功能

* 新增模板过滤器选项！ 现在，您可以在&#x200B;_[!UICONTROL 和]_&#x200B;内容[!DNL Create] > _[!UICONTROL 模板]_&#x200B;中优化&#x200B;_[!UICONTROL 选择模板]_&#x200B;列表。 请参阅[搜索模板](/help/user-guide/content/use-templates.md#search-templates)。 确保使用元数据正确标记模板，以使这些模板可通过这些过滤器发现。
* 启用了以下功能：[查看和选择体验的单个图层](/help/user-guide/create/manage-variants.md#view-layers)（可编辑文本字段或可编辑图像）以突出显示它们以进行修订，如重新生成内容或裁切图像。
* 添加了[新模板字段](/help/user-guide/content/use-templates.md#template-elements) `sub-headline`，用于在体验中添加其他文本以吸引受众关注并突出显示营销消息。
* 添加了对[将广告体验](/help/user-guide/activation/overview.md)从GenStudio for Performance Marketing发布到Google Campaign Manager 360的支持。 激活在发布到Google Campaign Manager 360广告商之前支持详细的Campaign Manager 360广告预览。 通过激活发布的广告一经上线，就会自动提取到分析中，使用户能够跟踪和报告广告效果。

+++

+++2025.03.13版注释

### 激活Meta广告

营销人员现在可以将GenStudio for Performance Marketing中的[广告体验](/help/user-guide/activation/overview.md)发布到元广告管理器。 [!DNL Activate]支持部署前的详细Meta广告预览。 通过[!DNL Activate]发布的Meta广告一旦上线即自动提取到[!DNL Insights]中，使用户能够跟踪和报告广告效果。

### 创建LinkedIn体验

[!BADGE Beta]{type=Informative tooltip="此功能当前位于Beta中，因此某些功能可能会受到限制或发生更改。"}

添加了对[创建LinkedIn体验](/help/user-guide/create/create-linkedin.md)的支持。 请参阅特定于渠道的指南中的[LinkedIn广告](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines)选项卡。

### 创建横幅体验

[!BADGE Beta]{type=Informative tooltip="此功能当前位于Beta中，因此某些功能可能会受到限制或发生更改。"}

添加了对[创建横幅体验](/help/user-guide/create/create-banner-experience.md)的支持。 请参阅特定于渠道的指南中的[横幅](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines)选项卡。

### 合规性

作为品牌验证流程的一部分，[内容检查](/help/user-guide/guidelines/overview.md)中引入了[合规性标准](/help/user-guide/guidelines/brand-validation.md)。 这些检查将根据[!DNL Brand]指南、平台指南(如Meta)和ADA标准审查体验中的每个变体。 此过程全面总结了需要修订的准则和标准，以更好地满足合规性要求。

### 可扩展性

新的GenStudio for Performance Marketing [可扩展性框架](/help/extensibility/setup.md)为组织提供了工具，使它们可以将自己的声明合规性协议纳入内容创建工作流并通过插件或可扩展应用程序进行验证。

### 模板

* **模板代码编辑器** — 新的[模板代码编辑器](/help/user-guide/content/code-editor.md)可帮助您验证和优化您的模板，以便在使用GenStudio for Performance Marketing生成新体验时获得最佳使用。

  ![代码编辑器视图](/help/assets/template-detected-fields.png "检查检测到的字段"){width="500" zoomable="yes"}

* **图像上的链接** — 通过启用图像链接来自定义您的电子邮件模板。 请参阅[自定义模板：映像](/help/user-guide/content/customize-template.md#link-on-image)上的链接。
* **AJO和Marketo模板** — 上传您在Adobe Journey Optimizer (AJO)或Marketo中创建的模板。 请参阅[使用AJO和Marketo中的模板](/help/user-guide/content/use-templates.md#templates-from-ajo-and-marketo)。

### 修复和增强功能

* 为[的](/help/user-guide/guidelines/brands.md#channel-guidelines)默认渠道[、](/help/user-guide/guidelines/brands.md#image-guidelines)图像[、](/help/user-guide/guidelines/brands.md#logos)徽标[和](/help/user-guide/guidelines/brands.md#colors)颜色[[!DNL Brands]](/help/user-guide/guidelines/brands.md)准则启用功能。
* 添加了将链接[添加到变体中的图像](/help/user-guide/create/manage-variants.md#add-image-link)的功能。
* 已将[内容检查](/help/user-guide/guidelines/brand-validation.md)和审核和批准功能移至新的右侧操作栏，以最大化画布上的空间并改善用户体验。
* 简化了[上传或手动添加品牌](/help/user-guide/guidelines/add-guidelines.md#add-brands)的流程。
* 引入了在画布上的变体[中](/help/user-guide/create/manage-variants.md#swap-image)添加或交换图像资产的功能。
* 通过将渠道类别[划分到自有媒体、付费媒体和内容部分，改进了创建主页](/help/user-guide/create/overview.md)上的用户体验和可见性。
* 改进了[!DNL Insights]表和图库视图中的筛选。

+++

+++2025.02.13版注释

### [!DNL Create]的登陆页面改进

GenStudio for Performance Marketing中的[!DNL Create]登陆页面包含可增强用户体验的UI改进。 _最近工作_&#x200B;部分已优化并使用列表视图配置为默认视图。 填充和其他视觉改进可简化[!DNL Create]画布的外观。

### 分析导出到CSV

您现在可以将可见表从任何[!DNL Insights]视图下载到CSV文件中。 此功能允许您从各种[!DNL Insights]视图导出和分析数据，从而方便数据分析和报告选项。

+++

+++2025.01.16版注释

### 与Adobe Workfront Proof集成

[!BADGE Beta]{type=Informative tooltip="此功能当前位于Beta中，因此某些功能可能会受到限制或发生更改。"}

GenStudio for Performance Marketing与Adobe Workfront Proof集成Beta程序将于本月启动。 Workfront Proof通过审批模板、多阶段工作流和注释来加快内容创建和激活生命周期。 拥有Workfront Proof权限的GenStudio for Performance Marketing用户可以使用GenStudio for Performance Marketing中的Proof高级功能来查看和评论GenStudio生成的内容。

Beta项目提供了一种帮助制定产品开发并确定一般可用性准备情况的方法。

### 生成新的行动号召

现在，您可以在管理变体时生成新的call-to-action (CTA)短语。 使用新的&#x200B;_重新短语_&#x200B;和&#x200B;_添加链接_&#x200B;选项来生成新短语并编辑CTA链接。 必须正确设置您的模板，这些新的CTA功能才能正常工作。 遵循&#x200B;_自定义模板_&#x200B;中的准则： [行动号召](/help/user-guide/content/customize-template.md#calls-to-action)。 有关管理变体中CTA的准则，请参阅[修订Call to action](/help/user-guide/create/manage-variants.md#revise-call-to-action)。<!-- GS-6676 -->

### 修复和增强功能

* 现在，字符计数将显示在所有生成的和手动的显示广告字段中。 查看&#x200B;_元体验_&#x200B;中的[字符数](/help/user-guide/create/meta-experiences.md#character-counts)。<!-- GS-7732 -->

* _协作者_&#x200B;现在可以查看资源，但不能创建、编辑或删除这些资源。 以前，[!DNL Create]中未按预期强制执行协作者授权。<!-- GS-7614 -->

* 内容编辑者现在可以编辑资产、体验和模板元数据。<!-- GS-4905 -->

* 现在支持Meta广告模板中的自定义图像大小。<!-- GS-7512 -->

* 现在，在生成模板期间会预加载角色、品牌和产品选择。<!-- GS-8069 -->

* 电子邮件call-to-action链接不再是必填字段。<!-- GS-8103 -->

* [!DNL Brand]选择器下拉菜单现在对模板按预期工作。 以前，某些模板的选择器无法成功加载。<!-- GS-8908 -->

* 现在，编辑人员最多可以为单面板电子邮件和Meta广告选择四个图像。<!-- GS-2631 -->

* 在编辑体验的元数据后，已批准体验的`Created by`字段的年份值现在与预期一致。<!-- GS-8344 -->

* 内容编辑者现在可以从[!DNL Create]中成功选择模板。 以前，当编辑器选择模板时，应用程序会引发控制台错误。 <!-- GS-8798 -->

* Meta广告的调整大小和重新生成操作问题已得到解决。<!-- GS-8900 -->

* 现在，**[!UICONTROL 返回]**&#x200B;按钮会按预期将用户返回到上一页或[!DNL Create]登陆页面。<!-- GS-8622 -->

+++

+++2024.12.12版注释

### 新增功能

编辑器现在可以执行以下与元数据相关的任务：

* 编辑资源、体验和模板元数据。 查看[资源详细信息](/help/user-guide/content/asset-details.md#user-defined-metadata)。<!-- GS-4905 6935-->

* 在使用资产的任何体验的&#x200B;_详细信息_&#x200B;视图中查看资产生成的标记。 查看&#x200B;_资产详细信息_&#x200B;中的[生成的标记](/help/user-guide/content/asset-details.md#generated-tags)。<!-- GS-3705 -->

编辑器现在可以为生成的变量的以下方面指定自定义值：

* 展示广告模板中的Web横幅的宽度和高度。 这些值现在另存为模板元数据。<!-- GS-6735 -->

* 图像上传期间显示广告体验中的图像尺寸。<!-- GS-7166 -->

* 请参阅[模板最佳实践](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines)中特定于渠道的准则。

导出选项现在包括：

* 将显示广告和元广告导出为HTML、JPEG或PNG。 请参阅[创建显示广告体验](/help/user-guide/create/create-display-ad.md)和[创建元广告体验](/help/user-guide/create/create-meta-ad.md)。<!-- GS-7093 6655 5152-->

通过其他新功能，编辑器可以：

* 使用&#x200B;**[!UICONTROL 模板]**&#x200B;资产详细信息[!DNL Content]视图上的&#x200B;_刷新_&#x200B;按钮刷新所选模板。<!-- GS-7102 -->

* 重新生成显示广告和电子邮件变体的部分。 请参阅[创建显示广告体验](/help/user-guide/create/create-display-ad.md#revise-generated-display-ads)和[创建电子邮件体验](/help/user-guide/create/create-email-experience.md#revise-generated-emails)。<!-- GS-5080 5078-->

* 复制现有品牌。 查看[管理品牌](/help/user-guide/guidelines/brands.md#manage-brands)。<!-- BRANDS-548 -->

### 修复和增强功能

* 显示广告标题现已按预期保存到[!DNL Content]。<!-- GS-7239 -->

* 当编辑器在抽屉下拉菜单外单击时，提示抽屉不再关闭。<!-- GS-7275 -->

* 当发生缩略图URL服务错误时，[!DNL Create] [!DNL Persona]/[!DNL Product]下拉菜单现在按预期加载。<!-- GS-7277 -->

* 包含叠加片段的元素的显示广告现在可以编辑。<!-- GS-7186 -->

* 现在未为体验生成品牌得分时，画布&#x200B;**[!UICONTROL 品牌]**&#x200B;按钮处于禁用状态。<!-- GS-6429 -->

* Canvas现在按一致的顺序显示调整大小的体验。<!-- GS-7123 -->

* 现在，在编辑显示广告时，手动裁切将使用图像尺寸，而不是模板尺寸。 以前，当图像小于显示广告模板中指定的尺寸时，边界框使用模板尺寸，而不是图像尺寸。<!-- GS-7315 -->

* 现在，编辑者在创建显示广告时最多可以选择四个图像。<!-- GS-7189 -->

* 现在，在其他浏览器中调整大小时，显示广告和Meta广告草稿会按预期加载。<!-- GS-7204 -->

* 未使用的模板字段不再显示在生成的内容中。 <!-- GS-5670 -->

* 编辑器现在可以单击链接，以按预期在生成的变体中进行编辑。<!-- GS-7423 -->

* [!DNL Create]现在正确尊重协作者权限。<!-- GS-7614 -->

* 在选择和呈现所有调整大小选项后，现在将禁用画布&#x200B;**[!UICONTROL 调整大小]**&#x200B;按钮。<!-- GS-5940 -->

* 现在，具有仅查看访问权限的审阅人在审阅期间可以放大和缩小变体。<!-- GS-7371 -->

* 已将键盘焦点添加到[!DNL Create] _最近工作_&#x200B;视图上仅可操作的按钮。<!-- GS-4060 -->

* 现在，在电子邮件片段保存操作期间显示的&#x200B;**正在保存**&#x200B;消息仅在保存操作期间显示。 以前，画布会无限期地显示此消息。<!-- GS-6964 -->

* 现在，当草稿无法在[!DNL Create] _最近工作_&#x200B;区域加载时，编辑人员会按预期看到错误消息。 <!-- GS-8081 -->

* Canvas现在按正确顺序显示调整大小的元广告和显示广告。 <!-- GS-7375 -->

* 编辑者现在可以单击进入电子邮件和显示广告的字段。<!-- GS-6297 -->

* 电子邮件和元广告的编辑片段功能现在会按预期通过一次单击触发。<!-- GS-8081 -->

* 改进了[!DNL Create] **[!UICONTROL 返回]**&#x200B;按钮的性能。<!-- GS-6767 -->

+++

+++2024.11.14版注释

### 新增功能

添加了对显示托管在外部域上的静态内容的支持。 GenStudio for Performance Marketing验证模板中定义的内容源，并嵌入一个副本以生成模板预览。 查看[静态内容](/help/user-guide/content/customize-template.md#static-content)。<!-- GS-6107 -->

### 修复和增强功能

* 在用于生成初始内容的浏览器以外的浏览器中调整大小时，草稿现在会按预期加载。<!-- GS-7204 -->

* 现在，导出的HTML中的所有字符均可正确显示。<!-- GS-7246 -->

* 在某些语言中，[!DNL Content] _体验_ **[!UICONTROL 导出]**&#x200B;弹出窗口上的按钮不再被截断。<!-- GS-6873 -->

* 现在，使用大小为50x50的模板创建的显示广告会以预期的图像大小导出。 以前，PNG文件的导出尺寸是预期尺寸的两倍。<!-- GS-7192 -->

* 现在可以解决调整显示广告大小时发生的模板错误。<!-- GS-7322 -->

### 本地化

此版本包括对整个UI的本地化的改进，包括：

* [!DNL Content] _上传资产_&#x200B;弹出窗口中的所有字符串现在都已正确本地化。<!-- GS-6872 6770 -->
* [!DNL Content] _Assets_&#x200B;视图&#x200B;**[!UICONTROL 搜索]**&#x200B;字段中的所有工具提示都已本地化。<!-- GS-6879 -->
* 替换[!DNL Create]画布上的电子邮件变体中的现有图像时，_从内容中选择_&#x200B;视图现在已本地化。<!-- GS-6906 -->

+++

+++2024.11.07版注释

### 修复和增强功能

* 当用户单击&#x200B;_上传新图像_&#x200B;然后在上传完成之前取消操作时，**[!UICONTROL 正在保存]**&#x200B;旋转图标不再显示。<!-- GS-6780 -->

* 现在，可在体验重新生成期间正确创建体验标题。<!-- GS-7006 -->

* 解决了在绘制加载期间滚动条闪烁的问题。<!-- GS-5587 -->

* `View documentation` [!DNL Content]添加您的批准模板&#x200B;_弹出窗口中的_&#x200B;链接现在按预期工作。<!-- GS-6881 -->

* 在调整大小操作期间从提示抽屉中删除图像不再导致错误。<!-- GS-7115 7009 -->

* 从&#x200B;**[!UICONTROL 操作菜单(...)中选择]**&#x200B;删除[!DNL Create]现在可按预期工作。<!-- GS-6871 -->

* 用户现在可以单独通过键盘控制所有元和模板交互元素。<!-- GS-4066 -->

* 将图像维度从模板图像字段提取添加到显示广告模板。 智能裁剪请求现在针对图像的实际维度而不是整个模板发送。 <!-- GS-6926 -->

* 已本地化生成的电子邮件和元广告中的`Zoom to fit to screen`字符串。<!-- GS-5063 -->

* 当用户点击离开时，[!DNL Create]提示抽屉现在会按预期关闭。<!-- GS-5254 -->

* Meta广告导出现在会按预期包含选定的call-to-action标签。<!-- GS-6504 -->

* 品牌分数现在会按预期更新并保留在重新生成的体验中。<!-- GS-6535 -->

* Meta广告和显示广告的HTML导出不再包含包装器`div`和`chrome`元素。<!-- GS-7116 -->

* 现已解决发布期间电子邮件草稿呈现问题。<!-- GS-6394 -->

* 未生成品牌分数时，画布&#x200B;**[!UICONTROL 品牌]**&#x200B;按钮现在已禁用。<!-- GS-6429 -->

* 启用`ReadOnly`画布设置后，画布操作栏上的Facebook/Instagram切换现在会按预期更新体验渲染。<!-- GS-7039 -->

#### 图像再生

* 现在，可按预期调整多个Meta广告变体的大小。 以前，画布不显示重新生成的变体，而是保持空白。<!-- GS-7010 -->

* 片段重新生成现在可以按预期方式用于调整大小的体验。<!-- GS-6836 -->

* 在调整Meta广告图像的大小后重新生成这些图像不再会导致错误。 以前，在重新生成之前调整图像大小会将渠道元数据从`meta`更改为`facebook`。<!-- GS-7042 -->

+++

+++2024.10.31版注释

### 新增功能

* **[!DNL Content]**&#x200B;搜索筛选器现在支持按颜色标记搜索。<!-- GS-5501 -->

* **[!DNL Create]**&#x200B;画布现在显示电子邮件片段的字符数。<!-- GS-5819 -->

### 修复和增强功能

* 缺少的屏幕阅读器标签已添加到移动设备和桌面`view`元素中。<!-- GS-5624 4729 -->

* **[!DNL Create]**&#x200B;画布电子邮件主题行和预标题文本区域的高度现在为动态的。<!-- GS-6258 -->

* 电子邮件边框的布局问题已得到解决。<!-- GS-6631 -->

* 在&#x200B;**[!DNL Content]** **[!UICONTROL 删除]**&#x200B;按钮上，键盘焦点现在可以按预期工作。 以前，用户无法通过键盘访问此按钮。  <!-- GS-4065 -->

+++

+++2024.10.14版发行说明

此发行版本引入了Adobe GenStudio for Performance Marketing，这是一个基于人工智能的创新型应用程序，可加快营销活动的规划、开发和分析。 GenStudio for Performance Marketing使营销团队能够为广告、电子邮件和营销活动创建基于品牌的多渠道内容，同时提供实时见解以优化内容性能。

### 特性

主要产品功能包括：

**[!DNL Create]**&#x200B;引入了Canvas，它提供了一种结构化的提示体验，使内容编辑者能够快速生成内容和变体。 系统管理员根据组织品牌准则对产品进行培训。 [!DNL Create]确保所有AI生成的内容都与您的品牌准则（品牌策略、客户角色和产品描述）保持一致，并简化产生高影响力、品牌一致的营销内容。

**[!DNL Content]**&#x200B;存储策划的、符合品牌标准的已批准资产和体验。 GenStudio for Performance Marketing用户可以轻松查找、编辑、重新调整用途和共享经过批准的资源，从而无需为每个活动从头开始重新创建内容。

**[!DNL Reviews and Approvals]**&#x200B;建立了一个框架，供利益相关者在保存到&#x200B;**[!DNL Content]**&#x200B;或导出之前审核和批准生成的变体。

**[!DNL Campaigns]**&#x200B;组织和管理营销活动，确保优化执行和跟踪。 协作者可以可视化、规划和跟踪活动，从而有效地管理多个计划并确保及时交付。

**[!DNL Insights]**&#x200B;提供内容性能的实时评估，帮助营销人员优化其策略并做出数据驱动型决策。

GenStudio for Performance Marketing与其他Adobe Experience Cloud产品集成，包括Adobe Express和Adobe AEM Assets。

+++
