---
title: 显示广告模板准则
description: 在Adobe GenStudio for Performance Marketing中使用显示广告和横幅模板时，请遵循最佳实践。
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 076239b3-9444-48f9-bdd6-ef2b757bdf0d
source-git-commit: f4bc3442678e6366e185d0c7a91c784d43b8e455
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# 显示广告模板准则

显示模板是预先设计的布局，用于创建吸引眼球的横幅和显示广告。 它们提供了一个灵活的框架来整合图像、文本和call to action，确保在生成多个广告变体时保持一致性和效率。 在准备用于GenStudio for Performance Marketing的模板时，请确保所有资源都针对Web显示进行了优化，并符合所需的文件格式和大小。

在自定义横幅和显示广告模板以用于GenStudio for Performance Marketing时，请遵循以下设计最佳实践：

- 使用Adobe或Google字体
- 准备以超薄尺寸完美显示的资产
- 仅需要一个图像字段
- **不**&#x200B;使用嵌入或编码的背景图像
- 使用上载到GenStudio for Performance Marketing内容存储库的背景图像（`image`字段）。 请遵循[上传显示广告的图像](#uploading-images-for-display-ads)中的准则，以获得最佳结果
- **不**&#x200B;使用JavaScript
- 只能使用一个部分，生成一组模板元素

## 可识别的字段名称

在自定义横幅或显示广告模板时，请为以下必填字段使用内容占位符：

- `headline`
- `sub_headline`
- `body`
- `image` (必需，从Content JPEG、PNG或GIF中选择)

GenStudio for Performance Marketing会自动生成以下字段。 您不必为以下内容应用内容占位符：

- `cta`

请参阅[内容占位符](/help/user-guide/content/customize-template.md#content-placeholders)以了解有关在模板中使用字段名的更多信息。

## 支持的维度

必须设置宽度x高度（像素）。

| 方向 | 尺寸（像素） | 注释 |
|--------------|-------------------------------------------------------------|------------------------------------------------------------------|
| 垂直 | 300 x 600<br>160 x 600 | 普通摩天大楼和半页横幅。 |
| 水平 | 300 x 250<br>728 x 90<br>336 x 280<br>320 x 50<br>970 x 250 | 标准排行榜、中等矩形和横幅尺寸。 |
| 自定义 | 50 x 50至2000 x 2000 | 用于非标准或唯一放置；检查平台限制。 |

## 上传显示广告的图像

显示广告中使用的图像应来自内容存储库，并且需要正确上传以确保图像在模板中准确显示。

当显示模板具有边缘到边缘（完全出血）图像时，所选图像会自动调整大小以适合完整模板尺寸。 但是，如果图像与模板长宽比不匹配，则会裁剪图像以适合模板尺寸，并且可能无法按预期显示。

显示广告模板中的图像没有“自动调整”功能。

要解决图像裁剪问题，用户必须定义图像上传到内容存储库后在模板中的纵横比。 上传已批准的显示广告模板时：

1. [继续模板上载过程](/help/user-guide/content/use-templates.md#add-a-template)，直到到达&#x200B;**[!UICONTROL 添加详细信息]**&#x200B;页面。

1. 以&#x200B;**[!UICONTROL 广告宽度(px)]**&#x200B;和&#x200B;**[!UICONTROL 广告高度(px)]**&#x200B;定义要在模板中使用的图像的宽高比。 这将为显示图像的模板部分定义图像窗口。

1. 在&#x200B;**[!UICONTROL 更多详细信息]**&#x200B;部分中，选择&#x200B;**[!UICONTROL 图像大小]**&#x200B;下拉列表，然后选择&#x200B;_裁切为固定大小_。
   ![裁切为固定大小](./crop-to-fixed-size.png "裁切为固定大小"){width="80%"}

要在浏览器中确定图像的大小和纵横比，请执行以下操作：

1. 检查图像。
   - Windows/Linux：
      - 按F12。
   - macOS：
      - 按Command + Option + I。

1. 将鼠标悬停在图像上。

1. 请注意纵横比。 使用此参数定义模板中图像的纵横比。

如果上传期间未应用这些详细信息，则假定图像是模板的整个纵横比，并且与该纵横比不完全匹配的图像将显示为已裁剪。

![在显示广告中裁切的图像](./cropped-display.png "图像裁切"){width="60%"}

显示广告模板中的&#x200B;**❌裁剪的图像**

![显示在显示广告中的图像](./full-fit.png "显示在显示广告中的图像"){width="60%"}

**✅图像已完全显示**
