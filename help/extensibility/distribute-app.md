---
title: 分发您的应用程序
description: 为GenStudio for Performance Marketing分发您的应用程序或加载项。
feature: Extensibility
exl-id: 4935356b-08df-402c-b1a2-b89627afc188
source-git-commit: 6ba402e9cdfb62d71c9993457a6d9952c4877553
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---

# 分发您的应用程序

分发加载项后，您的组织和他人便可以使用该加载项。您的分发工作流程取决于您的加载项是用于公共分发还是专用分发。

本主题讨论专用分发。 专用分发将加载项部署限制在由IMS组织标识的组织中。

公共分发使加载项作为Adobe Exchange上的应用程序提供。 [App Builder](https://developer.adobe.com/app-builder/docs/guides/distribution/public/)开发人员文档中的&#x200B;_公共分发_&#x200B;介绍了如何使您的应用程序可供任何Adobe组织使用。

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

1. 从[!UICONTROL Workspace概述]区域中选择&#x200B;_审批_。 _应用程序审批_&#x200B;窗格打开。

1. 在&#x200B;_应用程序提交详细信息_&#x200B;区域，添加有关加载项的信息性详细信息。 详细信息包括应用程序名称、描述和联系人电子邮件。

1. 完成所有字段后，单击[!UICONTROL 提交]。

1. 使用您用来登录Adobe Exchange的相同Adobe ID登录到[Developer Console](https://exchange.adobe.com/)。 如果您在此组织中没有系统管理员权限，请向组织系统管理员请求审批。

1. 选择[!UICONTROL 管理] > [!UICONTROL App Builder应用程序]以访问审阅该应用程序的请求。

1. 查看应用程序后，选择[!UICONTROL 批准]。 您还可以添加信息性注释。

您的加载项现已显示在贵组织的GenStudio for Performance Marketing实例中。
