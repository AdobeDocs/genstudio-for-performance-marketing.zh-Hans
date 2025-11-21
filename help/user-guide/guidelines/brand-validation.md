---
title: Adobe GenStudio for Performance Marketing中的Brand Validation
description: 了解内置品牌验证系统在GenStudio for Performance Marketing中的工作方式。
feature: Brand Personalization, Variant Generation, Compliance, Content Generation, Content Review, Generative AI
exl-id: 2e777186-3b7e-46a6-9d37-7c7b7c2aa7ae
source-git-commit: e2acf90ef5fef6af03a756882caf53ab125055c4
workflow-type: tm+mt
source-wordcount: '788'
ht-degree: 0%

---

# 品牌验证

在GenStudio for Performance Marketing中，品牌验证是与创作AI功能和准则 — [[!DNL Brands]](/help/user-guide/guidelines/brands.md)、[[!DNL Products]](/help/user-guide/guidelines/products.md)和[[!DNL Personas]](/help/user-guide/guidelines/personas.md) — 协作的基本组件。 它确保您的所有内容与品牌标识、ADA标准和各个渠道平台指导保持一致。

GenStudio for Performance Marketing从多个方面执行品牌验证和其他内容检查，包括：

* 已定义或默认的[!DNL Brand]准则
* 平台准则
* [美国残疾人法案(ADA)标准](/help/user-guide/guidelines/brand-validation.md#american-with-disabilities-act-ada-validation)
<!-- * Ethical considerations related to gender, ethnicity, race, disability status, and age in AI-generated content -->


## 内容检查摘要

可通过画布中每个变体的&#x200B;_内容检查_&#x200B;摘要图标访问每个已生成内容项目的品牌验证和其他内容检查信息的摘要。

_内容检查_&#x200B;摘要显示：

* 通过验证的[[!DNL Brand]](brands.md)准则[与测试的准则数之比，计算出](overview.md)的符合性百分比
* 平台准则的`Pass`或`Fail`结果，如Meta或LinkedIn
* ADA辅助功能标准的`Pass`或`Fail`结果

![内容检查摘要](/help/assets/content-check-summary.png){width="400" zoomable="yes"}

单击百分比以查看变体的兼容程度。 在您对变体或其他内容进行编辑时，得分会自动更新。 您可以单击&#x200B;_查看并修复问题_，以确保进一步的合规性。

请参阅[改善品牌一致性](#improve-brand-alignment)。

## 内容检查面板

从右操作栏&#x200B;_或_&#x200B;单击&#x200B;_内容检查_&#x200B;摘要图标&#x200B;[_时，_&#x200B;内容检查](#content-check-summary)面板将在画布右侧打开。 此面板提供了详细的品牌验证、平台指南和无障碍标准信息，并说明了改进的机会。

![内容检查面板](/help/assets/content-check-panel.png){width="400" zoomable="yes"}

_内容检查_&#x200B;面板显示图像和变体部分的验证和[合规性信息](/help/user-guide/guidelines/overview.md#compliance)：

* _的_&#x200B;内容检查[!DNL Brand]摘要信息、平台准则和辅助功能标准的表示形式
* _需要审核_&#x200B;部分，其中显示失败准则的数量以及有关每个需要修订的准则的详细信息
* _通过_&#x200B;部分，显示通过的准则数以及每个通过准则的详细信息

请参阅[改善品牌一致性](#improve-brand-alignment)，了解如何改善&#x200B;_内容检查_&#x200B;面板分数。

### 内容类型

在&#x200B;_内容检查_&#x200B;面板中，您可以切换执行了哪些准则和可访问性标准检查。 单击面板顶部的&#x200B;_内容类型_&#x200B;图标（级别图标）可打开或关闭：

* **[!DNL Brand]** — 执行与[!DNL Brand]准则相关的检查
* **平台准则** — 执行与特定于渠道的平台(如Meta)相关的检查
* **辅助功能** — 执行与ADA辅助功能标准相关的检查

要&#x200B;**为要执行的检查设置内容类型**，请单击关闭或打开可用类型，然后单击&#x200B;**应用**。

## 改善品牌一致性

若要最大限度地提高所生成内容的效率并保持一致的品牌标识，请使用&#x200B;[_内容检查_&#x200B;摘要](#content-check-summary)和&#x200B;[_内容检查_&#x200B;面板](#content-check-panel)。 您可以手动修改特定部分，以符合[[!DNL Brand] 指南](brands.md)、平台指南检查和辅助功能标准检查。

**要改善生成的变体的品牌一致性**：

1. 单击右侧操作栏中的&#x200B;_内容检查_&#x200B;面板图标以查看验证和辅助功能信息。

   您可以看到&#x200B;_需要审核_&#x200B;和&#x200B;_通过_&#x200B;检查的摘要，以查看哪些需要改进。

   >[!NOTE]
   >
   > _内容检查_&#x200B;面板中提到的&#x200B;_品牌声音_&#x200B;准则适用于整个变体，而不是单个部分。 将突出显示整个内容变体以便提出改进建议。

1. 单击以修复当前不兼容的准则。
1. 单击以展开并检查每个需要在可用部分（如&#x200B;_标题_、_颜色_&#x200B;和&#x200B;_品牌声音_）中审阅的检查。

   使用为每个检查提供的推理来指导您修订图像和变体。

1. 进行必要的修改后，单击&#x200B;**[!UICONTROL 重新检查分数]**&#x200B;以重新检查并验证所做的更改，确保它们符合您的品牌标识、平台准则和无障碍标准。

   内容检查过程将再次运行。 如果修订项目通过验证，则会在画布底部显示绿色横幅，以确认分数已更新。 如果重新检查后没有变化，横幅将确认分数没有变化。 修订变体的&#x200B;_内容检查_&#x200B;摘要图标中的百分比也会显示您的进度。

1. 继续修订各个部分，以确保整个变体通过验证和可访问性检查。 使用画布中单个变体旁边的箭头浏览每个变体。

## 美国残疾人法案(ADA)验证

这些无障碍检查包含在《美国残疾人法案》(ADA)的法律合规性中：

[WCAG 1.1.1非文本内容](https://www.w3.org/WAI/WCAG21/Understanding/non-text-content.html) — 确保图像提供`<alt>`属性。
[WCAG 1.4.3对比度（最小值）](https://www.w3.org/WAI/WCAG21/Understanding/contrast-minimum.html) — 确保生成的文本相对于背景具有4.5:1对比度。
[WCAG 3.1.3异常词](https://www.w3.org/WAI/WCAG21/Understanding/unusual-words.html) — 识别以异常或受限方式使用的单词或短语，包括成语和行话。
[WCAG 3.1.4缩写](https://www.w3.org/WAI/WCAG21/Understanding/abbreviations.html) — 用于识别缩写的扩展形式或含义的机制。
[WCAG 3.1.5读取级别](https://www.w3.org/WAI/WCAG21/Understanding/reading-level.html) — 确保内容在初中教育级别可读。

