---
title: 生成图像
description: 在Adobe [!DNL GenStudio] 中创建与参考图像的样式匹配的图像以进行性能营销。
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
badgeBeta: label="Beta" tooltip="此功能当前位于Beta中，因此某些功能可能会受到限制或发生更改。"
role: User
level: Beginner
recommendations: noDisplay
exl-id: c1118ada-7fee-43cd-aff4-eab69539afb4
source-git-commit: 47195c08f500e50a01db127c6badc461c10afaf9
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 0%

---

# 生成图像

使用GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) （画笔图标），您可以生成&#x200B;_[!DNL On-brand images]_&#x200B;生成的资源，这些资源从所选图像中获得灵感，捕捉其视觉效果和整体美感。<!-- [two types of images](#image-types) using GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (paintbrush icon)—_[!DNL On-brand images]_ and _[!DNL Similar images]_. -->

若要设计引人注目的有效图像，建议您[将准则添加到GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md)，并查看[编写提示的基础知识](/help/user-guide/effective-prompts.md)。

## 图像类型

_[!DNL On-brand images]_&#x200B;是生成的资产，从选定的图像获得灵感，捕捉其视觉效果和整体美感。 这些图像是使用[!DNL Content]中已有的图像以及精心编制的指导设计的提示创建的。 它们严格遵循品牌指南和在生成过程中选择的参数。

_[!DNL On-brand images]_<!-- and _[!DNL Similar images]_ -->合并了设置的准则、参数和[精心编制的提示](/help/user-guide/effective-prompts.md)，以提供引人注目的图像资产。

<!-- * _[!DNL Similar images]_—Image assets created with strong similarity to an existing selected image available in [!DNL Content]. When generating similar images, GenStudio for Performance Marketing redesigns the selected image, giving slight variations on the content to provide variety and nuance. -->

## 生成品牌内图像

您可以使用定义的准则、参数和选定的参考图像来生成[!DNL On-brand images]。 这些元素与您的提示一起指导生成一致的[!DNL On-brand image]变量。

### 选择参考图像

要创建&#x200B;_[!DNL On-brand images]_，请选择保存在[!DNL Content]中的现有图像。 有关支持的[维度的信息，请参阅](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines)模板的最佳实践[!DNL on-brand image]。

**选择参考图像**：

1. 在&#x200B;_[!DNL Create]_&#x200B;中，单击&#x200B;**[!UICONTROL 品牌上图像]**。
1. 使用&#x200B;_筛选器_&#x200B;旁边的搜索选项查找特定图像。

   ![选择参考图像](/help/assets/select-img.png){width="400" zoomable="yes"}

   若要使用已连接[!DNL AEM Assets Content Hub]存储库中的资源，请从&#x200B;_位置_&#x200B;下拉菜单中选择一个存储库。 筛选并选择一个图像。

1. 在&#x200B;_选择图像_&#x200B;视图中，单击图像。

   所选图像的大小最多可达10MB。

1. 单击&#x200B;**[!UICONTROL 使用]**。

   此时将显示画布，它是内容创建的中心中心。

### 添加参数

纳入[准则](/help/user-guide/guidelines/overview.md)和参数可增强内容生成过程，是生成[!DNL on-brand image]的重要准备步骤。

**要添加准则和参数**：

1. 在&#x200B;_基本_&#x200B;选项卡中，选择[!DNL Brand]以通知内容创建。

   如果此菜单中没有可用的品牌，请[将指南添加到您的GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md)。

1. 从&#x200B;_[!UICONTROL 图像类别]_&#x200B;中选择最适合您所需结果的图像类别。

   如果选择[!DNL Brand]，则图像类别可用。 这些选项由选定的[!DNL Brand]决定。

<!-- 1. _(Optional)_ Select a custom model from _[!UICONTROL Model]_.

   Models are available if you access to [custom models in Firefly](https://adobedx.slack.com/archives/CMF1JGMLY/p1743534402774569). The _Models_ list will be blank if you do not have access. -->

1. 从&#x200B;_[!UICONTROL 宽高比]_&#x200B;中选择所需的宽高比。
1. 单击&#x200B;**[!UICONTROL 从]**&#x200B;样式引用&#x200B;_[!UICONTROL 中的内容]_&#x200B;中选择以添加引用图像。 您选择的图像会影响所生成图像的视觉美感和深度。

   若要使用已连接[!DNL AEM Assets Content Hub]存储库中的资源，请从&#x200B;_位置_&#x200B;下拉菜单中选择一个存储库。 筛选并选择一个图像。

1. 在&#x200B;_高级_&#x200B;选项卡中，选择&#x200B;_内容类型_。

   已根据所选[!DNL Brand]—_Art_&#x200B;或&#x200B;_Photo_ — 存在的图像类别预先选择了该选项，并且不可编辑。

1. 在&#x200B;_[!UICONTROL 视觉强度]_&#x200B;中调整图像现有视觉特征的整体强度。

### 输入提示

选择参数后，使用自然语言编写提示以开始生成品牌图像。

请参阅[编写有效的提示](/help/user-guide/effective-prompts.md)。

**输入提示**：

1. 在提示框中输入提示。
1. 单击&#x200B;**[!UICONTROL 生成]**。

默认情况下，将生成四个变体（由所添加的提示、参数和内容提供）并显示在画布中。

### 在Adobe Express中编辑

生成图像变体后，您可以使用Adobe Express直接在Adobe GenStudio for Performance Marketing中编辑它们。

**要使用Adobe Express编辑单个图像**：

1. 将鼠标悬停在生成的图像变体上，然后单击&#x200B;_[!UICONTROL 在Adobe Express中编辑]_。

   出现&#x200B;_Powered by Adobe Express_&#x200B;窗口。

1. 执行图像编辑，如[裁剪图像](https://helpx.adobe.com/cn/express/create-and-edit-images/edit-images/crop-images.html)、[删除对象](https://helpx.adobe.com/cn/express/create-and-edit-images/create-and-modify-with-generative-ai/remove-objects-generative-fill.html)以及应用效果。

   请参阅[Adobe Express文档](https://helpx.adobe.com/cn/express/user-guide.html)，了解如何使用Adobe Express在GenStudio for Performance Marketing中修改图像。

1. 单击&#x200B;_[!UICONTROL 应用更改]_&#x200B;以保存您的编辑。
1. 根据需要继续编辑单个图像变体，并应用更改以保存进度。

### 验证内容检查对齐方式

要优化生成的变体并确保严格遵守品牌标识、平台准则和辅助功能标准，请利用&#x200B;[_内容检查_&#x200B;面板](/help/user-guide/guidelines/brand-validation.md#content-check-panel)的强大功能。 此面板可显示全面的内容检查详细信息并阐明改进领域。

**要执行内容检查**：

1. 单击右侧操作栏中的&#x200B;_内容检查_&#x200B;面板图标以打开&#x200B;[_内容检查_&#x200B;面板](/help/user-guide/guidelines/brand-validation.md#content-check-panel)。 查看&#x200B;*需要审核*&#x200B;和&#x200B;*通过*&#x200B;检查的摘要，以查看哪些部分和准则需要改进。

   ![_内容检查_&#x200B;面板](/help/assets/content-check-img.png){width="500" zoomable="yes"}

1. 修订图像变体以确保您的变体与执行的内容检查紧密对齐。

请参阅[品牌验证](/help/user-guide/guidelines/brand-validation.md)。

<!-- ## Generate Similar images

You can quickly generate images similar to a selected image within [!DNL Content] from the [!DNL Create] home.

**To create _[!DNL Similar images]_**:

1. In _[!DNL Create]_, click **[!UICONTROL Similar images]**.
1. Use the search option, adjacent to _Filter_, to find a specific image.

   To use assets from a connected [!DNL AEM Assets Content Hub] repository, choose a repository from the _Location_ drop-down menu. Filter and select one image.

1. In the _Select image_ view, click on an image.
1. Click **[!UICONTROL Use]**.

   The Canvas, which serves as the central hub for content creation, is displayed. Four image variations similar to the original selected image appear.

   ![Generate similar images](/help/assets/generate-similar.png){width="400" zoomable="yes"} -->

## 发布和导出图像

生成的图像草稿显示在&#x200B;_主页的_ Recents[!DNL Create]部分中。

要使生成的图像可用于当前和将来使用，请将它们发布到[!UICONTROL 内容]并将其导出以用于您的营销活动。

1. **要发布新图像**，请单击顶部工具栏中的&#x200B;**[!UICONTROL 发布]**。
   1. 如果需要，_[!UICONTROL 添加详细信息]_，如&#x200B;_[!UICONTROL 营销活动]_&#x200B;或&#x200B;_[!UICONTROL 渠道]_。
   1. 单击&#x200B;**[!UICONTROL 发布]**。

1. **要导出新图像**，请单击顶部工具栏中的&#x200B;**[!UICONTROL 导出]**。
   1. 选择格式 — JPG或PNG — 并单击&#x200B;**[!UICONTROL 导出]**。

请参阅[[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content)。
