---
title: 激活Google Campaign Manager 360广告
description: 了解如何激活Google促销活动管理器360体验。
feature: Ad Activation
exl-id: e4ee4e04-8dd0-4e05-a0f7-0ddca2fbb6be
TQID: https://experienceleague.adobe.com/pQbT2OC7-jK33HhJWgTBBtJrmEvr48mGkl8v-fTkOLQ
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
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%
---
# 激活Google Campaign Manager 360广告

Adobe GenStudio for Performance Marketing支持将广告体验激活到Google Campaign Manager 360。

**支持的格式**：静态显示、视频显示、HTML5 Zip显示。

激活Google Campaign Manager 360广告时遵循激活其他付费广告渠道所需的[相同常规步骤](create-activation.md)。 本页介绍特定于Google Campaign Manager 360的先决条件和设置字段。 在GenStudio for Performance Marketing中激活体验后，使用Google Campaign Manager 360查看体验并启动广告。

GenStudio的系统管理员和编辑人员可以激活广告体验。

## 先决条件

* 有权访问目标广告商的Google Campaign Manager 360帐户。
* 对广告商的管理员访问权限，可读取和写入Campaign Manager 360。

Campaign Manager 360在不同广告商中组织活动和广告，每个广告商都包含一个创意库。 目标广告商必须已存在于Campaign Manager 360中；GenStudio for Performance Marketing将广告体验发布到该广告商的创意库中，但不创建广告。

## 连接您的Google Campaign Manager 360帐户

GenStudio系统管理员或编辑者必须先将您的Google Campaign Manager 360帐户连接到GenStudio for Performance Marketing，然后您的组织才能在创意库中发布资产。 您必须具有广告商的管理员访问权限才能读写到Campaign Manager 360。 查看[连接付费媒体帐户](/help/user-guide/connectors/connect-channel.md)。

同步完成后，您可以查看添加的帐户。

## Google Campaign Manager 360设置字段

批准的资产已锁定，在激活期间无法编辑，因为它们已在[!DNL Content]中经过审阅和批准。 您可以编辑：

* **文本字段**：跟踪ID（用作平台创意名称）
* **平台设置字段**：广告商

激活完成后，您的创意体验将会交付到Google Campaign Manager 360中的选定广告商创意库。
