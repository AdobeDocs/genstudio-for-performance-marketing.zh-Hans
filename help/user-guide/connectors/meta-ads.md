---
title: 连接到元广告
description: 连接元广告帐户，以通过Adobe GenStudio for Performance Marketing激活和监控您的广告和媒体。
level: Intermediate
role: Admin, Data Engineer
recommendations: noDisplay
feature: Reporting and Insights
source-git-commit: 2f18b273684a9fe9b9b8903838ae09f5cd2b7842
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 0%

---

# 连接到元广告

将您的元广告配置文件帐户连接到GenStudio for Performance Marketing以管理营销活动、导出内容并访问活动营销活动的广告数据。

>[!BEGINSHADEBOX]

**先决条件**：

- 可访问所有元服务的Facebook/Meta登录

- 对元业务Portfolio和广告帐户&#x200B;_完全控制_，包括：

   - 管理营销活动
   - 查看性能
   - 管理Creative中心模型
   - 高级分析

- 删除浏览器中的所有弹出窗口阻止程序

>[!ENDSHADEBOX]

**要连接元广告帐户**：

1. 单击&#x200B;**[!UICONTROL 更多]** > **[!UICONTROL 设置]**。

1. 在&#x200B;_Data Connectors_&#x200B;部分中，单击&#x200B;_中继广告_&#x200B;卡上的&#x200B;**[!UICONTROL 连接]**。

1. 登录到您的Facebook帐户。

   您可能需要删除弹出窗口阻止程序，然后使用&#x200B;**[!UICONTROL 刷新]**&#x200B;重试。

1. 按照Facebook身份验证说明进行操作，验证帐户信息，然后单击&#x200B;**[!UICONTROL 继续为……]**

1. 在&#x200B;_[!UICONTROL Facebook Login for Business]_(Meta到Adobe符号)中，逐步完成以下选择以授予GenStudio for Performance Marketing访问权限：

   - 选择一个或多个元企业配置文件并单击&#x200B;**[!UICONTROL 继续]**
   - 选择一个或多个元页面并单击&#x200B;**[!UICONTROL 继续]**
   - 选择一个或多个Instagram帐户并单击&#x200B;**[!UICONTROL 继续]**
   - 查看选择并单击&#x200B;**[!UICONTROL 保存]**

     ![审核选择](/help/assets/meta/meta-review-selections.png "审核选择"){width="400" zoomable="yes"}

1. 收到帐户已连接的验证后，单击&#x200B;**[!UICONTROL 获得]**。

   此步骤可确保GenStudio for Performance Marketing获得对所有广告、元数据和量度的访问权限，以实现最佳性能。

1. 在&#x200B;_[!UICONTROL 元广告]_&#x200B;中，选择要包含在[!DNL Insights]中的一个或多个帐户，然后单击&#x200B;**[!UICONTROL 选择]**。

1. 收到&#x200B;_连接的平台_&#x200B;确认后，请单击&#x200B;**[!UICONTROL 查看帐户]**。

   _[!UICONTROL 元广告帐户]_&#x200B;视图列出了`Account name`、`Added by`、`Date added`和`Status`。

   ![元帐户列表](/help/assets/meta/meta-accounts-list.png "连接的元帐户列表"){zoomable="yes"}

使用&#x200B;**[!UICONTROL 添加帐户]**&#x200B;向列表中添加更多帐户。 当您添加链接到同一元业务配置文件的帐户时，授权流程可能会略有不同。 在连接过程中，只选择新的元广告帐户。
