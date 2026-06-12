---
source-git-commit: c3c6aa86f4f520d020f8928612d1be6be1599652
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 3%

---
# 参考：冲减版本来源(MCP)

## 仪式页面发现

| 模式 | 示例 |
|---------|---------|
| 标题 | **GenStudio**&#x200B;空间中的`YYYY/MM Release Ceremony` |
| 从Jira | 票证`description`中的Wiki链接（首选） |
| CQL回退 | `title ~ "2026/06 Release Ceremony" AND space = GenStudio` |

## 仪式专题组

发布仪式Wiki最多包含&#x200B;**两个**&#x200B;功能表。 从&#x200B;**storage** HTML中解析这两者。

### 正式发布版功能

- 章节标题： `GA Release Features` (`<h2>`)
- 子标题： `Feature Group:`，带有可选的Floodgate链接
- 表列包括&#x200B;**类型** （`GA`、`Limited`、`EA`、`Beta`或空）
- **KT文档**&#x200B;列： `<ac:link><ri:page ri:content-title="..."/></ac:link>`

每行提取：

| 字段 | 源 |
|-------|--------|
| `featureDescription` | 数据行中的前`<td>` |
| `type` | 键入列单元格文本 |
| `ktPageTitle` | KT列中的`ri:content-title` |
| `jiraKeys` | `ac:macro ac:name="jira"`→`key`参数（仅限内部） |
| `releaseTier` | 当Type为`GA`时`ga`；继承其他GA表值的类型 |

### Beta版本功能

- 分区标题： `Beta Release Features` （可能在某些月份中&#x200B;**缺席**）
- 第二个表；**no类型列** — 每一行都是Beta
- 与GA表相同的KT和Jira提取
- 在每个Beta分区行上设置`releaseTier: beta`和`requiresBetaBadge: true`

如果缺少Beta部分，请记录零Beta行并继续。

### 存储HTML模式

```html
<ac:link><ri:page ri:content-title="Translation on HZ Canvas" /></ac:link>
<ac:structured-macro ac:name="jira" ...><ac:parameter ac:name="key">GS-23218</ac:parameter></ac:structured-macro>
```

## MCP工具用法

| 步骤 | 工具 | 参数 |
|------|------|------------|
| 票证 | `jira_getIssue` | `issueKey`，可选`expand: renderedFields` |
| 仪式 | `confluence_getContent` | `contentId`, `bodyMode: storage` |
| KT查找 | `confluence_searchContent` | `cql: title = "<KT title>" AND space = GenStudio` |
| KT主体 | `confluence_getContent` | `contentId`, `bodyMode: text`, `maxBodyChars: 50000` |

在解析KT链接时，**不**&#x200B;将`bodyMode: text`用于仪式页面。

## KT字段映射（起草输入）

映射到生成发行说明；请勿逐字粘贴到公共发行说明中。

| KT节 | 使用 |
|------------|-----|
| 描述 | 核心功能 |
| 电梯间推介 | 价值主张 |
| 已交付的功能 | 具体行为 |
| 问题陈述 | 用户痛苦（仅限上下文） |
| 发行类型和日期 | GA/Beta/有限（内部）；驱动器徽章决策 |

## 包含过滤器

不明确时，与用户确认范围。 常用预设：

| 预设 | 包括 |
|--------|----------|
| `ga_only` | 类型= `GA`的GA表行 |
| `ga_and_beta` | **建议的未来月份默认值** — GA行，其中Type = `GA` **加上所有**&#x200B;个Beta版本功能表行 |
| `ga_plus_empty` | GA表：类型= `GA`或空类型 |
| `all_except_pilot` | 除`Limited`之外的GA表行；使用`ga_and_beta`时加上Beta节 |
| `all_with_badges` | 所有GA表行；Beta部分行始终获得Beta徽章 |

## Beta徽章移交

| 条件 | `requiresBetaBadge` |
|-----------|---------------------|
| **Beta版本功能**&#x200B;表中的行 | `true` |
| 类型为`Beta`的GA表行 | `true` |
| 类型为`GA`的GA表行 | `false` |

下游： [生成发行说明决策规则](../generate-release-notes/SKILL.md#decision-rules)和[Beta徽章片段](../generate-release-notes/SKILL.md#beta-badge)。

## 切换有效负载（非正式）

将生成发行说明作为项目列表传递：

```yaml
- featureDescription: "YouTube Shorts"
  releaseTier: ga
  requiresBetaBadge: false
  ktPageTitle: "YouTube Shorts (Create + Activate)"
  # extracted KT fields: description, elevatorPitch, featuresDelivered, ...
```
