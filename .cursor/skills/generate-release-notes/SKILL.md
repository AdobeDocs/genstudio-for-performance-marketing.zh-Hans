---
name: generate-release-notes
description: ""
source-git-commit: 1a33b08048233c5f9a82b5f428082aa5c71b0052
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---


# 生成GenStudio发行说明

**规范目标文件：** [help/user-guide/release-notes.md](help/user-guide/release-notes.md)

**完整示例：** [示例.md](examples.md)

**KT/wiki字段映射和文档路径：** [reference.md](reference.md)

## 工作流核对清单

按此顺序工作。 复制核对清单并跟踪多步编辑的进度。

1. [ ]打开`help/user-guide/release-notes.md`并读取当前`## YYYY.MM {#latest}`块和&#x200B;**早期发行说明**&#x200B;区域。
2. [ ]如果添加&#x200B;**新**&#x200B;月度版本：存档当前的最新版本（请参阅[存档先前的最新](#archive-previous-latest)）。
3. [ ]添加或编辑前`## YYYY.MM {#latest}`部分（最新月份在发行列表顶部）。
4. [ ]对于每个项目，应用[决策规则](#decision-rules)（功能`###`与&#x200B;**修复和增强功能**，是否为Beta徽章）。
5. [ ]添加或验证最相关短语的文档链接（请参阅[reference.md](reference.md#documentation-linking)）。
6. [ ]在完成前运行[质量检查](#quality-checks)。
7. [ ]在页面上保留[frontmatter](reference.md#frontmatter)，除非任务明确更新元数据。

## 决策规则

使用这些if/then规则，使内容登陆到正确的位置：

| 如果 | 则 |
|----|------|
| 此功能是Beta中的新功能 | 立即在`###`标题下添加Beta徽章行（请参阅[examples.md](examples.md)）。 |
| Source材料将该项显式标记为&#x200B;**fix**&#x200B;或&#x200B;**增强功能** | 仅使用`*`项目符号将其放在`### Fixes and enhancements`下。 |
| 该项目是一个全新功能或功能案例 | 使用包含1-3个句子（不是修复列表）的`###`功能部分。 |
| 您不确定某些内容是修复还是功能 | 默认使用`###`功能部分，除非源明确说明修复/增强功能。 |

**修复部分规则：**&#x200B;请勿向&#x200B;**修复和增强功能**&#x200B;添加项目符号，除非源被明确标记为修复或增强功能。

## 存档上一个最新的

引入新`## YYYY.MM {#latest}`时：

1. 剪切整个`## YYYY.MM {#latest}`部分（从标题一直到该版本内容的结尾，在下一个`##`或&#x200B;**以前的发行说明**&#x200B;之前）。
2. 将其粘贴到可折叠块中的&#x200B;**早期发行说明**&#x200B;中。
3. 将旧标题替换为： `+++Notes from YYYY.MM.DD+++` （使用实际发布日期；与文件中现有注释相同的格式）。
4. 从存档的标题中删除`{#latest}`；新的顶部区域是唯一具有`{#latest}`的部分。
5. 在&#x200B;**较早的发行说明**&#x200B;中按时间顺序排列（最新的存档块朝顶部排列，除非文件已使用不同的顺序 — **与现有文件**&#x200B;匹配）。

## 所需结构

### 页面标题和简介

在frontmatter之后，使用：

```markdown
# GenStudio for Performance Marketing release notes

This release information details the latest updates to the GenStudio for Performance Marketing application.
```

如果文件已使用略微不同的介绍句子（例如，“提供”而不是“详细信息”），请保持与页面其余部分的一致性。

### 最新版本标题

- 格式： `## YYYY.MM {#latest}`表示最新发行版块。
- 页面上只有一个`{#latest}`锚点。

### 功能部分

- 将`###`用于主要功能类别。
- 呈现时态，1-3个句子，澄清什么/原因以及用户行为是否有帮助。
- 产品名称： `[!DNL Create]`、`[!DNL Content]`、`[!DNL Insights]`等。
- UI： `[!UICONTROL Control Name]`（如果适用）。
- 强调： `_italics_`用于UI区域/部分；`**bold**`谨慎用于关键术语。

### Beta徽章

完全使用：

```markdown
[!BADGE Beta]{type=Informative tooltip="This feature is currently in Beta, so some functionality may be limited or subject to change."}
```

### 文档链接

- 模式： `[link text](/help/user-guide/section/page.md#anchor)`
- 首选锚点；链接用户关注的短语，而不是“单击此处”。

### 修复和增强功能

- 项目符号行使用`*`。
- 仅限在源材料中明确标记为修复/增强的项目。
- 与功能相同的链接和术语约定。

## 禁止的内容

- **不**&#x200B;在发布的发行说明中包含Jira密钥、内部问题编号、仅限内部的URL或公司Wiki链接。
- 请&#x200B;**不**&#x200B;引用知识转移文档、票证或内部工具作为证明 — 仅总结面向用户的结果。
- 请&#x200B;**不**&#x200B;在多个节上复制`{#latest}`。

## 质量检查

在完成任务之前：

- [ ]所有新的或更改的相对链接尽可能解析为`help/`下的真实路径。
- [ ]Beta功能根据需要包括Beta徽章片段。
- [ ]术语与现有发行说明(`[!DNL …]`， `[!UICONTROL …]`)匹配。
- [ ]扫描草稿以查找意外的内部ID (`[A-Z]+-\d+`)、Wiki URL或“参阅Jira”语言；删除它们。
- [ ] **修复和增强功能**&#x200B;仅包含明确标记的修复/增强功能。
- [ ]添加新月份时，上一最新分区已正确存档。

## 内容源（摘要）

从内部获取知识传输文档或发布Wiki时，按照[reference.md](reference.md#internal-sources-kt-and-release-wikis)中的说明映射字段。 提供的页面必须作为独立用户文档阅读。

## 可选：波兰新子节

在`{#latest}`下添加新`###`内容后，针对版面编辑器式的传递运行[波兰版发行说明](../polish-release-notes/SKILL.md)（权益转发音，每段&#x200B;**有** 2-3个句子，无操作说明）**仅限**&#x200B;这些&#x200B;**新的**&#x200B;子部分 — **非**（早期发行说明或预先存在的文本），除非明确要求。

## 其他资源

- [examples.md](examples.md) — 可粘贴的示例（功能、修复、存档块）。
- [reference.md](reference.md) — frontmatter注释、文档路径、链接策略。
- [波兰版发行说明](../polish-release-notes/SKILL.md) — 可选编辑传递给`{#latest}`下新添加的`###`。
