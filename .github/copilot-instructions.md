---
source-git-commit: 8ed1e6853c9f844c72431dc692b556ece9c215a8
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---
## 用途

帮助AI编码助手对GenStudio for Performance Marketing文档存储库进行小型、安全的编辑。

## 高级体系结构（简短）- 此存储库是一个文档网站，由`help/`下的Markdown和`help/_includes/`中的共享包含以及`help/_includes/assets/`下的策划图像组成。- 发行说明、用户指南和可扩展性内容位于`help/`下。 大型内容更改应保留前置内容和现有标题结构。- 该站点是使用Jekyll构建的，托管在GitHub页面上。 构建过程使用一些自定义插件的标准Jekyll约定。

## 特定于项目的约定- 游标规则：自定义自动化和指导存在于`.cursor/rules/*.mdc`中。 示例： `.cursor/rules/docs-lint.mdc` （lint进程）、`.cursor/rules/generate-release-notes.mdc` （发行说明格式）。 对于自动任务，请遵循这些步骤。- 文件名和前端内容：   - 发行说明需要特定的frontmatter（请参阅`.cursor/rules/generate-release-notes.mdc`）。   - 规则文件和`.mdc`扩展名使用kebab大小写。- 格式惯例：文档使用GitHub风格的Markdown。 标题通常遵循句子大写和短段落。 对于发行说明中的列表，首选`*`项目符号；对于功能部分，首选`###`。

## 文档样式指南- 有关技术文档最佳实践，请遵循[Microsoft写作风格指南](https://learn.microsoft.com/en-us/style-guide/)：   - 撰写以用户行为为中心的简明明明扼要的句子   - 使用主动语态和现在时态   - 将文本分成简短的可扫描块   - 保持温暖的直调，同时保持技术准确性- Markdown创作：   - 标题的句子大小写（仅首词大写）   - 保持段落简短（2-3句）以提高可读性   - 在标题和列表之前和之后添加空白行   - 对UI元素、文件路径和代码使用反撇号   - 包含所有图像的替换文本   - 使用描述性文本链接到特定章节

## 编辑的安全规则（AI应该做什么）- 切勿将Jira ID、内部链接或仅用于公司的引用添加到公共文档。 请参阅`generate-release-notes.mdc`“问题跟踪”部分。- 在编辑包含前端内容YAML的文件时，请完全保留前端内容YAML。 许多模板和发行说明依赖于固定键（标题、描述、角色、exl-id）。- 对于Lint修复，首选从`.cursor/rules/docs-lint.mdc`进行自动的幂等编辑（删除尾随空格，确保最后是换行符）。 人类使用的命令示例：

```sh
sed -i '' 's/ $//' <file>
sed -i '' '$ { /^$/d; }' <file> && echo "" >> <file>
```

## 示例（要更改什么以及如何更改）- 小副本修复：更新`help/` Markdown文件中的文本，保持标题和锚点不变。- 图像更新：引用`help/_includes/assets/`下的图像。 不更新所有引用时，请勿移动或重命名图像。

## 优先查看位置- `help/_includes/` — 共享片段和图像。- `.cursor/rules/` — 自动化和Litting指导；将这些指导用作格式化和流程的权威规则。- `markdownlint_custom.json` — 本地markdownlint覆盖。- `.github/pull_request_template.md` — PR期望。

## 什么时候问人- 如果更改要求运行或修改基于Docker的工具（链接规则提及Docker）或影响站点构建管道。- 如果文件引用未知的外部配置（例如`markdownlint.json`缺失） — 询问是创建还是忽略。

## 对人而言最简单的命令

```sh
# Install linter (if not present)
npm install -g markdownlint-cli

# Run lint locally using project config
markdownlint --config markdownlint_custom.json "help/**/*.md"

# Project lint via yarn (preferred if available in environment)
yarn lint
```

&#x200B;---
如果您愿意，我可以将它合并到存储库中的`.github/copilot-instructions.md`中（或调整措辞/长度）。 我应该更改或添加哪些内容？
