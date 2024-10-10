---
title: 使用模板
description: 了解如何在Adobe GenStudio for Performance Marketing中有效地使用模板来简化您的创作过程。
feature: Templates, Content
exl-id: 7705bb79-19ca-4c16-8f8b-95bf8687e96d
source-git-commit: 3a361134a0b56a2973399e38e62f4ab345a3dbc8
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 1%

---

# 使用模板

GenStudio for Performance Marketing使内容创建者能够使用&#x200B;_模板_&#x200B;快速生成一致的品牌营销内容。 模板通过提供包括预配置布局和设计元素的起点，显着减少了生成新内容所需的时间和精力。

## 模板元素

模板是使用HTML和内联CSS定义的一组指令，可用于生成电子邮件或元广告体验。

以下是在模板中使用的元素列表，以及有关其特征的一些详细信息。

- **预编译标头**

   - 用作电子邮件中的辅助主题行，增强主主题行
   - 40-50个字符
   - 在打开电子邮件之前，显示在收件箱中主题旁边
   - 在电子邮件模板中使用

- **页眉**

   - 收件人打开电子邮件时看到的电子邮件顶部部分
   - 设置音调并为包含的内容提供上下文
   - 在电子邮件模板中使用

- **标题**

   - 收件人看到的第一个内容
   - 应该具有吸引人的吸引力
   - 在元广告模板中使用

- **正文**

   - 传送主要消息的主要内容区域
   - 能够包括文本、图像和其他媒体
   - 在电子邮件和元广告模板中使用

- **CTA（行动号召）**

   - 鼓励收件人采取特定操作，例如单击链接或进行购买
   - 在电子邮件和元广告模板中使用

- **图像**

   - 增强视觉吸引力
   - 拆分文本
   - 支持此消息
   - 应该高品质、抢眼
   - 在电子邮件和元广告模板中使用

- **页脚**

   - 底部包含其他内容，如联系详情、社交媒体链接、免责声明和取消订阅选项
   - 在电子邮件模板中使用

- **文本叠加**

   - 图像上的文本
   - 用于支持和增强标题和正文
   - 在元广告模板中使用

>[!TIP]
>
>查看GenStudio for Performance Marketing支持的用于每种渠道类型模板的[可识别的字段名称](customize-template.md#recognized-field-names)。

## 配置渠道准则

在GenStudio for Performance Marketing中使用模板之前，最佳实践是为每个品牌配置[渠道准则](../guidelines/brands.md#channel-guidelines)。 渠道指南直接影响使用模板时生成的内容类型。 例如，您可以对电子邮件正文设置字符限制。

![正文规范](/help/assets/channel-email-body.png)

## 自定义模板

您[通过插入生成AI用于插入内容的内容占位符或字段自定义模板](customize-template.md)以便在GenStudio for Performance Marketing中使用。 GenStudio for Performance Marketing可识别某些字段，如`body`字段，并遵守为所选品牌配置的渠道准则。

>[!TIP]
>
>遵循有关生成模板的[辅助功能准则](accessibility-for-templates.md)，以便您可以接触到更多受众并提供最佳体验。

## 上传模板

在为GenStudio for Performance Marketing准备模板时，使用[自定义模板](customize-template.md)作为指南。 有关为所有受众提供更好的体验的指导，请参阅模板[无障碍准则](accessibility-for-templates.md)。

**添加模板**：

1. 在&#x200B;_[!DNL Content]_中，选择&#x200B;**[!UICONTROL 模板]**部分。

1. 单击&#x200B;**[!UICONTROL 添加模板]**。

1. 在&#x200B;_[!UICONTROL 添加您批准的模板]_&#x200B;窗格中，浏览HTML模板文件或将HTML模板文件拖放到放置空间。 单击&#x200B;**[!UICONTROL 下一步]**。

1. 在&#x200B;_[!UICONTROL 查看发现的字段]_&#x200B;窗格中，查看检测到的字段。 验证您使用的模板是否正确，以及所有详细信息是否均按预期显示。 单击&#x200B;**[!UICONTROL 下一步]**。

   电子邮件模板的示例预览：

   ![检测到预览字段](../../assets/template-detected-fields.png){width="650"}

   >[!TIP]
   >
   >如果模板不正确，请单击“上一步”****&#x200B;并返回上一步。 上载更正后的模板文件。

1. 在&#x200B;_[!UICONTROL 提供模板详细信息和上传]_&#x200B;窗格中，命名您的模板并选择&#x200B;**[!UICONTROL 渠道]**&#x200B;类型。

   模板名称和渠道类型为必填项。 其他要求可能包括：

   - **Meta**：需要宽高比
   <!-- - **Display ads**: requires Dimensions -->

1. 添加尽可能多的详细信息，以改进搜索和筛选中的模板识别。

1. 单击&#x200B;**[!UICONTROL 完成]**。

## 使用模板创建

在GenStudio for Performance Marketing中查找并使用现有模板来创建更多体验。

**要使用模板创建体验**：

1. 在&#x200B;_[!DNL Content]_中，选择&#x200B;**[!UICONTROL 模板]**部分。

   ![内容模板列表](../../assets/content-templates.png){width="650" zoomable="yes"}

1. 选择模板以查看完整视图和详细信息列表。

1. 单击右上角的&#x200B;**[!UICONTROL 创建体验]** （画笔）以使用该模板。

1. 继续[创建](/help/user-guide/create/overview.md)体验。
