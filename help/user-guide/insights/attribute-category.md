---
title: 属性类别
description: 了解GenStudio for Performance Marketing中使用的属性类别。
feature: Insights, Attributes, Generative AI
recommendations: noDisplay
source-git-commit: 3b5fc55595f766db0327b6aefb0e29c3896e00c0
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 1%

---

# 属性类别

属性类别是组织具有共同特征的相关属性的分类组。 这些类别通过提供更丰富的上下文并方便其应用和使用，有助于简化对特定属性的发现、识别和理解。

GenStudio for Performance Marketing使用Adobe的AI和机器学习功能来研究图像、视频和文本，并根据置信度级别应用[!UICONTROL 资产属性]。 _置信度_&#x200B;指的是AI分配给预测或分类的概率。 在机器学习的语境下，它是一种衡量AI对分类正确性的“信心”程度的评分。 置信度得分越高，确定性就越大。 例如，在分析图像时，AI可以识别多个特征，并为每个特征分配一个分数，这表示特征正确的信心程度。 资产的属性列表并非详尽无遗。 包含丰富功能集的Assets可以限制为置信度阈值，例如已识别的三个最主要特征。

## 图像特征

图像特征表示图像内用于与[!DNL Insights]一起分析的不同且信息性元素或图案。 下表列出了GenStudio for Performance Marketing AI识别的图像功能类别。

<!-- For the writer: turn off word wrap to work with these tables. Option + Z -->

| 类别 | 描述 | 示例 |
| ----------------------- | ----------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 相机角度 | 相机相对于主体的位置和角度。 |                                                                                                                                                                                |
| 目标距离 | 摄像头和图像目标之间的距离。 | `close up`、`mid shot`、`long shot` |
| 相机设置 | 用于生成图像的相机控件的配置。 |                                                                                                                                                                                |
| 颜色和色调 | 计算图像元素中使用的颜色。 在以下图像图层中，从一组40种预先确定的颜色中标识一到三种颜色： <br>**[!UICONTROL 前景颜色&#x200B;]**— 图像前图层中的元素<br>**[!UICONTROL 背景颜色]** — 图像后图层中的元素<p>**[!UICONTROL 色温]**&#x200B;描述图像中颜色的常规热度或冷度。<br>色调或温度值： `warm`、`cool`、`neutral` | ![颜色和淡色调](../../assets/category/image-color-temp.png){width="200" zoomable="yes"} |
| 图像样式 | 图像的视觉处理。 |                                                                                                                                                                                |
| 照明条件 | 图像中的光类型。 |                                                                                                                                                                                |
| 对象 | 标识构成图像的一个或多个项目、图元和元素。 | ![向日葵，飞机，花物件](../../assets/category/image-objects.png){width="200" zoomable="yes"} |
| 方向 | 图像相对于纵横比的位置。 | `landscape`、`portrait`、`square` |
| 人员 | 当至少一个人在场时，一个或多个属性可以描述图像中的一个或多个人。 | ![女性跳舞](../../assets/category/image-people.png){width="200" zoomable="yes"} |
| 摄影流派 | 检测用于捕获图像的对象和技术，如`abstract`或`landscape`（与横向不同）。 |           |
| 场景 | 检测映像中描述的设置或环境。 |                                             |
| 标记 | 检测不属于特定分类的对象、元素和其他图像特征。 |                                      |

<!-- Not yet approved by legal
| Attention distribution  | The level of viewer attention spread across an image.                                                 | `high`, `medium`, `low`                                                                                                                                                                                                    |
| Content density         | The amount of information or detail in an image.                                                      | `high`, `medium`, `low`                                                                                                                                                                                                    |
-->

## 视频功能

图像特征表示视频中用于分析[!DNL Insights]的不同且信息性元素、声音或模式。 下表列出了GenStudio for Performance Marketing AI识别的视频功能类别。

| 类别 | 描述 | 示例 |
| ------------------- | ------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------- |
| 音频流派 | 当存在音乐时，视频可能会收到一个音乐风格分类，如`electronic`或`classical`。 |          |
| 音频流派类别 | 当存在音乐时，视频可能会接收一个广泛的音乐流派，如`acoustic`或`traditional`。 |          |
| 音频心情 | 描述音频的一般气氛或音调，如`relaxing`或`energetic`。 |          |
| 音频类型 | 当音频存在时，视频可能会接收一个或多个音频类型（如`music`或`speech`）的标记。 |          |
| 对象 | 标识整个视频中显示的一个或多个项目、实体和元素。 | 视频中的![对象](../../assets/category/video-objects.png){width="200" zoomable="yes"} |
| 方向 | 相对于帧的长宽比的视频位置。 | `landscape`、`portrait`、`square` |
| 人员 | 当至少一个人在场时，一个或多个属性可以描述视频中的一个或多个人。 |        |
| 场景 | 视频中描述的设置或环境。 |        |
| 样式 | 检测应用于视频中元素的可视化处理，如`matte`或`neon`。 |        |
| 标记 | 检测不属于特定分类的对象、元素和其他视频特征。 |        |

## 文本功能

文本特征包括某些文本元素的计数，如词语、句子、表情符号，以及用于通过[!DNL Insights]进行分析的语义、情感和色调的分类。 文本也可以接收可读性分数。 即将推出。

<!-- Not yet approved by legal

The following table lists the image feature categories recognized by the GenStudio for Performance Marketing AI.

| Category             | Description | Example |
|----------------------|-------------|--------|
| Emojis Count         |             |        |
| HashTags Count       |             |        |
| Keywords             |             |        |
| Marketing Emotions   |             |        |
| Narratives           | Text that represents an overarching situation, theme, or a story. Narratives can communicate values, purpose, or identity that resonates with consumers on many levels.   |        |
| Persuasion Strategies|             |        |
| Readability          |             |        |
| Tone of voice        | | |
-->
