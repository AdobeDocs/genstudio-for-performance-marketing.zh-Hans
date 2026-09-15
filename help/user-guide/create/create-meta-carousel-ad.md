---
title: 创建Meta广告体验 — 轮播广告
description: 了解如何在[!DNL GenStudio for Performance Marketing]中创建多信息卡Meta轮播广告体验、管理信息卡并生成品牌内概念。
role: User
source-git-commit: 1b407c1c66a2426b21cbbf423774ebdff16a7dec
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 1%
---

# 创建Meta轮播广告体验

Meta轮播广告是一种付费广告格式，可显示两到十张可滑动卡，每张卡都有自己的图像或视频、标题和链接。

本页介绍特定于轮播广告的步骤。 对于此页不重复的共享步骤，例如选择模板、添加参数、修订变体和发布，请参阅[创建Meta广告体验](/help/user-guide/create/create-meta-ad.md)。

## 先决条件

在创建轮播广告之前，请确保您有一个模板，其所有页面都共享一个纵横比，即1:1或4:5。 每个模板页面会变成一张信息卡。 有关详细信息，请参阅[Meta广告模板准则](/help/user-guide/templates/meta-template.md)。

## 选择轮播格式

选择模板并打开画布后，在提示抽屉中选择轮播格式。

1. 在&#x200B;_[!DNL Create your ads]_面板中，展开_[!UICONTROL &#x200B;参数&#x200B;]_。
1. 从&#x200B;**[!UICONTROL 格式]**&#x200B;下拉菜单中，选择&#x200B;**[!UICONTROL 轮播广告]**。

   ![在“格式”下拉列表设置为“轮播广告”且卡片列表的情况下创建广告面板](./carousel-format-cards.png){width="70%" zoomable="yes"}

如果您从单页模板开始，则[!DNL GenStudio for Performance Marketing]将复制该页面以符合最小两张卡片的要求。 如果模板页面并非都共享一个纵横比，则在使用具有一致纵横比的模板之前，将阻止格式切换。

## 管理信息卡

生成之前，在提示抽屉中构建信息卡集。 要添加更多信息卡，请复制现有信息卡。

* **要复制信息卡**，请从信息卡选项中选择&#x200B;**[!UICONTROL 复制]**。
* **要重新排序卡片**，请通过其手柄将卡片拖动到新位置。
* **要删除卡片**，请从卡片选项中选择&#x200B;**[!UICONTROL 删除]**。 无法删除最后两张信息卡，因为轮播需要至少两张信息卡。

对于每个卡片，选择一个图像，并根据需要设置覆盖父产品的每个卡片产品。 您可以分别为每个信息卡选择一个图像。 稍后会在[!DNL Activate]中设置每张卡的目标URL。 有关详细信息，请参阅[激活Meta广告](/help/user-guide/activation/activate-meta-ad.md)。

## 编写轮播提示

您的提示表示轮播的意图，因此请描述卡片如何相互关联。 轮播复制可以采用以下两种方法之一：

* **模块化：**&#x200B;每张卡都是独立的广告，没有跨卡片的复制流程。 将此方法用于一组相关但独立的消息，如多种产品。
* **顺序：**&#x200B;副本跨卡片连接以讲述故事、逐步序列或操作方法。 当卡片相互构建时，请使用此方法。

您还可以描述轮盘是包含单个产品还是多个产品，以及任何每张卡的详细信息。

例如，此提示将描述一个具有多个产品的模块化轮播：

```properties
Create a multi-product carousel for our end-of-summer skincare sale. For each card, lead with the product's core benefit and emphasize the sale value.
```

此提示描述了一个顺序轮播，该轮播通过五张卡片讲述一个故事：

```properties
Create a narrative carousel for our compliance alert-management platform. Start with shared intro text about the cost of alert fatigue. Across five cards, build the story: rising review costs, too many low-value alerts, false positives as the hidden cost driver, a solution that cuts false positives by more than 50%, and a closing learn-more call to action.
```

有关提示基本信息，请参阅[编写有效提示](/help/user-guide/effective-prompts.md)。

## 生成和审查概念

设置信息卡和提示后，生成轮播并查看结果。

1. 选择&#x200B;**[!UICONTROL 生成]**。

   [!DNL GenStudio for Performance Marketing]生成四个轮播概念。 每个概念都是一个完整的多卡轮播，并具有自己的品牌得分。

   ![四个生成的轮播概念，每个概念具有品牌分数和编辑按钮](./carousel-concepts.png){width="80%" zoomable="yes"}

1. 选择一个概念，然后选择&#x200B;**[!UICONTROL 编辑]**&#x200B;以打开它进行编辑。
1. 使用箭头在信息卡之间移动，然后编辑文本或选择&#x200B;**[!UICONTROL 交换]**&#x200B;以更改信息卡的图像。 有关编辑的详细信息，请参阅[管理变体](/help/user-guide/create/manage-variants.md)。

如果在生成之前对卡片重新排序，则画布会立即更新。 如果在生成后对提示抽屉中的卡片重新排序，则仅在重新生成后才会应用更改，并且会出现再生警告。

## 了解每张卡和共享字段

某些轮播字段单独应用于每个卡片，而其他字段应用于整个广告。 下表描述了每个字段在Meta轮播广告中的行为方式。

| 字段 | 范围 |
|---|---|
| 标题 | 每张卡 |
| 描述 | 每张卡，可选，在[!DNL Activate]中设置 |
| call to action | 在广告中共享 |
| 主文本 | 在广告中共享 |
| 媒体 | 每张卡（图像、视频或混合） |
| 图像上文本 | 每张卡 |
| 目标URL | 每张卡，在[!DNL Activate]中设置 |

## 发布、导出和激活

当轮播准备就绪时，以与其他Meta广告相同的方式发布和导出轮播。 轮播存储为与某个概念对应的单个体验。 导出可提供CSV文件以及卡片介质。 请参阅[[!DNL Content]](/help/user-guide/content/overview.md)以了解已发布体验的存储方式。 若要将轮播激活到Meta，请参阅[激活Meta广告](/help/user-guide/activation/activate-meta-ad.md)。
