---
title: 显示广告模板准则
description: 在Adobe GenStudio for Performance Marketing中使用显示广告和横幅模板时，请遵循最佳实践。
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 076239b3-9444-48f9-bdd6-ef2b757bdf0d
source-git-commit: 4760da26d20e91489a74bb238e07f0d3b426c0a1
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 1%

---

# 显示广告模板准则

显示模板是预先设计的布局，用于创建吸引眼球的横幅和显示广告。 它们提供了一个灵活的框架来整合图像、文本和call to action，确保在生成多个广告变体时保持一致性和效率。 在准备用于GenStudio for Performance Marketing的模板时，请确保所有资源都针对Web显示进行了优化，并符合所需的文件格式和大小。

在自定义横幅和显示广告模板以用于GenStudio for Performance Marketing时，请遵循以下设计最佳实践：

- 使用Adobe或Google字体
- 准备以超薄尺寸完美显示的资产
- 仅需要一个图像字段
- **不**&#x200B;使用嵌入或编码的背景图像
- 使用上载到GenStudio for Performance Marketing内容存储库的背景图像（`image`字段）
- **不**&#x200B;使用JavaScript
- 只能使用一个部分，生成一组模板元素

## 可识别的字段名称

在自定义横幅或显示广告模板时，请为以下必填字段使用内容占位符：

- `headline`
- `sub_headline`
- `body`
- `image` (必需，从Content JPEG、PNG或GIF中选择)

GenStudio for Performance Marketing会自动生成以下字段。 您不必为以下内容应用内容占位符：

- `cta`

请参阅[内容占位符](/help/user-guide/content/customize-template.md#content-placeholders)以了解有关在模板中使用字段名的更多信息。

## 支持的维度

必须设置宽度x高度（像素）。

| 方向 | 尺寸（像素） | 注释 |
|--------------|-------------------------------------------------------------|------------------------------------------------------------------|
| 垂直 | 300 x 600<br>160 x 600 | 普通摩天大楼和半页横幅 |
| 水平 | 300 x 250<br>728 x 90<br>336 x 280<br>320 x 50<br>970 x 250 | 标准排行榜、中等矩形和横幅尺寸 |
| 自定义 | 50 x 50至2000 x 2000 | 用于非标准或唯一放置；检查平台限制 |

<!-- Potentially add an example

## Template example

+++Example: Display ad template

+++

-->
