---
title: LinkedIn模板准则
description: 将LinkedIn模板与Adobe GenStudio for Performance Marketing结合使用时，请遵循最佳实践。
level: Intermediate
role: Developer, User
feature: Media Templates
source-git-commit: 35a519a8d28e260bfa6d9ed671bd5bf1cfeda931
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 1%

---

# LinkedIn模板准则

LinkedIn模板提供了一种结构化方式，用于创建和自定义LinkedIn营销活动的广告创意。 这些准则可确保您的广告符合LinkedIn的规范，同时简化GenStudio for Performance Marketing中的创作流程。 本指南可帮助您为LinkedIn桌面和移动平台之间一致的品牌推广和有效性能做好准备。

在自定义LinkedIn广告模板以用于GenStudio for Performance Marketing时，请遵循以下设计最佳实践：

- 仅需要一个图像字段
- 最大图像大小5 MB
- 最大标题70个字符
- 介绍性文本的最大长度为150个字符
- 只能使用一个部分，生成一组模板元素

## 可识别的字段名称

自定义LinkedIn模板时，请为以下必填字段应用内容占位符：

- `image` (必需，从Content JPEG、PNG或GIF中选择)
- `on_image_text` （图像上显示的文本）

GenStudio for Performance Marketing会自动生成以下字段。 您不必为以下内容应用内容占位符：

- `headline`
- `introductory_text`
- `cta` (Call to action)

请参阅[内容占位符](/help/user-guide/content/customize-template.md#content-placeholders)以了解有关在模板中使用字段名的更多信息。

## 支持的宽高比

| 宽高比 | Platform | 最小大小（像素） | 最大大小（像素） | 注释 |
|-------------------|-----------------|---------------|----------------|-------------------------------------------------------------------------------------|
| 方形1:1 | 台式机、移动设备 | 360 x 360 | 4320 x 4320 | 最具通用性。 非常适合于跨设备和投放位置的一致外观。 |
| 水平1.91:1 | 桌面 | 640 x 360 | 7680 x 4320 | 标准横向格式。 通常用于赞助内容和动态信息源广告。 |
| 垂直1:1.91 | 移动设备 | 360 x 640 | 2430 x 4320 | 高垂直格式。 针对移动设备查看进行了优化，提供了更多屏幕显示。 |
| 垂直2:3 | 移动设备 | 360 x 640 | 2430 x 4320 | 略低于1:1.91。对于以移动为先的营销活动有益。 |
| 垂直4:5 | 移动设备 | 360 x 640 | 2430 x 4320 | 建议用于移动设备。 平衡可见性和内容，这通常会产生更大的影响。 |

<!-- Potentially add an example

## Template example

+++Example: LinkedIn template

+++

-->
