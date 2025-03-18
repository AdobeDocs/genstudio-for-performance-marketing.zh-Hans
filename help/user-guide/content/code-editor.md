---
title: 模板代码编辑器
description: 了解如何在GenStudio for Performance Marketing中使用模板代码编辑器。
level: Intermediate
feature: Media Templates, Content Generation
exl-id: b46fc7a9-88c1-474a-9d7b-1df7740d8f5a
source-git-commit: 19d0b8b929e293179a091cc7b5a6a1268b0abbbd
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 0%

---

# 模板代码编辑器

模板代码编辑器旨在帮助您验证和优化模板，以便在使用GenStudio for Performance Marketing生成新体验时实现最佳使用。 该编辑器支持Handlebars语法，该语法使用模板中的占位符来指示GenStudio for Performance Marketing应在何处为您生成内容。

>[!TIP]
>
>在[!DNL Content] _模板_&#x200B;视图中上传模板HTML代码之前，请通过插入[自定义模板](customize-template.md)指南中定义的内容占位符来准备模板。

## 检查检测到的字段

_[!UICONTROL 检查检测到的字段]_&#x200B;窗格显示GenStudio for Performance Marketing可在您的模板中识别的字段列表。 查看列表，然后您可以滚动HTML代码以查看模板的结构。

![代码编辑器视图](/help/assets/template-detected-fields.png "检查检测到的字段"){width="600" zoomable="yes"}

如果您发现列表中缺少字段，请搜索模板代码并找到缺失字段的位置。 使用Handlebars语法和[可识别的字段名](/help/user-guide/content/customize-template.md#recognized-field-names)插入正确的占位符。 使用代码编辑器底部显示的“查找和替换”表单来搜索代码中的特定字符串。 (Windows `CTRL`+`F`或macOS `CMD`+`F`)

### 进行更正

如果您的模板中存在错误，您可能会看到一则`Template is invalid`消息，其中包含问题的简短说明。 在以下示例中，消息指示`_image`字段不符合多面板模板中建立的字段命名约定。 该消息进一步建议您需要使用正确的前缀更新字段名称。 在模板代码编辑器中查找`_image`字段，并按照建议更新名称。

![更正无效模板](/help/assets/animation/template-code-editor.gif){width="600" zoomable="yes"}

_[!UICONTROL 检查检测到的字段]_&#x200B;窗格更新以反映您所做的更改。 在您满意这些字段正确且填写完毕后，请单击&#x200B;**[!UICONTROL 下一步]**&#x200B;继续[上载模板](/help/user-guide/content/use-templates.md#add-a-template)。
