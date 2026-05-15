---
title: 模板的最佳实践
description: 将模板与Adobe GenStudio for Performance Marketing结合使用时，请遵循最佳实践。
level: Intermediate
role: Developer, User
feature: Media Templates, Content Generation, Brand Personalization
exl-id: 3ff24fec-e836-4202-80f8-ba165e173b75
TQID: https://experienceleague.adobe.com/fiKHSZ-YFZ2gSD5iZ-aKaZtsC49Mrj1dqHpHqtbXZVM
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: cc72dcf1-72e1-48cc-b434-e7c27d62d67c
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 3322f783cd49ddcb897942e5e91590d53b554bdd
workflow-type: tm+mt
source-wordcount: 1347
ht-degree: 0%

---

# 使用模板的最佳实践

模板提供了一个包括预配置布局和设计元素的起点，可显着减少生成新内容所需的时间和精力。

在GenStudio for Performance Marketing中使用模板时，请遵循以下建议：

1. 了解[模板元素](#know-about-template-elements)
1. 配置[渠道准则](#configure-channel-guidelines)以便有效地个性化内容
1. 使用[辅助功能标准](accessibility-for-templates.md)进行设计以获得最佳体验
1. 遵循[特定于渠道的模板准则](#follow-channel-specific-template-guidelines)
1. 使用[Express模板](/help/user-guide/templates/express-templates.md)时，请考虑[Express to GenStudio模板最佳实践](#express-to-genstudio-template-best-practices)下的特定提示。
&#x200B;>>
了解[使用模板](use-templates.md)中模板元素和过程的基础知识。 深入了解[自定义模板](customize-template.md)以了解具体说明，以便在下一个营销活动中使用。

## 使用正确的模板元素

每种模板类型使用不同的元素来为特定于渠道的内容创建创建结构。 [熟悉模板的各个部分](use-templates.md#template-elements)并包含最适合您的内容和模板类型的元素。

在自定义模板时，请使用字段名称来代替您需要GenStudio for Performance Marketing生成内容的这些元素。

查看[模板元素](use-templates.md#template-elements)。

## 在模板中使用占位符文本

占位符文本有助于定义用户以后在模板中填充内容的语法或结构。 例如，{first_name}.{last_name}@email.等，用于定义电子邮件地址。 但是，一些常见分隔符已为GenStudio for Performance Marketing中的其他含义而保留：

❌ `< >` — 正在用于HTML标记。
❌ `{{ }}` — 用于Handlebar表达式。

使用单括号（直括号或大括号）表示占位符文本，以避免与现有标记混淆。

✅ `{first_name}` — 名字的占位符。

## 配置渠道准则

定义明确的渠道准则对于确保生成的内容与品牌的要求和目标保持一致至关重要。 渠道准则允许您为模板中使用的元素（如色调、长度和样式）指定规则。 例如，您可以为正文设置最大字符数或要求使用特定的call-to-action样式。 通过提前设置这些准则，您无需在每个AI提示中写出详细说明，从而简化内容生成过程并确保电子邮件的一致性。

查看并定义模板中所有关键字段的品牌的[渠道准则](/help/user-guide/guidelines/brands.md#channel-guidelines)。 如果您未定义准则，则应用[默认渠道准则](/help/user-guide/guidelines/brands.md#default-channel-guidelines)，这可能不能完全反映您的品牌要求。

![正文规范](/help/assets/channel-email-body.png)

了解[品牌、产品和角色准则](/help/user-guide/guidelines/overview.md)如何影响生成的内容，以及如何根据您的营销目标定制内容。

## 上传模板图像

模板中使用的图像应来自内容存储库，并且需要正确上传以确保图像准确显示。

当模板具有边缘到边缘（全出血）图像时，所选图像会自动调整大小以适合完整的模板尺寸。 但是，如果图像与模板长宽比不匹配，则会裁剪图像以适合模板尺寸，并且可能无法按预期显示。

模板中包含的图像没有“自动调整”功能。

要解决图像裁剪问题，用户必须定义在模板中将图像上传到内容存储库时要使用的图像的宽高比。 上传已批准的模板时：

1. [继续模板上载过程](/help/user-guide/templates/use-templates.md#add-a-template)，直到到达&#x200B;**[!UICONTROL 添加详细信息]**&#x200B;页面。

2. 以&#x200B;**[!UICONTROL 广告宽度(px)]**&#x200B;和&#x200B;**[!UICONTROL 广告高度(px)]**&#x200B;定义要在模板中使用的图像的宽高比。 这将为显示图像的模板部分定义图像窗口。

3. 在&#x200B;**[!UICONTROL 更多详细信息]**&#x200B;部分中，选择&#x200B;**[!UICONTROL 图像大小]**&#x200B;下拉列表，然后选择&#x200B;_裁切为固定大小_。
   ![裁切为固定大小](images/crop-to-fixed-size.png "裁切为固定大小"){width="80%"}

要在浏览器中确定图像的大小和纵横比，请执行以下操作：

1. 检查图像。
   - 在Windows/Linux上：
      - 按F12。
   - 在macOS上：
      - 按Command + Option + I。

1. 将鼠标悬停在图像上。

1. 请注意纵横比。 使用此参数定义模板中图像的纵横比。

如果上传期间未应用这些详细信息，则假定图像是模板的整个纵横比，并且与该纵横比不完全匹配的图像将显示为已裁剪。

![在显示广告中裁切的图像](images/cropped-display.png "图像裁切"){width="60%"}

显示广告模板中的&#x200B;**❌裁剪的图像**

![显示在显示广告中的图像](images/full-fit.png "显示在显示广告中的图像"){width="60%"}

**✅图像已完全显示**

## 遵循特定于渠道的模板准则

在创建模板时，请确保它们满足预期渠道的特定要求。 构建适应每个渠道的布局和视觉要求的模板。 有一些常规准则适用于任何模板，例如：

- 使用简洁且响应式的HTML和内联CSS
- 使用Adobe或Google字体
- **不**&#x200B;使用JavaScript

{{note-css-effects}}

在使用每种模板类型时查看更多提示和限制以确保最佳性能：

- [电子邮件](/help/user-guide/templates/email-template.md)
- [显示广告和横幅广告](/help/user-guide/templates/display-template.md)
- [LinkedIn](/help/user-guide/templates/linkedin-template.md)
- [Meta广告](/help/user-guide/templates/meta-template.md)

## 快速转到GenStudio模板最佳实践

在将设计从[!DNL Adobe Express]转换为[!DNL GenStudio for Performance Marketing]的模板时，以下提示可帮助您获得可靠的结果。

### 使用多变体模板

在[!DNL Adobe Express]中，页面可以在一个模板文件中表示多个大小或长宽比变化。
当您在[!DNL GenStudio for Performance Marketing]中选择模板时，所有变体都会显示在画布中。

此行为可改进HTML模板，这些模板仅支持每个文件一个变体。

### 锁定字段以控制营销人员可以编辑的内容

使用锁定来传达意图。 例如，锁定法律免责声明，使其从不由人工智能生成，但为一代人保留灵活的标题。

右键单击[!DNL Adobe Express]中的任何元素以设置锁定行为：

- **[!UICONTROL 完全锁定]** — 元素是静态的，AI不会为其生成内容。
- **[!UICONTROL 锁定，允许图像替换]** — 锁定大小和位置，但允许用户交换图像。 此选项非常适用于徽标。
- **[!UICONTROL 锁定，允许替换文本]** — 锁定大小和位置，但允许用户编辑文本。 AI不会自动为其生成内容。
- **完全灵活** （已解锁） — 用户可以移动元素并调整其大小，AI会将其视为要生成的内容。

### 命名图层以实现更好的AI映射

将设计转换为模板时，AI会扫描设计并映射标题、CTA和正文等字段。 与高度复杂的版面相比，AI更准确地映射简单模板。

**最佳实践：**&#x200B;在占位符副本中，包含所需的字段类型（例如，`headline`、`sub-headline`或`CTA`）以帮助AI映射字段正确无误。 此方法可减少映射错误。

### 转换为模板

1. 在[!DNL Adobe Express]中，单击&#x200B;**[!UICONTROL 共享]** > **[!UICONTROL 转换为模板]**。
1. 只有&#x200B;**[!UICONTROL 信息]**&#x200B;选项卡和&#x200B;**[!UICONTROL 锁定]**&#x200B;选项卡会转移到[!DNL GenStudio for Performance Marketing]。
1. 在转换时，选择解锁的工作方式：
   - **[!UICONTROL 允许用户解锁]**
   - **[!UICONTROL 阻止所有解锁]**
   - **[!UICONTROL 设置密码短语]** — 中间立场，不鼓励随意更改而不永久阻止访问。

### 保留原始设计文件的副本

转换会创建一个单独的[!DNL Adobe Express]模板文件，但原始设计文件仍可编辑。

**提示：**&#x200B;保留原始模板，以便以后修改设计、创建变体并生成新模板。

### 共享以提高可见性

转换后，默认情况下仅对您可见。 您可以将其与个人或整个组织共享。

**要求：** [!DNL Adobe Express]和[!DNL GenStudio for Performance Marketing]必须使用相同的IMS组织才能同步模板。 模板通常在转换后几乎立即出现在[!DNL GenStudio for Performance Marketing]中。

### 控制AI字段映射

选择模板后，AI为每个模板映射一次字段，分配标签，如&#x200B;**[!UICONTROL 主媒体]**、**[!UICONTROL 生成的]**&#x200B;或&#x200B;**[!UICONTROL 已锁定]**。 当AI错误地分配字段时，您可以手动调整映射。

使用&#x200B;**[!UICONTROL 为每个字段启用生成]**&#x200B;切换开关在生成之前打开或关闭。 当AI错误地分配字段时，您可以手动调整映射。 计划在未来版本中永久更正模板映射。

### 在[!DNL Adobe Express]中进行设计，在[!DNL GenStudio for Performance Marketing]中进行组装

请考虑这些设计工作流，以充分利用每项服务：

- 在[!DNL Adobe Express]中完成设计工作，例如颜色、布局和图形。
- 使用[!DNL GenStudio for Performance Marketing]从这些模板汇编和生成内容。
- 使用[!DNL Adobe Express]品牌（颜色、徽标、字体和图形）进行设计管理。
- 使用[!DNL GenStudio for Performance Marketing]品牌在生成后更改字体颜色。

### 电子邮件限制

在[!DNL Adobe Express]模板工作流的Horizon画布上，**不支持**&#x200B;电子邮件。 电子邮件会继续使用传统的HTML模板过程。

### 利用自定义字体

团队经常询问自定义字体如何与[!DNL Adobe Express]模板一起使用。 管理员可能需要在Admin Console中接受自定义字体资格鉴定选件，这些字体才可用；请参阅[使用 [!DNL Adobe Express] 模板](express-templates.md)。
