---
title: 创建横幅体验
description: 了解如何在Adobe [!DNL GenStudio] 中创建用于性能营销的横幅体验。
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
badgeBeta: label="Beta" tooltip="此功能当前位于Beta中，因此某些功能可能会受到限制或发生更改。"
role: User
level: Beginner
recommendations: noDisplay
exl-id: c5d541a9-a97b-44da-a15c-61aceefd0e8c
source-git-commit: f49a2bd241f98dda23f6612f8c699ec49d222a12
workflow-type: tm+mt
source-wordcount: '999'
ht-degree: 0%

---

# 创建横幅体验

本教程向您展示如何使用GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md)创建品牌[横幅体验](banner-experiences.md)（左侧导航区域中的画笔图标）。

若要设计引人入胜的横幅体验，建议在开始之前[将准则添加到GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md)并查看[编写提示的基础知识](/help/user-guide/effective-prompts.md)。

## 选择模板

要创建横幅体验，请使用可用的模板为内容提供框架。 有关支持的横幅维度的信息，请参阅[模板最佳实践](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines)。

**选择横幅模板**：

1. 在&#x200B;_[!DNL Create]_中，单击&#x200B;**[!UICONTROL 横幅]**。
1. 使用&#x200B;_筛选器_&#x200B;旁边的搜索选项查找特定的横幅模板。
1. 在&#x200B;_选择模板_&#x200B;视图中，单击横幅模板。
1. 单击&#x200B;**[!UICONTROL 使用]**。

   此时将显示画布，它是创建内容的基础。

## 添加参数

将[准则](/help/user-guide/guidelines/overview.md)和资产合并到提示抽屉中的&#x200B;_参数_&#x200B;中可增强内容生成过程，并且是创建横幅体验的重要准备步骤。

**要添加参数和资源**：

1. 单击&#x200B;_参数_&#x200B;图标以展开提示抽屉。
1. 在&#x200B;_参数_&#x200B;部分中，选择准则 — [!DNL Brands]、[!DNL Personas]和[!DNL Products] — 以通知内容创建。

   如果这些菜单中没有可用的品牌、角色或产品，请[将准则添加到您的GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md)。

1. 添加要在体验&#x200B;*和*&#x200B;中使用的内容以影响内容生成：
   * 单击&#x200B;**[!UICONTROL 从内容中选择]**&#x200B;以从[!DNL Content]存储库中选择资源（图像），筛选并选择一个或多个图像。

     若要使用已连接[!DNL AEM Assets Content Hub]存储库中的资源，请从&#x200B;_位置_&#x200B;下拉菜单中选择一个存储库。 筛选并选择一个或多个图像。

   * 或者，将资产拖放到&#x200B;**[!UICONTROL 从内容中选择]**&#x200B;部分以上传一个或多个新资产。
1. 单击&#x200B;**[!UICONTROL 使用]**。

添加完参数后，再次单击&#x200B;_参数_&#x200B;图标以折叠提示抽屉。

## 输入提示

选择准则后，使用自然语言创建提示，以开始为新横幅体验生成内容。 要确保高质量的结果，必须制作详细且描述性的提示。

![输入提示](/help/assets/prompt-displayad.png){width="650" zoomable="yes"}

请参阅[编写有效提示](/help/user-guide/effective-prompts.md)，了解有关编写提示的详细信息。

**输入提示**：

1. 在&#x200B;_“描述您要生成的体验”_&#x200B;提示框中输入提示。
1. 单击&#x200B;**[!UICONTROL 生成]**。

默认情况下，将生成四个变体（以提示、指南和添加的内容为动力）并显示在画布中。

## 修订生成的横幅

在选择要发送哪些内容以供审批或发布到[!DNL Content]之前，您可以编辑横幅部分和文本字段，或删除生成的变体。

**要修订生成的变体**：

* **要[编辑横幅草稿名称](/help/user-guide/create/manage-variants.md#change-draft-name)**，请单击画布顶部的&#x200B;_无标题草稿_&#x200B;标题，然后输入新标题。
* **要[手动编辑横幅](/help/user-guide/create/manage-variants.md#manually-edit-text)**，请双击任何横幅部分或字段(如标题或CTA)，然后根据需要进行编辑。
* **要[重新生成变体](/help/user-guide/create/manage-variants.md#re-generate-sections)**&#x200B;的部分，请单击可编辑文本字段并使用&#x200B;_[!UICONTROL 建议的编辑]_&#x200B;选项，或者在_[!UICONTROL 生成新文本_部分]中输入新提示，然后单击&#x200B;**[!UICONTROL 生成]**。
* **要[在变体中添加或交换图像](/help/user-guide/create/manage-variants.md#swap-image)**，请单击图像资源（如果图像当前不存在，则单击图像资源区域），然后单击&#x200B;**[!UICONTROL 从内容交换]**&#x200B;图标。
* **要[添加指向变体中的图像的链接](/help/user-guide/create/manage-variants.md#add-image-link)**，请单击图像资源（如果图像当前不存在，则单击图像资源区域），然后单击链接图标。
* **要[为变体中的图像添加替换文本](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)**，请单击图像资源并使用&#x200B;_替换文本_&#x200B;选项为每个图像手动添加或生成替换文本。
* **要[更改广告](/help/user-guide/create/manage-variants.md#change-aspect-ratio)**&#x200B;的大小和纵横比，请单击&#x200B;_[!UICONTROL 调整大小]_&#x200B;按钮（画布左侧带有按钮图标的框），然后选择要应用于所有变体的新大小和纵横比。 将复制变体并调整其大小。
* **要[裁切或重新定位图像](/help/user-guide/create/manage-variants.md#crop-assets)**，请将鼠标悬停在该图像上，单击显示的裁切图标，然后调整图像大小和位置。 单击&#x200B;**[!UICONTROL 应用]**。

<!-- # Preview for device
When revising and preparing email experiences, you can toggle between previews for desktop and mobile views to ensure coherence and visual appeal of draft variants.
**To preview variants for desktop and mobile devices** toggle the device preview option—between **desktop** and **mobile**—in the right menu bar (computer and phone icons) to preview how variants appear. -->

## 提交生成反馈

要[提交有关生成输出质量的反馈](/help/user-guide/create/manage-variants.md#generation-feedback)，请单击选项图标（三个点）并选择&#x200B;**[!UICONTROL 输出良好]**&#x200B;或&#x200B;**[!UICONTROL 输出不良]**。

## 验证内容检查对齐方式

要优化生成的变体并确保严格遵守品牌标识、平台准则和辅助功能标准，请利用&#x200B;[_内容检查_&#x200B;面板](/help/user-guide/guidelines/brand-validation.md#content-check-panel)的强大功能。 此面板可显示全面的内容检查详细信息并阐明改进领域。

**要对变体执行内容检查**：

1. 单击右侧操作栏中的&#x200B;_内容检查_&#x200B;面板图标以打开&#x200B;[_内容检查_&#x200B;面板](/help/user-guide/guidelines/brand-validation.md#content-check-panel)。 查看&#x200B;_需要审核_&#x200B;和&#x200B;_通过_&#x200B;检查的摘要，以查看哪些部分和准则需要改进。

   ![_内容检查_&#x200B;面板](/help/assets/content-check-panel.png){height="400" zoomable="yes"}

1. [手动修订变体](#revise-generated-variants)以确保您的变体与执行的内容检查紧密一致。

请参阅[品牌验证](/help/user-guide/guidelines/brand-validation.md)。

## 获取审阅和批准

使用画布右侧操作栏上的&#x200B;_批准_&#x200B;面板（可作为一个图标访问）以获取审核、跟踪审核评论并从利益相关者处获得批准。

**要获得审阅和批准**：

1. [启动审批请求](/help/user-guide/approvals/request-review.md)以请求[审批草稿的横幅体验](/help/user-guide/approvals/approve-content.md)。
1. [在审阅过程中删除或添加审阅人](/help/user-guide/approvals/review-and-edit.md#manage-approvals)。
1. [访问内容以供审阅](/help/user-guide/approvals/review-and-edit.md#access-content-for-review)并查看修订请求。
1. 编辑每次审阅评论的草稿并[发布您的横幅体验](#publish-and-export-experience)。

查看[审核和批准](/help/user-guide/approvals/overview.md)。

## 发布和导出体验

若要使生成的横幅可用于当前和将来使用，请将其发布到[!UICONTROL Content]，并将其导出以用于您的营销活动。

1. **要发布您的新横幅体验**，请单击顶部工具栏或审批流中的&#x200B;**[!UICONTROL 发布]**。
   1. 选择&#x200B;_[!UICONTROL [!DNL Campaigns]]_并添加_[!UICONTROL &#x200B;更多详细信息&#x200B;]_（如果需要）。
   1. 单击&#x200B;**[!UICONTROL 发布]**。

      ![发布横幅](/help/assets/publish-displayad.png){width="450" zoomable="yes"}

1. **要导出新横幅**，请单击顶部工具栏中的&#x200B;**[!UICONTROL 导出]**。
   1. 选择格式 — HTML and images、PNG或JPG — 并单击&#x200B;**[!UICONTROL 导出]**。

      导出的HTML应放置在预定义的Web属性中，如模板或`div`容器。 如果没有这些设定的尺寸，独立查看图像时可能会出现扭曲。

请参阅[[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content)。
