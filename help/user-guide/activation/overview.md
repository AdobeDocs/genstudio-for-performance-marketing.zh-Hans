---
title: 激活概述
description: 了解如何使用Adobe CX企业版和第三方应用程序激活内容。
level: Beginner
feature: Ad Activation
exl-id: 365fe253-d189-467e-a723-f54cd74ff60b
TQID: https://experienceleague.adobe.com/-Nal0YqjTzKw4g2SM3IuMf0a13e87CWdTqBZPd0dBkU
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
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%
---
# Adobe GenStudio for Performance Marketing激活

在GenStudio for Performance Marketing [!DNL Activate]中，您可以准备广告体验并将其发送到付费广告渠道，如Meta或LinkedIn。 _激活_&#x200B;采用批准的广告体验及其资源，应用特定渠道所需的设置，然后以非活动、关闭状态直接将其交付给该渠道。 从那里，您可以在广告上线之前，在渠道自己的广告经理中进行最终审核。

[!DNL Activate]将您的体验直接提供给渠道，因此您无需导出文件或手动将文件上传到渠道自己的广告管理器。

GenStudio系统管理员或编辑器必须连接每个付费广告渠道的广告帐户，然后才能将广告体验激活到该渠道。

## 激活功能

使用[!DNL Activate]为其目标付费广告渠道准备广告体验。 在单个激活表中[跨多个付费广告渠道批量激活体验](create-activation.md)。 然后，[管理您的激活](manage-activations.md)以查看每个激活体验的状态和详细信息。

>[!VIDEO](https://video.tv.adobe.com/v/3503546?captions=chi_hans&learn=on)

### 从内容激活已批准的体验

从[!DNL Content]中选择一个或多个已批准、已发布的体验，或从[!DNL Activate]登陆页面开始操作。 与[!DNL Activate]的早期版本不同，单个激活表可以同时包含按广告格式和渠道组织的多个付费广告渠道的体验。

>[!NOTE]
>
>[!DNL Content]在&#x200B;**channel**&#x200B;中调用Meta或LinkedIn等目标。 [!DNL Activate]调用同一目标的&#x200B;**平台**（例如，在&#x200B;**[!UICONTROL 平台设置]**&#x200B;中）。 这两个术语指的是一样的。

### 配置广告和平台设置详细信息

激活表中的每一行代表一个广告。 已获批准的创意资产、标题和正文已锁定，因为它们已获得审阅和批准。 您可以编辑其余字段，如call-to-action文本、目标URL和平台设置详细信息，如广告帐户、营销活动和广告集。 一次编辑一行的字段，或选择多行以批量编辑共享字段。

### 审核您的体验并将其发布到其广告渠道

确认每一行都显示[!UICONTROL 准备激活]。 [!DNL Activate]标记缺少字段或字段无效、不兼容的操作调用以及重复的跟踪ID为[!UICONTROL 需要注意]。 当每行都就绪时，单击&#x200B;**[!UICONTROL 发送到平台]**&#x200B;以发布表中的所有广告。 [!DNL Activate]近乎实时地报告每个广告的状态，并且成功发布的广告包含指向目标平台原生广告管理器中广告的深层链接。 失败的广告返回错误消息，可重试。
