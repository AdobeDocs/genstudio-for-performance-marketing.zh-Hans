---
title: 创建显示广告体验
description: 了解如何在Adobe [!DNL GenStudio] 中为性能营销创建显示广告体验。
feature: Brands Service, Guidelines, Content Generation, Generative AI, Create, Experiences, Variant Generation
role: User
level: Beginner
recommendations: noDisplay
source-git-commit: 885900eb259246c2d86a07791a1b7070e0dbf12a
workflow-type: tm+mt
source-wordcount: '875'
ht-degree: 0%

---

# 创建显示广告体验

本教程演示如何使用GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md)生成品牌[显示广告体验](display-ad-experiences.md)（左侧导航区域中的画笔图标）。

若要设计引人入胜的显示广告体验，建议您[将准则添加到GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md)，并在开始之前查看[编写提示的基础知识](/help/user-guide/effective-prompts.md)。

## 选择模板

要创建显示广告体验，请使用可用的模板为您的内容提供框架。

**选择显示广告模板**：

1. 在&#x200B;_[!DNL Create]_中，在“_”中单击&#x200B;**[!UICONTROL 显示广告]**“您今天要创建什么内容？”_节。
1. 使用&#x200B;_筛选器_&#x200B;旁边的搜索选项查找特定的显示广告模板。
1. 在&#x200B;_选择模板_&#x200B;视图中，单击显示广告模板。
1. 单击&#x200B;**[!UICONTROL 使用]**。

   此时将显示画布，它是内容创建的中心中心。

## 添加参数

在提示抽屉中添加&#x200B;_参数_&#x200B;中的[准则](/help/user-guide/guidelines/overview.md)和资产，会增加内容生成过程的开销，是生成显示广告体验的必要准备步骤。

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

选择准则后，使用自然语言制作提示，开始为新的显示广告体验生成内容。 为了提高生成的显示广告体验的质量，制作详细的描述性提示至关重要。

![输入提示](/help/assets/prompt-displayad.png){width="650" zoomable="yes"}

请参阅[编写有效提示](/help/user-guide/effective-prompts.md)，了解有关编写提示的详细信息。

**输入提示**：

1. 在&#x200B;_“描述您要生成的体验”_&#x200B;提示框中输入提示。
1. 单击&#x200B;**[!UICONTROL 生成]**。

默认情况下，将生成四个变体（以提示、指南和添加的内容为动力）并显示在画布中。

## 修订生成的显示广告

在选择要发送哪些内容以供审批或发布到[!DNL Content]之前，您可以编辑显示广告部分和文本字段，或删除生成的变体。

**要修订生成的变体**：

* **要[编辑显示广告草稿名称](/help/user-guide/create/manage-variants.md#change-draft-name)**，请单击画布顶部的&#x200B;_无标题草稿_&#x200B;标题，然后输入新标题。
* **要[手动编辑显示广告](/help/user-guide/create/manage-variants.md#manually-edit-text)**，请双击显示广告的任何部分或字段（例如主题行、标题或正文），然后根据需要进行编辑。
* **要[更改广告](/help/user-guide/create/manage-variants.md#change-aspect-ratio)**&#x200B;的大小和纵横比，请单击&#x200B;_[!UICONTROL 调整大小]_&#x200B;按钮（画布左侧带有按钮图标的框），然后选择要应用于所有变体的新大小和纵横比。 将复制变体并调整其大小。
* **要[裁切或重新定位图像](/help/user-guide/create/manage-variants.md#crop-assets)**，请将鼠标悬停在该图像上，单击显示的裁切图标，然后调整图像大小和位置。 单击&#x200B;**[!UICONTROL 应用]**。

<!-- # Preview for device
When revising and preparing email experiences, you can toggle between previews for desktop and mobile views to ensure coherence and visual appeal of draft variants.
**To preview variants for desktop and mobile devices** toggle the device preview option—between **desktop** and **mobile**—in the right menu bar (computer and phone icons) to preview how variants appear. -->

## 提交生成反馈

要[提交有关生成输出质量的反馈](/help/user-guide/create/manage-variants.md#generation-feedback)，请单击选项图标（三个点）并选择&#x200B;**[!UICONTROL 输出良好]**&#x200B;或&#x200B;**[!UICONTROL 输出不良]**。

## 验证品牌一致性

要优化生成的广告并确保严格遵守品牌标识，请利用&#x200B;[_品牌验证面板_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel)&#x200B;的强大功能，该面板可显示全面的品牌验证详细信息并阐明改进领域。

**验证品牌一致性**：

1. 单击顶部菜单栏中的“品牌验证”图标以打开&#x200B;[_品牌验证面板_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel)。 您可以查看片段的详细信息和需要改进的准则。

1. 切换每个广告，了解如何改进生成的内容以使内容更具品牌一致性。
1. [手动修改广告](#revise-generated-display-ads)以确保您的电子邮件与品牌紧密一致。

请参阅[品牌验证](/help/user-guide/guidelines/brand-validation.md)。

## 获取审阅和批准

使用画布顶部菜单栏上的“批准”面板，可获取审核、跟踪审核评论并从利益相关者处获得批准。

**要获得审阅和批准**：

1. [启动审批请求](/help/user-guide/approvals/request-review.md)以请求[审批草拟的电子邮件体验](/help/user-guide/approvals/approve-content.md)。
1. [在审阅过程中删除或添加审阅人](/help/user-guide/approvals/review-and-edit.md#manage-approvals)。
1. [访问内容以供审阅](/help/user-guide/approvals/review-and-edit.md#access-content-for-review)并查看修订请求。
1. 编辑每个审阅评论的草稿，并[发布您的显示广告体验](#publish-and-export-experience)。

查看[审核和批准](/help/user-guide/approvals/overview.md)。

## Publish和导出体验

若要使生成的显示广告可用于当前和将来使用，请将其发布到[!UICONTROL 内容]并将其导出以用于您的营销活动。

1. **要发布您的新显示广告体验**，请单击顶部工具栏或审批流中的&#x200B;**[!UICONTROL Publish]**。
   1. 选择&#x200B;_[!UICONTROL [!DNL Campaigns]]_并添加_[!UICONTROL &#x200B;更多详细信息&#x200B;]_（如果需要）。
   1. 单击&#x200B;**[!UICONTROL 发布]**。

      ![Publish显示广告](/help/assets/publish-displayad.png){width="450" zoomable="yes"}

1. **要导出您的新显示广告体验**，请单击顶部工具栏中的&#x200B;**[!UICONTROL 导出]**。
   1. 选择格式(仅JPG)，然后单击&#x200B;**[!UICONTROL 导出]**。

      导出的HTML应放置在预定义的Web属性中，如模板或`div`容器。 如果没有这些设定的尺寸，独立查看图像时可能会出现扭曲。

请参阅[[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content)。
