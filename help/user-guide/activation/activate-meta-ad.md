---
title: 激活元广告
description: 了解如何激活元广告体验。
feature: Ad Activation
exl-id: 157df612-a774-422c-bca3-2fde9e9d1c88
source-git-commit: 2d43b1b3373c5ed0b80d9740906d372955816831
workflow-type: tm+mt
source-wordcount: '1908'
ht-degree: 1%

---

# 激活元广告

Adobe GenStudio for Performance Marketing支持将元广告体验激活到Instagram和Facebook。

您可以在GenStudio for Performance Marketing中[创建元体验](/help/user-guide/create/create-meta-ad.md)并选择它进行激活，或在[!DNL Activate]中利用批准的资源构建新体验。

激活元广告遵循激活其他付费渠道所需的[相同常规步骤](create-activation.md)。 激活过程支持根据Meta的特定要求准备您的广告体验。 在GenStudio for Performance Marketing中激活元体验后，使用[元广告管理器](https://adsmanager.facebook.com/)在最终发布之前优化特定元广告投放的体验。

GenStudio的系统管理员和编辑人员可以激活广告体验。

## 步骤1：设置元帐户

在启动激活之前，[登录到元](https://adsmanager.facebook.com/)以访问您的元广告管理器帐户。

>[!BEGINSHADEBOX]

**先决条件**：

确认您连接的元广告帐户拥有在元广告平台的以下组件中管理广告的完全权限：

* Facebook页面
* 元营销活动
* 元广告集
* Instagram个人资料（可选）

>[!ENDSHADEBOX]

## 步骤2：连接到您的元帐户

在您的组织能够激活体验之前，GenStudio系统管理员必须将您的元帐户连接到GenStudio for Performance Marketing。 利用此连接，数据可在GenStudio和外部营销工具（如Meta）之间流动，从而启用激活过程。

查看[连接到元广告](/help/user-guide/connectors/meta-ads.md)。

同步完成后，您可以查看添加的帐户。 大量数据需要更长的时间才能同步。

## 步骤3：准备激活体验

您可以通过两种方式启动激活：

* **直接从[!DNL Content]**&#x200B;激活。 选择具有预定义设置的已批准体验是启动对单个渠道的激活的最简化方式。

* **从[!DNL Activate] > _体验设置_**&#x200B;收集您的广告体验。 您可以通过从[!DNL Content]中选择可视资产、添加文本元素以及选择长宽比来创建体验。 此方法包含更多步骤，但在创作创意体验时可提供更大的灵活性。

### 从内容激活已批准的体验

您可以选择多个体验来激活到单个付费渠道。 在继续激活之前，系统可能会要求您选择平台。

如果您选择了多个体验作为组激活，请使用左侧边栏将&#x200B;_体验设置_&#x200B;视图焦点置于所选体验的详细信息。

1. 使用[!DNL Content]图库的搜索和筛选工具识别要激活的体验，然后单击&#x200B;**[!UICONTROL 激活]**。

   将打开此体验的元广告&#x200B;_体验设置_&#x200B;页面。 该界面中已预填充所选体验的详细信息。 您可以编辑&#x200B;**[!UICONTROL Call-to-action]**、**[!UICONTROL 网站URL]**&#x200B;和&#x200B;**[!UICONTROL 显示链接]**&#x200B;字段。 如果您选择激活多个体验，_体验设置_&#x200B;视图将包含一个左侧边栏，其中显示所有选定体验的缩略图。 使用此左侧边栏将&#x200B;_体验设置_&#x200B;视图的焦点置于所选体验的详细信息。

1. 从&#x200B;**[!UICONTROL 营销活动]**&#x200B;下拉菜单中选择一个营销活动。

   如果您使用多个体验，请在左侧边栏上切换体验，直到您完成每个体验的准备为止。

1. 单击&#x200B;**[!UICONTROL 下一步]**&#x200B;确认您的元广告设置。

1. 为每个体验分配一个名称。 激活后，您可以使用此名称在&#x200B;_激活的体验_&#x200B;表中搜索此体验。

### 组合体验组件

如果选择不直接从[!DNL Content]激活已批准的体验，则可以选择资源、分配长宽比和草稿文本元素。

**要为激活准备体验**：

1. 在[!DNL Activate]中，单击代表您选择的付费渠道的图标上的&#x200B;**[!UICONTROL 新建]**。 将打开&#x200B;_体验设置_&#x200B;视图。

   _体验设置_&#x200B;页面提供了一个用于准备广告激活的中心位置。 准备广告包括以下三个任务：

1. 为您的体验分配一个名称。 激活后，您可以使用此名称在&#x200B;_激活的体验_&#x200B;表中搜索此体验。
1. 选择媒体资源。 您可以使用[!DNL Content]中的资源或上传外部资源(例如，从OneDrive或Dropbox)。
1. [添加文本](#add-ad-text)。
1. [添加元数据](#assign-metadata)。

   _预览面板_&#x200B;支持在特定广告投放的上下文中以交互方式查看您的文本和资源。 使用&#x200B;_选择投放位置_&#x200B;下拉菜单在支持的广告投放位置之间切换。 预览提供最终确定有关特定投放位置的广告元素的决策的机会。 在&#x200B;_预览_&#x200B;面板中选择版面时，只有广告视图会受到影响。 未保存&#x200B;_预览_&#x200B;面板中的版面选择。

### 选择您的媒体资产

使用&#x200B;_媒体_&#x200B;部分至少选择一个要包含在体验中的图像资产。 广告投放与支持的图像长宽比相关联，这些长宽比在&#x200B;_投放位置_&#x200B;下拉菜单中作为选项列出。 此菜单显示Facebook帖子或Instagram故事支持的广告投放，按长宽比组织。

上传后，资产将保存到[!DNL Content]。 默认情况下，_媒体_&#x200B;区域以1:1的纵横比显示图像。 替代宽高比仅包括付费广告渠道支持的值。 它们按垂直和水平方向分组。 GenStudio for Performance Marketing支持每个激活体验最多包含六个纵横比。

**从内容上载资产**：

[!DNL Content]为您的组织的已批准资产和体验提供一个中心视图。 您可以使用&#x200B;**[!UICONTROL 搜索]**（放大镜）和&#x200B;_筛选器_&#x200B;菜单选项来聚焦[[!DNL Content] 图库](/help/user-guide/content/manage-assets.md)显示的资产清单。

1. 从[!DNL Activate]，单击渠道卡片上的&#x200B;**[!UICONTROL 新建]**。 将打开&#x200B;_体验设置_&#x200B;视图。

1. 单击&#x200B;**[!UICONTROL 选择]**，然后选择&#x200B;**[!UICONTROL 从内容中选择]**。 _选择内容_&#x200B;视图打开，显示您搜索或筛选的图像资源库。

1. 使用[!DNL Content]图库的搜索和筛选工具选择至少一个要上载的资产。

1. 单击&#x200B;**[!UICONTROL 使用]**&#x200B;以将所选资源包含在您的广告体验中。 _体验设置_&#x200B;窗口在&#x200B;_媒体_&#x200B;区域的默认纵横比中包括资产。 _预览_&#x200B;面板在广告投放中预览支持此宽高比的资源。

如果上传不成功，则会打开一条信息性错误消息，其中包含&#x200B;_[!DNL Content]_&#x200B;中资产的链接。

**要上传外部资源**：

您可以从Microsoft OneDrive或Dropbox上传最多6个位于[!DNL Content]图库外部的静态图像。

1. 从[!DNL Activate]，单击元磁贴上的&#x200B;**[!UICONTROL 新建]**。 将打开&#x200B;_体验设置_&#x200B;窗口。

1. 在&#x200B;_媒体_&#x200B;部分中，单击&#x200B;**[!UICONTROL 选择]**。 下拉菜单显示&#x200B;_从“内容”_&#x200B;或&#x200B;_上传_&#x200B;中选择的选项。

1. 单击&#x200B;**[!UICONTROL 上传]**。 将打开&#x200B;_添加宽高比_&#x200B;窗口。

1. 通过将图像文件拖放到图像上传区域，以受支持的长宽比选择图像。 或者，您可以浏览设备以查找资源。

1. （可选）若要从设备上传资源，请单击&#x200B;**[!UICONTROL 浏览]**，然后选择&#x200B;_浏览文件_&#x200B;或&#x200B;_浏览文件夹_&#x200B;以标识要上传的资源。

1. 在&#x200B;_添加详细信息_&#x200B;区域，将信息性详细信息添加到您上传的资产，以便在&#x200B;_[!DNL Content]_&#x200B;中进行搜索和筛选。 这些详细信息将另存为元数据。

1. 上传资源并分配详细信息后，单击右下方的&#x200B;**[!UICONTROL 添加Assets]**。

### 添加广告文本

使用&#x200B;_激活元广告_&#x200B;页面的&#x200B;_文本_&#x200B;部分向必填文本字段添加引人注目的品牌文本。 文本包括广告的主要（正文）文本和行动号召文本。 您无法编辑&#x200B;_主文本_、_标题_&#x200B;和&#x200B;_描述_&#x200B;字段。 您可以编辑&#x200B;_Call-to-action_、_显示链接_&#x200B;和&#x200B;_网站URL_&#x200B;字段。

| 字段 | 必填 | 字符数限制（最大） |
|-----------------|---------------------------|---------------------------------|
| 广告名称 | 是 | 500 |
| 主文本 | 是 | 500 |
| 标题 | 是 | 255 |
| 描述 | 否 | 125 |
| 行动号召 | 是 | 仅下拉菜单选项 |
| 显示URL | 否 | 1000 |
| 网站URL | 是 | 1000 |
| 图像 | 至少需要一个 |                                 |

GenStudio for Performance Marketing需要&#x200B;_主文本_&#x200B;和&#x200B;_标题_，而不是Meta。

### 分配元数据

体验详细信息将另存为元数据，并在搜索体验时帮助用户。 这些详细信息增强了体验在[!DNL Content]中的可见性。 使用这些可选的用户定义详细信息来识别体验的目的以及从中部署该体验的上下文或营销活动。

| 详细信息 | 描述 |
|------------|-------------|
| 营销活动 | 广告体验所属的所有GenStudio for Performance Marketing营销活动 |
| 品牌 | 用户定义的或默认的准则，它允许用户建立品牌准则，以捕捉品牌标识的实质。 |
| 产品 | 与您的组织关联并在GenStudio for Performance Marketing中标识的产品 |
| 角色 | 与您的组织关联并在GenStudio for Performance Marketing中标识的角色 |
| 时间范围 | 广告体验有效的季度、季、年或其他组织定义的时间单位 |
| 区域 | 在其中启动体验的地理区域 |
| 语言 | 使用广告体验的语言 |
| 关键字 | 便于广告体验搜索和分类的用户定义关键词 |

组合或选择您的体验后，单击&#x200B;**[!UICONTROL 下一步]**&#x200B;以确认您的元设置。

## 步骤4：确认元帐户设置

准备广告体验后，必须确认您的元帐户信息。 _元广告设置_&#x200B;视图填充了从配置的元帐户派生的选项。

| 详细信息 | 描述 |
|------------|-------------|
| 帐户 | 已连接到GenStudio for Performance Marketing的元帐户 |
| Facebook页面 | 发布体验的Facebook页面 |
| Instagram帐户 | 已连接到GenStudio for Performance Marketing的Instagram帐户 |
| 营销活动 | 广告体验所属的元营销活动 |
| 广告集 | 激活的广告体验所属的元广告集。 这些设置决定广告的最终投放位置。 |

### 创建新广告集

您可以在平台设置期间通过克隆现有广告集来创建新的广告集。 元广告集定义特定广告的时间、渠道详细信息和受众。 元营销活动可以包含多个广告集，但一个广告集仅与一个营销活动关联。

**创建新广告集**：

1. 从&#x200B;_元营销活动_&#x200B;下拉菜单中选择一个营销活动。

   选定的营销活动确定&#x200B;_广告集_&#x200B;下拉菜单中作为选项可用的广告集。

1. 单击&#x200B;**[!UICONTROL +新建广告集]**。

   将打开&#x200B;_新建广告集_&#x200B;弹出窗口，标识创建新广告集的元营销活动。

1. 从&#x200B;_从_&#x200B;的“使用配置”下拉菜单中选择要克隆的广告集。

   GenStudio for Performance Marketing通过将`- Copy`附加到所选广告集名称来分配默认广告集名称。

1. （可选，但是推荐）在&#x200B;**[!UICONTROL 新广告集名称]**&#x200B;字段中输入唯一的广告名称以替换默认值。

1. 单击&#x200B;**[!UICONTROL 创建广告集]**。

   您返回到&#x200B;_平台设置_&#x200B;视图，该视图已预先选择新广告集。 此时会显示一条成功消息，包括指向元广告管理器中广告集的链接。 此广告集可用于未来的激活。

>[!NOTE]
>
>如果广告集已成功创建，但无法保存广告集名称，则广告集将保存在“元广告管理器”中，并使用其默认名称（_原始广告集名称 — 副本_）。

### 跟踪Id

跟踪ID（广告名称）提供了一种机制，可用于收集与体验性能关联的量度。 在此字段中输入广告名称。

单击右上角的&#x200B;**[!UICONTROL 下一步]**&#x200B;以预览您的广告体验并完成激活。

## 步骤5：预览和激活广告

_审阅_&#x200B;页面将显示在&#x200B;_体验设置_&#x200B;中收集的广告体验，并提供查看和编辑体验的最终机会。 单击&#x200B;_体验设置_&#x200B;标签旁边的&#x200B;**[!UICONTROL 编辑部分]**&#x200B;以进行更改。 您还可以单击右上角的&#x200B;**[!UICONTROL 上一步]**&#x200B;以返回&#x200B;_体验设置_&#x200B;页面。

### 步骤6：完成广告体验的激活

1. 单击&#x200B;**[!UICONTROL 发布]**。

   完整的元广告体验及其相关元数据将直接推送到选定的元广告管理器广告集中。 体验会以非活动状态交付到元广告管理器。 通过元广告管理器，您可以管理部署广告体验和元营销活动的最后步骤。

1. [登录元广告管理器](https://adsmanager.facebook.com/)以查看您的广告体验并完成特定元渠道的发布。
