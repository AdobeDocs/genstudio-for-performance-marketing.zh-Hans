---
title: 激活工作流
description: 了解广告体验的激活工作流。
feature: Ad Activation
exl-id: 17e1bade-d52a-4953-a85c-c10d093e73d6
source-git-commit: 8db25ba42a8eebc2d17f8b8b1a5f5fbede1a6e0f
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 0%

---

# 激活工作流

_[!DNL Activate]_支持以创意形式激活特定于渠道的格式的广告体验，例如Meta或Google Campaign Manager 360广告体验。

GenStudio for Performance Marketing体验是一种营销活动组件（如广告），它通过付费广告渠道或电子邮件为特定受众准备作为创意。 创意包含三个主要组成部分：

* **媒体资源**：媒体资源是广告体验中包含的图像(GIF、PNG、JPEG)。 激活当前支持静态图像。
要为广告体验选择图像资源，需要选择适当的纵横比。 长宽比定义图像的宽度和高度之间的比例关系，它们对于广告投放的有效性至关重要。 付费媒体渠道仔细为其平台上的每个广告投放指定有效的宽高比。 将图像资产添加到激活时，必须根据体验的最终广告投放位置选择纵横比。 文件类型仅限于JPEG、PNG和GIF。

* **文本**：文本包含广告中包含的所有形式的副本，包括标题、正文和行动号召元素。

* **元数据**：可分配给内容的用户定义属性。 元数据增强了性能分析、筛选和跟踪。 它通常对用户不可见。

创建激活涉及优化这些广告组件的每一个以用于指定的渠道投放和营销活动。 GenStudio for Performance Marketing支持将一个体验激活到一个付费渠道。

## 工作流阶段

尽管唯一的投放位置要求定义了每个付费渠道，但所有广告激活都共享相同的高级步骤。 将体验激活到任何付费渠道有三个核心阶段：

* **将GenStudio for Performance Marketing连接到您的Target频道**。 GenStudio系统管理员必须连接您的渠道帐户，然后才能激活体验。

* **准备激活体验**。 准备工作包括以适合您特定广告投放的宽高比选择媒体资产，并将文本分配给行动号召元素和正文。 您还可以添加信息性元数据，帮助用户在激活后搜索体验。 每个广告渠道投放都为投放中包含的可视资源指定有效的长宽比。

>[!TIP]
>
>您可以直接从&#x200B;_[!DNL Content]_体验库中选择批准的广告体验，以准备作为Google Campaign Manager 360创意内容。 从_[!DNL Content]_&#x200B;图库中选择体验后，您便无法编辑资产或将其添加到创意内容。

* **查看您的体验并将其发布到Target频道**。 在创作设置期间使用&#x200B;_预览_&#x200B;面板可在最终激活前评估您选择的广告版面和文本元素。 最终的发布前审核将在目标渠道的广告管理应用程序中进行。 例如，在GenStudio for Performance Marketing中激活元广告体验后，您必须登录到元广告管理器，查看您的创意，然后选择其特定属性，才能发布该体验。

一旦创意内容在其目标付费媒体频道上线，_[!DNL Insights]_就可以跟踪和分析其性能数据。

## 支持的渠道

每个付费媒体渠道都有一个独特的激活工作流。 为激活指南选择付费渠道：

* [元](activate-meta-ad.md)
* [Google Campaign Manager 360](activate-cm360-ad.md)
