---
title: 打造LinkedIn体验
description: 了解如何使用Adobe GenStudio for Performance Marketing创建符合品牌要求的LinkedIn体验。
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
badgeBeta: label="Beta" tooltip="此功能当前位于Beta中，因此某些功能可能会受到限制或发生更改。"
recommendations: noDisplay
exl-id: abe10fc8-d6d5-4cad-9273-400b622f22b7
source-git-commit: d5019f1cdceccb8ce2fdd86c54cf2d36673a90aa
workflow-type: tm+mt
source-wordcount: '914'
ht-degree: 0%

---

# 创建LinkedIn体验

本教程演示如何使用[&#128279;](/help/user-guide/create/meta-experiences.md)GenStudio进行绩效营销[[!DNL Create]](/help/user-guide/create/overview.md)（左侧导航区域中的画笔图标）生成符合品牌指南的LinkedIn体验。

在开始生成LinkedIn广告之前，请务必[在GenStudio中添加效果营销指南](/help/user-guide/guidelines/add-guidelines.md)，并学习创建提示[&#128279;](/help/user-guide/effective-prompts.md)的基础知识。

## 选择模板

若要生成新的 LinkedIn 体验，需要一个模板来为内容提供框架。 有关支持的LinkedIn宽高比的信息，请参阅 [模板](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) 的最佳做法。

**要选择LinkedIn模板**，请执行以下作：

1. In _[!DNL Create]_, click **[!UICONTROL LinkedIn]**.
1. Use the search option, adjacent to _Filter_, to find a specific template.
1. 单击以选择模板，然后单击&#x200B;**[!UICONTROL 使用]**。

   此操作将打开画布，它是内容创建的中心中心。

## 添加参数

在提示抽屉中添加&#x200B;_参数_&#x200B;中的[准则](/help/user-guide/guidelines/overview.md)和资产可增强内容生成过程，是准备生成LinkedIn体验的关键步骤。

**要添加参数和资源**：

1. 单击&#x200B;_参数_&#x200B;图标以展开提示抽屉。
1. 在&#x200B;_参数_&#x200B;部分中，选择准则 — [!DNL Brands]、[!DNL Personas]和[!DNL Products] — 以通知内容创建。

   ![选择角色](/help/assets/persona-select.png){width="600" zoomable="yes"}

   如果这些菜单中没有可用的品牌、角色或产品，请[将准则添加到您的GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md)。

1. 添加内容以用于体验 *并* 影响内容生成：
   * 单击从 **[!UICONTROL 内容]** 中选择要从 [!DNL Content] 存储库中选择资源（图像），请过滤并选择一个或多个图像。

     ![选择视觉内容](/help/assets/content-select-meta.png){width="500" zoomable="yes"}

     若要使用已连接[!DNL AEM Assets Content Hub]存储库中的资源，请从&#x200B;_位置_&#x200B;下拉菜单中选择一个存储库。 筛选并选择一个或多个图像。

   * 或者，将资产拖放到&#x200B;**[!UICONTROL 从内容中选择]**&#x200B;部分以上传一个或多个新资产。
1. 单击“ **[!UICONTROL 使用]**”。

添加完参数后，可以通过再次单击“参数&#x200B;_”_&#x200B;图标来折叠提示抽屉。

## 输入提示

选择指南后，使用自然语言制作提示，开始为新的LinkedIn体验生成内容。 详细的提示可确保您收到高质量和有用的输出。

请参阅 [编写有效提示](/help/user-guide/effective-prompts.md) 以了解有关编写提示的详细信息。

**输入提示**：

1. 在&#x200B;_“描述您要生成的体验”_&#x200B;提示框中输入提示。
1. 单击&#x200B;**[!UICONTROL 生成]**。

默认情况下，将生成四个变体（全部由提示、指南和您添加的内容提供），并显示在画布中。

生成的内容会以渐进方式加载 — 在生成LinkedIn体验的每个部分时，这些部分都会显示在画布中。 请参阅[LinkedIn体验](/help/user-guide/create/linkedin-experiences.md#progressive-loading)，了解如何在画布中加载这些更改。

## 修订生成的LinkedIn广告

在将变体发送以供审批或发布到[!DNL Content]之前，您可以编辑LinkedIn广告或从生成的广告集中删除变体。

**要修订生成的变体**：

* **要[编辑LinkedIn广告草稿名称](/help/user-guide/create/manage-variants.md#change-draft-name)**，请单击画布顶部的&#x200B;_无标题草稿_&#x200B;标题并输入新标题。
* **要[手动编辑LinkedIn广告](/help/user-guide/create/manage-variants.md#manually-edit-text)**，请单击任意广告部分（如主题行、标题或正文）并根据需要进行编辑。
* **要更改或选择号召性用语**，请单击号召性用语按钮，然后从可用的按钮文本选项中进行选择。 在“链接”_中_，输入号召性用语文本的 URL。
* **要[重新生成变体](/help/user-guide/create/manage-variants.md#re-generate-sections)**&#x200B;的部分，请单击可编辑文本字段并使用&#x200B;_[!UICONTROL 建议的编辑]_&#x200B;选项，或者在_[!UICONTROL 生成新文本_部分]中输入新提示，然后单击&#x200B;**[!UICONTROL 生成]**。
* **要[裁切或重新定位图像](/help/user-guide/create/manage-variants.md#crop-assets)**，请将鼠标悬停在图像上，单击显示的裁切图标，然后调整图像大小和位置。
* **要[删除LinkedIn广告](/help/user-guide/create/manage-variants.md#delete-variant)**，请单击变体的选项菜单，然后单击&#x200B;**[!UICONTROL 删除变体]**。

## 提交生成反馈

要[提交有关生成输出质量的反馈](/help/user-guide/create/manage-variants.md#generation-feedback)，请单击选项图标（三个点），然后选择“良好输出&#x200B;**”或**“**[!UICONTROL 差输出]**”。

## 验证内容检查对齐方式

要优化生成的变体并确保严格遵守品牌标识、平台准则和辅助功能标准，请利用&#x200B;[_内容检查_&#x200B;面板](/help/user-guide/guidelines/brand-validation.md#content-check-panel)的强大功能。 此面板可显示全面的内容检查详细信息并阐明改进领域。

**要对变体执行内容检查**：

1. 单击右侧操作栏中的&#x200B;_内容检查_&#x200B;面板图标以打开&#x200B;[_内容检查_&#x200B;面板](/help/user-guide/guidelines/brand-validation.md#content-check-panel)。 查看&#x200B;*需要审核*&#x200B;和&#x200B;*通过*&#x200B;检查的摘要，以查看哪些部分和准则需要改进。

   ![_内容检查_&#x200B;面板](/help/assets/content-check-panel.png){height="400" zoomable="yes"}

1. [手动修订变体](#revise-generated-variants)以确保您的变体与执行的内容检查紧密一致。

请参阅[品牌验证](/help/user-guide/guidelines/brand-validation.md)。

## 获取审阅和批准

使用画布顶部菜单栏上的“批准”面板，可获取审核、跟踪审核评论并从利益相关者处获得批准。

**要获得审核和批准**，请执行以下作：

1. [发起审批请求](/help/user-guide/approvals/request-review.md) ，征求 [对已起草的 Meta 广告体验](/help/user-guide/approvals/approve-content.md)的批准。

   ![发送草稿以供审阅和审批](/help/assets/send-approval-meta.png){width="450" zoomable="yes"}

1. [在审阅过程中删除或添加审阅人](/help/user-guide/approvals/review-and-edit.md#manage-approvals)。
1. [访问内容以供审阅](/help/user-guide/approvals/review-and-edit.md#access-content-for-review)并查看修订请求。
1. 编辑每个审阅评论的草稿并[发布您的元广告体验](#publish-and-export-experience)。

有关详细信息，请参阅 [审核和批准](/help/user-guide/approvals/overview.md) 。

## 发布和导出体验

要使生成的LinkedIn广告可供当前和将来使用，请将其发布到 [!UICONTROL 内容] 并导出以用于营销活动。

1. **要发布新体验**，请单击顶部工具栏中或审批流程中的“发布&#x200B;**”。**
1. **要导出新体验**，请单击顶部工具栏中的“导出&#x200B;**”。**
   1. 选择格式 — JPG、PNG或GIF — 并单击&#x200B;**[!UICONTROL 导出]**。

有关详细信息，请参阅[[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content)。
