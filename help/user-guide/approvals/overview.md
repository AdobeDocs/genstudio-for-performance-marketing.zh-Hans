---
title: Adobe GenStudio for Performance Marketing审阅和批准
description: 了解GenStudio for Performance Marketing审核和批准流程。
level: Beginner
feature: Content Review, Content Management
exl-id: c83f47c0-e8ae-4c54-84b3-c50f67d6b3c2
source-git-commit: 7955796949c17f7cd877b115cba45c58cdd614a7
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 0%

---

# Adobe GenStudio for Performance Marketing审阅和批准

审查和批准工作流程确保所有利益相关者（从创意团队到法律专家）都能高效地审查和批准活动资源和体验，包括创意人工智能生成的品牌资产。

>[!NOTE]
>
> 此功能也作为与Adobe Workfront Proof[&#128279;](/help/user-guide/approvals/proof-integration.md)的集成提供。 此集成在GenStudio for Performance Marketing画布中提供验证功能。 通过Workfront Proof集成，GenStudio for Performance Marketing获得更加结构化、透明和协作的审核流程，帮助团队更自信、更明确地从草稿走向最终。

## 审核和批准工作流的优势

* **支持稳健的迭代生成AI内容创建**。 在组织中创建和部署品牌一致的内容是一个非常反复的过程。 GenStudio for Performance Marketing的创作AI功能支持快速创建数百种资源变体。 每个审核者在批准资产草稿之前，可能会请求对资产草稿进行多项更改。 审核者越多，在所有利益相关者就最终变体达成一致之前，潜在的迭代次数越多。

* **支持创意完整性**。 批准通过让内容创建者参与批准过程，保护品牌资产的创意完整性。 通过让创意利益相关者（例如，内容创建者和创意总监）参与审阅和批准流程，您可以确保最终输出符合您的愿景和品牌识别。

* **遵守活动目标和法律要求**。 审批流程有助于验证内容是否支持活动目标。 它确保所有营销材料都符合法律和法规标准，从而最大程度地降低风险和潜在法律问题。

* **与Adobe Workfront Proof集成**。 用户可以从GenStudio for Performance Marketing中访问Workfront Proof强大的审核和批准功能。 在GenStudio for Performance Marketing中审阅的内容会同步到Workfront Proof，并且审阅评论和状态会保留。 [集成亮点](/help/user-guide/approvals/proof-integration.md)识别Proof如何扩展GenStudio for Performance Marketing的审批工作流。

## 审核和批准生命周期

审阅和批准工作流程的主要阶段包括：

* [请求审阅和批准您创建的内容](/help/user-guide/approvals/request-review.md)。 GenStudio for Performance Marketing简化了请求批准和管理批准者的流程。 Workfront Proof批准模板可以进一步简化此任务。

* [审阅和编辑内容](/help/user-guide/approvals/review-and-edit.md)。 通知使内容创建者与请求的更改和批准保持同步。 修订内容会触发新的自动审批周期。

* [批准内容](/help/user-guide/approvals/approve-content.md)。 指定的批准者将内容标记为已批准或准备发布。

* [发布内容](/help/user-guide/approvals/publish-content.md)。 将批准的内容发布到[!DNL Content]后，组织中的其他人便可以使用或引用该内容。

## 关于内容草稿

_草稿_&#x200B;是尚未完成审阅和批准过程的资产或体验的初步版本。 草稿状态标识草稿处于审阅和批准流程中的位置。 唯一的草稿ID可标识每个草稿。 此ID在草稿获得批准并发布到[!DNL Content]之前有效。 草稿的审阅评论和批准与此单个草稿ID关联。 GenStudio内容草稿没有版本控制。

当草稿完成审阅和批准流程并发布到[!DNL Content]时，草稿ID将过期。 GenStudio for Performance Marketing不会保存关联的评论和审批状态。 草稿URL不再有效。

草稿状态捕获内容草稿在审核和批准流程中的状态。 创建受审核资产的GenStudio for Performance Marketing内容编辑者会收到通知，告知您对草稿或审批进行了任何请求的更改。 审批人更改草稿状态以指明草稿是需要进一步修订还是可以批准。 所有指定的批准者必须批准资产或体验，然后才能发布。

可用草稿状态：

**通知**：内容编辑者已通知审批者草稿已准备好进行审阅，从而开始了审阅和审批流程。
**需要工作**：指示一个或多个批准者已请求对内容草稿进行更改。 无法将此状态下的内容保存到[!DNL Content]。
**已批准**：所有指定的批准者均已批准该资产或体验。 内容编辑者现在可以将元数据添加到资源或体验并将其保存到[!DNL Content]。

>[!NOTE]
>
> 草稿对应于Workfront Proof集成用户的&#x200B;_验证_。 [草稿和校样](/help/user-guide/approvals/proof-integration.md#drafts-and-proofs)在持久性和版本控制方面有所不同。

## 审批角色

_审阅人_&#x200B;可以添加评论，但不能批准内容。 审阅者的参与很有帮助，但并非至关重要。 _审批者_&#x200B;必须先审批内容，然后才能通过审批流程。 Workfront Proof集成支持更广泛的用户角色。

## 通知

GenStudio for Performance Marketing产品内通知会实时更新审批者和内容编辑器，以更新资源状态更改和`@mention`备注。 通知支持在多个审阅、编辑和批准周期中快速迭代。

内容编辑者和批准者可以注册以在Slack中接收这些通知。 请参阅[在Experience Cloud中订阅服务](https://experienceleague.adobe.com/en/docs/core-services/interface/services/customer-attributes/subscription)。

批准参与者执行的操作会触发自动产品内通知和电子邮件通知。 开始审批流程时，指定的审批者会收到电子邮件和产品内通知。 每当审批者添加`@mention`评论或做出决定时，您就会与产品内通知和电子邮件通知保持同步。 通知包括指向内容草稿的链接。

如果您启动了内容的审阅和批准流程，您将收到所有批准和审阅注释的通知。 但是，审批者仅会收到包含他们且带有`@mention`的注释的通知。
