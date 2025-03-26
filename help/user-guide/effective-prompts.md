---
title: 编写有效提示
description: 了解如何为 Adobe GenStudio for Performance Marketing 编写有效的提示。
role: User
level: Beginner
feature: Create Prompt, Generative AI
exl-id: 0cd4db4f-d031-4c1f-a4e7-adc220f947fc
source-git-commit: 8a5d15df7a347c4ee7767610fc9bb23fc7b71db4
workflow-type: tm+mt
source-wordcount: '752'
ht-degree: 2%

---

# 编写有效提示

与创新型人工智能进行通信对于在Adobe GenStudio for Performance Marketing中有效工作至关重要。

每次有机会修改资源时，GenStudio for Performance Marketing都会提供创作AI提示。 有效提示的组件应包括描述性语言、示例和配置准则中未提供的信息。

作为最佳实践，请使用[准则](/help/user-guide/guidelines/overview.md)向GenStudio for Performance Marketing提供您的品牌信息，然后您可以充分利用创作AI来生成与品牌一致的内容体验。

## 描述性语言

您可以使用自然语言来表达您的想法以创造体验。 您的提示将指导AI生成个性化的渠道内容以及补充您视觉效果的图像。 您提供的详细信息越多，就越有可能生成符合您需求的图像或体验。 使用清晰而具描述性的语言提供尽可能多的详细信息：

- 对于&#x200B;**图像**，请使用描述氛围、情绪、颜色、作文和风格的词语。
- 对于&#x200B;**副本**，请使用描述受众、用途、新功能描述、示例和操作的词语。

下面是一个示例提示，其中阐述了有关您的意图、目标受众和样式的信息。

```bash
Write an email to motivate infrequent users of Photoshop to follow an in-app tutorial that teaches them to combine elements of two photos into a beautiful work of art. Highlight the generative AI capabilities of Photoshop and use references to natural imagery.
```

+++查看示例结果

![三个生成的电子邮件](/help/assets/sample-email.png)

+++

## 提示条件

在GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md)中，您可以在提示抽屉中使用&#x200B;**[!UICONTROL 提示条件]** （[_参数_](/help/user-guide/create/overview.md#parameters)&#x200B;和提示）通过选择添加详细信息以改进AI解释。

对于[电子邮件](/help/user-guide/create/email-experiences.md)，提示条件可能包括在&#x200B;_参数_&#x200B;中添加[准则](/help/user-guide/guidelines/overview.md)、上传要在电子邮件变体中使用的资源以及说明性提示。 对于[元广告](/help/user-guide/create/create-meta-ad.md)，提示条件可能包括&#x200B;_参数_&#x200B;中的品牌指南、选择或上传现有资产、与图像或资产相关的设置（如长宽比）以及提示。 实际功率以[配置准则](/help/user-guide/guidelines/add-guidelines.md)开始。

>[!NOTE]
>
>如果在提示抽屉中的&#x200B;_参数_&#x200B;中添加了准则，则无需在提示中包含对这些准则的引用。 GenStudio for Performance Marketing在内容生成中利用这些[!DNL Brands]、[!DNL Products]和[!DNL Personas]。

### 准则

GenStudio for Performance Marketing指南帮助创作AI个性化您的资源组合。 当出现提示条件时，您可以从配置的准则中选择[[!DNL Brand]](/help/user-guide/guidelines/brands.md)、[[!DNL Persona]](/help/user-guide/guidelines/personas.md)和[[!DNL Product]](/help/user-guide/guidelines/products.md)。

>[!TIP]
>
>您可以控制GenStudio for Performance Marketing使用您的[!DNL Brand]指南的方式和时间。 请参阅[指南](/help/user-guide/guidelines/overview.md)以了解如何配置和管理您的品牌指南。

### 结构化提示

对于多节电子邮件，您可以构建提示以提供特定于节的说明，以便为电子邮件中的每个节生成各种内容。 结构化提示应直接引用电子邮件模板](/help/user-guide/content/customize-template.md#sections-or-groups)中的[节名称，以便生成的内容可以插入到相应的内容占位符中。

例如，您可以在第一部分中指示GenStudio for Performance Marketing为推广新产品的电子邮件生成内容，并在第二部分中详细介绍可节省成本的好处。

结构化提示应：

- 在电子邮件模板中对节名称使用以下引用之一：
   - Pod
   - 组
   - 分区
   - 模块

  例如，如果您的模板使用`moduleA`或`Group-3`作为节名称，则您可以在提示中引用这些节名称。

- 遵循建议的规则/结构。 如果提示结构不符合提供的格式，则该提示将应用于&#x200B;*所有*&#x200B;电子邮件节，并且仍然有助于内容生成。
- 使用在电子邮件模板中定义的节名称。 提示引用必须与电子邮件模板中编码的部分名称匹配。
- 不区分大小写。 例如，您可以在电子邮件模板和结构化提示中使用`Pod`或`pod`。
- 首先引用常规用户提示，然后引用特定于部分的指令。
- 使用冒号、连字符、逗号或其他分隔(`,:;#$!~|@=-%&*^_`)作为节名引用和指令之间的分隔。 例如，您可以使用以下内容作为特定节的提示指令： `Pod1; Describe how to easily edit text and swap images.`

下面是一个示例提示，它阐明了建议的提示结构，并利用一个电子邮件模板，该模板在`Pod1`、`Pod2`和`Pod3`中使用了标识词`Pod`。

```properties
Create an exciting multi-pod email focusing on Creative Cloud and its powerful generative AI capabilities.

Encourage customers to convert to Photoshop or use a free Photoshop trial. We want to better educate them about app features.

Pod1: Focus on Adobe Photoshop and its new generative AI tools that enable creators to bring images to life in minutes.

Pod2: Focus on Adobe Illustrator and its new generative AI tools, such as Generative Shape Fill, which allows you to quickly fill your vector outline and explore a variety of options that match the look and feel of your own artwork.

Pod3: Focus on Adobe Acrobat Pro. Make users aware that with Acrobat Pro they can edit images and text inside a PDF.
```

查看[使用模板的最佳实践](/help/user-guide/content/best-practices-for-templates.md)。

## 重试

提示是一个反复的过程。 如果结果不符合您的预期，请查看您的提示并进行一些更改或添加更多详细信息。 或者，您可以粘贴营销活动简介中的各个部分。 您甚至可以请求GenStudio for Performance Marketing避免使用某些单词、元素或主题。

## 最佳实践

制作有效提示的一些简单最佳实践：

- 具体说明并提供有关具体操作和不操作的详细信息。
- 使用外部引用提供上下文。
- 利用GenStudio for Performance Marketing准则。
- 定期审查和调整指南。
- 迭代和优化。
- 通过试验学习。

{{in-academy}}
