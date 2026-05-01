---
title: 在模板中设置徽标交换
description: 在模板中配置品牌徽标占位符以在 [!DNL GenStudio for Performance Marketing]中启用徽标交换。
feature: Create Canvas
role: User
level: Intermediate
source-git-commit: 98cb7ba338878495e6d7b68f3b8c620abae10127
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 2%

---

# 在模板中设置徽标交换

本指南介绍如何在模板中配置品牌徽标占位符，以在[!DNL GenStudio for Performance Marketing]中启用[徽标交换功能](/help/user-guide/create/logo-swap.md)。 请遵循以下准则以确保占位符在各种图像大小和长宽比中正确显示。

## 快速设置

为您的徽标图像使用以下基本模板代码：

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="my-logo"
>
```

必需：

- `src="{{brand_logo}}"` — 启用徽标交换功能。
- `style="{{defaultLogo}}"` — 应用占位符边框样式。

可选：

- `class="my-logo"` — 用于调整大小和样式的自定义CSS类。

## 了解占位符边框

未选择徽标时，`{{brand_logo}}`包含透明的1×1像素图像。 `{{defaultLogo}}`样式会自动应用大纲，以便占位符可见：

```css
outline: clamp(1px, 0.1em, 5px) dashed #FFF;
```

边框行为：

- 显示默认占位符时显示。
- 更换徽标后自动消失。
- 根据父字体大小进行缩放。

### 边框大小

`clamp()`函数根据模板大小调整大纲粗细：

| 父字体大小 | 大纲大小 |
| --- | --- |
| 10px | 1像素（分钟） |
| 16px | 1.6px |
| 24px | 2.4px |
| 32px | 3.2px |
| 50px+ | 5像素（最大） |

公式： `0.1em`等于继承的字体大小的10%，固定在`1px`和`5px`之间。

## 自定义占位符边框

可以使用CSS类覆盖默认大纲。 `{{defaultLogo}}`样式应用基本轮廓，并且您的类可以自定义颜色、宽度和样式。

模板HTML：

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-custom-border"
>
```

模板CSS：

```css
.logo-custom-border {
  outline-color: #0066CC !important;
  outline-width: 2px !important;
  outline-style: dotted !important;
}
```

>[!NOTE]
>自定义轮廓样式仅影响占位符。 交换徽标后，所有大纲样式都会自动删除。

## 设置建议的徽标大小

要确保占位符可见并防止版面偏移，请在CSS类中设置明确的大小：

模板HTML：

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-standard"
>
```

模板CSS：

```css
.logo-standard {
  width: 120px;
  height: 60px;
}
```

## 控件徽标定位

使用`object-fit`和`object-position`控制徽标在其容器中的缩放方式。

### 以徽标为中心（最常见）

徽标会缩放以适合150×80像素，在水平和垂直方向上居中。

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-centered"
>
```

```css
.logo-centered {
  width: 150px;
  height: 80px;
  object-fit: contain;
  object-position: center center;
}
```

### 徽标左对齐

徽标缩放以适合，与左边缘对齐，垂直居中。

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-left"
>
```

```css
.logo-left {
  width: 200px;
  height: 60px;
  object-fit: contain;
  object-position: left center;
}
```

### 右上角的徽标

徽标缩放以适合，位于右上角。

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-top-right"
>
```

```css
.logo-top-right {
  width: 100px;
  height: 100px;
  object-fit: contain;
  object-position: right top;
}
```

## 完整示例

### 最小设置

```html
<img src="{{brand_logo}}" style="{{defaultLogo}}">
```

>[!NOTE]
>虽然可以进行此设置，但占位符可能几乎不可见，因为透明1×1像素图像会折叠到其自然大小。 为可见占位符使用带有`width`和`height`的CSS类。

### 建议的设置

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="brand-logo"
>
```

```css
.brand-logo {
  width: 120px;
  height: 60px;
  object-fit: contain;
  object-position: center center;
}
```

### 使用自定义边框进行高级设置

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="sponsor-logo"
>
```

```css
.sponsor-logo {
  width: 180px;
  height: 90px;
  object-fit: contain;
  object-position: left center;
  outline-color: #0066CC !important;
  outline-width: 2px !important;
  outline-style: solid !important;
}
```

### 灵活的设置，具有大小限制

将`min-*`和`max-*`属性用于响应模板或各种徽标大小。

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-flexible"
>
```

```css
.logo-flexible {
  min-width: 20px;
  min-height: 20px;
  max-width: 200px;
  max-height: 100px;
  object-fit: contain;
  object-position: center center;
}
```

工作原理：

- `min-width`和`min-height`保持占位符可见。
- `max-width`和`max-height`防止过大的徽标破坏布局。
- 徽标将按比例在这些边界内缩放。

## CSS属性引用

| 类别 | 属性 | 值 | 用途 |
| --- | --- | --- | --- |
| 必需(HTML) | `src` | `{{brand_logo}}` | 启用徽标交换功能。 |
| 必需(HTML) | `style` | `{{defaultLogo}}` | 应用占位符大纲。 |
| 推荐（CSS类） | `width` | `120px` | 设置最大徽标宽度。 |
| 推荐（CSS类） | `height` | `60px` | 设置最大徽标高度。 |
| 推荐（CSS类） | `object-fit` | `contain` | 缩放徽标而不进行裁剪。 |
| 推荐（CSS类） | `object-position` | `center center` | 控制徽标对齐方式。 |
| 可选（CSS类） | `outline-color` | `#FF0000` | 更改轮廓颜色。 |
| 可选（CSS类） | `outline-width` | `3px` | 更改轮廓粗细。 |
| 可选（CSS类） | `outline-style` | `solid` | 更改大纲样式。 |
| 灵活调整大小（CSS类） | `min-width` | `20px` | 确保占位符可见性。 |
| 灵活调整大小（CSS类） | `min-height` | `20px` | 确保占位符可见性。 |
| 灵活调整大小（CSS类） | `max-width` | `200px` | 防止溢出。 |
| 灵活调整大小（CSS类） | `max-height` | `100px` | 控制布局边界。 |

## 最佳做法

执行：

- 始终包括`{{brand_logo}}`和`{{defaultLogo}}`。
- 定义`width`和`height`，使占位符可见。
- 使用CSS类进行大小调整和大纲自定义。
- 使用`object-fit: contain`保留徽标外观比例。
- 使用不同大小和宽高比的徽标进行测试。

请勿：

- 使用`border`而不是`outline`（边框不会自动隐藏）。
- 将大小调整属性置于内联样式中。
- 省略大小限制（占位符以1×1像素呈现）。
- 使用`object-fit: cover`（它可能会裁切标志）。

## 故障排除

边框不可见：

- 确保包括`style="{{defaultLogo}}"`。
- 确认已在您的CSS类中定义`width`和`height`。

占位符太小(1px)：

- 将显式`width`和`height`添加到您的CSS类。

交换后边框未消失：

- 在CSS类中使用大纲属性，而不是`border`。

将裁剪徽标：

- 使用`object-fit: contain`而不是`cover`。

徽标太小或太大：

- 调整CSS类中的`width`和`height`。

未显示自定义边框：

- 确认`{{defaultLogo}}`在`style`属性中。
- 将自定义`outline-*`属性放入CSS类中。
