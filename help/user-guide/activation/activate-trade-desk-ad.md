---
title: 在交易台激活广告
description: 了解如何向交易台激活静态显示广告体验。
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
source-wordcount: '461'
ht-degree: 0%
---
# 激活交易台广告

Adobe GenStudio for Performance Marketing支持向交易台激活广告体验。

**支持的格式**：静态显示（仅限单个资产）。

在交易台激活广告时，请遵循激活其他付费广告渠道所需的[相同常规步骤](create-activation.md)，但有一个区别。 由于交易台是一项受管理的企业服务，而不是自助服务和平台，因此帐户访问的工作方式与其他渠道不同。 本页介绍了这些差异，以及特定于交易台的先决条件和设置字段。

GenStudio的系统管理员和编辑人员可以激活广告体验。

## 先决条件

* 一个现有的、实时的交易台帐户。 在将其连接到GenStudio for Performance Marketing之前，请直接在交易台中设置此项。
* 交易台帐户团队已启用API访问。 对于交易台，您的帐户团队使用API令牌（而不是其他付费广告渠道使用的OAuth登录）代表您启用此访问权限。
* 由The Trade Desk为GenStudio for Performance Marketing集成启用的正确广告商、名额和权限。
* 交易台帐户团队提供的API令牌或凭据，具有将创意发布到目标广告商帐户的权限。
* 交易台中已存在的目标营销活动。 GenStudio for Performance Marketing会将广告激活到该现有营销活动中。

## 连接您的交易台帐户

在贵组织激活体验之前，请与您的交易台帐户团队合作以启用API访问，然后GenStudio系统管理员将该帐户连接到GenStudio for Performance Marketing：

1. 请联系您的交易台帐户团队，并请求访问权，以将创意内容从GenStudio for Performance Marketing发布到您的交易台帐户。 确认激活时要使用的广告商ID、名额或合作伙伴详细信息。
1. 从交易台帐户团队获取API令牌或凭据，并确认该令牌支持目标广告商帐户的创意发布权限。
1. 在GenStudio for Performance Marketing中，转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 渠道]**，然后单击&#x200B;**[!UICONTROL 交易台]**&#x200B;磁贴上的&#x200B;**[!UICONTROL 连接]**。 输入帐户名称、广告商ID以及API令牌或凭据，然后保存连接。

如果连接失败，请与您的交易台客户团队确认，已启用API访问，并且令牌具有正确的广告商和客户座权限。

## 交易台设置字段

批准的资产已锁定，在激活期间无法编辑，因为它们已在[!DNL Content]中经过审阅和批准。 您可以编辑：

* **文本字段**：跟踪ID（用作平台创意名称）
* **平台设置字段**：帐户、营销活动

目前，对Trade Desk的激活仅支持单一资产静态显示广告。
