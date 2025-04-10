---
title: 模板最佳实践
description: 将模板与Adobe GenStudio for Performance Marketing结合使用时，请遵循最佳实践。
level: Intermediate
role: Developer, User
feature: Media Templates, Content Generation, Brand Personalization
exl-id: 3ff24fec-e836-4202-80f8-ba165e173b75
source-git-commit: 0f296fe6ec92178498e2e0eeb3e190a194e46aa0
workflow-type: tm+mt
source-wordcount: '922'
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

在使用GenStudio for Performance Marketing中的模板之前，为每个品牌配置渠道准则。 渠道指南直接影响使用模板时生成的内容类型。 例如，您可以对电子邮件正文设置字符限制。

![正文规范](/help/assets/channel-email-body.png)

请参阅[渠道准则](/help/user-guide/guidelines/brands.md#channel-guidelines)。

## 遵循特定于渠道的模板准则

在创建模板时，请确保它们满足预期渠道的特定要求。 构建适应每个渠道的布局和视觉要求的模板。 有一些常规准则适用于任何模板，例如：

- 使用简洁且响应式的HTML和内联CSS
- 使用Adobe或Google字体
- **不**&#x200B;使用JavaScript

在使用每种模板类型时，请考虑以下提示和限制以确保最佳性能和兼容性：

>[!BEGINTABS]

>[!TAB 电子邮件]

在自定义电子邮件模板以用于GenStudio for Performance Marketing时，请遵循以下设计最佳实践：

- 使用Adobe或Google字体
- 使用简洁且响应式的HTML和内联CSS
- **不**&#x200B;使用JavaScript
- 请&#x200B;**不**&#x200B;在正文或容器中使用固定宽度
- 请&#x200B;**不**&#x200B;对图像使用base64编码，因为它会显着增加模板大小

**约束**：

- [节](customize-template.md#sections-or-groups)的使用：
   - 基本模板（仅一个部分）可以生成一组模板元素。
   - 一个复杂的模板（多个部分）最多可生成三组模板元素。
- 模板中允许的最大字段数为20
- HTML文件最大大小为102 KB

**可识别的字段名称**：

对于电子邮件，`subject`字段会自动包含在内。 对以下字段使用内容占位符：

- `pre_header`
- `headline`
- `sub_headline`
- `body`
- `cta`
- `image` (从Content JPEG、PNG或GIF中选择)

请参阅[内容占位符](customize-template.md#content-placeholders)以了解有关在模板中使用字段名的更多信息。

>[!TAB 元广告]

在自定义元广告模板以用于GenStudio for Performance Marketing时，请遵循以下设计最佳实践：

- 对列布局使用360像素宽度
- 图像的最低分辨率为1080 x 1080像素
- 请&#x200B;**不**&#x200B;使用相对字体大小
- 请&#x200B;**不**&#x200B;定义视区
- **不**&#x200B;使用JavaScript
- 请&#x200B;**不**&#x200B;覆盖CSS中的HTML元素
- 使用`<img>`标记而不是`background-image`
- 使用蒙版提高背景图像上的文本可读性

**约束**：

- [节](customize-template.md#sections-or-groups)的使用：
   - 只能使用一个部分，生成一组模板元素。

**支持的宽高比**：

- 正方形1:1（1080 x 1080像素）
- 垂直4:5（1080 x 1350像素）
- 文章9:16 （1080 x 1920像素）
- 自定义图像大小： （最小图像宽度50 x 50像素）

**可识别的字段名称**：

对于元广告，`headline`、`body`和`CTA`字段是自动生成的。 对以下字段使用内容占位符：

- `image` (从Content JPEG、PNG或GIF中选择)
- `on_image_text`

请参阅[内容占位符](customize-template.md#content-placeholders)以了解有关在模板中使用字段名的更多信息。

>[!TAB 横幅和显示广告]

在自定义横幅和显示广告模板以用于GenStudio for Performance Marketing时，请遵循以下设计最佳实践：

- 使用Adobe或Google字体
- 准备以超薄尺寸完美显示的资产
- **不**&#x200B;使用嵌入或编码的背景图像
- 使用上载到GenStudio for Performance Marketing内容存储库的背景图像（`image`字段）
- **不**&#x200B;使用JavaScript

**约束**：

- [节](customize-template.md#sections-or-groups)的使用：
   - 只能使用一个部分，生成一组模板元素。

**支持的维度**：

- 垂直：（像素）
   - 300 x 600
   - 160 x 600&#x200B;
- 水平： （像素）
   - 300 x 250
   - 728 x 90
   - 336 x 280
   - 320 x 50
   - 970 x 250&#x200B;
- 自定义： （像素）
   - 50 x 50至2000 x 2000

**可识别的字段名称**：

对于横幅广告和显示广告，会自动生成`CTA`字段。 对以下字段使用内容占位符：

- `headline`
- `sub_headline`
- `body`
- `image` (从Content JPEG、PNG或GIF中选择)

请参阅[内容占位符](customize-template.md#content-placeholders)以了解有关在模板中使用字段名的更多信息。

>[!TAB LinkedIn广告]

[!BADGE Beta]{type=Informative tooltip="此功能当前位于Beta中，因此某些功能可能会受到限制或发生更改。"}

在自定义LinkedIn广告模板以用于GenStudio for Performance Marketing时，请遵循以下设计最佳实践：

**约束**：

- [节](customize-template.md#sections-or-groups)的使用：
   - 只能使用一个部分，生成一组模板元素。
- 最大图像大小5 MB
- 最大标题70个字符
- 介绍性文本的最大长度为150个字符

**支持的宽高比**：

- 方形1:1
   - 桌面或移动设备
   - 最小值：360 x 360像素
   - 最大：4320 x 4320像素
- 水平1.91:1
   - 桌面
   - 最小值：640 x 360像素
   - 最大：7680 x 4320像素
- 垂直1:1.91
   - 移动设备
   - 最小值：360 x 640像素
   - 最大：2430 x 4320像素
- 垂直2.3
   - 移动设备
   - 最小值：360 x 640像素
   - 最大：2430 x 4320像素
- 垂直4.5（推荐）
   - 移动设备
   - 最小值：360 x 640像素
   - 最大：2430 x 4320像素

**可识别的字段名称**：

对于LinkedIn广告，`headline`、`introductory_text`和`CTA`字段是自动生成的。 对以下字段使用内容占位符：

- `image` (从Content JPEG、PNG或GIF中选择)
- `on_image_text`

请参阅[内容占位符](customize-template.md#content-placeholders)以了解有关在模板中使用字段名的更多信息。

>[!ENDTABS]
