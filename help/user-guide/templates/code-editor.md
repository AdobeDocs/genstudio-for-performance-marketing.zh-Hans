---
title: 模板代码编辑器
description: 了解如何在GenStudio for Performance Marketing中使用模板代码编辑器。
level: Intermediate
role: Developer
feature: Media Templates, Content Generation
exl-id: b46fc7a9-88c1-474a-9d7b-1df7740d8f5a
source-git-commit: 9e51e853542d20f0b90b10071f4f26aaae1d6aad
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 0%

---

# 模板代码编辑器

模板代码编辑器旨在帮助您验证和优化模板，以便在使用GenStudio for Performance Marketing生成新体验时实现最佳使用。 该编辑器支持Handlebars语法，该语法使用模板中的占位符来指示GenStudio for Performance Marketing应在何处为您生成内容。

>[!TIP]
>
>在[!DNL Content] _模板_&#x200B;视图中上传模板HTML代码之前，请通过插入[自定义模板](customize-template.md)指南中定义的内容占位符来准备模板。

## 检查检测到的字段

_[!UICONTROL 检查检测到的字段]_&#x200B;窗格显示GenStudio for Performance Marketing可在您的模板中识别的字段列表。 查看列表，然后您可以滚动HTML代码以查看模板的结构。

![代码编辑器视图](/help/assets/template-detected-fields.png "检查检测到的字段"){width="600"}

如果您发现列表中缺少字段，请搜索模板代码并找到缺失字段的位置。 使用Handlebars语法和[可识别的字段名](/help/user-guide/templates/customize-template.md#recognized-field-names)插入正确的占位符。 使用代码编辑器底部显示的“查找和替换”表单来搜索代码中的特定字符串。 (Windows `CTRL`+`F`或macOS `CMD`+`F`)

## 调整变量的角色

您可以在模板结构检查期间通过下拉菜单为基于文本的字段角色（例如，`headline`、`sub_headline`、`body`、`cta`、`on_image_text`、`custom`）选择和更改字段角色。 在模板编辑过程中会保留字段角色选择，以便不会丢失自定义项，从而提高工作流的效率。

>[!NOTE]
>
>无法调整图像变量的角色。

![多角色字段选择](/help/assets/multirole-dropdown-field.png "多角色字段选择"){width="600"}

要为变量分配角色，请执行以下操作：

1. 在&#x200B;_[!UICONTROL 检查检测到的字段]_&#x200B;窗格中找到变量。 这些变量会被自动发现。
2. 查看分配给每个变量的角色。 虽然会自动分配角色，但可以使用模板中任何变量的下拉菜单进行调整。
3. 通过从下拉菜单中选择新角色来调整角色。
4. 单击&#x200B;**[!UICONTROL 下一步]**&#x200B;以继续。

## 进行更正

如果您的模板中存在错误，您可能会看到一则`Template is invalid`消息，其中包含问题的简短说明。 在以下示例中，消息指示`_image`字段不符合多面板模板中建立的字段命名约定。 该消息进一步建议您需要使用正确的前缀更新字段名称。 在模板代码编辑器中查找`_image`字段，并按照建议更新名称。

![更正无效模板](/help/assets/animation/template-code-editor.gif){width="600"}

_[!UICONTROL 检查检测到的字段]_&#x200B;窗格更新以反映您所做的更改。 在您满意这些字段正确且填写完毕后，请单击&#x200B;**[!UICONTROL 下一步]**&#x200B;继续[上载模板](/help/user-guide/templates/use-templates.md#add-a-template)。

## 常见模板问题和解决方案

| **错误** | **描述** | **解决方案** |
|-----------------------------|---------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|
| 未能分析 | 无法将模板内容解析为有效的Handlebars。 | 检查您的模板中是否存在HTML和Handlebars语法错误，并更正它们以确保[内容占位符](/help/user-guide/templates/customize-template.md#content-placeholders)的格式有效。 |
| 未分配组 | 多组电子邮件模板中的图像字段未分配给任何组。 | 检查节前缀的使用是否一致。 每个[节](/help/user-guide/templates/customize-template.md#sections-or-groups)只能使用每个字段类型(`headline`、`body`、`image` `cta`)中的一个。 将`image`字段分配给模板中的有效组。 |
| 缺少图像 | 缺少所需的图像字段。 | 某些模板类型(如Meta、显示或横幅广告)只需要一个`image`字段。 将所需的`image`字段添加到您的模板。 |
| 单个组无效 | 电子邮件模板只包含一个组，该组无效。 | 基本电子邮件模板包含一组模板元素，这些元素不需要[节或组](/help/user-guide/templates/customize-template.md#sections-or-groups)中定义的组命名约定。 通过删除任何组命名语法，将模板调整为零部分。 |
| 无字段 | 模板不包含任何字段。 | 在需要GenStudio for Performance Marketing生成特定类型内容的模板中，使用Handlebars语法添加[可识别的字段名称](/help/user-guide/templates/customize-template.md#recognized-field-names)。 |
| 缺少所需的属性 | 缺少某些必需的元数据属性。 | 每种模板类型都有基于渠道准则的要求和限制。 例如，Meta需要宽高比，而显示广告需要尺寸。 [遵循特定于渠道的模板准则](/help/user-guide/templates/best-practices-for-templates.md#follow-channel-specific-template-guidelines)。 |
| 使用的保留名称 | 正在使用禁止或保留的字段名称。 | 某些[字段名称](/help/user-guide/templates/customize-template.md#recognized-field-names)（如`subject`或`introductory_text`）已保留。 重命名使用保留名称或禁止名称的字段。 |
| 字段过多 | 字段数超过全局限制(20)。 | 删除不必要的字段，以确保总数不超过20。 |
| 组过多 | 组的数量超出了渠道允许的最大值。 | Meta、display和LinkedIn模板不允许使用多个部分。 定义两个或三个部分时，电子邮件需要组命名。 减少模板中的组数以满足[渠道的要求](/help/user-guide/templates/best-practices-for-templates.md#follow-channel-specific-template-guidelines)。 |
| 不支持的字段 | 模板正在使用渠道不支持的字段。 | 根据[可识别的字段名称](/help/user-guide/templates/customize-template.md#recognized-field-names)替换或删除不支持的字段。 |
