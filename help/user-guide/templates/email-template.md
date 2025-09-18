---
title: 电子邮件模板准则
description: 将电子邮件模板与Adobe GenStudio for Performance Marketing结合使用时，请遵循最佳实践。
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 8b1e8d32-5a23-45ce-a2d4-ae6de3698c45
source-git-commit: 49d8d5daa2f3c93c18cd9132dab5207871b51237
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 0%

---

# 电子邮件模板准则

营销电子邮件模板用作吸引视力和响应式电子邮件营销活动的基础。 通常，通过HTML模板，您可以根据品牌准则控制布局、排版规则、颜色和图像。 在准备要在GenStudio for Performance Marketing中使用的模板时，请使用语义HTML和内联CSS进行样式设置，并避免使用脚本或外部依赖项。 结构良好的HTML模板可以增强收件人的体验并提高可投放性和参与率。

在自定义电子邮件模板以用于GenStudio for Performance Marketing时，请遵循以下设计最佳实践：

- 使用Adobe或Google字体
- 使用简洁且响应式的HTML和内联CSS
- **不**&#x200B;使用JavaScript
- 请&#x200B;**不**&#x200B;在正文或容器中使用固定宽度
- 请&#x200B;**不**&#x200B;对图像使用base64编码，因为它会显着增加模板大小
- HTML文件最大大小为102 KB

## 可识别的字段名称

在自定义电子邮件模板时，请使用内容占位符来填写以下必填字段：

- `headline`
- `sub_headline`
- `body`
- `cta`
- `image` (从Content JPEG、PNG或GIF中选择)

GenStudio for Performance Marketing会自动生成以下字段。 未启用富文本。 您不必为以下内容应用内容占位符：

- `pre_header`
- `subject`

模板中允许的最大字段数为20。 请参阅[内容占位符](/help/user-guide/content/customize-template.md#content-placeholders)以了解有关在模板中使用字段名的更多信息。

## 多节电子邮件

_节_&#x200B;允许您将内容组织为不同的组，从而支持更复杂的布局。 在GenStudio for Performance Marketing中，您可以使用组命名约定定义每个部分。 请参阅[自定义模板节](/help/user-guide/content/customize-template.md#sections-or-groups)。

多节模板可以包含0、2或3节：

- 基本模板（零部分）可以生成一组不需要组命名约定的模板元素。
- 一个复杂的模板（多个部分）最多可以生成三组模板元素，这需要您遵守组命名约定： `<groupname_fieldname>`。
- 使用多个部分时，不会填充在部分之外任何保持独立的元素。

以下是两个部分中使用组命名约定的字段名称示例：

- 在第1部分：`pod1_headline`，`pod1_body`，`pod1_cta`
- 在第2部分中：`pod2_headline`，`pod2_body`，`pod2_cta`

## 模板示例

+++示例：电子邮件模板包含一个部分

以下是具有一个部分的HTML电子邮件模板的基本示例。 `<head>`包含用于样式设置的简单内联CSS，`<body>`使用内容占位符（如`pre_header`、`headline`、`sub_headline`、`body`、`cta`和`image`）以及链接和。 这些占位符允许GenStudio for Performance Marketing在电子邮件生成期间插入动态内容。

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Marketing Email</title>
        <style>
            .container {
                width: 100%;
                padding: 20px;
                font-family: Arial, sans-serif;
            }
            .cta-button {
                display: inline-block;
                background-color: #fff;
                color: #000;
                border: 2px solid #000;
                padding: 10px 20px;
                text-decoration: none;
                font-family: 'Source Sans Pro', Arial, sans-serif;
                font-weight: 600;
                font-size: 14px;
                margin-top: 20px;
                text-align: center;
            }
        </style>
    </head>
    <body>
        <div class="container">
            {{pre_header}}
            <h1>{{headline}}</h1>
            <p>
                <a href="{{link}}">
                    <img alt="banner headline" src="{{image}}" width="600" height="600">
                </a>
            </p>
            <h2>{{sub_headline}}</h2>
            <p>{{body}}</p>
            <a href="#" class="cta-button">{{cta}}</a>
        </div>
    </body>
</html>
```

+++

+++示例：具有多个分区的电子邮件模板

以下是上述示例中的相同HTML模板，但添加了另外两个部分。 标头包含用于设置组样式的内联CSS。 正文使用两个组，其中[个内容占位符](#content-placeholders)使用前缀。

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
            .cta-button {
            display: inline-block;
            background-color: #fff; /* Background color to white */
            color: #000; /* Text color to black */
            border: 2px solid #000; /* Border color to black */
            padding: 10px 20px;
            text-decoration: none;            
            font-family: 'Source Sans Pro', Arial, sans-serif;
            font-weight: 600; /* Semibold */
            font-size: 14px;
            margin-top: 20px;
            text-align: center;
            }
        </style>
    </head>
    <body>{{pre_header}}
        <div class="container">
            <!-- Pod1 -->
            <div class="pod">
                <h2>{{pod1_headline}}</h2>
                <p><img alt="pic1" src="{{pod1_image}}" width="200" height="200" border="0"></p>
                <p>{{pod1_body}}</p>
            </div>
            <!-- End of Pod1 -->
            <!-- Pod2 -->
            <div class="pod">
                <h2>{{pod2_headline}}</h2>
                <p><img alt="pic2" src="{{pod2_image}}" width="200" height="200" border="0"></p>
                <p>{{pod2_body}}</p>
            </div>
            <!-- End of Pod2 -->
            <a href="#" class="cta-button">{{cta}}</a>
        </div>
    </body>
</html>
```

+++
