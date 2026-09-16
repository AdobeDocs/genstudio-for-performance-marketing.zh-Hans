---
title: 激活Meta广告
description: 了解如何激活Meta广告体验。
feature: Ad Activation
exl-id: 157df612-a774-422c-bca3-2fde9e9d1c88
TQID: https://experienceleague.adobe.com/hDR0ngNiGnCXCCOgNhVG8gX4kHGrNvfybPbuMLwYk7U
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
    internal-label: Guidelines
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
source-wordcount: '382'
ht-degree: 0%
---
# 激活Meta广告

Adobe GenStudio for Performance Marketing支持将Meta广告体验激活到Instagram和Facebook。

**支持的格式**：图像、视频、轮播。

[在GenStudio for Performance Marketing中创建Meta体验](/help/user-guide/create/create-meta-ad.md)，然后将其选中以进行激活。

激活Meta广告时遵循激活其他付费广告渠道所需的[相同常规步骤](create-activation.md)。 本页介绍特定于Meta的先决条件和设置字段。 在GenStudio for Performance Marketing中激活Meta体验后，使用[Meta广告管理器](https://adsmanager.facebook.com/)查看体验并启动广告。

与某些其他渠道不同，Meta广告可以在单个广告中包含多个长宽比。 如果您的体验具有多个纵横比，则[!DNL Activate]仍只为其生成一行，而不是为每个纵横比生成一行。

GenStudio的系统管理员和编辑人员可以激活广告体验。

## 先决条件

确认您连接的Meta广告帐户拥有在Meta广告平台的以下组件中管理广告的完全权限：

* Meta广告帐户
* Facebook页面
* Meta营销活动
* Meta广告集
* Instagram个人资料（可选）

Meta Ads Manager中必须已存在目标Meta促销活动和广告集。 GenStudio for Performance Marketing当前不创建营销活动或广告集。

## 连接您的Meta帐户

在您的组织能够激活体验之前，GenStudio系统管理员必须将您的Meta帐户连接到GenStudio for Performance Marketing。 通过此连接，数据可以在GenStudio for Performance Marketing和Meta之间流动，从而启用激活过程。 请参阅[连接到Meta Ads](/help/user-guide/connectors/meta-ads.md)。

要选择Instagram帐户，请确保在Meta Business Manager中[要使用的Instagram帐户连接到新用户引导期间选择的相同广告帐户](/help/user-guide/connectors/meta-ads.md#connect-an-instagram-account)。 如果缺少此连接，则在激活期间Instagram帐户可能不会显示在&#x200B;**[!UICONTROL Instagram配置文件]**&#x200B;下拉菜单中。

同步完成后，您可以查看添加的帐户。 大量数据需要更长的时间才能同步。

## Meta设置字段

批准的资产、标题和正文已锁定，在激活期间无法编辑，因为它们已在[!DNL Content]中经过审阅和批准。 您可以编辑：

* **文本字段**：描述、Call-to-action、目标URL、URL参数、跟踪ID（用作Meta广告名称）
* **平台设置字段**：广告帐户、Facebook页面、Instagram个人资料、Meta促销活动、Meta广告集
