---
title: Workfront Proof与审阅和批准集成
description: Workfront Proof与Adobe GenStudio for Performance Marketing集成。
feature: Content Review, Content Management
source-git-commit: f8508ee9440714137141e933cfe0f5761a510c7a
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# Workfront Proof与GenStudio for Performance Marketing集成

与Workfront Proof集成通过高级功能（包括审批模板、多阶段工作流和[比较校对版本](https://experienceleague.adobe.com/en/docs/workfront/using/workfront-proof/work-with-proofs-in-wf-proof/review-proofs-web-proofing-viewer/compare-proofs)）增强了GenStudio for Performance Marketing审阅和审批生命周期。 这种结构化版本控制确保了内容审查生命周期中的透明度、责任制和简化的协作。

>[!BEGINSHADEBOX]

**先决条件**：

安装[Adobe Workfront Web Viewer扩展](https://experienceleague.adobe.com/en/docs/workfront/using/review-and-approve-work/proofing/review-proofs-in-workfront/review-a-proof/review-proof-in-web-viewer-extension)

>[!ENDSHADEBOX]

Workfront Proof的[!DNL Proofing Viewer]是一个丰富的工作区，可用于查看、评论和比较验证。 从[!DNL Proofing Viewer]，您可以

* 比较内容的不同版本
* 向验证添加注释和绘图标记
* 审批证明

当您单击审批请求电子邮件或产品内通知中的校对URL时，[!DNL Proofing Viewer]加载。 [!DNL Proofing Viewer] _我的新审批_&#x200B;视图打开。 在此视图中，您可以使用核心[!DNL Proofing Viewer]注释工具查看内容并提供注释。

要退出[!DNL Proofing Viewer]，请单击&#x200B;**[!UICONTROL 返回到GenStudio]**。

## Genstudio for Performance Marketing and Workfront Proof：功能比较

下表比较了标准GenStudio for Performance Marketing审阅和批准功能与通过Workfront Proof集成提供的更高级功能。

| 功能        | GenStudio for Performance Marketing                                                                 | Workfront Proof                                                                 |
|-------------------------------|------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|
| **草稿/校对生命周期**        | 草稿内容将在发布后过期。 | 基于角色的多阶段审批链，带有时间戳的永久日志。<br>所有版本将无限期保留。 |
| **个评论**                | 评论绑定到草稿ID，并在发布后丢弃。                                           | 保留永久注释和批注以供审核和合规性使用。     |
| **版本**           | 草稿被视为唯一实例。<br>没有并排比较。                                      | 使用并排和叠加比较工具进行完整版本控制。        |
| **项目管理** | 基本营销活动管理。 | 完整的营销活动生命周期管理，包括自定义、模板、报告和详细审核。 |

### 许可证和用户角色

许可证标识产品中的用户权利集合。 Workfront Proof比GenStudio for Performance Marketing提供更多的许可证类型或用户角色。 [验证角色概述](https://experienceleague.adobe.com/en/docs/workfront/using/review-and-approve-work/proofing/proofing-overview/proof-roles)介绍了与Workfront Proof审阅和审批工作流关联的用户角色。

| GenStudio for Performance Marketing许可证       | Workfront许可证                 | 描述                                                                                                                                                      |
|---------------------------------------------------|-----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| GenStudio系统管理器                          | Workfront管理员/超级用户 | 完全访问GenStudio性能营销功能，如品牌、角色和产品管理。 管理工作流和设置。 创建审批模板。 |
| 内容创建者和编辑者（超级用户许可证）   | 校对创建者（标准许可证）  | 生成并提交内容草稿。 在验证查看器中，上传资源并启动验证。 需要Workfront Proof许可证。                              |
| 审阅者/批准者（Collaborator许可证）        | 审阅者/批准者                 | 参与多阶段审阅、添加注释、批准或拒绝内容。                                                                             |

Adobe系统管理员在Adobe Admin Console中管理这两种产品的用户配置和权限。

>[!NOTE]
>
> Workfront Proof还提供[个其他用户角色](https://experienceleague.adobe.com/en/docs/workfront/using/review-and-approve-work/proofing/proofing-overview/proof-roles)。 并非所有角色在Performance Marketing中均可见。 但是，系统会遵循Workfront Proof模板中设置的任何角色。

### 草稿和校样

Workfront [!DNL Proofing Viewer]通过更加结构化的审阅和批准功能，扩展了GenStudio for Performance Marketing的基本审阅和批准流程。 此集成中审查的验证仅限于GenStudio for Performance Marketing支持的格式。

### 版本控制

GenStudio for Performance Marketing不支持审批模板，但Workfront Proof支持。 Proof的版本控制功能显着增强了GenStudio的内容审阅和批准流程。 验证工作流中的每个提交都被视为内容草稿或&#x200B;_验证_&#x200B;的不同版本。 校样会自动保存，并且可与以前的迭代并排比较。 利益相关者可以在整个审核周期中跟踪更改、提供精确反馈并保持一致性。 Proof保留所有评论、决策和版本的完整历史记录，支持审核准备工作和合规性要求。 每个版本还支持基于角色的多阶段审批工作流，每个操作（批准、拒绝或评论）都明确记录并加盖时间戳。

### 审批模板

Workfront Proof审批模板提供了可以简化验证审批工作流的预定义步骤。 这些模板包括选定的审阅人和审批人、验证角色和截止日期，以确保一致性和效率。 启动审阅的内容创建者可以从一组预定义的模板中进行选择，以用于单阶段和多阶段审批工作流。

工作流模板的每个阶段都标识分配的审阅人。 来自Workfront Proof工作流的所有状态更新和注释在校对查看器中可见，从而增强了透明度和协作能力。

批准模板支持多阶段批准，这有助于协调不同利益相关者组的审查。

### 评论

查看者可以直接单击验证的特定区域以留下精确的上下文注释。 所有评论都加盖时间戳，并另存为校样版本历史记录的一部分。 评论历史记录在GenStudio for Performance Marketing中不可用。

您可以[比较两个版本的验证](https://experienceleague.adobe.com/en/docs/workfront/using/workfront-proof/work-with-proofs-in-wf-proof/review-proofs-web-proofing-viewer/compare-proofs)以评估审核评论和内容。

## 通知和提醒

当新验证可供审阅或正在进行的审阅状态已更改时，审阅人和审批人会收到电子邮件通知。
[验证通知和提醒](https://experienceleague.adobe.com/en/docs/workfront/using/workfront-proof/proof-notifications-and-reminders/proof-notifications-and-reminders/proof-notifications-and-reminders)包括验证的个性化链接、有关验证及其审批流程进度的详细信息以及版本控制信息。
