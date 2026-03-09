---
title: 分发您的应用程序
description: 为GenStudio for Performance Marketing分发您的应用程序或加载项。
feature: Extensibility
exl-id: 4935356b-08df-402c-b1a2-b89627afc188
TQID: https://experienceleague.adobe.com/6SHsqsafwqCWS3dspM65BTVAqZ09WwW2IxF-PIecINE
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 303
ht-degree: 0%

---

# 分发您的应用程序

分发加载项可使其可供您的组织和其他人使用。 您的分发工作流程取决于您的加载项是用于公共分发还是专用分发。

本主题讨论专用分发。 专用分发将加载项部署限制在由IMS组织标识的组织中。

公共分发使加载项作为Adobe Exchange上的应用程序提供。[_App Builder_&#x200B;开发人员文档中的公共分发](https://developer.adobe.com/app-builder/docs/guides/distribution/public/)介绍了如何使您的应用程序可供任何Adobe组织使用。

>[!BEGINSHADEBOX]

**先决条件**：

确认以下权限：

* 您从中提交应用程序以供审批的组织中的开发人员权限

* 审批应用程序的系统管理员权限

必须在App Builder项目中部署您的App Builder应用程序。

>[!ENDSHADEBOX]

**要私密分发您的应用程序**：

专用分发使您的应用程序仅对贵组织的成员可用。

1. 从[Adobe Developer Console](https://developer.adobe.com/console/)中，选择部署应用程序的组织、项目和工作区。

1. 从&#x200B;_Workspace概述_&#x200B;区域中选择&#x200B;**[!UICONTROL 审批]**。 _应用程序审批_&#x200B;窗格打开。

1. 在&#x200B;_应用程序提交详细信息_&#x200B;区域，添加有关加载项的信息性详细信息。 详细信息包括应用程序名称、描述和联系人电子邮件。

1. 完成所有字段后，单击&#x200B;**[!UICONTROL 提交]**。

1. 使用您用来登录Adobe Exchange的相同Adobe ID登录到[Developer Console](https://exchange.adobe.com/)。 如果您在此组织中没有系统管理员权限，请向组织系统管理员请求审批。

1. 选择&#x200B;**[!UICONTROL 管理]** > **[!UICONTROL App Builder应用程序]**&#x200B;以访问审阅该应用程序的请求。

1. 查看应用程序后，选择&#x200B;**[!UICONTROL 批准]** 。 您还可以添加信息性注释。

您的加载项现已显示在贵组织的GenStudio for Performance Marketing实例中。
