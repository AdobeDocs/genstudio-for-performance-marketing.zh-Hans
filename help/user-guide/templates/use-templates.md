---
title: 使用模板
description: 了解如何在Adobe GenStudio for Performance Marketing中有效地使用模板来简化您的创作过程。
level: Intermediate
role: Developer
feature: Media Templates
exl-id: 7705bb79-19ca-4c16-8f8b-95bf8687e96d
source-git-commit: a18b4f89ffde43432885dc2c2e323eaf19361fc7
workflow-type: tm+mt
source-wordcount: '1366'
ht-degree: 1%

---

# 使用模板

GenStudio for Performance Marketing使内容创建者能够使用&#x200B;_模板_&#x200B;快速生成一致的品牌营销内容。 模板通过提供包括预配置布局和设计元素的起点，显着减少了生成新内容所需的时间和精力。 若要开始，请在[!DNL Content]中上传自定义模板，或在[!DNL Create]中使用起始模板。 [入门模板](/help/user-guide/templates/starter-templates.md)提供了从标准设计开始的快速方法，而自定义模板允许您使用独特的设计和布局。

虽然GenStudio for Performance Marketing不支持在应用程序中直接创建模板，但您可以使用流行的设计工具(如Adobe InDesign、Illustrator或Express)轻松设计和准备模板。 设计完成后，您可以对其进行调整以用于GenStudio for Performance Marketing。 可按照以下步骤开始使用模板：

1. **设计模板**：使用首选设计工具创建[模板的可视布局，该模板包含元素](#template-elements)，例如页眉、标题、正文、CTA、图像和页脚。

2. **对您的模板进行编码**：将您的设计转换为HTML和内联CSS，以确保它在各种设备上均干净且响应迅速。 请考虑[辅助功能准则](accessibility-for-templates.md)，以帮助实现您的最大目标受众。

3. **准备GenStudio for Performance Marketing**：使用Handlebars模板语言调整HTML模板。 插入占位符以指示GenStudio for Performance Marketing应在何处动态生成内容。 了解如何[自定义GenStudio for Performance Marketing的模板](customize-template.md)。

通过执行以下步骤，您可以创建专业且有效的模板，以便在GenStudio for Performance Marketing中使用，使您能够快速高效地制作品牌内内容。

## 模板元素

模板是使用HTML和内联CSS定义的一组指令，可用于生成电子邮件、社交广告或显示广告体验。 模板元素为内容创建提供了结构。

以下是在模板中使用的元素列表，以及有关其特征的一些详细信息：

| **元素** | **频道** | **描述** |
|----------------------|------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **预编译标头** | 电子邮件 | 电子邮件中的次要主题行，通常为40-50个字符，用于增强主主题行。 在打开电子邮件之前，它显示在收件箱中主题旁边。 |
| **页眉** | 电子邮件 | 收件人打开电子邮件时看到的电子邮件顶部设置了提示音并为包含的内容提供了上下文。 |
| **标题** | Meta广告、横幅和显示广告、LinkedIn | 收件人看到的第一个内容应具有吸引人的吸引力。 |
| **副标题** | 电子邮件、横幅和显示广告 | 支持标题的次要文本元素。 它通常简洁，旨在补充主标题，进一步吸引读者关注内容。 |
| **介绍性文本** | LinkedIn | 主消息传送核心消息，类似于正文副本。 它最多可包含150个字符，包括空格、最多四个表情符号和标点。 |
| **正文** | 电子邮件、Meta广告、横幅和显示广告 | 广告的主文本传达核心消息。 它应具有吸引力、信息性和说服力，以鼓励受众采取所需的行动。 |
| **行动号召 (CTA)** | 电子邮件、Meta广告、横幅和显示广告、LinkedIn | call-to-action按钮使用短语和链接来鼓励收件人采取特定操作，例如单击链接或进行购买。 |
| **图像** | 电子邮件、Meta广告、横幅和显示广告、LinkedIn | 增强视觉吸引力，分解文本并支持消息。 图像应高品质且抢眼。 |
| **页脚** | 电子邮件 | 电子邮件的底部包含其他内容，如联系详情、社交媒体链接、免责声明和取消订阅选项。 |
| **文本叠加** | Meta广告 | 放置在图像上的文本，用于支持和增强标题和正文内容。 |

>[!TIP]
>
>查看GenStudio for Performance Marketing支持的用于每种渠道类型模板的[可识别的字段名称](customize-template.md#recognized-field-names)。

## 自定义模板

您[通过插入生成AI用于插入内容的内容占位符或字段自定义模板](customize-template.md)以便在GenStudio for Performance Marketing中使用。 GenStudio for Performance Marketing可识别某些字段，如`body`字段，并遵守为所选品牌配置的渠道准则。

>[!TIP]
>
>遵循[辅助功能准则](accessibility-for-templates.md)和[最佳实践](/help/user-guide/templates/best-practices-for-templates.md)，以便您可以接触到更多受众并提供最佳体验。

## 管理模板

_[!DNL Templates]_&#x200B;图库会显示您为在GenStudio for Performance Marketing中生成体验而自定义的模板清单。

### 搜索模板

每个[!DNL Content]视图都提供筛选选项，以缩小搜索范围，从而缩小搜索范围，以找到理想的资产、体验或模板。 存在基于[准则](/help/user-guide/guidelines/overview.md)、[关键字](../content/asset-details.md#user-defined-metadata)和[属性类别](/help/user-guide/insights/attributes.md#categories)的筛选器以缩小搜索结果范围。

例如，您可能希望查找由您创建的特定渠道类型或纵横比的模板：

- **[!UICONTROL 创建者]**：限制&#x200B;_[!UICONTROL 模板]_&#x200B;列表仅显示您或特定人员创建的模板。
- **[!UICONTROL 宽高比]**：限制&#x200B;_[!UICONTROL 模板]_&#x200B;列表以显示针对特定宽高比设计的模板。

下面显示了按渠道类型(如电子邮件、展示广告、Meta广告和LinkedIn广告)过滤的内容。

![内容模板列表](/help/assets/content-templates-filter.png "搜索LinkedIn模板"){width="650"}

在为自有或付费媒体选择模板时，模板搜索功能在[!UICONTROL 创建]期间可用。 如果某些过滤器选项不可见，则表示存储库中没有符合相应元数据条件的模板。 确保使用元数据正确标记模板，以使这些模板可通过这些过滤器发现。

### 添加模板

在上传模板之前，请按照[自定义模板](customize-template.md)中的指导，确保模板已完全准备好，可以在GenStudio for Performance Marketing中使用。

**添加模板**：

1. 在&#x200B;_[!DNL Content]_&#x200B;中，选择&#x200B;**[!UICONTROL 模板]**&#x200B;部分。

2. 单击&#x200B;**[!UICONTROL 添加模板]**。

3. 在&#x200B;_[!UICONTROL 添加批准的模板]_&#x200B;窗格中，浏览HTML模板文件或将HTML模板文件拖放到放置空间。 单击&#x200B;**[!UICONTROL 下一步]**。

4. 在&#x200B;_[!UICONTROL 检查检测到的字段]_&#x200B;窗格中，查看这些字段。 验证您使用的模板是否正确，以及所有详细信息是否均按预期显示。

   电子邮件模板的示例预览：

   ![检测到预览字段](/help/assets/template-detected-fields.png){width="650"}

   >[!TIP]
   >
   >如果模板不正确，请单击“上一步”**&#x200B;**&#x200B;并返回上一步。 上载更正后的模板文件。 或者使用[模板代码编辑器](/help/user-guide/templates/code-editor.md)进行简单的更正。

5. 对模板预览感到满意时，请单击&#x200B;**[!UICONTROL 下一步]**。

6. 在&#x200B;_[!UICONTROL 提供模板详细信息并上传]_&#x200B;中，命名您的模板并选择&#x200B;**[!UICONTROL 渠道]**&#x200B;类型。

   模板名称和渠道类型为必填项。 其他要求可能包括：

   - **Meta**：需要宽高比
   - **横幅和显示广告**：需要维度

7. 添加尽可能多的详细信息，以改进搜索和筛选中的模板识别。

8. 单击&#x200B;**[!UICONTROL 完成]**。

### 刷新模板

模板可能包括静态文件，如图标或徽标。 创建模板预览后未存储[静态内容](/help/user-guide/templates/customize-template.md#static-content)。 GenStudio for Performance Marketing将继续引用模板中提供的源链接。 使用刷新可更新模板预览，以显示这些资源的最新版本。

**刷新模板**：

1. 在&#x200B;_[!DNL Content]_&#x200B;中，选择&#x200B;**[!UICONTROL 模板]**&#x200B;部分。

2. 单击模板可查看完整视图和详细信息列表。

3. 单击右上角的&#x200B;**[!UICONTROL 刷新]**（循环箭头）以刷新模板中使用的所有资源。

### 使用模板创建体验

在GenStudio for Performance Marketing中查找并使用现有模板来创建更多体验。

**要使用模板创建体验**：

1. 在&#x200B;_[!DNL Content]_&#x200B;中，选择&#x200B;**[!UICONTROL 模板]**&#x200B;部分。

2. 单击模板可查看完整视图和详细信息列表。

3. 单击右上角的&#x200B;**[!UICONTROL 创建体验]** （画笔）以使用该模板。

4. 继续[创建](/help/user-guide/create/overview.md#create-use-cases)体验。

## AJO和Marketo中的模板

您可以上传在Adobe Journey Optimizer (AJO)或Marketo中创建的模板。 GenStudio for Performance Marketing会检测特定于应用程序的模式并忽略它们，从而保留原始表单以供在AJO或Marketo中继续使用。 您无需对原始AJO或Marketo语法进行任何更改。

可识别的应用模式包括：

- **AJO**： `{{profile.*}}`，`{{context.*}}`
- **Marketo**： `{{my.*}}`，`{{lead.*}}`，`{{system.*}}`

>[!BEGINSHADEBOX]

**先决条件**

- 应用程序(AJO、Marketo)和GenStudio for Performance Marketing必须属于同一个IMS组织才能进行集成
- 用户必须具有“协作者”角色（最低级别）或更高版本

>[!ENDSHADEBOX]

接下来，[使用占位符自定义您的模板](/help/user-guide/templates/customize-template.md)，以指示GenStudio for Performance Marketing应在何处为您生成内容。 [将模板](#add-a-template)添加到[!DNL Content]存储库并验证模板。 使用代码编辑器进行任何较小的更正。
