---
title: 图像功能
description: 了解GenStudio for Performance Marketing中使用的属性类别的图像功能。
level: Intermediate
feature: Reporting and Insights, Image Attributes, Generative AI
exl-id: b7e3d202-4085-48a4-a6ba-c950dfd52233
source-git-commit: c0f45fb0ffc61d20611693498f1b12d3946ca6ca
workflow-type: tm+mt
source-wordcount: '1056'
ht-degree: 0%

---

# 图像特征

图像特征表示图像内用于与[!DNL Insights]一起分析的不同且信息性元素或图案。 这些功能有助于对可视内容进行分类和了解，从而实现更准确、更详细的分析。 通过识别样式、颜色和对象等各种属性，AI可以提供图像的全面分析，帮助更好地决策和策略制定。

## 样式检测

确定&#x200B;_图像样式_&#x200B;是识别其他图像特征的基础。 AI可以应用适当的分析技术并识别相关特征，从而更全面地了解图像。 每种风格都具有独特的视觉特性，这些特性会影响图像感知和分析的方式。

如果图像样式被识别为`photograph`，则AI将分析`camera settings`、`camera proximity`和`Photography genres`的其他特征。 这些特征特定于照片，可让您更深入地了解图像的构成和质量。 查看Adobe的[学习摄影](https://www.adobe.com/creativecloud/photography/discover/types-of-photography.html)中的&#x200B;_28种摄影样式_&#x200B;并了解流行类型的摄影和基础术语。

如果图像样式被识别为`sketch`或`digital cartoon`，则可能涉及一组不同的特征。 这种分层方法可确保分析在语境上准确并且针对被检查的特定图像类型量身定制。

## 搜索图像功能

**要查看特定属性类别中的图像**：

1. 在&#x200B;_[!DNL Insights]_&#x200B;中，选择&#x200B;**[!UICONTROL 属性]**&#x200B;视图。

1. 通过选择&#x200B;**[!UICONTROL 图像]**&#x200B;更改表视图。

1. 从&#x200B;**[!UICONTROL 属性类别]**&#x200B;列表中选择图像功能，如`Scenes`。

1. 选择共享该类别的图像详细视图的属性。

   例如，`Scenes`类别可以将`restaurant`作为属性。

1. _属性详细信息_&#x200B;页面列出了具有此属性的所有图像。

下表列出了GenStudio for Performance Marketing AI识别的图像功能类别。 检测到的媒体内容属性列表并不完整。 包含丰富功能的媒体可能仅限于AI确定的三个最主要的特征。

<!-- For the writer: turn off word wrap to work with these tables. Option + Z -->

| 类别 | 描述 | 示例 |
| ----------------------- | ----------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 注意力分布 | 查看者的注意力水平分散在图像上，指示图像不同区域可能获得的焦距。 较高的分布意味着没有单一区域支配观看者的注意力，而较低的分布意味着一两个焦点吸引观看者的注意力。 | `high`、`medium`、`low`<p>左侧的`low`分发和右侧的`high`分发示例：<p>![低分布和高分布球赛](/help/assets/category/image-attn-lowhigh.png "低分布和高分布差异"){width="200" zoomable="yes"} |
| 相机角度 | 照相机拍摄主体的视角，这将影响查看者对图像的认知和解释。 如果图像样式为`photograph`，则标识此特征。 | `Low angle`，`High angle`，`Eye level`，`Neutral angle`，`Overhead view`，`Bird's eye view`<p>`Overhead view`示例：<p>![管理费用视图](/help/assets/category/image-camera-angle.png "管理费用短信息对"){width="200" zoomable="yes"} |
| 相机设置 | 影响图像最终外观和质量的相机控制的特定调整和配置。 如果图像样式为`photograph`，则标识此特征。 | `Fast shutter speed`，`Long exposure`，`Bokeh blur`，`Motion blur`，`Tilt-shift blur`，`Flash`，`Wide-angle`，`Black and white`，`Double-exposure`，`Macro`，`Normal mode`<p>`Fast shutter speed`设置示例：<p>![快门速度](/help/assets/category/image-camera-setting.png "在波浪上冲浪"){width="200" zoomable="yes"} |
| 颜色和色调 | 图像中的颜色和色调品质。 从不同图像图层中的预定义40种颜色集中标识最多三种颜色：<p>**[!UICONTROL 前景色]** — 图像前层的颜色<br>**[!UICONTROL 背景色&#x200B;]**— 图像后层的颜色 | 颜色值： `Red`、`Dark Red`、`Green`、`Bright Green`、`Dark Green`、`Light Green`、`Mud Green`、`Blue`、`Dark Blue`、`Light Blue`、`Royal Blue`、`Black`、`White`、`Off White`、`Gray`、`Dark Gray`、`Silver`、`Cream`、`Magenta`、`Cyan`、`Yellow`、`Mustard`、`Khaki`、`Brown`、`Dark Brown`、`Violet`、`Pink`、`Dark Pink`、`Maroon` `Tan`、`Purple`、`Lavender`、`Turquoise`、`Plum`、`Gold`、`Emerald`、`Orange`、`Beige`、`Lilac`、`Olive` |
| 色温 | 描述图像中颜色的一般温暖或冷度。 | 色调或温度值： `warm`、`cool`、`neutral`<br>![颜色和冷色调](/help/assets/category/image-color-temp.png "具有冷背景和多色对象的色温"){width="200" zoomable="yes"} |
| 内容密度 | 图像中的视觉元素和细节的集中程度，指示有多少信息被填充到视觉空间中。<p>与注意力分布不同（注意力分布测量的是观看者焦点在图像不同区域的分布情况），内容密度侧重于视觉信息呈现的数量。 较高的内容密度意味着存在更多的元素。 | `high`、`medium`、`low`<p>左侧`low`密度和右侧`high`密度的示例：<p>![低密度和高密度球赛](/help/assets/category/image-attn-lowhigh.png "低密度和高内容密度差异"){width="200" zoomable="yes"} |
| 图像样式 | 图像的视觉处理，如照片或草图。 一旦AI确定图像样式，就可以识别其他特征。 例如，如果图像是照片，则可能应用相机设置、相机邻近性和照明条件。 | `Photograph`，`Photograph with text overlay`，`Sketch`，`Painting`，`Digital cartoon`，`Infographics`，`Graphic design`，`Collage`，`Software screenshot`<p>`digital cartoon`图像样式![卡通图像样式](/help/assets/category/image-style.png "猫图像样式卡通示例"){width="200" zoomable="yes"} |
| 照明条件 | 描述图像中的光线的质量和特征，影响其情绪、色调和可见性。 | `Golden hour`，`Blue hour`，`Midday`，`Overcast`，`Night`，`Daylighting`，`Incandescent`，`Fluorescent`，`Colorful`，`Studio`<p>`daylighting`条件的示例：<p>![在日光下人行道上的人和狗](/help/assets/category/image-lighting.png "日光下条件"){width="200" zoomable="yes"} |
| 对象 | 标识构成图像的一个或多个项目、图元和元素。 | 值太多，但某些示例包括：`backpack`、`book`、`hawk`、`glasses`、`fish`、`pencil`、`mountain bike`、`soap`<p>`toucan`和`bird`对象的示例：<p>![Bird， Toucan对象](/help/assets/category/image-objects-bird.png "Toucan Bird对象的图形设计"){width="200" zoomable="yes"} |
| 方向 | 相对于图像的宽度和高度的图像对齐方式。 检测它是否比高（横向）宽、比宽（纵向）高或宽高相等（正方形）。 | `landscape`、`portrait`、`square`<p>`square`方向示例：<p>![方形草图](/help/assets/category/image-orientation-square.png "方形方向花草图"){width="200" zoomable="yes"} |
| 人员 | 当至少一个人在场时，一个或多个属性可以描述图像中的一个或多个人。 | `person`，`woman`，`man`，`girl`，`boy`，`social group`，`kid`，`crowd`，`people`<p>人员`woman`和`person`类别的示例：<p>![带有摄像机的女性](/help/assets/category/image-people.png "管理摄像机的人员"){width="200" zoomable="yes"} |
| 摄影流派 | 检测用于捕获图像的对象和技术，如`Abstract`或`Landscape`（与横向不同）。 | `Architecture`、`Astro`、`Landscape`、`Pet`、`Interior`、`Wildlife`、`Night`、`Cityscape`、`Seascape`、`Underwater`、`Storm`、`Adventure sports`、`Fashion`、`Portrait`、`Sports`、`Food`、`Street`、`Event`、`Lifestyle`、`Commercial`、`Group`、`Abstract`、`Minimalist`、`Composite`、`Surreal` <p>查看[摄影类型](https://www.adobe.com/creativecloud/photography/discover/types-of-photography.html)。<p>`Adventure sports`示例：<p>![与独木舟站在一起](/help/assets/category/image-photography-genres.png "与独木舟站在一起"){width="200" zoomable="yes"} |
| 场景 | 标识图像中的设置或环境，提供有关捕获图像的位置或描述的位置类型的上下文。 | 值太多，但某些示例包括：`lake`、`underwater`、`highway`、`hill`、`log cabin`、`island`、`beach`、`lounge`<p>反映在头盔上的示例`snow`、`sky`、`winter`和`mountain`场景：<p>![冬季雪景](/help/assets/category/image-scenes.png "冬雪、天空和山景反射"){width="200" zoomable="yes"} |
| 目标距离 | 摄像头和图像目标之间的距离。 | `close up`、`mid shot`、`long shot`<p>`Long shot`示例：<p>![长镜头山顶](/help/assets/category/image-subject-distance.png "远山山顶上的人"){width="200" zoomable="yes"} |
| 样式 | 检测应用于图像元素的可视化处理，例如在Lightroom或Photoshop中使用的处理。 | `design`，`illustration`，`logo`，`square`，`cartoon`，`art`，`circle`，`circular`<p>`circular`样式的示例：<p>![珊瑚礁中的圆形网关](/help/assets/category/image-styles-circular.png "珊瑚礁中的圆形门户"){width="200" zoomable="yes"} |
| 标记 | 检测不属于特定分类的其他图像特征。 标记提供有关图像的其他上下文和元数据。 例如，AI可能检测到图像中的`helmet`和`motorobike`对象，并包含`riding`作为标记。 | 值太多，但某些示例包括：`construction`、`gothic`、`healing`、`military`、`selfie`、`football`、`typing`、`dancer`、`dancing`<p>`dancer`和`dancing`标记的示例：<p>跳舞和跳舞的![标记](/help/assets/category/image-tags.png "跳舞的人"){width="200" zoomable="yes"} |
