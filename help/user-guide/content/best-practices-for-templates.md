---
title: 模板最佳实践
description: 将模板与Adobe GenStudio for Performance Marketing结合使用时，请遵循最佳实践。
level: Intermediate
role: Developer, User
feature: Media Templates, Content Generation, Brand Personalization
exl-id: 3ff24fec-e836-4202-80f8-ba165e173b75
source-git-commit: adf987b016825861b5522b44b61263000eb63859
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# 使用模板的最佳实践

模板提供了一个包括预配置布局和设计元素的起点，可显着减少生成新内容所需的时间和精力。

将模板与GenStudio for Performance Marketing结合使用时，请使用以下建议：

1. 了解[模板元素](#know-about-template-elements)
1. 配置[渠道准则](#configure-channel-guidelines)以便有效地个性化内容
1. 使用[辅助功能标准](accessibility-for-templates.md)进行设计以获得最佳体验
1. 遵循[特定于渠道的模板准则](#follow-channel-specific-template-guidelines)

>[!TIP]
>
>在[使用模板](use-templates.md)中了解有关基本模板元素和过程的更多信息。 深入了解[自定义模板](customize-template.md)以用于您的下一个营销活动。

## 了解模板元素

最佳做法是熟悉模板的各个部分。 每种模板类型使用不同的元素来为特定于渠道的内容创建创建结构。 要自定义模板，请使用字段名称来代替您需要GenStudio for Performance Marketing生成内容的这些元素。

查看[模板元素](use-templates.md#template-elements)。

## 配置渠道准则

定义明确的渠道准则对于确保生成的内容与品牌的要求和目标保持一致至关重要。 渠道准则允许您为模板中使用的元素（如色调、长度和样式）指定规则。 例如，您可以为正文设置最大字符数或要求使用特定的call-to-action样式。 通过提前设置这些准则，您无需在每个AI提示中写出详细说明，从而简化内容生成过程并确保电子邮件的一致性。

查看并定义模板中所有关键字段的品牌的[渠道准则](/help/user-guide/guidelines/brands.md#channel-guidelines)。 如果您未定义准则，则应用[默认渠道准则](/help/user-guide/guidelines/brands.md#default-channel-guidelines)，这可能不能完全反映您的品牌要求。

![正文规范](/help/assets/channel-email-body.png)

了解[品牌、产品和角色准则](/help/user-guide/guidelines/overview.md)如何影响生成的内容，以及如何根据您的营销目标定制内容。

## 遵循特定于渠道的模板准则

在创建模板时，请确保它们满足预期渠道的特定要求。 构建适应每个渠道的布局和视觉要求的模板。 有一些常规准则适用于任何模板，例如：

- 使用简洁且响应式的HTML和内联CSS
- 使用Adobe或Google字体
- **不**&#x200B;使用JavaScript

{{note-css-effects}}

使用每种模板类型时，请参阅其他提示和限制以确保最佳性能和兼容性：

- [电子邮件](/help/user-guide/templates/email-template.md)
- [显示广告和横幅广告](/help/user-guide/templates/display-template.md)
- [LinkedIn](/help/user-guide/templates/linkedin-template.md)
- [元广告](/help/user-guide/templates/meta-template.md)
