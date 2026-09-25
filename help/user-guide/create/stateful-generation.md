---
title: 通过有状态生成来生成和优化内容
description: 了解如何生成品牌内内容并在[!DNL GenStudio for Performance Marketing]中轮流通过语音打印和视觉提示进行优化和改进。
feature: Create Prompt, Generative AI, Content Generation
role: User
level: Beginner
source-git-commit: 22db02c07a9f33cb1c70df9286ad6eb143dafd38
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%
---
# 通过有状态生成来生成和优化内容

[!DNL GenStudio for Performance Marketing]使用状态生成功能帮助您创建品牌内内容，然后轮流在对话中对其进行优化，而不是每次都以新的提示重新开始。 优化后，层代会记住您之前的说明和保存的变体，然后仅应用您要求的更改。

有状态层代可为您的层代添加三种上下文：声纹功能会保留品牌语音中的复本，图像或视频中的视觉提示地面复本，以及网页URL会从您选择的页面添加引用上下文。

## 生成和优化内容

1. 在[!DNL GenStudio for Performance Marketing]中，开始生成渠道和格式。 请参阅[[!DNL Create] 概述](/help/user-guide/create/overview.md)以开始为每个渠道生成报表。
1. _可选_：要在您自己的创意中植入副本，请选择&#x200B;**[!UICONTROL 从内容中选择]**，然后选择要用作[视觉提示的图像或视频](#ground-content-in-an-image-or-video)。
1. 选择&#x200B;**[!UICONTROL 生成]**。 [!DNL GenStudio for Performance Marketing]创建一组变体并将您的[品牌语音](#keep-copy-in-your-brand-voice)自动应用于支持的渠道。
1. 在提示抽屉中优化结果。 键入所需的更改，如`shorten the headline`、`make variant 2 punchier`或`change the headline`。 该层代仅应用该更改并保留您之前的说明。
1. 要在继续优化时保留变体，请在提示抽屉中键入说明，如`keep variant 2`。
1. 内容准备就绪后，将其导出或发送以供审阅。

## 图像或视频中的背景内容

通过视觉提示，这一代用户可读取您附加的图像或视频，然后编写反映该创意的副本。 **[!UICONTROL Creative选项]**&#x200B;切换控件可控制视觉提示，默认情况下处于打开状态。

若要使用视觉提示，请选择&#x200B;**[!UICONTROL 从内容中选择]**，然后在生成之前选择图像或视频。 若要在没有视觉提示的情况下生成，请关闭&#x200B;**[!UICONTROL Creative选项]**。

>[!NOTE]
>可视提示不适用于多框架显示广告或轮播广告。

## 保持品牌语调中的文案风格

声纹功能可将您品牌所学到的声音应用到生成的文案中，因此无需额外的提示，即可让声纹在品牌中响起。 对于具有[Insights](/help/user-guide/insights/overview.md)的渠道（如LinkedIn和Meta），默认情况下会开启此功能。

## 使用网页作为上下文

您可以将生成的内容指向一个网页，并将其内容用作上下文。 在提示抽屉中，键入包含URL的说明，如`Use this URL to generate an ad for this channel: https://www.example.com`。

>[!NOTE]
>在提示符下输入URL。 不要通过&#x200B;_参数_&#x200B;添加它。

## 相关功能

- [管理变量](/help/user-guide/create/manage-variants.md)：直接在画布上编辑和微调生成的变量。
- [编写有效的提示](/help/user-guide/effective-prompts.md)：制作产生更好结果的提示。
