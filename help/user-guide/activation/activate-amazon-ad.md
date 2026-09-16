---
title: 激活Amazon广告
description: 了解如何激活Amazon广告体验。
feature: Ad Activation
exl-id: 539cb43c-a9d8-4473-8a7d-e81967111741
TQID: https://experienceleague.adobe.com/4L4JHcYLSsoQ50QbCW7Mof52h5jpz3z8n0UL8CaqLA8
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
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%
---
# 激活Amazon广告

Adobe GenStudio for Performance Marketing支持将广告体验激活到Amazon广告。

**支持的格式**：静态显示。

激活Amazon广告体验时，遵循激活其他付费广告渠道所需的[相同常规步骤](create-activation.md)。 本页介绍特定于Amazon Ads的先决条件和设置字段。 在GenStudio for Performance Marketing中激活体验后，使用Amazon广告查看体验并启动广告。

GenStudio的系统管理员和编辑人员可以激活广告体验。

## 先决条件

* 访问目标Amazon Ads帐户。
* 具有该帐户的管理员访问权限，可读取和写入Amazon Ads。

Amazon Ads在不同帐户中组织营销活动和广告，每个帐户都包含一个创意库。 Target帐户必须已存在于Amazon Ads中；GenStudio for Performance Marketing将广告体验发布到该帐户的创意库中，但不创建帐户。

## 连接您的Amazon Ads帐户

GenStudio系统管理员必须先将您的Amazon Ads帐户连接到GenStudio for Performance Marketing，贵组织才能在创意库中发布资产。 您必须拥有该帐户的管理员访问权限才能阅读和写入Amazon Ads。 查看[连接付费媒体帐户](/help/user-guide/connectors/connect-channel.md)。

同步完成后，您可以查看添加的帐户。

## Amazon Ads设置字段

批准的资产已锁定，在激活期间无法编辑，因为它们已在[!DNL Content]中经过审阅和批准。 您可以编辑：

* **文本字段**：跟踪ID（用作平台创意名称）
* **平台设置字段**：帐户

激活完成后，您的创意体验将会交付到Amazon Ads中的选定帐户创意库。
