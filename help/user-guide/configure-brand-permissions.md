---
title: 分配 [!DNL Brand] 权限
description: 了解如何为GenStudio for Performance Marketing [!DNL Brand] 创建者和编辑者分配权利。
level: Intermediate
feature: Brand Personalization, Generative AI
exl-id: fc33ecd3-4403-4045-87af-012a0377226c
source-git-commit: 8ed591795cee157760159cca6e899cab15792252
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 1%

---

# 分配[!DNL Brand]权限

默认情况下，GenStudio系统管理员可以创建并编辑[!DNL Brands]。 内容编辑者和协作者角色具有编辑和创建权限，但可能不需要任何系统管理权限。

要授予内容编辑者和协作者这些与[!DNL Brand]相关的权限，Adobe系统管理员必须在Adobe Admin Console中执行一些其他配置任务。 请参阅[企业和团队管理指南](https://helpx.adobe.com/cn/enterprise/using/admin-console.html#Overview)中的&#x200B;_Adobe Admin Console_。

添加用户和用户组是所有具有通过Admin Console管理的权限的Adobe产品所共有的基本任务。 有关用户管理和添加用户和用户组的过程的概述，请参阅[企业和团队管理指南](https://helpx.adobe.com/cn/enterprise/using/users.html)中的&#x200B;_Adobe Admin Console用户_。

观看本视频演练或执行以下步骤。

>[!VIDEO](https://video.tv.adobe.com/v/3470499/?learn=on&enablevpops)

## 第1步：创建用户组

**创建用户组**：

1. 登录到Admin Console并导航到&#x200B;**[!UICONTROL 用户]** > **[!UICONTROL 用户组]**。

1. 单击&#x200B;**[!UICONTROL 新建用户组]**。 将打开&#x200B;_创建新用户组_&#x200B;弹出窗口。

1. 向&#x200B;**[!UICONTROL 用户群组名称]**&#x200B;字段添加一个信息性用户群组名称，以标识新群组的用途。 例如，“品牌经理”。

1. （可选）添加组及其用途的说明。

1. 单击&#x200B;**[!UICONTROL 保存]**。Admin Console将打开带有新创建组的名称的&#x200B;_新建组_&#x200B;弹出窗口。

请参阅[企业和团队管理指南](https://helpx.adobe.com/cn/enterprise/using/user-groups.html)中的&#x200B;_管理用户组_。

## 步骤2：将GenStudio系统管理器配置文件分配给用户组

创建新用户组并添加用户后，您可以将&#x200B;**Adobe GenStudio系统管理员**&#x200B;配置文件分配给此组。 与已分配配置文件关联的权利授予该组GenStudio中的所有用户[!DNL Brands]权限（创建、更新和删除品牌）。

**要将配置文件分配给用户组**：

1. 导航到新创建的用户组，然后单击&#x200B;_已分配的产品配置文件_&#x200B;选项卡。

1. 在&#x200B;_已分配的产品配置文件_&#x200B;选项卡中，单击&#x200B;**[!UICONTROL 分配配置文件]**。 将打开&#x200B;_分配产品和配置文件_&#x200B;弹出窗口。

1. 从`Adobe GenStudio`选择产品&#x200B;_列表中选择_。

1. 单击&#x200B;**[!UICONTROL 应用]**。 将打开&#x200B;_选择产品配置文件_&#x200B;弹出窗口，显示与Adobe GenStudio关联的产品配置文件。

1. 选择 `Adobe GenStudio system manager`。

1. 单击&#x200B;**[!UICONTROL 应用]**。 将打开&#x200B;_分配产品和配置文件_&#x200B;弹出窗口，显示新创建的用户组的产品配置文件。

1. 单击&#x200B;**[!UICONTROL 保存]**。

请参阅[企业和团队管理指南](https://helpx.adobe.com/cn/enterprise/using/user-groups.html)中的&#x200B;_将产品配置文件分配给用户组_。

## 第3步：将用户添加到用户组

要向用户分配创建、编辑和发布[!DNL Brands]的权限，请将其添加到新创建的用户组。

>[!NOTE]
>
>您必须先将至少一个用户添加到此用户组，然后才能将组添加到项目中。

**要将用户添加到用户组**：

1. 从&#x200B;_Admin Console_，导航到&#x200B;**[!UICONTROL 用户]** > **[!UICONTROL 用户组]**。

1. 选择您之前创建的用户组的名称。 打开&#x200B;_将用户添加到此用户组_&#x200B;弹出窗口。

1. 通过用户名或电子邮件地址添加新用户或现有用户。 为现有用户输入名称或电子邮件地址时，将自动为属于此IMS组织的已知用户填充匹配名称。 了解如何在[企业和团队管理指南](https://helpx.adobe.com/cn/enterprise/using/user-groups.html)的&#x200B;_管理用户组_&#x200B;中管理用户组。

添加到组时，用户将获得Adobe GenStudio系统管理员的[!DNL Brand]创建、编辑和发布权限。 用户还会收到自动发送的电子邮件邀请，以编辑Adobe GenStudio for Performance Marketing [!DNL Brands]项目。

## 步骤4：创建[!DNL Brands]项目

_项目_&#x200B;提供了一个存储位置，选定的用户可以在该位置保存资源，在本例中为[!DNL Brands]个资源。

**从[!DNL Brands]存储&#x200B;_选项卡_创建**&#x200B;项目：

1. 导航到Admin Console中的&#x200B;_存储_&#x200B;选项卡。

1. 单击侧面导航中的&#x200B;**[!UICONTROL 项目]**。 _项目_&#x200B;选项卡打开。

1. 单击&#x200B;**[!UICONTROL 创建项目]**。 将打开&#x200B;_新建项目_&#x200B;弹出窗口。

1. 在项目名称字段中输入`Adobe GenStudio Brands`。 输入与此处显示的完全相同的项目名称。 请勿包含额外的空格或更改字母大小写。

1. 单击&#x200B;**[!UICONTROL 创建]**。_邀请加入项目_&#x200B;弹出窗口打开。

请参阅[企业和团队管理指南](https://helpx.adobe.com/cn/enterprise/using/projects-in-business-storage.html)中的&#x200B;_管理项目_。

## 步骤5：邀请用户组加入项目

您现在可以将刚刚创建的用户组添加到`Adobe GenStudio [!DNL Brands]`项目。

**邀请用户组加入新创建的项目**：

1. 从&#x200B;_邀请加入项目_&#x200B;弹出窗口中，将刚刚创建的用户组添加到此项目。

1. 选择&#x200B;**可以编辑**&#x200B;权限选项。

1. 单击&#x200B;**[!UICONTROL 邀请]**。
