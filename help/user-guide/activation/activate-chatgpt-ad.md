---
title: 激活ChatGPT广告
description: 了解如何激活ChatGPT广告体验。
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
source-wordcount: '272'
ht-degree: 0%
---
# 激活ChatGPT广告

Adobe GenStudio for Performance Marketing支持激活ChatGPT广告体验。

**支持的格式**：聊天卡。

您可以[在GenStudio for Performance Marketing中创建ChatGPT体验](/help/user-guide/create/create-chatgpt-ad.md)，然后选择它进行激活。

激活ChatGPT广告遵循激活其他付费广告渠道所需的[相同常规步骤](create-activation.md)。 本页介绍特定于ChatGPT的先决条件和设置字段。 在GenStudio for Performance Marketing中激活ChatGPT体验后，使用OpenAI广告管理器运行最终检查并启动广告。

GenStudio的系统管理员和编辑人员可以激活广告体验。

## 先决条件

* OpenAI广告帐户以及该帐户的API密钥。
* OpenAI广告管理器中必须已存在目标ChatGPT营销活动和广告组。 GenStudio for Performance Marketing不会创建新的促销活动或广告组。

## 连接您的ChatGPT帐户

在您的组织能够激活体验之前，GenStudio系统管理员必须将您的OpenAI广告帐户连接到GenStudio for Performance Marketing：

1. 在OpenAI广告管理器中，转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL API密钥]** > **[!UICONTROL 创建新密钥]**。
1. 在GenStudio for Performance Marketing中，转到&#x200B;**[!UICONTROL 更多]** > **[!UICONTROL 设置]** > **[!UICONTROL ChatGPT]** > **[!UICONTROL 连接]** > **[!UICONTROL 添加帐户]**。
1. 输入OpenAI广告帐户的名称，粘贴您的API密钥，然后单击&#x200B;**[!UICONTROL 添加帐户]**。

## ChatGPT设置字段

批准的资产、标题（标题）和正文已锁定，在激活期间无法编辑，因为它们已在[!DNL Content]中通过了审阅和批准。 您可以编辑：

* **文本字段**：目标URL、跟踪ID（用作平台广告名称）
* **平台设置字段**： OpenAI广告帐户、OpenAI营销活动、OpenAI广告组

目标URL必须使用有效的`https://`格式，例如`https://www.example.com`。
