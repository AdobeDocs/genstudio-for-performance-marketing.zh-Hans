---
title: 激活无痕广告
description: 了解如何激活无痕体验。
feature: Ad Activation
exl-id: ebb2aa9e-8efb-45b0-9ba2-7b27b8888708
TQID: https://experienceleague.adobe.com/VTzk2CDlTqawM1ckdHPVzs2ES-y0Ui0mkOLnVD88bJk
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
    internal-label: Insights
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
    internal-label: Assets
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
    internal-label: Experiences
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%
---
# 激活无痕广告

Adobe GenStudio for Performance Marketing支持将广告体验激活为Innovid。

**支持的格式**：静态显示、HTML5 Zip显示。

激活无痕体验遵循激活其他付费广告渠道所需的[相同常规步骤](create-activation.md)。 本页介绍特定于Innovid的先决条件和设置字段。 在GenStudio for Performance Marketing中激活体验后，使用Innovid查看体验并启动广告。

GenStudio的系统管理员和编辑人员可以激活广告体验。

## 先决条件

* 访问目标Innovid帐户
* 管理员可以访问该帐户，以对Innovid进行读写操作。

Innovid在不同帐户中组织营销活动和广告，每个帐户都有一个创意库。 Innovid中必须已存在目标创意库；GenStudio for Performance Marketing将广告体验发布到该创意库中，但不创建帐户或创意库。

## 连接您的无名帐户

在您的组织能够在创意库中发布资产之前，GenStudio系统管理员必须将您的无病毒帐户连接到GenStudio for Performance Marketing。 您必须拥有该帐户的管理员访问权限才能在Innovid中读取和写入。 查看[连接付费媒体帐户](/help/user-guide/connectors/connect-channel.md)。

同步完成后，您可以查看添加的帐户。

## 无设置字段

批准的资产已锁定，在激活期间无法编辑，因为它们已在[!DNL Content]中经过审阅和批准。 您可以编辑：

* **文本字段**：跟踪ID（用作平台创意名称）
* **平台设置字段**：帐户、Creative库、概念名称

激活完成后，您的创意体验将以无忧状态交付到选定的创意库。
