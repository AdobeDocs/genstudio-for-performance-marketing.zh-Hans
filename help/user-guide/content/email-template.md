---
title: 为Adobe GenStudio for Performance Marketing准备电子邮件模板
description: 了解如何为Adobe GenStudio for Performance Marketing构建自定义电子邮件模板。
level: Intermediate
feature: Templates, Content
exl-id: 8b1e8d32-5a23-45ce-a2d4-ae6de3698c45
source-git-commit: 478815d74a742cdc05d3f1faebf27d5adc04d417
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# 为Adobe GenStudio for Performance Marketing准备电子邮件模板

通常，设计人员会在设计程序(如Adobe XD)中创建模板的可视化设计。 设计、编码和测试电子邮件模板后，即可准备将其上传和用于GenStudio for Performance Marketing。

查看[模板元素](use-templates.md#template-elements)。

## 添加准则

在准备元广告模板之前，请确保已将[准则](/help/user-guide/guidelines/overview.md)添加到您的GenStudio for Performance Marketing中，并为其填充了相关品牌的综合信息。 [品牌准则](/help/user-guide/guidelines/brands.md)直接影响生成的内容。

**示例**：如果您希望电子邮件模板正文不超过500个字符，请将该要求添加到“正文”字段的[渠道准则](/help/user-guide/guidelines/brands.md#channel-guidelines)中。

如果未将准则添加到GenStudio for Performance Marketing，则使用默认值。

## 对电子邮件模板进行编码

设计模板后，使用HTML和内联CSS对其进行编码。 对于各种设备，代码应该是干净和响应式的。

请参阅[模板示例](/help/user-guide/content/customize-template.md#template-examples)。

### 多节电子邮件

您可以在内容生成期间使用[结构化提示](/help/user-guide/effective-prompts.md#structured-prompts)来指示GenStudio for Performance Marketing在电子邮件的每个部分生成不同的内容。

例如，如果电子邮件模板中的部分以`Pod`—`Pod1`和`Pod2`为前缀，则用于生成内容的结构化提示可以包含这些电子邮件部分的特定指令。 GenStudio for Performance Marketing会将提示中特定于部分的指令与相关电子邮件部分相匹配，并生成与指令一致的内容。

请参阅[结构化提示](/help/user-guide/effective-prompts.md#structured-prompts)。

## 测试电子邮件模板

使用您的电子邮件投放或验证平台来测试您的电子邮件，并验证它是否在不同电子邮件客户端和设备之间正确呈现。

测试以确保您的电子邮件模板满足以下条件：

* 使用CSS媒体查询调整不同屏幕大小的布局
* 按钮可点击，可导航到目标位置
* 电子邮件模板可在移动设备上读取和使用

## 定义生成的内容区域

定义电子邮件模板中应使用GenStudio for Performance Marketing中的内容动态填充的区域。

要定义生成的内容区域，请执行以下操作：

* 确定GenStudio for Performance Marketing应自动生成的模板中的文本元素，如标题或CTA。
* 通过使用Handlebars语法在HTML模板中插入占位符来调整模板。

请参阅[内容占位符](/help/user-guide/content/customize-template.md#content-placeholders)。

## 预览模板

使用内置帮助程序控制特定内容区域的可见性。 例如，您可以在导出的模板中包含指向链接的跟踪参数，同时保持预览链接干净。

请参阅[模板预览](/help/user-guide/content/customize-template.md#template-preview)。

## 上传和使用模板

设计、编码、测试和预览模板后，您可以将其上传到GenStudio for Performance Marketing以用于生成全新的营销内容。

请参阅[使用模板](use-templates.md)。
