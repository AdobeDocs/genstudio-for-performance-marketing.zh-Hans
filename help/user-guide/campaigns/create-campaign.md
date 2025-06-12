---
title: Adobe GenStudio for Performance Marketing Campaigns
description: 了解如何创建和管理利用创作AI资源和体验的数字营销活动。
feature: Campaign Planning, Campaign Brief
badgeBeta: label="Beta" tooltip="此功能当前位于Beta中，因此某些功能可能会受到限制或发生更改。"
exl-id: b7c4194f-fa61-4739-acd6-7acbdd98e9b2
source-git-commit: 5279caaf4651ed81c3cf3d8a4de2f17c3f151ec8
workflow-type: tm+mt
source-wordcount: '859'
ht-degree: 0%

---

# 创建营销活动

GenStudio for Performance Marketing营销活动定义关键的数字营销活动特征，并随着部署和评估阶段而发展。 GenStudio for Performance Marketing支持启动营销活动、跟踪各个营销活动组件的性能以及根据性能量度重新调整广告体验焦点的动态过程。

促销活动的关键元素存储在促销活动对象中，这将为所有标记为相同唯一促销活动名称的资源和体验创建一个共享上下文。 此标签在整个GenStudio for Performance Marketing中标识营销活动。

GenStudio系统管理员和GenStudio编辑人员可以创建营销活动。

## 定义营销活动详细信息

{{$include /help/_includes/campaign-details.md}}

**要输入促销活动详细信息**，请执行以下操作：

1. 从[!DNL Campaigns]，单击&#x200B;**[!UICONTROL 添加营销活动]**。 将打开&#x200B;_创建营销活动_&#x200B;视图。

   详细信息包括定义营销策划的可选和必填字段。 这些详细信息将作为营销活动的元数据属性保存在[!DNL Campaigns]中。

1. 双击&#x200B;_New campaign_&#x200B;标题并输入信息性的唯一名称。

   此名称会成为GenStudio for Performance Marketing中的&#x200B;_营销活动标签_，从而允许您在上传和创建期间将资源或体验与该营销活动关联。

1. 在描述您的促销活动的&#x200B;_详细信息_&#x200B;字段中输入值。 请参阅&#x200B;_促销活动详细信息_&#x200B;表，了解这些促销活动功能的定义。

## 分配渠道和区域

渠道和区域设置确定营销活动的部署位置及其分发渠道。

GenStudio for Performance Marketing使用名为&#x200B;_记录_&#x200B;的预定义模板来表示关键促销活动组件，如渠道、地区、角色和产品。 创建营销策划时，需将其与每个组件的相关记录相关联。

* **渠道设置** — 定义营销活动的公共分发渠道，包括付费媒体帐户、电子邮件营销服务和显示广告网络。 有关这些渠道中促销活动、资产和体验性能的数据将馈送到[[!DNL Insights]](/help/user-guide/insights/overview.md)，以进行特定于渠道的分析。

* **区域设置** — 指定部署营销活动的地理区域。 通过连接到区域数据源，GenStudio for Performance Marketing可以根据本地受众偏好定制内容和策略。 这样可基于区域量度进行更准确的定位和性能分析。

**要为您的营销活动选择分发渠道**：

1. 单击&#x200B;**[!UICONTROL 渠道]**&#x200B;旁边的+号（**[!UICONTROL 连接记录+]**）。

   将打开&#x200B;_选择渠道_&#x200B;弹出窗口。

1. 选择部署营销活动的渠道。 有效值包括`Email`、`Paid media`、`Web`和`Display ads`。

   （可选）选择&#x200B;**[!UICONTROL 查看全部]**&#x200B;以打开所有受支持通道的视图。

**要为您的营销活动分配地区**：

1. 单击&#x200B;**[!UICONTROL 区域]**&#x200B;旁边的+号（**[!UICONTROL 连接记录+]**）。

   将打开&#x200B;_选择区域_&#x200B;弹出窗口。 您可以搜索特定的受支持区域。

1. 为您的营销活动选择一个或多个目标区域。 有效区域包括`AMER`、`LATAM`、`EMEA`、`APAC`和`Japan`。

   （可选）选择&#x200B;**[!UICONTROL 查看全部]**&#x200B;以打开所有受支持区域的视图。

## 分配角色和产品

[角色](/help/user-guide/guidelines/personas.md)和[产品](/help/user-guide/guidelines/products.md)保存为记录。 角色记录定义了特定客户区段的特征，即所生成内容的目标受众。 其中可能包括人口统计细节和客户交互的历史记录。

产品记录根据您的品牌指南定义关键产品规范和属性。 属性可以包括您的品牌中的功能、相关图像和产品定位。

_角色_&#x200B;和&#x200B;_产品_&#x200B;下拉菜单中的选项在组织级别定义。 在创建营销活动时，您可以从这些预定义记录中进行选择，以确保一致的产品表示并支持准确定位、消息传送和性能跟踪。

**要为营销活动分配角色**：

1. 单击&#x200B;**[!UICONTROL 角色]**&#x200B;旁边的+号（**[!UICONTROL 连接记录+]**）。

   将打开&#x200B;_选择角色_&#x200B;弹出窗口。 您可以搜索特定的受支持角色。

1. 选择您的营销活动要定位的角色。 有效角色由您的组织在[准则创建](/help/user-guide/guidelines/personas.md)期间定义。

   （可选）选择&#x200B;**[!UICONTROL 查看全部]**&#x200B;以打开所有可用角色的视图。

**要将产品分配给营销活动**：

1. 单击&#x200B;**[!UICONTROL 产品]**&#x200B;旁边的+号（**[!UICONTROL 连接记录+]**）。

   将打开&#x200B;_选择产品_&#x200B;弹出窗口。 您可以搜索特定的受支持产品。

1. 选择一个或多个产品。 产品由您的组织在[指南创建](/help/user-guide/guidelines/products.md)期间定义。

   （可选）选择&#x200B;**[!UICONTROL 查看全部]**&#x200B;以打开所有可用产品的视图。

## 完成营销活动创建

单击&#x200B;**[!UICONTROL 创建]**&#x200B;以保存输入的值并创建营销活动。

新的营销活动名称现已在[!DNL Content]和[!DNL Create]中作为营销活动标签提供。 您可以通过[!DNL Content]向营销活动添加批准的资源和体验，或在内容创建期间向营销活动分配资源和体验。

## 向营销活动添加内容

GenStudio for Performance Marketing使用存储在[!DNL Content]元数据中的促销活动标签将内容链接到促销活动。 单个内容可以与多个营销活动关联。

营销活动标签标识营销活动及其属性。 为资源或体验分配标签会将其连接到相应的营销策划。

**从[!DNL Content]**&#x200B;添加资源和体验：

1. 从[!DNL Content] _体验_&#x200B;或&#x200B;_Assets_&#x200B;库中，选择批准的体验或资源。

1. 从&#x200B;_详细信息_&#x200B;视图中，从&#x200B;_营销活动_&#x200B;下拉菜单中选择营销活动的名称。

**要在内容创建期间添加资源和体验**：

在内容创建期间，您可以将新创建的资源或体验发布到[!DNL Content]。

1. 从&#x200B;_确认已批准内容的详细信息_&#x200B;弹出窗口中，从&#x200B;_营销活动_&#x200B;下拉菜单中选择一个营销活动。

1. 单击&#x200B;**[!UICONTROL 发布]**。

此营销活动现在可在&#x200B;_营销活动_&#x200B;功能板中使用。
