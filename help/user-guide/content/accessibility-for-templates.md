---
title: 创建无障碍模板
description: 在Adobe GenStudio for Performance Marketing中构建模板，这些模板能够吸引更多受众并提供最佳体验。
feature: Media Templates
exl-id: eaaa5d9f-ad45-4fd0-826d-c250deb6d238
source-git-commit: 28c128ad6f3d173b7516a6b1309555c12e6a4e2d
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---

# 创建无障碍模板

Adobe致力于为所有受众提供最佳体验。 请参阅Adobe上的[辅助功能计划](https://www.adobe.com/trust/accessibility/initiatives.html)以了解更多内容。

在GenStudio for Performance Marketing中，您可以上传资源和模板，以便为各种体验创建内容。 遵守辅助功能标准有助于您的内容触及最大目标受众。

使用以下建议，使用最佳辅助功能标准准备模板。

## 替换文本

为非文本内容（如图像）提供替换文本。

```html
<img alt="Collage of ideas, books, man holding giant pencil, computer" src="card-create-assets.png">
```

![创意拼贴、书籍、拿着巨铅笔的男人、计算机](/help/assets/card-create-assets.png){width="400"}

在自定义模板时，为`alt`和`aria-label`属性使用内容占位符：

- [替换文本](/help/user-guide/content/customize-template.md#alternative-text)
- [辅助功能标签](/help/user-guide/content/customize-template.md#accessibility-label)

## 字体

使用易于阅读的字体。 例如，Sans Serif字体具有干净、块状的外观，这有助于提高可读性。

在文本和背景之间提供相应的对比度。 避免使用在深色背景上生成深色文本，而在浅色背景上生成浅色文本的字体颜色。 考虑对比度准则以获得最佳比例：

- 文本的文本和图像：对比度至少为4.5:1
- 大型文本和图像大型文本：对比度至少为3:1

## 链接目的（仅限链接）

创建描述链接目的和位置的纯链接文本。

例如，使用“单击此处”或“了解更多”之类的链接文本不会清楚地描述链接的目的：

```html
<a href="product-site.html">Click here</a>
```

作为最佳实践，您应该使用清晰描述链接位置的文本。 更好的示例可能使用链接源的标题和目的：

```html
<a href="product-site.html">Explore Product Site</a>
```

## 语言

许多产品和服务都以富有创意或独一无二的方式使用语言。 避免使用行话、长句和复杂短语。 使用与目标受众兼容的清晰、简洁、易读语言。

- 尽可能使用清晰的描述、内联定义或可关联的示例。 翻译一个独特的白话可能很困难。

- 拼出或链接到首字母缩写或缩写实例的定义。 缩写可能很难翻译。

- 尽可能使用可视化元素来补充文本或复杂想法。
