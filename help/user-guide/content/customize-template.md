---
title: 自定义模板
description: 了解如何针对Adobe GenStudio for Performance Marketing个性化和优化模板。
level: Intermediate
feature: Templates, Content
exl-id: 292c1689-1b12-405d-951e-14ee6aebc75a
source-git-commit: 8930d3284f9dd1223067239c0077e481ea98335a
workflow-type: tm+mt
source-wordcount: '1173'
ht-degree: 0%

---

# 自定义模板

通过插入创作AI用于插入内容的内容占位符或字段，可以自定义在GenStudio for Performance Marketing中使用的模板。

以下几个部分将说明如何使用&#x200B;_Handlebars_ HTML语言来调整模板以用于GenStudio for Performance Marketing。 [!DNL Handlebars]语法使用带双大括号的常规文本作为内容占位符。 查看[什么是 [!DNL Handlebars]？_Handlebars语言指南_&#x200B;中的](https://handlebarsjs.com/guide/#what-is-handlebars)以了解如何准备模板。


模板准备就绪后，您可以[将其上传到GenStudio for Performance Marketing](use-templates.md#upload-a-template)，并开始根据您的自定义模板生成个性化电子邮件。

>[!TIP]
>
>遵循[辅助功能准则](accessibility-for-templates.md)和[最佳实践](/help/user-guide/content/best-practices-for-templates.md)，以便您可以接触到更多受众并提供最佳体验。

## 内容占位符

GenStudio for Performance Marketing可识别模板中的某些[元素](use-templates.md#template-elements)，但前提是使用可识别的字段名称标识它们。

在模板的head或正文中，可以使用[!DNL Handlebars]语法作为内容占位符，其中要求GenStudio for Performance Marketing使用实际内容填充模板。 GenStudio for Performance Marketing根据[识别的&#x200B;_字段_&#x200B;名称](#recognized-field-names)来识别和解释内容占位符。

例如，您可以使用带有[!DNL Handlebars]语法的`{{ headline }}`来指示电子邮件标题的放置位置：

```handlebars
<div>{{headline}}</div>
```

### 可识别的字段名称

下表列出了GenStudio for Performance Marketing识别用于填充到模板中的字段名称。 在需要GenStudio for Performance Marketing生成内容的模板中使用[!DNL Handlebars]语法添加这些字段名称。

| 字段 | 角色 | 渠道模板 |
| ------------------ | ---------------------- | -------------------------------- |
| `{{pre_header}}` | 预标题 | 电子邮件 |
| `{{headline}}` | 标题 | 电子邮件<br>元广告<br>显示广告 |
| `{{body}}` | 正文 | 电子邮件<br>元广告<br>显示广告 |
| `{{cta}}` | 行动号召 | 电子邮件<br>元广告<br>显示广告 |
| `{{on_image_text}}` | 在图像文本上 | 元广告 |
| `{{image}}` | 图像 — 从内容中选择 | 电子邮件<br>元广告<br>显示广告 |
| `{{brand_logo}}` | 所选品牌的徽标<br>请参阅[品牌徽标字段名称](#brand-logo-field-name)以了解建议用法。 | 电子邮件<br>元广告 |

GenStudio for Performance Marketing会自动填充以下模板中的特定字段：

- **电子邮件模板**&#x200B;不需要您识别`subject`字段
- **元广告模板**&#x200B;不要求您识别`headline`、`body`和`CTA`字段
- **显示广告模板**&#x200B;不要求您识别`CTA`字段

>[!WARNING]
>
>对于Instagram广告，生成的标题不会显示在最终体验中。

将模板上传到GenStudio for Performance Marketing时限制为20个字段。 由于`subject`字段是在电子邮件中自动生成的，因此它计为一个字段。 这意味着电子邮件模板中允许有19个字段。

>[!TIP]
>
>您可以使用GenStudio for Performance Marketing中的[模板预览](#template-preview)来验证您的模板。

#### 品牌徽标字段名称

此时，您无法选择用于模板上传的品牌徽标。 以下示例演示了两种有条件地呈现品牌徽标的方法。 每种方法都验证源，提供默认或替代图像（如果品牌徽标不可用），并应用样式：

**示例1**：直接在HTML`img src`属性中使用[!DNL Handlebars]内置帮助程序条件：

```html
<img src="{{#if brand_logo}}{{brand_logo}}{{else}}<default-image>{{/if}}" alt="img alt text" style="max-width: 88px; margin: 10px auto; display: block;">
```

**示例2**：使用[!DNL Handlebars]内置条件语句包装HTML`img`标记：

```handlebars
{{#if brand_logo}}
    <img src="{{brand_logo}}" alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
    {{else}}
    <img src="data:image/png;base64,iVBORw0KGgo..." alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
{{/if}}
```

#### 手动字段名称

所有其他字段名称均被视为手动填充的字段。

要创建可编辑的节，请在节名称两侧添加双括号：

```handlebars
{{customVariable}}
```

### 区域或组

_节_&#x200B;通知GenStudio for Performance Marketing此节中的字段需要高度一致性。 建立这种关系有助于AI生成与部分中的创意元素匹配的内容。

在字段名称中使用您选择的前缀来指示字段是部分或组的一部分。 在下划线(`_`)之后使用字段名称（`headline`、`body`、`image`或`cta`）。 例如，以下标题和正文属于`pod1`部分：

- `pod1_headline`
- `pod1_body`

每个部分只能使用每种字段类型中的一种。 在上述示例中，`pod1`节只能使用一个`pod1_headline`字段。 由于此规则，无法嵌套这些部分。

每种模板类型（如电子邮件或元广告）都包含特定于渠道的部分使用限制。 请参阅&#x200B;_使用模板的最佳实践_&#x200B;主题中的[特定于渠道的指南](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/content/templates/best-practices-for-templates#follow-channel-specific-template-guidelines)。

例如，电子邮件模板最多可包含三个部分；因此，您可以包含三个标题部分和正文部分：

- `pre-header`
- `pod1_headline`
- `pod1_body`
- `pod2_headline`
- `pod2_body`
- `pod3_headline`
- `pod3_body`
- `cta`

GenStudio for Performance Marketing了解`pod1_headline`与`pod1_body`的关系比`pod2_body`更密切。

请参阅[结构化提示](/help/user-guide/effective-prompts.md#structured-prompts)，了解如何制作一个提示，为电子邮件中的每个部分生成不同的内容。

## 模板预览

当您[上载模板](use-templates.md#upload-a-template)时，GenStudio for Performance Marketing会扫描HTML文件以查找可识别的字段。 使用该预览查看您的[模板元素](use-templates.md#template-elements)，并确认您使用[可识别的字段名称](#recognized-field-names)正确识别了这些元素。

电子邮件模板的示例预览：

![检测到预览字段](/help/assets/template-detected-fields.png){width="650"}

### 控件预览

您可以使用内置帮助程序（执行特定操作的[!DNL Handlebars]模板语言中的特殊表达式）控制特殊内容的可见性。 例如，您可以添加一个条件语句，该语句可在保持预览链接干净的同时，将跟踪参数添加到导出模板中的链接。

在呈现模板时设置`_genStudio.browser`值，在导出模板时设置`genStudio.export`值。 例如，当模板用于导出时，您可以决定在电子邮件顶部使用条件包装器包含某些内容：

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

另一个示例可能是为了防止在GenStudio for Performance Marketing中预览模板时使用跟踪代码。 以下示例说明如何在保持预览链接整洁的同时向导出的模板中的链接添加跟踪参数：

```handlebars
<a class="button" {{#if _genStudio.browser }}
   href="{{ link }}"{{/if}}{{#if _genStudio.export }}
   href="{{ link }}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{ cta }}</a>
```

## 静态内容

电子邮件和元模板通常链接到托管在GenStudio for Performance Marketing外部的图像和CSS文件。 当GenStudio for Performance Marketing为这些模板或从中派生的体验生成缩略图时，如果外部资源没有正确的跨源资源共享(CORS)标头，则可能会忽略这些外部资源。

要确保这些资源在缩略图生成过程中可用，请考虑两个选项：

1. **使用CORS标头**：主机服务器必须发送响应，其中生产环境的`Access-Control-Allow-Origin`标头设置为`https://experience.adobe.com`值。 此方法允许GenStudio for Performance Marketing访问并包含资源。

1. **使用数据URL**：使用数据URL将外部资源直接嵌入模板。 此方法绕过CORS限制，并确保资源在生成缩略图期间可用。

>[!TIP]
>
>使用[refresh](/help/user-guide/content/use-templates.md#refresh-template)用最新的静态内容更新模板预览。

## 模板示例

+++示例：带一个部分的电子邮件模板

以下是包含一节的电子邮件的HTML模板的基本示例。 标头包含用于样式设置的简单内联CSS。 正文包含`pre-header`、`headline`和`image` [占位符](#content-placeholders)，供GenStudio for Performance Marketing在电子邮件生成过程中用于插入内容。

```handlebars {line-numbers="true" highlight="13"}
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
        <p><img alt="{{ headline }}"
                src="{{ image }}"
                width="600" height="600"
                border="0"/></p>
        <p>{{ body }}</p>
    </div>
</body>
</html>
```

+++

+++示例：具有多个部分的电子邮件模板

以下是上述示例中的相同HTML模板，但添加了两个部分。 标头包含用于设置组样式的内联CSS。 正文使用两个组，其中[个内容占位符](#content-placeholders)使用前缀。

```handlebars {line-numbers="true" highlight="33"}
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
        <p><img alt="{{ headline }}"
                src="{{ image }}"
                width="600" height="600"
                border="0"/></p>
        <p>{{ body }}</p>
    <!-- Pod1 -->
        <div class="pod">
            <h2>{{ pod1_header }}</h2>
            <p>{{ pod1_body }}</p>
        </div>
        <!-- End of Pod1 -->
    <!-- Pod2 -->
        <div class="pod">
            <h2>{{ pod2_header }}</h2>
            <p>{{ pod2_body }}</p>
        </div>
        <!-- End of Pod2 -->
    </div>
</body>
</html>
```

+++

+++示例：元广告模板

以下是元广告模板的基本示例。 标头包含用于样式化的内联CSS。 正文使用带有前缀的[内容占位符](#content-placeholders)。

```handlebars {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Adobe</title>
    <style>
        .ad-container {
            width: 300px;
            border: 1px solid #ddd;
            padding: 16px;
            font-family: Arial, sans-serif;
        }
        .ad-image {
            width: 100%;
            height: auto;
        }
        .ad-headline {
            font-size: 18px;
            font-weight: bold;
            margin: 12px 0;
        }
        .ad-body {
            font-size: 14px;
            margin: 12px 0;
        }
        .ad-cta {
            display: inline-block;
            padding: 10px 20px;
            background-color: #007bff;
            color: #fff;
            text-decoration: none;
            border-radius: 4px;
            text-align: center;
        }
    </style>
</head>
<body>
<div class="ad-container">
    <img src="{{ image }}" alt="Ad Image" class="ad-image">
    <div class="ad-headline">"{{ headline }}"</div>
    <div class="ad-body">"{{ body }}"</div>
    <a href="(https://example.com)" class="ad-cta">"{{ CTA }}"</a>
</div>
</body>
</html>
```

+++
