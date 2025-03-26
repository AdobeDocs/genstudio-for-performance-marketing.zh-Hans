---
title: 视频功能
description: 了解GenStudio for Performance Marketing中使用的属性类别的视频功能。
level: Intermediate
feature: Reporting and Insights, Video Attributes, Generative AI
exl-id: 0dfdd735-b365-4a15-a6fd-e981697442cb
source-git-commit: 8a5d15df7a347c4ee7767610fc9bb23fc7b71db4
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 1%

---

# 视频功能

视频功能表示视频中用于分析[!DNL Insights]的不同且信息性元素、声音或模式。 这些功能有助于分类和了解视频内容，从而实现更准确和详细的分析。 通过识别音频情绪、音乐流派和对象等各种属性，人工智能可以提供对视频的综合分析，有助于更好地决策和策略制定。

## 音频检测

GenStudio for Performance Marketing中的音频检测涉及分析视频的音频轨道以识别各种属性。 该检测过程通过识别呈现的音频类型、标记特定的流派或音乐类别以及从语音中提取关键字来确定音频的整体情绪。 通过了解这些音频元素，AI可以对视频的内容和上下文提供更深入的见解，从而增强整体分析和分类过程。

## 搜索视频功能

**要预览视频并聆听音频示例**，请执行以下操作：

1. 在&#x200B;_[!DNL Insights]_中，选择&#x200B;**[!UICONTROL 属性]**视图。

1. 通过选择&#x200B;**[!UICONTROL 视频]**&#x200B;更改表视图。

1. 从&#x200B;**[!UICONTROL 属性类别]**&#x200B;列表中选择一个功能。 对于音频示例，请选择&#x200B;**音乐流派**。

1. 选择共享该类别的视频详细视图的属性。

   例如，`Music genre`类别可以将`electronic`作为属性。

1. _属性详细信息_&#x200B;页面列出了具有此属性的所有视频。 将鼠标指针悬停在列表中的任何视频上以开始视频预览。

1. 切换&#x200B;**取消静音**（位于视频预览的左下角）按钮并收听视频预览的音频。

下表列出了GenStudio for Performance Marketing AI识别的视频功能类别。 检测到的媒体内容属性列表并不完整。 包含丰富功能的媒体可能仅限于AI确定的三个最主要的特征。

<!-- For the writer: turn off word wrap to work with these tables. Option + Z -->

| 类别 | 描述 | 示例 |
| ------------------- | ------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------- |
| 音频心情 | 确定音轨的整体情绪音调或氛围，如`calm`、`upbeat`或`tense`。 | `Energetic`，`Happy`，`Emotional Ambient/atmospheric`，`Relaxing`，`Dramatic`，`Expressive/characterful`，`Intense`，`Slow`，`Neutral` |
| 音频类型 | 为视频添加一个或多个音频类型的标记，如`music`或`speech`。 | `Music`，`Speech`，`Silence`，`Special effects`，`Ambience` |
| 类别 | 将视频分类为一个或多个广义内容类别。 | `Entertainment`、`Sports`、`Music`、`Gaming`、`Howto tutorials`、`Fashion and style`、`Film and animation`、`Science and technology`、`Autos and vehicles`、`Pets and animals`、`People and blogs`、`News and politics`、`Social causes and activism`、`Travel and events`、`Education`、`Sales and offers` |
| 音乐类别 | 当音乐出现在视频中时，音乐类型的广泛分类。 这有助于识别音乐的一般类型，如`contemporary`或`traditional`样式。 | `Contemporary/pop music`，`Traditional/folk-based music`，`Instrumental/orchestral music`，`Rock music`，`Acoustic/unplugged music`，`Specialised/occasional music`，`Experimental/unique music` |
| 音乐流派 | 当视频中存在音乐时音乐风格的特定分类，它提供了更详细的音乐标识，如`electronic`或`jazz`。 | `electronic`，`hip-hop`，`dance`，`novelty`，`rock`，`world`，`reggae`，`pop`，`film`，`jazz`，`background`，`latin` |
| 对象 | 标识视频中显示的一个或多个项目、实体和元素。 | 值太多，但某些示例包括：`backpack`、`book`、`hawk`、`glasses`、`fish`、`pencil`、`mountain bike`、`soap` |
| 方向 | 视频相对于其宽度和高度的对齐方式。 检测它是否比高（横向）宽、比宽（纵向）高或宽高相等（正方形）。 | `landscape`、`portrait`、`square` |
| 人员 | 当至少有一个人在场时，一个或多个属性可以描述视频中存在的一个或多个人。 | `person`，`woman`，`man`，`girl`，`boy`，`social group`，`kid`，`crowd`，`people` |
| 场景 | 标识视频中的设置或环境，提供有关视频制作位置或所描述位置类型的上下文。 | 值太多，但某些示例包括：`lake`、`underwater`、`highway`、`hill`、`log cabin`、`island`、`beach`、`lounge` |
| 样式 | 检测应用于视频元素的可视化处理，例如在After Effects或Lightroom中使用的处理。 | `design`，`illustration`，`logo`，`square`，`cartoon`，`art`，`matte`，`neon` |
| 标记 | 检测不属于特定分类的其他视频特征。 标记提供有关视频的其他上下文和元数据。 | 值太多，但某些示例包括：`construction`、`gothic`、`healing`、`military`、`selfie`、`football`、`typing`、`dancer`、`dancing` |
