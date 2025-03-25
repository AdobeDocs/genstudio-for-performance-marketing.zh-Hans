---
title: 自定义模板
description: 了解如何针对Adobe GenStudio for Performance Marketing个性化和优化模板。
level: Intermediate
role: Developer
feature: Media Templates, Content Generation
exl-id: 292c1689-1b12-405d-951e-14ee6aebc75a
source-git-commit: 0a1f13db9a976bac026f49e908b6b8c124bc5df7
workflow-type: tm+mt
source-wordcount: '1442'
ht-degree: 0%

---

# 自定义模板

通过插入创作AI用于插入内容的内容占位符或字段，可以自定义在GenStudio for Performance Marketing中使用的模板。

接下来的几个部分将说明如何使用&#x200B;_[!DNL Handlebars]_模板语言来调整HTML模板以用于GenStudio for Performance Marketing。 [!DNL Handlebars]语法使用带双大括号的常规文本作为内容占位符。 请参阅_ Handlebars语言指南&#x200B;_中的[什么是 [!DNL Handlebars]](https://handlebarsjs.com/guide/#what-is-handlebars)以了解如何准备模板。

模板准备就绪后，您可以[将其上传到GenStudio for Performance Marketing](use-templates.md#upload-a-template)，并开始根据您的自定义模板生成个性化电子邮件。

>[!TIP]
>
>遵循[辅助功能准则](accessibility-for-templates.md)和[最佳实践](/help/user-guide/content/best-practices-for-templates.md)，以便您可以接触到更多受众并提供最佳体验。

## 内容占位符

GenStudio for Performance Marketing可识别模板中的某些[元素](use-templates.md#template-elements)，但必须使用[可识别的字段名](#recognized-field-names)来识别它们。

在HTML模板的head或body中，可以使用[!DNL Handlebars]语法插入内容占位符，在其中需要GenStudio for Performance Marketing使用实际内容填充模板。 GenStudio for Performance Marketing根据[识别的&#x200B;_字段_&#x200B;名称](#recognized-field-names)来识别和解释内容占位符。

例如，您可以使用带有[!DNL Handlebars]语法的`{{ headline }}`来指示电子邮件的标题应放在何处。 GenStudio可识别此字段，根据您的准则和提示标准生成相关标题，并将标题插入此位置：

```handlebars
<div>{{ headline }}</div>
```

### 可识别的字段名称

下表列出了GenStudio for Performance Marketing识别用于将占位符添加到模板的字段名称。 在需要GenStudio for Performance Marketing生成特定类型内容的模板中，使用[!DNL Handlebars]语法添加这些字段名称。

| 字段 | 角色 | 渠道模板 |
| ----------------------- | ------------------------- | ------------------------------------------------ |
| `{{pre_header}}` | 预编译标头 | 电子邮件 |
| `{{headline}}` | 标题 | 电子邮件<br>元广告<br>横幅和显示广告<br>LinkedIn广告 |
| `{{introductory_text}}` | 介绍性文本 | LinkedIn广告 |
| `{{body}}` | 正文 | 电子邮件<br>元广告<br>横幅和显示广告 |
| `{{cta}}` | 行动号召 | 电子邮件<br>元广告<br>横幅和显示广告<br>LinkedIn广告 |
| `{{image}}` | 图像 — 从[!DNL Content]中选择 | 电子邮件<br>元广告<br>横幅和显示广告<br>LinkedIn广告 |
| `{{on_image_text}}` | 在图像文本上 | 元广告<br>LinkedIn广告 |
| `{{link}}` | 对映像<br>的行动号召，请参阅映像](#link-on-image)上的[链接。 | 电子邮件 |
| `{{brand_logo}}` | 所选品牌<br>的徽标请参阅[品牌徽标字段名称](#brand-logo-field-name)。 | 电子邮件<br>元广告<br>链接加入广告 |

GenStudio for Performance Marketing会自动填充以下模板中的特定字段：

- **电子邮件模板**&#x200B;不需要您识别`subject`字段
- **元广告模板**&#x200B;不要求您识别`headline`、`body`和`CTA`字段
- **横幅和显示广告模板**&#x200B;不需要您识别`CTA`字段
- **LinkedIn广告模板**&#x200B;不需要您识别`headline`、`introductory_text`和`CTA`字段

>[!WARNING]
>
>对于Instagram广告，生成的标题不会出现在最终体验中。

将模板上传到GenStudio for Performance Marketing时限制为20个字段。 由于`subject`字段是在电子邮件中自动生成的，因此它计为一个字段。 这意味着电子邮件模板中允许有19个字段。

>[!TIP]
>
>您可以使用GenStudio for Performance Marketing中的[模板预览](#template-preview)来验证您的模板。

### 行动号召

行动号召(CTA)包括短语和链接。 为了使&#x200B;_[!UICONTROL 重写]_&#x200B;和&#x200B;_[!UICONTROL 添加链接]_&#x200B;功能在变体生成过程中正常工作，您必须在模板中包含链接和短语的占位符。

使用下面的指南设置CTA占位符：

- CTA短语可用且链接可编辑

  ```html
  <a class="button" href="{{pod1_link}}" >{{cta}}</a>
  ```

- CTA重新短语可用，但链接&#x200B;**不可编辑**，因为模板中提供了实际链接

  ```html
  <a align="center" href="https://link">{{cta}}</a>
  ```

- CTA链接可编辑，但重新短语是&#x200B;**不可用的**，因为模板中提供了短语

  ```html
  <a class="button" href="{{pod1_link}}" >Register now</a>
  ```

GenStudio for Performance Marketing也可以提供各种行动号召短语。 请参阅[修改行动要求](/help/user-guide/create/manage-variants.md#revise-call-to-action)。

### 图像上的链接

您可以自定义电子邮件模板，以允许创意人员添加指向图像的链接。 与CTA链接类似，使用下列指南将`link`占位符应用于图像标记：

```html
<a href="{{link}}"><img src="image-source.jpg" alt="description"></a>
```

在此示例中：

- `{{link}}`是实际URL的占位符。
- `src="image-source.jpg"`应替换为实际图像源URL。
- `alt="description"`为图像提供替换文本，这对于辅助功能和SEO很有用。

### 品牌徽标字段名称

此时，您无法选择用于模板上传的品牌徽标。 以下示例演示了两种有条件地呈现品牌徽标的方法。 每种方法都验证源，提供默认或替代图像（如果品牌徽标不可用），并应用样式：

**示例1**：直接在HTML `img src`属性中使用[!DNL Handlebars]内置帮助程序条件：

```html
<img src="{{#if brand_logo}}{{brand_logo}}{{else}}<default-image>{{/if}}" alt="img alt text" style="max-width: 88px; margin: 10px auto; display: block;">
```

**示例2**：使用[!DNL Handlebars]内置条件语句封装HTML `img`标记：

```html
{{#if brand_logo}}
    <img src="{{brand_logo}}" alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
    {{else}}
    <img src="data:image/png;base64,iVBORw0KGgo..." alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
{{/if}}
```

### 手动字段名称

所有其他字段名称均被视为手动填充的字段。 例如，您可能需要为页脚内容保留部分。

要创建可编辑的节，请在节名称两侧添加双括号：

```html
<tbody>
    <tr>
        <td>
            <p><span class="s1">{{ footerLegal }}</span></p>
        </td>
    </tr>
</tbody>
```

## 区域或组

_节_&#x200B;通知GenStudio for Performance Marketing此节中的字段需要高度一致性。 建立这种关系有助于AI生成与部分中的创意元素匹配的内容。

在字段名称中使用您选择的前缀来指示字段是部分或组的一部分。 在下划线(`_`)之后使用字段名称（`headline`、`body`、`image`或`cta`）。

- _正确_ (??)： `pod1_body`
- _不正确_ (❌)： `pod1_link`

每个部分只能使用每种字段类型中的一种。 例如，以下字段属于`pod1`部分：

- `pod1_headline`
- `pod1_body`
- `pod1_image`
- `pod1_cta`

由于此规则，无法嵌套这些部分。

每种模板类型（如电子邮件或元广告）都包含特定于渠道的部分使用限制。 请参阅&#x200B;_使用模板的最佳实践_&#x200B;主题中的[特定于渠道的指南](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/content/templates/best-practices-for-templates#follow-channel-specific-template-guidelines)。

例如，电子邮件模板最多可包含三个部分；因此，您可以包含三个标题部分和正文部分：

- `pre_header`
- `pod1_headline`
- `pod1_body`
- `pod2_headline`
- `pod2_body`
- `pod3_headline`
- `pod3_body`
- `cta`

GenStudio for Performance Marketing了解`pod1_headline`与`pod1_body`的关系比`pod2_body`更密切。

请参阅[结构化提示](/help/user-guide/effective-prompts.md#structured-prompts)，了解如何在多节电子邮件中制作为每个节生成不同内容的提示。


## 模板预览

当您[上载模板](use-templates.md#upload-a-template)时，GenStudio for Performance Marketing会扫描HTML文件以查找可识别的字段。 使用该预览查看您的[模板元素](use-templates.md#template-elements)，并确认您使用[可识别的字段名称](#recognized-field-names)正确识别了这些元素。

电子邮件模板的示例预览：

![检测到预览字段](/help/assets/template-detected-fields.png "检查检测到的字段"){zoomable="yes"}

请参阅[模板代码编辑器](/help/user-guide/content/code-editor.md)。

### 控件预览

您可以使用内置帮助程序（执行特定操作的[!DNL Handlebars]模板语言中的特殊表达式）控制特殊内容的可见性。 例如，您可以添加一个条件语句，该语句可在保持预览链接干净的同时，将跟踪参数添加到导出模板中的链接。

在呈现模板时设置`_genStudio.browser`值，在导出模板时设置`genStudio.export`值。 例如，当模板用于导出时，您可以决定在电子邮件顶部使用条件包装器包含某些内容：

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

另一个示例可能是为了防止在GenStudio for Performance Marketing中预览模板时使用跟踪代码。 以下示例说明如何在保持预览链接整洁的同时向导出的模板中的链接添加跟踪参数：

```html
<a class="button" {{#if _genStudio.browser }}
   href="{{ link }}"{{/if}}{{#if _genStudio.export }}
   href="{{ link }}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{ cta }}</a>
```

## 静态内容

电子邮件和元模板通常链接到托管在其他域上的图像和CSS文件。 当GenStudio for Performance Marketing为模板预览或从中派生的体验生成缩略图时，它将验证内容源并嵌入副本以进行预览。

临时嵌入外部文件仅用于创建模板预览，这可确保预览准确反映内容在创建时显示的情况。 这些外部文件&#x200B;**不是**&#x200B;永久存储在GenStudio for Performance Marketing中。 创建模板预览后，GenStudio for Performance Marketing将继续引用模板中提供的原始源链接。

### 刷新内容

如果在创建初始预览后源发生更改，请使用[refresh](/help/user-guide/content/use-templates.md#refresh-template)函数以外部源内容的最新版本更新模板预览。

## 模板示例

+++示例：带一个部分的电子邮件模板

以下是包含一节的电子邮件的HTML模板的基本示例。 标头包含用于样式设置的简单内联CSS。 正文包含`pre_header`、`headline`和`image` [占位符](#content-placeholders)，供GenStudio for Performance Marketing在电子邮件生成过程中用于插入内容。

```html {line-numbers="true" highlight="13"}
<!DOCTYPE html>
<html>
    <head>
        <title>Adobe</title>
        <style>
            .container {
            width: 100%;
            padding: 20px;
            font-family: Arial, sans-serif;
            }
        </style>
    </head>
    <body>{{ pre_header }}
        <div class="container">
            <h1>{{ headline }}</h1>
            <p><a href="{{ link }}">
            <img alt="{{ headline }}"
                    src="{{ image }}"
                    width="600" height="600"
                    border="0"/></a></p>
            <p>{{ body }}</p>
        </div>
    </body>
</html>
```

+++

+++示例：具有多个部分的电子邮件模板

以下是上述示例中的相同HTML模板，但添加了两个部分。 标头包含用于设置组样式的内联CSS。 正文使用两个组，其中[个内容占位符](#content-placeholders)使用前缀。

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Adobe</title>
        <style>
            .container {
            width: 100%;
            padding: 20px;
            font-family: Arial, sans-serif;
            }
            .pod {
            background-color: #f8f8f8;
            margin: 10px;
            padding: 20px;
            border-radius: 5px;
            }
            .pod h2 {
            color: #333;
            }
            .pod p {
                color: #666;
            }
        </style>
    </head>
    <body>{{ pre_header }}
        <div class="container">
            <h1>{{ headline }}</h1>
            <p>{{ body }}</p>
            <!-- Pod1 -->
            <div class="pod">
                <h2>{{ pod1_headline }}</h2>
                <p><img alt="{{ headline }}" src="{{ pod1_image }}" width="200" height="200" border="0"></p>
                <p>{{ pod1_body }}</p>
            </div>
            <!-- End of Pod1 -->
            <!-- Pod2 -->
            <div class="pod">
                <h2>{{ pod2_headline }}</h2>
                <p><img alt="{{ headline }}" src="{{ pod2_image }}" width="200" height="200" border="0"></p>
                <p>{{ pod2_body }}</p>
            </div>
            <!-- End of Pod2 -->
        </div>
    </body>
</html>
```

+++

+++示例：元广告模板

以下是元广告模板的基本示例。 标头包含用于样式化的内联CSS。 正文使用[内容占位符](#content-placeholders)（如`image`和`on_image_text`）来指示GenStudio for Performance Marketing可在何处生成内容。

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
            <img src="{{ image }}" alt="Ad Image" class="ad-image" />
            <div class="ad-text">{{ on_image_text }}</div>
        </div>
    </body>
</html>
```

+++
