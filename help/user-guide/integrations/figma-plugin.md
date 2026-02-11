---
title: 适用于Adobe GenStudio for Performance Marketing的Figma插件
description: 了解如何配置和使用GenStudio for Performance Marketing的Figma插件。
feature: Generative AI
role: User
exl-id: 232fbbc6-c523-4525-8d26-a8ac8d62c035
source-git-commit: c6080555812fa82a7b71eee7e2deb963a881d9f4
workflow-type: tm+mt
source-wordcount: '2124'
ht-degree: 0%

---

# 适用于GenStudio for Performance Marketing的Figma插件

GenStudio for Performance Marketing Figma插件会在Figma应用程序中添加一个新面板，以便您生成品牌内内容。

本页介绍如何配置和使用插件。

此插件的功能包括：

* 将Figma文本元素映射到GenStudio for Performance Marketing字段，如`headline`、`body`、`on_image_text`等。
* 根据品牌、角色、产品和文本提示生成新的Meta、LinkedIn或显示广告[!DNL Experiences]。
* 通过将映射的Figma元素中的文本替换为GenStudio for Performance Marketing生成的值，直接在Figma文档中创建[!DNL Experiences]。
* 根据提示重新短语、缩短、延长或翻译现有内容。
* 将生成的[!DNL Experiences]翻译成多种语言。
* 将生成的[!DNL Experiences]作为平面化图像导出到本地源。
* 将生成的[!DNL Experiences]导出到GenStudio for Performance Marketing。
* 使用可适应Figma画布中所选元素的插件选项。

>[!VIDEO](https://video.tv.adobe.com/v/3478819?captions=chi_hans&learn=on)

## 创建模板

该插件要求Figma文档的前两个级别遵循以下约定：

* **节** — 这表示父项目，它可以包含多个模板。
* **框架** — 表示项目中的模板。 模板中可以填充文本、图像、组件和其他元素。

### Meta模板

支持以下模板大小：

对于Instagram或Facebook帖子：

* 宽度：1080像素（固定）
* 高度：1080像素或1350像素

对于Instagram或Facebook故事：

* 宽度：1080像素（固定）
* 高度：1920像素

插件会根据模板的高度确定所生成体验的颜色。

### 显示模板

没有固定大小要求。 显示模板支持任何大小。

### LinkedIn模板

* 宽度：1200像素（固定）
* 高度：1200像素、628像素、2292像素、1800像素或1500像素

### 字段角色映射

该插件需要了解模板的不同元素，例如标题、正文或图像。

要分配元素角色，请执行以下操作：

1. 在模板中选择元素（文本、图像等）。
1. 使用下拉菜单分配角色。

插件会记住这些映射，以便用于生成的内容。 一个字段角色可以映射到多个模板元素。

![字段角色映射](./field-role-mapping.png){width="600"}

### 字段映射例外

{{$include /help/_includes/field-mapping-exceptions.md}}

## 生成新内容

使用GenStudio for Performance Marketing AI生成或制作图形模板中元素的变体。

1. 如果您使用GenStudio插件游乐场或已经准备好的模板，请选择包含广告模板的部分节点。 您可以在&#x200B;**图层**&#x200B;面板中或通过直接单击画布中的部分来执行此操作。
   ![分区选择或变体](./plugin-playground.png){width="500" zoomable="yes"}
1. 在插件窗口中，输入变体的项目名称，选择内容的平台，并填写其他必需信息。 然后单击&#x200B;**[!UICONTROL 完成设置]**&#x200B;按钮。
   ![设置项目窗口](./setup-project.png){width="300" zoomable="yes"}
1. 选择要用于内容生成的[!DNL Brand]、[!DNL Persona]和[!DNL Product]。
1. 选择要生成的变体数（最多八个）。
1. 使用&#x200B;**[!UICONTROL 选择内容]**&#x200B;下的按钮浏览和选择资源中的图像。 40个最近添加的资产显示在最前，您可以搜索其他资产。 所选图像会自动调整大小以适合您的模板。
1. 输入文本提示。 **[!UICONTROL 字段]**&#x200B;列表中的每个字段都将&#x200B;**[!UICONTROL 操作]**&#x200B;选项设置为&#x200B;**[!UICONTROL 为新内容生成]**。
1. 映射所有字段角色。 查看[字段角色映射](#field-role-mapping)。
1. 单击&#x200B;**[!UICONTROL 生成]**&#x200B;按钮。

## 从现有内容翻译或生成广告复制变体

使用GenStudio for Performance Marketing人工智能生成广告复制变体或翻译图形模板。

1. 选择包含广告模板的部分节点。 您可以在&#x200B;**图层**&#x200B;面板中或通过直接单击画布中的部分来执行此操作。
   ![分区选择或变体](./plugin-playground.png){width="500" zoomable="yes"}
1. 在插件窗口中，输入变体的项目名称，然后选择内容的平台。
1. 在&#x200B;**[!UICONTROL 中，目标是什么？]**，选择&#x200B;**[!UICONTROL 生成变体]**&#x200B;或&#x200B;**[!UICONTROL 翻译]**，然后单击&#x200B;**[!UICONTROL 完成设置]**&#x200B;按钮。
   ![设置项目窗口](./setup-project.png){width="300" zoomable="yes"}
1. 选择要用于内容生成的[!DNL Brand]、[!DNL Persona]和[!DNL Product]。
1. 选择要生成的变体数量。
1. 使用&#x200B;**[!UICONTROL 选择内容]**&#x200B;下的按钮浏览和选择资源中的图像。 40个最近添加的资产显示在最前，您可以搜索其他资产。 所选图像会自动调整大小以适合您的模板。
1. 输入文本提示。 **[!UICONTROL 字段]**&#x200B;列表中的每个字段都将&#x200B;**[!UICONTROL 操作]**&#x200B;选项设置为&#x200B;**[!UICONTROL 为新内容生成]**。
1. 映射所有字段角色。 查看[字段角色映射](#field-role-mapping)。
1. 在插件左侧的面板中选择每个字段类型以生成变体或翻译，并将初始内容粘贴到每个&#x200B;**[!UICONTROL 初始内容]**&#x200B;框中。
   ![初始内容框中的示例文本](./initial-content-box.png){width="60%" zoomable="yes"}
1. 单击&#x200B;**[!UICONTROL 生成]**&#x200B;按钮。

## 生成后翻译内容

1. 选择要翻译的层代。
   ![选择层代](./select-generation.png){width="200" zoomable="yes"}
1. 选择&#x200B;**[!UICONTROL 翻译]**，然后单击&#x200B;**[!UICONTROL 翻译]**。
1. 选择目标语言。
1. 单击&#x200B;**[!UICONTROL 选择]**。

翻译结果包括：

* 此时将显示一个新页面，其中包含已翻译的内容。
* 每个翻译都会显示目标语言或区域设置。
* 原始内容在原始页面中保持不变。

![翻译结果](./translation-results.png){width="60%" zoomable="yes"}

## 生成后对内容字段执行的其他操作

编辑字段中的现有内容时，插件面板中会显示有用的选项。

![插件操作选项](./figma-other-actions.png){width="300" zoomable="yes"}

选项包括：

* 更改&#x200B;**[!UICONTROL 值]**&#x200B;以直接更改文本。 更改此内容会自动应用于所有选定的变体。
* AI可以执行许多&#x200B;**[!UICONTROL 操作]**&#x200B;选项，包括：

| 操作 | 描述 |
| --- | --- |
| **[!UICONTROL 生成]** | 生成文本的新变体。 |
| **[!UICONTROL 重新短语]** | 生成文本的新变体。 |
| **[!UICONTROL 缩短]** | 生成较短的文本变体。 |
| **[!UICONTROL 长度]** | 生成较长的文本变体。 |

选择&#x200B;**[!UICONTROL 操作]**&#x200B;选项后，使用&#x200B;**[!UICONTROL 重新生成]**&#x200B;按钮重新生成内容。

## 生成图像

使用文本提示生成要在模板中使用的图像。

1. 选择&#x200B;**[!UICONTROL 生成图像]**。
1. 从下拉菜单中选择一个模型。 您还可以选择已创建的任何自定义模型。
1. 选择设置图标可调整层代设置。
1. 可选：选择纵横比。
1. 可选：通过执行以下操作之一来调整图像的样式：
   * 通过选择&#x200B;**[!UICONTROL 上传图像]**，从设备或AEM上传参考图像。
   * 通过选择&#x200B;**[!UICONTROL 浏览图库]**，从Adobe的其中一个Stock图像中选择。
   * 使用滑块选择强度值。 力量会调整Firefly对您提供的样式的遵守程度。
1. 选择&#x200B;**&lt;**&#x200B;按钮。
1. 输入提示。
1. 选择生成图标。 图像会显示在插件面板中。
1. 使用以下方法之一将图像放到画布上：
   * 将任意图像拖放到画布上。
   * 在Figma画布上选择一个框架，然后在插件窗口中选择要插入到框架中的图像。
   * 选择上传图标以将图像上传到画布上。
   * 选择3个点，然后&#x200B;**[!UICONTROL 全部下载到Figma]**。
1. 可选：选择这3个点以执行进一步操作：
   * 选择&#x200B;**[!UICONTROL 生成更多]**&#x200B;以再次运行提示。
   * 选择&#x200B;**[!UICONTROL 复制提示]**&#x200B;以复制提示。
1. 可选：选择铅笔图标以在单个图像上使用生成填充和生成类似操作。

## 生成类似图像

生成一组类似的图像。

1. 选择&#x200B;**[!UICONTROL 生成类似]**&#x200B;卡。
1. 通过执行以下操作之一，选择图像作为参照：
   * 在Figma画布上选择图像。
   * 选择&#x200B;**[!UICONTROL 上传图像]**&#x200B;以从您的设备上传。
   * 选择&#x200B;**[!UICONTROL 浏览AEM资源]**&#x200B;以从AEM上传。
1. 选择生成图标。 变体会显示在插件面板中。
1. 使用以下方法之一将图像放到画布上：
   * 将任意图像拖放到画布上。
   * 在Figma画布上选择一个框架，然后在插件窗口中选择要插入到框架中的图像。
   * 选择上传图标以将图像上传到画布上。
   * 选择3个点，然后&#x200B;**[!UICONTROL 全部下载到Figma]**。
1. 可选：选择这3个点以执行进一步操作：
   * 选择&#x200B;**[!UICONTROL 生成更多]**&#x200B;以再次运行提示。
1. 可选：选择铅笔图标以在单个图像上使用生成填充和生成类似操作。

## 移除背景

删除图像的背景。

1. 选择&#x200B;**[!UICONTROL 删除背景]**&#x200B;卡。
1. 通过执行以下操作之一，选择图像作为参照：
   * 在Figma画布上选择图像。
   * 选择&#x200B;**[!UICONTROL 上传图像]**&#x200B;以从您的设备上传。
   * 选择&#x200B;**[!UICONTROL 浏览AEM资源]**&#x200B;以从AEM上传。
1. 选择&#x200B;**[!UICONTROL 删除]**。 如果从画布中选择了图像，则该图像将会在“图像”画布上被替换。 如果图像是从设备或AEM中选择的，则可以将图像拖放到画布上，也可以选择&#x200B;**[!UICONTROL 插入图像]**&#x200B;将图像放在画布上。

## 生成填充

为图像的区域应用生成填充。

1. 选择&#x200B;**[!UICONTROL 生成填充]**&#x200B;卡。
1. 通过执行以下操作之一，选择图像作为参照：
   * 在Figma画布上选择图像。
   * 选择&#x200B;**[!UICONTROL 上传图像]**&#x200B;以从您的设备上传。
   * 选择&#x200B;**[!UICONTROL 浏览AEM资源]**&#x200B;以从AEM上传。
1. 选择画笔工具并创建蒙版。
1. 可选：选择下拉插入符号并调整画笔大小。
1. 选择“重置”按钮以删除蒙版。
1. （可选）选择删除背景图标以删除背景。
1. 输入提示以引导生成所选掩码，然后选择&#x200B;**[!UICONTROL 生成]**&#x200B;按钮。
1. 使用以下方法之一将图像放到画布上：
   * 将任意图像拖放到画布上。
   * 在Figma画布上选择一个框架，然后在插件窗口中选择要插入到框架中的图像。
   * 选择上传图标以将图像上传到画布上。
   * 选择3个点，然后&#x200B;**[!UICONTROL 全部下载到Figma]**。
1. 可选：选择这3个点以执行进一步操作：
   * 选择&#x200B;**[!UICONTROL 复制提示]**&#x200B;以复制提示。
1. 可选：选择铅笔图标以在单个图像上使用生成填充和生成类似操作。

## 提示编辑

编辑带有文本提示的图像内容。

1. 选择&#x200B;**[!UICONTROL 提示编辑]**&#x200B;信息卡。
1. 通过执行以下操作之一，选择图像作为参照：
   * 在Figma画布上选择图像。
   * 选择&#x200B;**[!UICONTROL 上传图像]**&#x200B;以从您的设备上传。
   * 选择&#x200B;**[!UICONTROL 浏览AEM资源]**&#x200B;以从AEM上传。
1. 选择设置图标可调整层代设置。
1. 可选：选择长宽比并选择&#x200B;**&lt;**&#x200B;按钮。
1. 输入提示以引导生成，然后选择&#x200B;**[!UICONTROL 生成]**&#x200B;按钮。
1. 使用以下方法之一将图像放到画布上：
   * 将任意图像拖放到画布上。
   * 在Figma画布上选择一个框架，然后在插件窗口中选择要插入到框架中的图像。
   * 选择上传图标以将图像上传到画布上。
   * 选择3个点，然后&#x200B;**[!UICONTROL 全部下载到Figma]**。
1. 可选：选择这3个点以执行进一步操作：
   * 选择&#x200B;**[!UICONTROL 生成更多]**&#x200B;以再次运行提示。
   * 选择&#x200B;**[!UICONTROL 复制提示]**&#x200B;以复制提示。
1. 可选：选择铅笔图标以在单个图像上使用生成填充和生成类似操作。

## 生成扩展

展开图像的尺寸，并使用生成性展开添加生成性内容。 创成性展开允许您将不合适的图像转换为横幅、Meta广告、LinkedIn广告或显示广告模板最合适的纵横比。

1. 选择&#x200B;**[!UICONTROL 生成Expand]**&#x200B;卡。
1. 选择画布上的图像。
1. 将Gen Expand Temporary框架的大小调整为所需的新维度。
1. 可选：将图像移动到框架内的任意位置。
1. 输入提示以引导生成，然后选择&#x200B;**[!UICONTROL 生成]**&#x200B;按钮。
1. 选择画布上的任意图像，将原始图像替换为生成的结果。

## 导出体验

变体可以作为GenStudio for Performance Marketing [!DNL Experiences]从Figma导出。

1. 通过执行以下操作之一，选择要在Figma画布中导出的内容：
   * 在画布中选择生成部分，然后在插件面板中单击&#x200B;**[!UICONTROL 全部标记为导出]**。
     ![生成节选择](./select-generation-section.png){width="200" zoomable="yes"}
   * 在画布中选择单个层代，然后在插件面板中单击&#x200B;**[!UICONTROL 标记为导出]**。
     ![单个层代选择](./select-generation.png){width="200" zoomable="yes"}
1. 从侧栏菜单中选择“导出”项目。
   为Meta广告显示![标记为导出按钮](./mark-for-export.png){width="60%" zoomable="yes"}
1. 选择目标。
1. 单击&#x200B;**[!UICONTROL 导出]**&#x200B;以导出内容。

在插件面板中创建ZIP文件，或显示指向&#x200B;**[!UICONTROL 在GenStudio中打开]**&#x200B;的链接。 使用ZIP链接选择保存文件的位置，或选择&#x200B;**[!UICONTROL 在GenStudio中打开]**。

## 生成历史记录

插件会维护每个字段的更改历史记录。 在模板页面上，在插件侧边栏中选择&#x200B;**[!UICONTROL 生成历史记录]**。

为Meta广告显示![生成历史记录选项](./generation-history.png){width="80%" zoomable="yes"}

## 故障排除

如果生成的变体中未替换文本或图像，请考虑这些最佳实践和提示。

### 映射字段

如果未替换文本或图像，请检查是否已将字段映射到插件UI中的GenStudio字段角色。 查看[字段角色映射](#field-role-mapping)。

### 确认字体可用

文本字段的字体必须在计算机上可用，才能在生成期间替换。 确认文件中使用的所有字体在您的计算机上都可用，尤其是当文件是在其他人的计算机上创建时。

### 考虑现场角色支持

某些渠道仅支持在特定字段中进行替换。 请注意[字段角色映射](#field-role-mapping)的异常。
