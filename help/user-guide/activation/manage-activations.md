---
title: 管理激活
description: 了解如何使用Adobe GenStudio for Performance Marketing管理激活的体验。
feature: Ad Activation
exl-id: 7cf340d4-37ab-4906-9aad-088a26db0818
TQID: https://experienceleague.adobe.com/ird0IiW8L5Axjj2FmEjlUcD1sPaNCNfxj9XNqGfQWiI
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%
---
# 管理激活

您的激活表显示在[!DNL Activate]登陆页上。 每个表都列出了其广告及其状态：

| 状态 | 含义 |
|---|---|
| [!UICONTROL 需要注意] | 激活表中至少有一个广告的字段缺失或无效，例如不兼容的call to action或重复的跟踪ID。 |
| [!UICONTROL 准备激活] | 激活表中的所有广告都通过验证并准备发布。 |
| [!UICONTROL 挂起] | 整个激活表已提交并由目标平台处理。 |
| [!UICONTROL 已发布] | 已成功发布整个激活表。 |
| [!UICONTROL 失败] | 目标平台拒绝了表中至少有一个广告。 将鼠标悬停在状态工具提示上可查看平台的错误消息。 |

您可以通过单击右上角的&#x200B;**[!UICONTROL 重试]**&#x200B;来自动重试失败的激活。

已发布行会被锁定以防止重新提交，并在目标平台的原生广告管理器中包含指向广告的深层链接，因此您可以直接跳转到该链接以进行查看或启动。

## 详细信息视图

单击广告行可打开其激活详细信息的集中视图。 只读详细信息视图会捕获已激活广告的定义详细信息（包括失败的激活），其中信息派生自GenStudio for Performance Marketing和目标平台：

* **发布时间和日期**：从目标平台发布的时间和日期
* **广告ID**：由目标平台分配并用于跟踪的ID，带有指向平台原生广告管理器中已发布广告的深层链接
* **广告详细信息**：广告使用的已批准资源、副本和元数据
* **平台设置**：用于激活广告的帐户、营销活动和其他平台设置字段

失败的激活的详细信息视图包括失败的原因。
