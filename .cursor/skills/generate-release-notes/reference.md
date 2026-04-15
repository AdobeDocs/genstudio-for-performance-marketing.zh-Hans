---
source-git-commit: f6a305c6a4e700525b570bbe280e5d1049d06537
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 6%

---
# 引用：发行说明创作

## Frontmatter

实时页面[help/user-guide/release-notes.md](../../help/user-guide/release-notes.md)包含的最小集之外的Experience League元数据（例如`TQID`、`product_v2`、`feature_v2`、分类ID）。

**规则：**

- 编辑发行说明&#x200B;**正文**&#x200B;内容时，**保留现有的前件**&#x200B;键和值，除非任务明确要求更改元数据。
- 请勿剥离分类或产品元数据以匹配较短的模板。
- ExL页面的所需概念通常包括`title`、`description`和`role`；对于新页面，请遵循[Experience League元数据指南](https://experienceleague.adobe.com/en/docs/authoring-guide/using/authoring/using-metadata)。

## 内部源（KT和发行Wiki）

仅在起草&#x200B;**时使用这些字段**；发布的发行说明不得引用内部文档。

### 知识转移(KT)文档

提取自：

| 字段 | 使用 |
|-------|-----|
| 描述 | 核心功能说明 |
| 电梯间营销 | 价值主张 |
| 已交付的功能 | 具体行为 |
| 问题陈述 | 用户棘手问题 |
| 发行类型和日期 | 计时 |

### 发布Wiki页面

分组和范围依据：

| 字段 | 使用 |
|-------|-----|
| 发行日期（修复版本） | 相同日期→相同发行说明批次 |
| 计划 | 仅上下文；不在内部以公共文本链接 |
| PM使用KT呈现该功能 | 可能存在更深层KT细节的信号 |

**范围规则：**&#x200B;共享相同发布日期（修复版本）的项目属于同一每月发布块。

## 文档链接

- 链接到&#x200B;**最相关的**&#x200B;短语（例如，将“不支持的图像和视频资源”链接到广告格式部分）。
- 首选`#anchor`个链接进入右侧子部分。
- 不存在更深的锚点时，可以接受概述页面。

## 常见文档路径

| 面积 | 路径前缀 |
|------|-------------|
| 创建 | `/help/user-guide/create/` |
| 内容 | `/help/user-guide/content/` |
| 激活 | `/help/user-guide/activation/` |
| 审批 | `/help/user-guide/approvals/` |
| 洞察 | `/help/user-guide/insights/` |
| 准则 | `/help/user-guide/guidelines/` |
| 模板 | `/help/user-guide/templates/` |
| 营销活动 | `/help/user-guide/campaigns/` |
| 可扩展性 | `/help/extensibility/` |
