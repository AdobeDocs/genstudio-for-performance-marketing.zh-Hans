---
title: 创建ChatGPT广告体验
description: 了解如何在Adobe GenStudio for Performance Marketing中创建、审阅、发布和激活ChatGPT付费媒体体验。
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
source-git-commit: 0f5bc2b5416193c01cc4b2fc96d9cb575e209aa3
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 9%

---


# 创建ChatGPT广告体验

在[!DNL GenStudio for Performance Marketing]中使用[[!DNL Create]](/help/user-guide/create/overview.md)生成&#x200B;**ChatGPT广告**&#x200B;作为付费媒体体验 — 从准则和资产到生成、品牌和渠道检查、审批、发布到[!DNL Content]，以及在用于Meta和Google Campaign Manager 360等渠道的相同[!DNL Activate]流中激活。

在开始之前，[根据需要添加准则](/help/user-guide/guidelines/add-guidelines.md)并审阅[有效提示](/help/user-guide/effective-prompts.md)，以使标题提示产生强变体。

## 先决条件

在[!DNL GenStudio for Performance Marketing]中创建或激活ChatGPT广告之前，需要根据这些先决条件进行设置。

### 访问和角色

* 您在[!DNL GenStudio for Performance Marketing]中具有&#x200B;**编辑者**&#x200B;角色或更高版本。 查看[用户角色和权限](/help/user-guide/user-roles.md)。
* 您拥有&#x200B;**OpenAI广告帐户**&#x200B;和来自该帐户的&#x200B;**API密钥**。
* **ChatGPT广告**&#x200B;帐户已连接到[!DNL GenStudio for Performance Marketing]。

要在OpenAI广告管理器中创建API密钥，请执行以下操作：

1. 在OpenAI广告管理器中，转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL API密钥]** > **[!UICONTROL 创建新密钥]**。

要在[!DNL GenStudio for Performance Marketing]中连接ChatGPT广告帐户，请执行以下操作：

1. 在左下角区域，单击&#x200B;**[!UICONTROL 更多]** > **[!UICONTROL 设置]** > **[!UICONTROL ChatGPT]** > **[!UICONTROL 连接]** > **[!UICONTROL 添加帐户]**。
1. 输入OpenAI广告帐户的名称，粘贴您的API密钥，然后单击&#x200B;**[!UICONTROL 添加帐户]**。

当流程成功完成时，您的广告帐户已连接。

### 创建配置

* 已配置&#x200B;**[!DNL Brands]**、**[!DNL Products]**&#x200B;和&#x200B;**[!DNL Personas]**，以便应用程序可以生成品牌内副本。 请参阅[指南概述](/help/user-guide/guidelines/overview.md)。
* 您要使用的图像在[[!DNL Content]](/help/user-guide/content/overview.md)中可用。

## 生成ChatGPT广告

您在[!DNL Create]工作区中创建ChatGPT广告作为付费媒体体验。

### 开始ChatGPT体验

要打开ChatGPT创建，请执行以下操作：

1. 转到&#x200B;**[!UICONTROL 创建]** > **[!UICONTROL ChatGPT]**。 您不为ChatGPT选择模板；将使用单个广告布局。
   创建工作流中的![ChatGPT磁贴](./create-chatgpt-clp.png){width="60%"}
1. 在&#x200B;_画布_&#x200B;中，选择&#x200B;**[!DNL Brand]**、**[!DNL Product]**、**[!DNL Persona]**&#x200B;和&#x200B;**语言**。
1. 从[!DNL Content]中选择图像。
1. 输入ChatGPT标题副本的提示。
1. 单击&#x200B;**[!UICONTROL 生成]**。

[!DNL GenStudio for Performance Marketing] **生成四个**&#x200B;创意变体。

您可以：

* 使用&#x200B;**[!UICONTROL 重新生成]**&#x200B;或&#x200B;**[!UICONTROL 优化]**&#x200B;调整色调、长度或强调。
* 直接在&#x200B;_画布_&#x200B;中编辑文本。
* 使用&#x200B;**[!UICONTROL 交换]**&#x200B;从[!DNL Content]中选择替代图像。

有关编辑生成的体验的更多方法，请参阅[管理变体](/help/user-guide/create/manage-variants.md)。

### 运行品牌和渠道检查

在保存或发送体验以供审阅之前，请根据品牌和渠道规则验证复制和布局。

要运行内容检查，请执行以下操作：

1. 单击&#x200B;**[!UICONTROL 内容检查]**（品牌和渠道检查）。
1. 在&#x200B;[_内容检查_&#x200B;面板](/help/user-guide/guidelines/brand-validation.md#content-check-panel)中查看验证结果。
1. 通过根据需要编辑变体或再生来解决任何标记的问题，例如复制长度或密集的屏幕文本。

请参阅[品牌验证](/help/user-guide/guidelines/brand-validation.md)。

## 在[!DNL GenStudio for Performance Marketing]中保存ChatGPT广告

保存会将您的ChatGPT广告体验移到[!DNL Content]中，以便对其进行审核、重复使用和激活。

有两种状态：

* **草稿体验** — 正在工作且未获得批准。
* **已发布的体验** — 已批准并在[!DNL Content]中可供激活。

### 发送以供审查

1. 在体验标题中，单击&#x200B;**[!UICONTROL 请求审阅]**。
1. 选择批准者（例如，品牌、法律或绩效利益相关者）。
1. 可选：在&#x200B;**[!UICONTROL 设置]**&#x200B;中添加注释。
1. 单击&#x200B;**[!UICONTROL 发送审阅]**。

审批者可以查看ChatGPT体验、品牌和渠道检查结果以及&#x200B;**[!UICONTROL 批准]**&#x200B;或请求更改。

请参阅[请求审阅和批准](/help/user-guide/approvals/request-review.md)和[审阅和批准](/help/user-guide/approvals/overview.md)。

### 发布到内容

在所有必需的审批之后，发布到[!DNL Content]：

1. 单击&#x200B;**[!UICONTROL 发布到内容]**。
1. 确认元数据 — 例如促销活动或激活名称、地区、语言、角色、funnel阶段和&#x200B;**渠道：ChatGPT**。
1. 单击&#x200B;**[!UICONTROL 发布]**。

ChatGPT广告出现在[!DNL Content]中 — 可通过渠道或营销活动等筛选器发现 — 并准备在[!DNL Activate]中进行选择。

查看[发布批准的内容](/help/user-guide/approvals/publish-content.md)和[[!DNL Content] 概述](/help/user-guide/content/overview.md)。

## 激活ChatGPT广告

ChatGPT激活使用与Meta和Google Campaign Manager 360相同的[[!DNL Activate]](/help/user-guide/activation/overview.md)模块。 请参阅[为共享激活工作流创建激活](/help/user-guide/activation/create-activation.md)。

### 启动ChatGPT激活

您可以从[!DNL Content]或[!DNL Activate]开始。

**来自[!DNL Content]**

* 选择一个或多个&#x200B;**已发布** ChatGPT体验。

**来自[!DNL Activate]**

* 打开&#x200B;**ChatGPT**&#x200B;卡并单击&#x200B;**[!UICONTROL +新建]**。

每个体验都映射到&#x200B;**一个** ChatGPT广告。

### 配置体验设置

对于每个选定的体验，请确认：

* **标题**
* **正文**
* **目标URL** — 必须使用有效的`https://`格式（例如`https://www.example.com`）。

### 配置平台设置

选择ChatGPT广告管理器详细信息：

* **OpenAI广告帐户**
* **ChatGPT营销活动** — 必须已存在于OpenAI广告管理器中。
* **ChatGPT广告组** — 必须已存在于OpenAI广告管理器中。
* **ChatGPT广告名称** — 每个ChatGPT广告有一个不同的名称。

### 审阅并发布

1. 查看所有创意和平台详细信息。
1. 单击&#x200B;**[!UICONTROL 发布]**。

[!DNL GenStudio for Performance Marketing]在&#x200B;**不活动**&#x200B;状态下将广告推送到ChatGPT广告管理器，以便您的媒体团队与其他付费渠道一样，控制最终启动时间和预算。 请参阅[激活概述](/help/user-guide/activation/overview.md)。

### 发布后发生的情况

* **正在发布**&#x200B;模式随即出现并自动关闭。
* 您将被重定向到&#x200B;**ChatGPT激活**&#x200B;表，其中列出了最新激活。 处理完成时状态显示&#x200B;**[!UICONTROL 挂起]**。
* 您可以在发布完成时导航离开。

处理完成时：

* 确认弹出窗口显示&#x200B;**成功**&#x200B;或&#x200B;**失败**。
* 如果单击弹出窗口或在激活表中打开ChatGPT激活，则会看到&#x200B;**详细信息**&#x200B;页面。
* 如果激活&#x200B;**[!UICONTROL 失败]**，则表显示该状态并显示ChatGPT的错误消息。

在OpenAI广告管理器中，媒体团队可以运行最终检查，并在准备就绪后使广告或广告组处于活动状态。
