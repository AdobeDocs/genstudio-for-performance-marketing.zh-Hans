---
title: 连接到Meta Ads
description: 连接Meta Ads帐户以通过Adobe GenStudio for Performance Marketing激活和监控您的广告和媒体。
level: Intermediate
role: Admin, Data Engineer
recommendations: noDisplay
feature: Reporting and Insights
exl-id: 78110edf-947b-4e05-a3f1-de4b1eabda44
source-git-commit: fb5fe4885340639f8179c8de6944ac21bfe009ec
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

# 连接到Meta Ads

本页介绍如何将您的Meta广告配置文件帐户关联并管理到GenStudio for Performance Marketing，以便管理营销活动、导出内容并访问活跃营销活动的广告数据。

>[!BEGINSHADEBOX]

**先决条件**：

- 可访问所有Meta服务的Facebook/Meta登录

- _完全控制_ Meta商业Portfolio和广告帐户，包括：

   - 管理营销活动
   - 查看性能
   - 管理Creative中心模型
   - 高级分析

- 在浏览器中禁用任何弹出窗口阻止程序

>[!ENDSHADEBOX]

## 连接Meta ads帐户

1. 单击&#x200B;**[!UICONTROL 更多]** > **[!UICONTROL 设置]**。

1. 在&#x200B;_Data Connectors_&#x200B;部分中，单击&#x200B;**[!UICONTROL Meta Ads]**&#x200B;卡上的&#x200B;_连接_。

1. 登录到您的Facebook帐户。

   您可能需要删除弹出窗口阻止程序，然后使用&#x200B;**[!UICONTROL 刷新]**&#x200B;重试。

1. 按照Facebook身份验证说明进行操作，验证帐户信息，然后单击&#x200B;**[!UICONTROL 继续为……]**

1. 在&#x200B;_[!UICONTROL Facebook企业登录]_ (Meta到Adobe符号)中，逐步完成以下选择以授予GenStudio for Performance Marketing访问权限：

   - 选择一个或多个Meta业务配置文件并单击&#x200B;**[!UICONTROL 继续]**
   - 选择一个或多个Meta页面并单击&#x200B;**[!UICONTROL 继续]**
   - 选择一个或多个Instagram帐户并单击&#x200B;**[!UICONTROL 继续]**
   - 查看选择并单击&#x200B;**[!UICONTROL 保存]**

     ![审核选择](/help/assets/meta/meta-review-selections.png "审核选择"){width="400" zoomable="yes"}

1. 收到帐户已连接的验证后，单击&#x200B;**[!UICONTROL 获得]**。

   此步骤可确保GenStudio for Performance Marketing获得对所有广告、元数据和量度的访问权限，以实现最佳性能。

1. 在&#x200B;_[!UICONTROL Meta广告]_&#x200B;中，选择要包含在[!DNL Insights]中的一个或多个帐户，然后单击&#x200B;**[!UICONTROL 选择]**。

1. 收到&#x200B;_连接的平台_&#x200B;确认后，请单击&#x200B;**[!UICONTROL 查看帐户]**。

   _[!UICONTROL Meta广告帐户]_&#x200B;视图列出了`Account name`、`Added by`、`Date added`和`Status`。

   ![Meta帐户列表](/help/assets/meta/meta-accounts-list.png "连接的Meta帐户列表"){zoomable="yes"}

使用&#x200B;**[!UICONTROL 添加帐户]**&#x200B;向列表中添加更多帐户。 当您添加链接到同一Meta商业用户档案的帐户时，授权流程可能会略有不同。 在连接过程中，您只能选择新的Meta Ads帐户。

## 断开Meta Ads集成并排除其故障

有时GenStudio for Performance Marketing实例未正确连接到Meta广告帐户。 可能导致问题的常见设置包括：

- 选择Instagram帐户时没有选择与其关联的Facebook页面
- 已撤销执行初始连接的用户的权限

在这些情况下，最好将Meta广告帐户重新连接到GenStudio for Performance Marketing实例。 首先，用户必须直接从其Meta Business Manager中删除应用程序集成，从而为重置权限创建一个全新的平台。 这需要管理员访问Meta Business Manager。

以下步骤清除缓存的权限并重置集成流：

1. 通过访问Facebook网站访问[Meta Business Manager](https://business.facebook.com)。
1. 使用您的帐户登录。 该帐户必须具有对Business Manager的管理员访问权限。
1. 单击左下角的&#x200B;**[!UICONTROL 设置]**&#x200B;代码图标以导航到您的Business Portfolio设置。
1. 在左侧菜单中，单击&#x200B;**[!UICONTROL 集成]**。
1. 选择&#x200B;**[!UICONTROL 连接的应用程序]**。 您将在连接的应用程序列表中看到Adobe GenStudio。
   ![Meta Business Manager连接应用](./meta-connected-apps.png "Meta Business Manager连接应用窗格")
1. 单击应用程序名称。
1. 单击&#x200B;**[!UICONTROL 删除]**。
1. 出现提示时，确认删除。

您现在可以重新连接Meta广告帐户、Instagram个人资料和Facebook页面。
