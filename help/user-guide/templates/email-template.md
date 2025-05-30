---
title: 电子邮件模板准则
description: 将电子邮件模板与Adobe GenStudio for Performance Marketing结合使用时，请遵循最佳实践。
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 8b1e8d32-5a23-45ce-a2d4-ae6de3698c45
source-git-commit: d9d774f727b69b18af6114965fdb8ffb450f797b
workflow-type: tm+mt
source-wordcount: '406'
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

GenStudio for Performance Marketing会自动为电子邮件生成`subject`字段。 在自定义模板时，请使用内容占位符来填写以下必填字段：

- `pre_header` （未启用RTF文本）
- `headline`
- `sub_headline`
- `body`
- `cta`
- `image` (从Content JPEG、PNG或GIF中选择)

模板中允许的最大字段数为20。 请参阅[内容占位符](/help/user-guide/content/customize-template.md#content-placeholders)以了解有关在模板中使用字段名的更多信息。

## 多节电子邮件

_节_&#x200B;允许您将内容组织到不同的组中，这支持更复杂的布局。 在Genstudio for Performance Marketing中，您可以使用组命名约定定义每个节。 请参阅[自定义模板节](/help/user-guide/content/customize-template.md#sections-or-groups)。

多节模板可以包含0、2或3节：

- 基本模板（零部分）可以生成一组不需要组命名约定的模板元素。
- 一个复杂的模板（多个部分）最多可以生成三组模板元素，这要求您遵循组命名约定： (`groupname_fieldname`)

两个部分的示例字段名称：

- `pod1_headline`，`pod1_body`，`pod1_cta`
- `pod2_headline`, `pod2_body`, `pod2_cta`

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
    <body>{{pre_header}}
        <div class="container">
            <h1>{{headline}}</h1>
            <p><a href="{{link}}">
            <img alt="{{headline}}"
                    src="{{image}}"
                    width="600" height="600"
                    border="0"/></a></p>
            <p>{{body}}</p>
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
    <body>{{pre_header}}
        <div class="container">
            <h1>{{headline}}</h1>
            <p>{{body}}</p>
            <!-- Pod1 -->
            <div class="pod">
                <h2>{{pod1_headline}}</h2>
                <p><img alt="{{ headline }}" src="{{pod1_image}}" width="200" height="200" border="0"></p>
                <p>{{pod1_body}}</p>
            </div>
            <!-- End of Pod1 -->
            <!-- Pod2 -->
            <div class="pod">
                <h2>{{pod2_headline}}</h2>
                <p><img alt="{{headline}}" src="{{pod2_image}}" width="200" height="200" border="0"></p>
                <p>{{pod2_body}}</p>
            </div>
            <!-- End of Pod2 -->
        </div>
    </body>
</html>
```

+++
