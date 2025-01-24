---
title: Adobe GenStudio for Performance Marketing发行说明
description: 了解 Adobe GenStudio for Performance Marketing 的最新功能和增强功能。
recommendations: noDisplay
last-substantial-update: 2025-01-16T00:00:00Z
exl-id: 32f5104e-ae15-4092-8a34-642fc641baf9
source-git-commit: a14da101907c3e7dd990082723f7c59f7f5ff3fd
workflow-type: tm+mt
source-wordcount: '1676'
ht-degree: 1%

---

# GenStudio for Performance Marketing发行说明

此发行信息详细介绍了GenStudio for Performance Marketing应用程序的最新更新。

## 2025.1.16 {#latest}

### 与Adobe Workfront Proof集成

[!BADGE Beta]{type=Informative tooltip="此功能当前位于Beta中，因此某些功能可能会受到限制或发生更改。"}

GenStudio for Performance Marketing与Adobe Workfront Proof集成Beta程序将于本月启动。 Workfront Proof通过审批模板、多阶段工作流和注释来加快内容创建和激活生命周期。 拥有Workfront Proof权限的GenStudio for Performance Marketing用户可以使用GenStudio for Performance Marketing中的Proof高级功能来查看和评论GenStudio生成的内容。

Beta项目提供了一种帮助制定产品开发并确定一般可用性准备情况的方法。 有关GenStudio for Performance Marketing/Workfront Proof集成Beta计划的信息，请联系Etienne Bosch (etienneb@adobe.com) 。

### 生成新的行动号召

现在，您可以在管理变体时生成新的行动号召(CTA)短语。 使用新的&#x200B;_重新短语_&#x200B;和&#x200B;_添加链接_&#x200B;选项来生成新短语并编辑CTA链接。 必须正确设置您的模板，这些新的CTA功能才能正常工作。 遵循&#x200B;_自定义模板_&#x200B;中的准则： [行动号召](/help/user-guide/content/customize-template.md#calls-to-action)。 有关管理变体中CTA的准则，请参阅[修改行动号召](/help/user-guide/create/manage-variants.md#revise-call-to-action)。<!-- GS-6676 -->

以下预览显示CTA字符计数、新选项以及重新短语和替换示例：

![CTA重新短语操作](/help/assets/animation/rephrase-cta.gif "CTA重新短语"){width="250" zoomable="yes"}

### 修复和增强功能

* 现在，字符计数将显示在所有生成的和手动的显示广告字段中。 查看[元体验](/help/user-guide/create/meta-experiences.md#character-counts)中的&#x200B;_字符数_。<!-- GS-7732 -->

* _协作者_&#x200B;现在可以查看资源，但不能创建、编辑或删除这些资源。 以前，协作者权限未按[!DNL Create]中的预期执行。<!-- GS-7614 -->

* 内容编辑者现在可以编辑资产、体验和模板元数据。<!-- GS-4905 -->

* 现在支持在元广告模板中自定义图像大小。<!-- GS-7512 -->

* 现在，在生成模板期间会预加载角色、品牌和产品选择。<!-- GS-8069 -->

* 电子邮件行动号召链接不再是必填字段。<!-- GS-8103 -->

* [!DNL Brand]选择器下拉菜单现在对模板按预期工作。 以前，某些模板的选择器无法成功加载。<!-- GS-8908 -->

* 现在，编辑者最多可以为单面板电子邮件和元广告选择四个图像。<!-- GS-2631 -->

* 在编辑体验的元数据后，已批准体验的`Created by`字段的年份值现在与预期一致。<!-- GS-8344 -->

* 内容编辑者现在可以从[!DNL Create]中成功选择模板。 以前，当编辑器选择模板时，应用程序会引发控制台错误。 <!-- GS-8798 -->

* 解决了为元广告调整大小和重新生成操作的问题。<!-- GS-8900 -->

* 现在，**[!UICONTROL 返回]**&#x200B;按钮会按预期将用户返回到上一页或[!DNL Create]登陆页面。<!-- GS-8622 -->

## 早期发行说明

+++2024.12.12版注释

### 新增功能

编辑器现在可以执行以下与元数据相关的任务：

* 编辑资源、体验和模板元数据。 查看[资源详细信息](/help/user-guide/content/asset-details.md#user-defined-metadata)。<!-- GS-4905 6935-->

* 在使用资产的任何体验的&#x200B;_详细信息_&#x200B;视图中查看资产生成的标记。 查看[资产详细信息](/help/user-guide/content/asset-details.md#generated-tags)中的&#x200B;_生成的标记_。<!-- GS-3705 -->

编辑器现在可以为生成的变量的以下方面指定自定义值：

* 展示广告模板中的Web横幅的宽度和高度。 这些值现在另存为模板元数据。<!-- GS-6735 -->

* 图像上传期间显示广告体验中的图像Dimension。<!-- GS-7166 -->

* 请参阅[模板最佳实践](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines)中特定于渠道的准则。

导出选项现在包括：

* 将展示广告和元广告导出为HTML、JPEG或PNG。 请参阅[创建显示广告体验](/help/user-guide/create/create-display-ad.md)和[创建元广告体验](/help/user-guide/create/create-meta-ad.md)。<!-- GS-7093 6655 5152-->

通过其他新功能，编辑器可以：

* 使用[!DNL Content]模板&#x200B;_资产详细信息_&#x200B;视图上的&#x200B;**[!UICONTROL 刷新]**&#x200B;按钮刷新所选模板。<!-- GS-7102 -->

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

* 现在，在其他浏览器中调整大小时，显示广告和元广告草稿会按预期加载。<!-- GS-7204 -->

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

* 现在，所有字符在导出的HTML中均可正确显示。<!-- GS-7246 -->

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

* 当用户单击&#x200B;**[!UICONTROL 上传新图像]**&#x200B;然后在上传完成之前取消操作时，_正在保存_&#x200B;旋转图标不再显示。<!-- GS-6780 -->

* 现在，可在体验重新生成期间正确创建体验标题。<!-- GS-7006 -->

* 解决了在绘制加载期间滚动条闪烁的问题。<!-- GS-5587 -->

* [!DNL Content] _添加您的批准模板_&#x200B;弹出窗口中的`View documentation`链接现在按预期工作。<!-- GS-6881 -->

* 在调整大小操作期间从提示抽屉中删除图像不再导致错误。<!-- GS-7115 7009 -->

* 从[!DNL Create]操作菜单(...)中选择&#x200B;**[!UICONTROL 删除]**&#x200B;现在可按预期工作。<!-- GS-6871 -->

* 用户现在可以单独通过键盘控制所有元和模板交互元素。<!-- GS-4066 -->

* 将图像维度从模板图像字段提取添加到显示广告模板。 智能裁剪请求现在针对图像的实际维度而不是整个模板发送。 <!-- GS-6926 -->

* 已本地化生成的电子邮件和元广告中的`Zoom to fit to screen`字符串。<!-- GS-5063 -->

* 当用户点击离开时，[!DNL Create]提示抽屉现在会按预期关闭。<!-- GS-5254 -->

* 元广告导出现在包括按预期显示的行动号召标签。<!-- GS-6504 -->

* 品牌分数现在会按预期更新并保留在重新生成的体验中。<!-- GS-6535 -->

* 元广告和显示广告的HTML导出不再包含包装器`div`和`chrome`元素。<!-- GS-7116 -->

* 现已解决发布期间电子邮件草稿呈现问题。<!-- GS-6394 -->

* 未生成品牌分数时，画布&#x200B;**[!UICONTROL 品牌]**&#x200B;按钮现在已禁用。<!-- GS-6429 -->

* 启用`ReadOnly`画布设置后，画布操作栏上的Facebook/Instagram切换现在会按预期更新体验渲染。<!-- GS-7039 -->

#### 图像再生

* 调整多个元广告变体的大小现在可按预期工作。 以前，画布不显示重新生成的变体，而是保持空白。<!-- GS-7010 -->

* 片段重新生成现在可以按预期方式用于调整大小的体验。<!-- GS-6836 -->

* 在调整元广告图像大小后重新生成它们不再会导致错误。 以前，在重新生成之前调整图像大小会将渠道元数据从`meta`更改为`facebook`。<!-- GS-7042 -->

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

### 功能

主要产品功能包括：

**[!DNL Create]**&#x200B;引入了Canvas，它提供了一种结构化的提示体验，使内容编辑者能够快速生成内容和变体。 系统管理员根据组织品牌准则对产品进行培训。 [!DNL Create]确保所有AI生成的内容都与您的品牌准则（品牌策略、客户角色和产品描述）保持一致，并简化产生高影响力、品牌一致的营销内容。

**[!DNL Content]**&#x200B;存储策划的、符合品牌标准的已批准资产和体验。 GenStudio for Performance Marketing用户可以轻松查找、编辑、重新调整用途和共享经过批准的资源，从而无需为每个活动从头开始重新创建内容。

**[!DNL Reviews and Approvals]**&#x200B;建立了一个框架，供利益相关者在保存到&#x200B;**[!DNL Content]**&#x200B;或导出之前审核和批准生成的变体。

**[!DNL Campaigns]**&#x200B;组织和管理营销活动，确保优化执行和跟踪。 协作者可以可视化、规划和跟踪活动，从而有效地管理多个计划并确保及时交付。

**[!DNL Insights]**&#x200B;提供内容性能的实时评估，帮助营销人员优化其策略并做出数据驱动型决策。

GenStudio for Performance Marketing与其他Adobe Experience Cloud产品集成，包括Adobe Express和AdobeAEM Assets。

+++
