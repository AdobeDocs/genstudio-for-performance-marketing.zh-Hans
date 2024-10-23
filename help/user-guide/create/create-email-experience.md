---
title: 创建电子邮件体验
description: 了解如何在Adobe GenStudio中为性能营销创建电子邮件体验。
feature: Content, Brands Service, Guidelines, Content Generation, Create, Experiences, Variant Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 34446202-da98-45ff-869a-b43496a477f8
source-git-commit: 11bd93e90a01d89adb9ed12d1e93774c67f27b6b
workflow-type: tm+mt
source-wordcount: '996'
ht-degree: 0%

---

# 创建电子邮件体验

本教程演示如何使用GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md)生成品牌[电子邮件体验](/help/user-guide/create/email-experiences.md)（左侧导航区域中的画笔图标）。

若要创建有效的电子邮件体验，建议您[向GenStudio添加准则以进行性能营销](/help/user-guide/guidelines/add-guidelines.md)，并在开始之前[复习构建提示的基础知识](/help/user-guide/effective-prompts.md)。

## 选择模板

要创建新的电子邮件体验，请使用可用的模板为您的内容提供框架。

**要选择电子邮件模板**：

1. 在&#x200B;_[!DNL Create]_中，在_“今天要创建什么？”中单击&#x200B;**[!UICONTROL 电子邮件]**_节。
1. 使用&#x200B;_筛选器_&#x200B;旁边的搜索选项查找特定的电子邮件模板。
1. 单击以选择电子邮件模板，然后单击&#x200B;**[!UICONTROL 使用]**。

   即会显示内容创建的中心“画布”。

## 添加参数

在提示抽屉中添加&#x200B;_参数_&#x200B;中的[准则](/help/user-guide/guidelines/overview.md)和资产，会增加内容生成过程的费用，是生成电子邮件体验的必要准备步骤。

**要添加参数和资源**：

1. 单击&#x200B;_参数_&#x200B;图标以展开提示抽屉。
1. 在&#x200B;_参数_&#x200B;部分中，选择准则 — [!DNL Brands]、[!DNL Personas]和[!DNL Products] — 以通知内容创建。

   ![选择角色](/help/assets/persona-select.png){width="600" zoomable="yes"}

   如果这些菜单中没有可用的品牌、角色或产品，请[将准则添加到您的GenStudio以进行性能营销](/help/user-guide/guidelines/add-guidelines.md)。

1. 添加要在体验&#x200B;*和*&#x200B;中使用的内容以影响内容生成：
   * 单击&#x200B;**[!UICONTROL 从内容中选择]**&#x200B;以从[!DNL Content]存储库中选择资源（图像），筛选并选择一个或多个图像。

     ![选择视觉内容](/help/assets/content-select-email.png){width="500" zoomable="yes"}

     若要使用已连接[!DNL AEM Assets Content Hub]存储库中的资源，请从&#x200B;_位置_&#x200B;下拉菜单中选择一个存储库。 筛选并选择一个或多个图像。

   * 或者，将资产拖放到&#x200B;**[!UICONTROL 从内容中选择]**&#x200B;部分以上传一个或多个新资产。
1. 单击&#x200B;**[!UICONTROL 使用]**。

>[!NOTE]
>如果您的电子邮件模板有多个分区，请为&#x200B;_多分区电子邮件_&#x200B;中的每个电子邮件分区选择[!DNL Products]和内容（可视资产）。 多节电子邮件支持每节一个可视资产。 您只能从[!DNL Content]向多节电子邮件添加可视资产，而不能从本地源拖放或上传资产。
>![为每个电子邮件节](/help/assets/parameters-multisection-email.png){width="450" zoomable="yes"}添加内容和参数

添加完参数后，您可以通过再次单击&#x200B;_参数_&#x200B;图标来折叠提示抽屉。

## 输入提示

选择准则后，使用自然语言编写提示，以开始为新的电子邮件体验生成内容。 详细提示比模糊或不描述性提示产生更高的输出质量。

请参阅[编写有效提示](/help/user-guide/effective-prompts.md)，了解有关编写提示的详细信息。

**输入提示**：

1. 在&#x200B;_“描述您要生成的体验”_&#x200B;提示框中输入提示。
1. 单击&#x200B;**[!UICONTROL 生成]**。

默认情况下，将生成四个变体（全部由提示、指南和您添加的内容提供），并显示在画布中。

生成的内容以渐进方式加载 — 在生成电子邮件体验的每个部分时，这些部分都会显示在画布中。 请参阅[电子邮件体验](/help/user-guide/create/meta-experiences.md#progressive-loading)，了解如何在画布中加载这些更改。

## 修订生成的电子邮件

在选择要发送哪些内容以供审批或发布到[!DNL Content]之前，您可以编辑电子邮件部分或从生成的电子邮件集中删除变体。

**要修订生成的变体**：

* **要[编辑电子邮件草稿名称](/help/user-guide/create/manage-variants.md#change-draft-name)**，请单击画布顶部的&#x200B;_无标题草稿_&#x200B;标题并输入新标题。
* **要[手动编辑电子邮件](/help/user-guide/create/manage-variants.md#manually-edit-text)**，请双击任何可编辑的文本字段（如主题行、标题或正文）并根据需要进行编辑
* **要[重新生成变体的部分](/help/user-guide/create/manage-variants.md#re-generate-sections)**，请单击可编辑文本字段并使用&#x200B;_[!UICONTROL 建议的编辑]_&#x200B;选项，或者输入新提示并单击&#x200B;**[!UICONTROL 生成]**。
* **要[在变体中添加或交换图像](/help/user-guide/create/manage-variants.md#swap-image)**，请单击图像资源（如果图像当前不存在，则单击图像资源区域），然后单击&#x200B;**[!UICONTROL 从内容中选择/交换]**&#x200B;或&#x200B;**[!UICONTROL 上传新图像]**，以便在单个变体中添加或交换图像。
* **要[删除电子邮件](/help/user-guide/create/manage-variants.md#delete-variant)**，请单击以选择电子邮件标题（例如，“电子邮件1/4”），然后单击&#x200B;**[!UICONTROL 删除变体]**。

## 提交生成反馈

要[提交有关生成输出质量的反馈](/help/user-guide/create/manage-variants.md#generation-feedback)，请单击选项图标（三个点）并选择&#x200B;**[!UICONTROL 输出良好]**&#x200B;或&#x200B;**[!UICONTROL 输出不良]**。

## 设备预览

在修订和准备电子邮件体验时，您可以[在桌面视图和移动设备视图的预览之间切换](/help/user-guide/create/manage-variants.md#preview-for-device)，以确保草稿变体的一致性和视觉吸引力。

## 验证品牌一致性

要优化生成的电子邮件并确保严格遵守品牌标识，请利用&#x200B;[_品牌指南检查_](/help/user-guide/guidelines/brand-validation.md#brand-guidelines-check)（为变体提供品牌一致性摘要）和&#x200B;[_品牌验证_&#x200B;面板](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel)的强大功能，其中显示全面的品牌验证详细信息并阐明改进领域。

**验证品牌一致性**：

1. 单击变体的[**[!UICONTROL [!DNL Brand]准则检查]**](/help/user-guide/guidelines/brand-validation.md#brand-guidelines-check)图标，并查看针对您的品牌检查该变体时的性能摘要。

   ![品牌指南检查](/help/assets/brand-guidelines-check.png){width="350" zoomable="yes"}

1. 若要获取需要改进的部分和准则的详细信息，请单击&#x200B;**[!UICONTROL 查看]** _或_，单击顶部菜单栏中的“品牌验证”图标以打开&#x200B;[_品牌验证面板_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel)。

1. 切换每封电子邮件，了解如何改进生成的内容，使其更具品牌一致性。

   ![品牌验证面板](/help/assets/brand-validation-panel.png){width="600" zoomable="yes"}

1. [手动修改电子邮件](#revise-generated-emails)以确保您的电子邮件与品牌紧密一致。

请参阅[品牌验证](/help/user-guide/guidelines/brand-validation.md)。

## 获取审阅和批准

使用画布顶部菜单栏上的“批准”面板，可获取审核、跟踪审核评论并从利益相关者处获得批准。

**要获得审阅和批准**：

1. [启动审批请求](/help/user-guide/approvals/request-review.md)以请求[审批草拟的电子邮件体验](/help/user-guide/approvals/approve-content.md)。
1. [在审阅过程中删除或添加审阅人](/help/user-guide/approvals/review-and-edit.md#manage-approvals)。
1. [访问内容以供审阅](/help/user-guide/approvals/review-and-edit.md#access-content-for-review)并查看修订请求。
1. 编辑每个审核评论的草稿并[发布您的电子邮件体验](#publish-and-export-experience)。

有关详细信息，请参阅[审核和批准](/help/user-guide/approvals/overview.md)。

## Publish和导出体验

若要使生成的电子邮件可用于当前和将来使用，请将其发布到[!UICONTROL 内容]并将其导出以用于您的营销活动。

1. **要发布您的新电子邮件体验**，请单击顶部工具栏或审批流中的&#x200B;**[!UICONTROL Publish]**。
1. **要导出您的新电子邮件体验**，请单击顶部工具栏中的&#x200B;**[!UICONTROL 导出]**。
   1. 选择格式(仅限CSV和图像或HTML)，然后单击&#x200B;**[!UICONTROL 导出]**。

有关详细信息，请参阅[[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content)。
