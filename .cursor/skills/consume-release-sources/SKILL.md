---
name: consume-release-sources
description: ""
source-git-commit: c3c6aa86f4f520d020f8928612d1be6be1599652
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 1%

---


# 冲减发放来源(Jira + Confluence MCP)

**下游草稿：** [生成发行说明](../generate-release-notes/SKILL.md) →可选的[波兰发行说明](../polish-release-notes/SKILL.md)

**正在分析引用：** [reference.md](reference.md)

**目标输出文件（仅限下游）：** [help/user-guide/release-notes.md](../../help/user-guide/release-notes.md)

## 先决条件

- **Jira MCP** (`jira_getIssue`， `jira_searchIssues`)已验证
- **Confluence MCP** (`confluence_getContent`， `confluence_searchContent`)已验证
- 来自分支名称(`GS-#####`)、用户输入或票证说明的Jira票证密钥

## 工作流核对清单

1. [ ] **解析Jira票证** — `jira_getIssue`与`issueKey`。 阅读`description`以了解仪式Wiki链接和发布月份。
2. [ ] **查找仪式页面** — 使用票证中的Wiki URL；后备CQL： `title ~ "YYYY/MM Release Ceremony" AND space = GenStudio`。
3. [ ] **提取仪式正文** — `confluence_getContent`，带有`bodyMode: storage` （必需；`text`丢失KT链接和表结构）。
4. [ ] **分析功能组** — 从&#x200B;**GA版本功能**&#x200B;和&#x200B;**Beta版本功能**&#x200B;中提取行（请参阅[reference.md](reference.md#ceremony-feature-groups)）。
5. [ ] **应用包含筛选器** — 每个用户范围（请参阅[reference.md](reference.md#inclusion-filters)）；确认Beta行计数（可能为零）。
6. [ ] **解析KT页面** — 每个KT标题`confluence_searchContent`；使用`bodyMode: text`的`confluence_getContent`。
7. [ ] **提取KT字段** — 描述、电梯间推介、已传送的功能、问题陈述、发布类型和日期。
8. [ ] **设置Beta标志** — `requiresBetaBadge: true`，用于Beta节行或类型为`Beta`的GA表行。
9. [ ] **将**&#x200B;交给具有结构化行列表的[生成发行说明](../generate-release-notes/SKILL.md)（发送的副本中没有wiki/Jira参考）。

## Beta标签设置（移交以产生技能）

当`requiresBetaBadge: true`时，下游`###`部分必须立即包含在标题下：

```markdown
[!BADGE Beta]{type=Informative tooltip="This feature is currently in Beta, so some functionality may be limited or subject to change."}
```

不要为Beta添加斜体计划免责声明；支持此模式。

## 在已发运的发行说明中禁用

内部ID、Wiki URL、KT引文和Jira密钥仅保留在此提取阶段。 按照[生成发行说明禁止的内容](../generate-release-notes/SKILL.md#prohibited-content)总结公共页面中面向用户的结果。

## 回退

如果MCP调用失败，请要求用户粘贴仪式和KT内容，然后使用[reference.md KT字段映射](../generate-release-notes/reference.md#internal-sources-kt-and-release-wikis)继续生成发行说明。

## 其他资源

- [reference.md](reference.md) — 仪式解析、CQL、包含过滤器、MCP参数
- [生成发行说明](../generate-release-notes/SKILL.md) — 存档、草稿、链接、质量检查
- [polish-release-notes](../polish-release-notes/SKILL.md) — editorial在`{#latest}`下传递新的`###`
