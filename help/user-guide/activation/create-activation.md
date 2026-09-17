---
title: 激活工作流
description: 了解广告体验的激活工作流。
feature: Ad Activation
exl-id: 17e1bade-d52a-4953-a85c-c10d093e73d6
TQID: https://experienceleague.adobe.com/HSwFeL1qCzgFao2Ii64Hx-kaADRnd3dxaswFMzJ7nfA
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
    internal-label: Insights
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
    internal-label: Guidelines
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
    internal-label: Assets
  - id: dd48f9df-f2e2-49fe-a918-332a8e240ffe
    internal-label: Channels
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: c8d964aa325aee782c175abf3fce880fb17ae6ca
workflow-type: tm+mt
source-wordcount: '1250'
ht-degree: 1%
---
# 激活工作流

[!DNL Activate]将发布的体验激活到其付费广告平台。 GenStudio for Performance Marketing体验是一种营销活动组件（如广告），为付费广告平台上的特定受众做准备。 激活体验包含三个主要组件：

* **媒体资产**：广告体验中的图像或视频，其文件类型和长宽比因平台和格式而异。

* **文本**：广告中包含的所有形式的副本，包括标题、正文文本和call-to-action元素。

* **元数据**：用户定义的属性，通常对广告受众不可见，可增强性能分析、筛选和跟踪。

在激活之前，您可以在[!DNL Content]中准备并批准这些组件。 [!DNL Activate]不会创建或编辑已批准的资产、标题或正文。 它只应用每个平台所需的设置，然后发布体验。

单个激活表可以包含多个付费广告平台和广告格式的体验。

>[!VIDEO](https://video.tv.adobe.com/v/3503538?learn=on)

## 连接您的平台帐户

GenStudio系统管理员或编辑器必须连接每个付费广告平台的广告帐户，然后才能将体验激活到该平台。 要查看此进程的步骤，请参阅[连接付费媒体帐户](/help/user-guide/connectors/connect-channel.md)。

## 开始激活

从以下两个入口点之一开始激活：

* **从[!DNL Content]**：筛选到体验，选择一个或多个已发布的体验，然后单击顶部操作栏上的&#x200B;**[!UICONTROL 激活]**。

  ![在“内容”中选择已发布的体验，然后单击“激活”以开始激活](./images/content-select-activate.png)

* **从[!DNL Activate]**：在[!DNL Activate]登陆页面上，单击&#x200B;**[!UICONTROL +新激活]**。 这将打开同一体验库，您可以在其中选择要激活的体验。

无论属于哪种情况，都可按体验名称搜索，或按多个渠道进行筛选以查找所需的体验。

如果您的选择包括显示格式体验，请指定要使用的显示平台：Google Campaign Manager 360、Innovid、Amazon Ads或交易台。 然后单击&#x200B;**[!UICONTROL 开始激活]**。 对于其他格式，如Meta、LinkedIn、TikTok、YouTube和ChatGPT，[!DNL Activate]推断来自体验渠道的平台并跳过此步骤。

[!DNL Activate]随后生成一个激活表，其中列出了您选择的所有体验。

![新生成的激活表已分组到Meta和LinkedIn子表中，每个标记为“需要”的广告需要注意，直到其字段完成](./images/activation-table.png)

[!DNL Activate]按广告格式和平台将表组织为子表，例如Meta单个图像或LinkedIn单个图像。 每一行表示一个广告。 对于大多数平台（如LinkedIn、TikTok和显示平台），具有多个长宽比的体验会为每个长宽比生成一行；删除您不需要的任何行。 Meta是个例外。 Meta广告可以在单个广告中包含多个长宽比，因此多长宽比Meta体验仍只会生成一行。

## 管理您的激活表

激活表在打开时自动另存为草稿。 您可以在发布之前随时离开并继续草稿。

若要向已打开的激活表添加更多体验，请单击表右上角的&#x200B;**[!UICONTROL 添加更多体验]**。 这将重新打开体验库，以便您能够选择[!DNL Activate]添加到现有表中的其他体验。

**[!UICONTROL 添加更多体验]**&#x200B;还允许您激活到同一表中的多个显示平台。 显示格式体验会要求您首先选择单个显示平台，但您可以单击&#x200B;**[!UICONTROL 添加更多体验]**，选择更多显示格式体验，并选择与表格中已有的显示平台不同的显示平台。 例如，您可以将交易台广告添加到已包含Innovid广告的表中。

您的表格具有正确的体验后，请接下来配置每个广告的字段。

## 配置广告和平台设置详细信息

编辑每行内嵌的字段，或选择同一格式表中的多行，然后单击工具栏上的&#x200B;**[!UICONTROL 编辑详细信息]**，该工具栏似乎可以同时批量编辑这些字段。

![在激活表中选择多个广告以批量编辑详细信息或平台设置](./images/bulk-edit-action-bar.png)

批准的资产、标题和正文已锁定，无法在激活表中编辑，因为它们已在[!DNL Content]中经过审阅和批准。 其余字段可以编辑，并且因平台而异。 [!DNL Activate]仅显示与您选择的平台和格式相关的列。 使用下表作为每个平台可编辑内容的参考。

**可按平台编辑的字段**

| 平台 | 支持的格式 | 锁定的副本 | 可编辑的文本字段 | 可编辑的平台设置字段 |
|---|---|---|---|---|
| Meta | 图像、视频、轮播 | 标题，正文 | 描述、Call-to-action、目标URL、URL参数、跟踪ID | 广告帐户、Facebook页面、Instagram个人资料、Meta促销活动、Meta广告集 |
| LinkedIn | 单个图像、单个视频 | 标题，介绍性文本 | 描述、Call-to-action、目标URL、URL参数、跟踪ID | 广告帐户、营销活动、广告集 |
| Google Campaign Manager 360 | 静态显示、视频显示、HTML5 Zip显示 | 不适用 | 跟踪Id | 广告商 |
| Amazon Ads | 静态显示 | 不适用 | 跟踪Id | 帐户 |
| 无病毒 | 静态显示、HTML5 Zip显示 | 不适用 | 跟踪Id | 帐户， Creative库，概念名称 |
| TikTok | 信息源内视频广告 | 主文本 | call-to-action，目标URL，跟踪ID | 广告帐户、营销活动、广告组 |
| YouTube | Google中的Shorts Ads Demand Gen促销活动 | 描述 | call-to-action、业务名称、目标URL、URL参数、跟踪ID | 帐户、营销活动、广告组、徽标 |
| ChatGPT | 聊天卡 | 标题、正文 | 目标URL，跟踪ID | OpenAI广告帐户、OpenAI营销活动、OpenAI广告组 |
| 交易台 | 静态显示 | 不适用 | 跟踪Id | 帐户、营销活动 |

要为一组广告格式配置平台设置字段，请单击&#x200B;**[!UICONTROL 管理平台设置]**&#x200B;并编辑结果对话框中的字段。

![用于选择Meta广告帐户、营销活动和广告集的“管理平台设置”对话框](./images/manage-platform-settings.png)

**[!UICONTROL 跟踪ID]**&#x200B;字段最初为空。 跟踪ID与广告平台的广告名称或创意名称相同，且广告平台会将其用作广告的标识名称。 使用此字段可标识该广告，以用于报告和疑难解答。 在&#x200B;**[!UICONTROL 跟踪ID]**&#x200B;字段中输入要使用的值。

![正在编辑激活表中内联的跟踪ID字段](./images/tracking-id-edit.png)

若要更快地在&#x200B;**[!UICONTROL 跟踪ID]**&#x200B;字段之间移动，请使用以下键盘快捷键：

* 按&#x200B;**Enter**&#x200B;打开所选&#x200B;**[!UICONTROL 跟踪ID]**&#x200B;的编辑字段。
* 按&#x200B;**向上**&#x200B;或&#x200B;**向下**&#x200B;箭头键移至该列的上一个或下一个&#x200B;**[!UICONTROL 跟踪ID]**&#x200B;字段。
* 再次按&#x200B;**Enter**&#x200B;保存您的编辑。

## 查看您的体验并将其发布到他们的广告平台

确认每一行都显示[!UICONTROL 准备激活]。 [!DNL Activate]标记缺少字段或字段无效、不兼容的操作调用以及重复的跟踪ID为[!UICONTROL 需要注意]。 当每行都就绪时，单击&#x200B;**[!UICONTROL 发送到平台]**&#x200B;并在发布对话框中确认。

![每个行都显示“准备激活”的激活表，启用“发送到平台”](./images/ready-to-activate.png)

[!DNL Activate]近乎实时地报告每个广告的状态：“待定”、“发送到平台”或“失败”。 如果广告失败，请将鼠标悬停在其状态上以查看平台的错误。 您可以通过单击&#x200B;**[!UICONTROL 重试]**&#x200B;来一次重试表中的每个失败广告，而不是分别重试每个广告。 已发送到平台的行会被锁定以防止重新提交，并在目标平台的原生广告管理器中包含指向广告的深层链接。 您的最终发布前审核和启动广告会在目标平台自己的广告管理器中进行： [!DNL Activate]始终以非活动状态投放广告。

![显示发布后“待处理”和“发送到平台”状态的混合激活表](./images/activation-status-pending.png)

您的激活表显示在[!DNL Activate]登陆页上。

## 支持的平台

每个付费广告平台都有特定的设置字段和先决条件。 为激活指南选择付费广告平台：

* [Meta](activate-meta-ad.md)
* [LinkedIn](activate-linkedin-ad.md)
* [Google Campaign Manager 360](activate-cm360-ad.md)
* [Amazon广告](activate-amazon-ad.md)
* [无](activate-innovid-ad.md)
* [TikTok](activate-tiktok-ad.md)
* [YouTube](activate-youtube-ad.md)
* [ChatGPT](activate-chatgpt-ad.md)
* [交易台](activate-trade-desk-ad.md)
