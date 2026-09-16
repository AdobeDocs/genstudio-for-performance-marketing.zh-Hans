---
title: 激活LinkedIn广告
description: 了解如何激活LinkedIn广告体验。
feature: Ad Activation
exl-id: edc95319-36c3-4cbf-a5c0-865b49482b50
TQID: https://experienceleague.adobe.com/1mcxWePqYd8tYp3e1D2UTSeBHSvPj4WrqeSyiUCxD8c
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
subfeature_v2:
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
    internal-label: Experiences
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%
---
# 激活LinkedIn广告

Adobe GenStudio for Performance Marketing支持将LinkedIn广告体验激活到[LinkedIn营销活动管理器](https://business.linkedin.com/marketing-solutions)。

**支持的格式**：单个图像、单个视频。

您可以在GenStudio for Performance Marketing中[创建一个LinkedIn体验](/help/user-guide/create/create-linkedin.md)，然后选中它进行激活。

激活LinkedIn广告遵循激活其他付费广告渠道所需的[相同常规步骤](create-activation.md)。 本页介绍特定于LinkedIn的先决条件和设置字段。 在GenStudio for Performance Marketing中激活LinkedIn体验后，使用LinkedIn营销活动管理器查看该体验并启动广告。

GenStudio的系统管理员和编辑人员可以激活广告体验。

## 先决条件

* 具有管理营销活动和广告的完全权限的LinkedIn营销活动管理器帐户。 此帐户必须包含现有营销活动。
* 具有在LinkedIn页面上创建广告和发布内容的完全权限的LinkedIn广告帐户。

LinkedIn营销活动管理器中必须已存在目标LinkedIn营销活动和广告集。 GenStudio for Performance Marketing不会创建营销活动或广告集。

>[!NOTE]
>
>LinkedIn重命名了其促销活动层次结构：LinkedIn促销活动管理器以前称为&#x200B;**促销活动组**&#x200B;现在称为&#x200B;**促销活动**，而它以前称为&#x200B;**促销活动**&#x200B;现在称为&#x200B;**广告集**。 [!DNL Activate]中的&#x200B;**[!UICONTROL LinkedIn营销活动]**&#x200B;和&#x200B;**[!UICONTROL LinkedIn广告集]**&#x200B;设置字段使用此当前术语。

GenStudio for Performance Marketing当前支持“单图像”和“单视频”LinkedIn广告，此类广告在每篇帖子中仅包含一个图像或视频。 如果您的体验包含多个纵横比，则[!DNL Activate]会在激活表中为每个纵横比生成一个单独的行，以便每个行都可以作为自己的广告运行；删除您不需要的任何行。

## 连接您的LinkedIn帐户

在您的组织能够激活体验之前，GenStudio系统管理员或编辑器必须将您的LinkedIn广告帐户连接到GenStudio for Performance Marketing。 要成功连接，您必须对广告帐户和LinkedIn配置文件页面具有完全管理员访问权限。 您只需在&#x200B;**[!UICONTROL 设置]**&#x200B;中连接一次广告帐户。 之后，任何有权访问该实例的人都可以访问该实例。

此连接允许数据在GenStudio for Performance Marketing和LinkedIn之间流动，从而启用激活过程。

同步完成后，您可以查看添加的帐户。 大量数据需要更长的时间才能同步。

## LinkedIn设置字段

批准的资产、标题和介绍性文本已锁定，在激活期间无法编辑，因为它们已在[!DNL Content]中经过审阅和批准。 您可以编辑：

* **文本字段**：描述、Call-to-action、目标URL、URL参数、跟踪ID（用作平台广告名称）
* **平台设置字段**： LinkedIn广告帐户、LinkedIn营销活动、LinkedIn广告集
