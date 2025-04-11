---
title: 连接付费媒体
description: 连接渠道帐户，以通过Adobe GenStudio for Performance Marketing激活和监控您的广告和媒体。
level: Intermediate
role: Admin, Data Engineer
feature: Reporting and Insights
exl-id: e699041e-b462-45b3-8c4c-4de0d52cf0e6
source-git-commit: 2844914d25d9bc3a2be7f47d0cd7f26f7c921555
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---

# 连接付费媒体帐户

_[!DNL Data connectors]_支持GenStudio for Performance Marketing与您的付费媒体网络帐户之间的无缝集成。 通过连接到第三方渠道帐户，您可以交换关键数据，例如[[!DNL Insights]](/help/user-guide/insights/overview.md)中的促销活动绩效指标，并且可以通过[[!DNL Activate]](/help/user-guide/activation/overview.md)投放新的广告位置。 通过此集成，GenStudio for Performance Marketing可以管理您的媒体和广告，同时从您的活跃营销活动中接收有价值的见解，包括展示次数、点击次数和转化次数。

**连接到付费媒体帐户**：

1. 单击省略号&#x200B;**[!UICONTROL ...左下角导航中的More]**。

1. 使用齿轮图标选择&#x200B;**[!UICONTROL 设置]**。

1. 在&#x200B;_[!UICONTROL 设置]_&#x200B;中，从&#x200B;_[!UICONTROL Data Connectors]_&#x200B;部分中选择连接器类型，然后单击&#x200B;**[!UICONTROL 连接]**。

   或者，如果存在已连接的帐户，您可以单击&#x200B;_已连接的帐户_&#x200B;以查看帐户名称、详细信息和状态的列表。

1. 查看您选择的[连接器类型](#connector-types)，查看先决条件，并继续执行连接步骤。

## 付费媒体连接

GenStudio for Performance Marketing支持使用各种连接器类型与您的首选营销平台集成。 每种连接器类型都有特定的先决条件和设置步骤，需要完成这些步骤才能成功连接。

### 元广告连接

>[!BEGINSHADEBOX]

**先决条件**：

- Facebook/元广告帐户
- 访问具有`View performance`权限级别的元广告帐户，以访问报告和查看广告
- 删除浏览器中的所有弹出窗口阻止程序

>[!ENDSHADEBOX]

**要连接元广告帐户**：

1. 在&#x200B;_Data Connectors_&#x200B;部分中，单击&#x200B;_中继广告_&#x200B;卡上的&#x200B;**[!UICONTROL 连接]**。

1. 登录到您的Facebook帐户。

   您可能需要删除弹出窗口阻止程序，然后使用&#x200B;**[!UICONTROL 刷新]**&#x200B;重试。

1. 按照Facebook身份验证说明操作。

1. 在&#x200B;_[!UICONTROL Facebook企业登录]_&#x200B;弹出窗口(Meta到Adobe符号)中，逐步完成以下选择。

   - 验证帐户信息，然后单击&#x200B;**[!UICONTROL 继续作为]**
   - 授予对选定页面的访问权限，然后单击&#x200B;**[!UICONTROL 继续]**
   - 向选定的企业授予访问权限，然后单击&#x200B;**[!UICONTROL 继续]**
   - 选择加入一个或多个Instagram帐户并单击&#x200B;**[!UICONTROL 继续]**
   - 查看选择并单击&#x200B;**[!UICONTROL 保存]**

1. 在&#x200B;_[!UICONTROL 元广告]_&#x200B;视图中，选择一个或多个帐户并单击&#x200B;**[!UICONTROL 选择]**。

_[!UICONTROL 元广告帐户]_&#x200B;视图列出了`Account name`、`Added by`、`Date added`和`Status`。 使用&#x200B;**[!UICONTROL 添加帐户]**&#x200B;向列表中添加更多帐户。

## 数据摄取

最初，GenStudio for Performance Marketing会导入最近六个月的历史数据。 这种做法可确保您立即获得相关见解，以分析趋势、评估绩效和做出明智决策。 摄取过程可能需要一到五天，具体取决于您帐户中的数据量。

>[!BEGINSHADEBOX]

**数据摄取和保留策略**

GenStudio for Performance Marketing会将渠道数据保留13个月。 此保留策略包括在初始连接期间摄取的6个月的数据，从而确保全面的历史数据分析和报告。

>[!ENDSHADEBOX]
