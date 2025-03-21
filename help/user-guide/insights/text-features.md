---
title: 文本功能
description: 了解GenStudio for Performance Marketing中使用的属性类别的文本功能。
feature: Reporting and Insights, Text Attributes, Generative AI
exl-id: 7b81b0ae-0c62-468f-965c-fd8070644fb3
source-git-commit: ac2e18899f910a47ec5013a13c2ee2771684ddad
workflow-type: tm+mt
source-wordcount: '1290'
ht-degree: 1%

---

# 文本功能

文本特征包括某些文本元素的计数，如词语、句子、表情符号，以及用于通过[!DNL Insights]进行分析的语义、情感和色调的分类。 文本也可以接收可读性分数。

GenStudio for Performance Marketing使用Adobe的AI和机器学习功能来学习文本，并根据关联的文本音调和营销叙述应用[!UICONTROL 媒体属性]。 该过程验证输入文本以确保它包含字母数字字符，去除多余的空格和不可打印的字符，并将文本截断到最大允许的1500个单词。 在应用检测到的属性标记之前，AI预测流行色调。

## 语调

语调代表通过语言展现的一般性格、态度或气氛。 选择简单的字词和标点、句子结构和样式可以改变消息的语调。 例如，考虑以下使用三个基本音调级别的紧急消息：

| 色调 | 描述 | 示例 |
| -------------- | ----------------------------------- | --------------------------------------------------------- |
| 正式 | 精致而专业的语言。 | `Take advantage of this distinctive and exceptional opportunity!` |
| 对话 | 友好而非正式的语言。 | `Don't miss out on this great opportunity!` |
| 直接 | 直截了当，切中要害。 | `Don't miss the chance!` |

音调的其他次要值可以更准确地区分您邮件的性质和态度。 与前面紧急消息的示例一样，GenAI可能在此奇特示例中检测到&#x200B;_诗意_&#x200B;音调： `Embrace the moment, without delay, for this occasion won't always stay.`

下表列出了GenStudio for Performance Marketing AI识别的色调值。

| 色调 | 描述 | 示例 |
| -------------- | ------------------------------------------------ | --------------------------------------------------------- |
| 自信 | 自信而强悍的表情。 | `You need to act now to secure this deal!` |
| 直接 | 直截了当，切中要害。 | `Don't miss the chance!` |
| 同理心 | 显示理解和敏感度。 | `We understand your needs, and this is perfect for you.` |
| 热心 | 显示强烈且渴望的享受、兴趣或认可。 | `This is an amazing opportunity you can't miss!` |
| 幽默/威蒂 | 清醒，聪明。 | `Why wait? Grab this deal before it's gone!` |
| 励志 | 鼓舞人心，振奋人心。 | `Believe in yourself and seize this opportunity!` |
| 诗意 | 富有艺术性和表现力。 | `Embrace the dawn of a new opportunity.` |
| 定量 | 基于数值数据。 | `99% of users loved this offer, and you will too.` |
| 感官 | 与感官接触。 | `Feel the excitement with this incredible offer!` |
| 讲故事 | 讲述故事以传达信息。 | `Once upon a time, there was an offer you couldn't refuse.` |

## 情感诉求

营销人员利用人类情感的力量，在受众和品牌之间建立强大的联系。 营销人员利用快乐、恐惧、兴奋或怀旧等感官，可以制作更深层次上产生共鸣的信息，促进参与并影响消费者行为。 情感吸引力有助于提供更易理解和难忘的内容，最终培养品牌忠诚度，并鼓励期望的行动。

说服策略、营销情感和叙述风格共同针对客户细分市场。

- **叙事风格**，如真实性、庆祝和社区，有助于传达与目标受众产生共鸣的价值观和身份，从而创建更吸引人和更通俗易懂的信息。
- **说服策略**，例如稀缺、社会证明和互惠，旨在通过吸引消费者的情感和偏好来影响他们的行为。
- **营销情感**&#x200B;旨在激发增强参与度和与品牌联系的感情。

GenStudio for Performance Marketing AI通过分析文本中的情感提示、语调和叙述风格来检测和区分这些特征。 人工智能使用自然语言处理(NLP)和机器学习算法来识别模式，并根据预定义的情感和说服属性对文本进行分类。

### 叙事风格

叙事或上诉因素属性有助于识别传达与目标受众产生共鸣的值、目的或身份的媒体。 下表列出了GenStudio for Performance Marketing AI识别的叙述样式。

| 上诉系数 | 描述 | 示例 |
| ----------------- | --------------------------------------------------------------------- | ------------------------------------------ |
| 真实性 | 真诚和真实，经常强调透明度和诚实。 | `A behind-the-scenes look at how our products are made.` |
| 庆祝 | 以喜悦和节日来纪念特殊场合或成就。 | `Join us in celebrating our 10th anniversary with special offers!` |
| 社区 | 培养团体的归属感和团结感。 | `Our brand is built on the strength of our community.` |
| 便利性 | 强调易用性和节省时间的好处。 | `Get what you need with just one click.` |
| 赋权 | 鼓励和扶持个人掌握控制权并做出决策。 | `Empower yourself with our latest tools and resources.` |
| 探索 | 邀请探索和冒险，通常与新体验有关。 | `Discover new horizons with our travel packages.` |
| 未来主义 | 强调创新和前瞻性思维。 | `Experience the future of technology today.` |
| 炒作 | 围绕产品或活动产生兴奋和期待。 | `Don't miss out on the most anticipated event of the year!` |
| 放任 | 吸引幻想、欲望或快乐。 | `Treat yourself to the finest gourmet chocolates.` |
| 完全安心 | 提供保证和安全感。 | `Rest easy knowing your data is safe with us.` |
| 个性化 | 根据个人偏好定制体验或产品。 | `Get a custom-fit solution just for you.` |
| 威望 | 与高地位和排他性相关联。 | `Join the elite with our premium membership.` |
| 无时限 | 强调经久不衰的品质和经典吸引力。 | `Our designs are timeless and never go out of style.` |
| 多功能 | 强调适应性和多种用途。 | `Our product fits seamlessly into any lifestyle.` |
| 福利 | 促进健康、幸福和整体健康。 | `Enhance your well-being with our holistic approach.` |

### 说服策略

说服技术用于影响消费者行为和驱动期望的动作。 这些策略针对特定的心理触发器和客户群体，以提高营销消息的有效性。 下表列出了GenStudio for Performance Marketing AI识别的说服策略。

| 策略 | 描述 | 示例 |
| --------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------- |
| 拟态 | 将人的特征归因于产品或品牌。 | `Our friendly chatbot is here to help you.` |
| 比较 | 突出显示影响选择的选项之间的差异。 | `See how we compare to the competition.` |
| 具体 | 提供具体细节，使报文更加明确。 | `Save 20% on your next purchase.` |
| 认可 | 获得可靠消息来源或影响者的认可。 | `Recommended by top industry experts.` |
| 踏进门 | 从较小的请求开始，以增加同意较大请求的可能性。 | `Try our free trial today.` |
| 克服电抗 | 通过承认和处理异议来减少阻力。 | `We understand your concerns, and here's how we address them.` |
| 互惠 | 提供有价值的东西以鼓励回报的恩惠。 | `Get a free gift with your purchase.` |
| 稀缺 | 通过突出显示的有限可用性营造紧迫感。 | `Only a few items left in stock!` |
| 社交身份 | 利用消费者的群体归属感。 | `Join our community of innovators.` |
| 社会影响 | 强调对社会或环境的积极影响。 | `Your purchase helps plant a tree.` |
| 社交证明 | 使用口碑或用户生成的内容来建立信任。 | `See why thousands of users love our product.` |

### 营销情感

在营销消息中，情绪是目标性的，以唤起观众的特定感受和反应，这可能会增强与品牌的参与度和联系。 下表列出了GenStudio for Performance Marketing AI识别的情绪。

| 情绪 | 描述 | 示例 |
| ------------- | --------------------------------------------------------------------------- | --------------------------------------------------------- |
| 抱负 | 激发实现或取得更大成就的欲望。 | `Imagine the possibilities with our premium service.` |
| 挑战 | 鼓励受众克服障碍或接受新任务。 | `Are you ready to take the next step in your career?` |
| 好奇 | 激发对更多知识的兴趣和渴望。 | `Discover the secrets behind our success.` |
| 排他性 | 创建成为选定组的一部分的感觉。 | `Join our exclusive club for members-only benefits.` |
| 迷恋 | 通过有趣或令人兴奋的内容吸引受众。 | `Be amazed by our latest innovations.` |
| 满足 | 提供使用产品或服务的满意度和乐趣。 | `Enjoy the ultimate comfort with our luxury bedding.` |
| 识别 | 承认和评价受众的成就或地位。 | `Get the recognition you deserve with our award-winning service.` |
| 信任 | 树立品牌的信心和可靠性。 | `Trust us to deliver quality and excellence every time.` |
| 紧急 | 通过强调时间敏感型机会来立即采取行动。 | `Act now before this limited-time offer expires!` |

## 可读性评分

可读性评分评估文本阅读和理解的难易程度。 它有助于确保您的内容适合您的目标受众。 得分基于各种因素，包括句子长度和单词复杂度。 下表列出了GenStudio for Performance Marketing AI识别的可读性级别。

| 可读性级别 | 描述 | 示例 |
| ------------------- | ------------------------------------------------------------------ | --------------------------------------------------------- |
| 五年级 | 非常简单的语言，适合年幼的孩子使用。 | `The cat sat on the mat.` |
| 6年级 | 简单清晰的语言，适合一般受众。 | `You can find great deals on our website.` |
| 七年级 | 易于理解，具有直接的词汇和结构。 | `Our new product is simple to use and very effective.` |
| 八年级和九年级 | 简洁明了，适合青少年使用。 | `This guide will help you understand the basics of our service.` |
| 10至12年级 | 更复杂的语言，适用于年长青少年和成年人。 | `The comprehensive manual provides detailed instructions for setup.` |
| 大学 | 高级语言，适合受过良好教育的受众。 | `The study explores the multifaceted implications of the new policy.` |
| 大学毕业生 | 高级语言，适合专家和专家使用。 | `The dissertation delves into the intricacies of quantum mechanics.` |

## 计数

了解并利用井号标签计数、字数、句数和停用词率等计数属性可以显着增强您的内容策略。 这些指标为您的营销工作的效率和范围提供了有价值的见解。 下表列出了GenStudio for Performance Marketing AI识别的计数类别。

| 类别 | 描述 | 示例 |
| --------------------- | --------------------------------------------------------------------------- | --------------------- |
| 表情符号计数 | 文本中存在的emoji编号。 表情符号可以增强参与度，并迅速传达情感。 | `😊`、`🚀`、`❤️` |
| HashTags计数 | 文本中使用的井号标记数。 井号标签有助于对内容进行分类并提高在社交媒体上的可发现性。 | `#Marketing`、`#Sale` |
| 每句单词数 | 文本中每句的平均字数。 较短的句子通常更容易阅读和理解。 | `10` |
| 字数 | 文本中的总字数。 较高的字数可以提供更详细的信息，但也可能需要更大的阅读工作。 | `1500 words` |
| 停用词比率 | 文本中停用词与有意义词的比率。 搜索查询和结果中通常会忽略停用词（例如“a”、“an”、“the”）。 停用词比例高可能会使内容不那么吸引人且更难阅读。 | `0.375` |
| 句子数 | 文本中的句子总数。 更多的句子可以表示更详细的内容，但过长的文本可能会失去读者的兴趣。 | `75 sentences` |
