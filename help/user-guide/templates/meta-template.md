---
title: Meta广告模板准则
description: 将Meta广告模板与Adobe GenStudio for Performance Marketing结合使用时，请遵循最佳实践。
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: e69039b0-272d-4f39-b0e4-916be710fd5f
source-git-commit: 3251d81a6bfb0c1f7d2bf3c5bd319ad4e2237699
workflow-type: tm+mt
source-wordcount: '375'
ht-degree: 1%

---

# Meta广告模板准则

Meta广告模板可帮助您跨Meta平台创建视觉上一致且有效的广告。 通过遵循推荐的设计实践并使用支持的字段，您可以确保模板已针对GenStudio for Performance Marketing进行了优化。 本指南介绍如何构建、自定义和准备Meta广告模板，以实现无缝集成和高成效的结果。

在自定义Meta广告模板以用于GenStudio for Performance Marketing时，请遵循以下设计最佳实践：

- 对列布局使用360像素宽度
- 图像的最低分辨率为1080 x 1080像素
- 仅需要一个图像字段
- 请&#x200B;**不**&#x200B;使用相对字体大小
- 请&#x200B;**不**&#x200B;定义视区
- **不**&#x200B;使用JavaScript
- 请&#x200B;**不**&#x200B;覆盖CSS中的HTML元素
- 使用`<img>`标记而不是`background-image`
- 使用蒙版提高背景图像上的文本可读性
- 只能使用一个部分，生成一组模板元素

## 可识别的字段名称

在自定义Meta广告模板时，请为以下必填字段应用内容占位符：

- `image` (必需，从Content JPEG、PNG或GIF中选择)
- `on_image_text` （图像上显示的文本）

GenStudio for Performance Marketing会自动生成以下字段。 您不必为以下内容应用内容占位符：

- `headline`
- `body`
- `cta`

请参阅[内容占位符](/help/user-guide/templates/customize-template.md#content-placeholders)以了解有关在模板中使用字段名的更多信息。

## 支持的宽高比

| 宽高比 | 尺寸（像素） | 注释 |
|------------------|----------------------------|-----------------------------------------------------------------------|
| 方形1:1 | 1080 x 1080 | 大多数Meta投放位置的标准；建议用于广泛兼容。 |
| 纵向4:5 | 1080 x 1350 | 针对移动馈送进行了优化；提供了更多垂直空间。 |
| 故事9:16 | 1080 x 1920 | 非常适合于故事和胶卷；填充整个移动设备屏幕。 |
| 横向1.91:1 | 1080 x 566 | 最适合链接广告和新闻馈送投放；宽格式。 |
| 自定义 | 最小50 x 50（宽度） | 仅在需要时使用；可能会导致裁切或缩放。 |

如果广告不是按上述某个纵横比设计的，GenStudio for Performance Marketing会自动将图像裁剪为适当的大小。

## 模板示例

+++示例：Meta广告模板

<!-- Does this need to be a precise size? -->

以下是Meta广告模板的基本示例。 标头包含用于样式化的内联CSS。 正文使用[内容占位符](#content-placeholders)（如`image`和`on_image_text`）来指示GenStudio for Performance Marketing可在何处生成内容。

```html {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Adobe</title>
        <style>
            .ad-container {
            font-family: Helvetica, sans-serif;
            position: relative;
            text-align: center;
            height: 100%;
            }
            .ad-image {
            width: 100%;
            height: 100%;
            object-fit: cover;
            }
            .ad-text {
            position: absolute;
            top: 0;
            left: 0;
            margin: 1em;
            background-color: rgba(0, 0, 0, 0.5);
            color: white;
            padding: 1em;
            font-size: 75px;
            }
        </style>
    </head>
    <body>
        <div class="ad-container">
            <img src="{{image}}" alt="Ad Image" class="ad-image" />
            <div class="ad-text">{{on_image_text}}</div>
        </div>
    </body>
</html>
```

+++
