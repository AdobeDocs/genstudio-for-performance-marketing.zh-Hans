---
title: 激活TikTok广告
description: 了解如何激活TikTok信息源中的视频广告体验。
feature: Ad Activation
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
subfeature_v2:
  - id: d87258a7-722c-4afd-b632-adddc447c7aa
    internal-label: Ad activation
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
source-wordcount: '294'
ht-degree: 1%
---
# 激活TikTok广告

Adobe GenStudio for Performance Marketing支持激活TikTok广告体验。

**支持的格式**：信息源中的视频广告。

您可以[在GenStudio for Performance Marketing中创建TikTok体验](/help/user-guide/create/tiktok-experiences.md)，然后选择它进行激活。

激活TikTok广告时遵循激活其他付费广告渠道所需的[相同常规步骤](create-activation.md)。 本页介绍特定于TikTok的先决条件和设置字段。 在GenStudio for Performance Marketing中激活TikTok体验后，使用TikTok Ads Manager运行最终检查并启动广告。

GenStudio的系统管理员和编辑人员可以激活广告体验。

## 先决条件

* 具有操作员或管理员访问权限的TikTok Ads帐户。
* 至少一个已启用的可使用TikTok广告帐户，由GenStudio系统管理员或编辑器连接。
* TikTok Ads Manager中必须已存在目标TikTok促销活动。 TikTok广告管理器而不是GenStudio for Performance Marketing定义了广告组的预算、竞价、优化和定位。

## 连接您的TikTok帐户

在您的组织激活体验之前，GenStudio系统管理员必须将您的TikTok Ads帐户连接到GenStudio for Performance Marketing：

1. 转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL TikTok]** > **[!UICONTROL 连接]**。
1. 在打开的窗口中登录到您的TikTok广告管理器帐户，并完成OAuth登录。 您的帐户必须具有广告帐户的“操作员”或“管理员”访问权限。

连接完成后，请确认至少启用了一个TikTok广告帐户以供使用。

## TikTok设置字段

批准的资源和主文本已锁定，在激活期间无法编辑，因为它们已在[!DNL Content]中经过审阅和批准。 您可以编辑：

* **文本字段**：Call-to-action、目标URL、跟踪ID（用作平台广告名称）
* **平台设置字段**： TikTok广告帐户、营销活动、广告组
