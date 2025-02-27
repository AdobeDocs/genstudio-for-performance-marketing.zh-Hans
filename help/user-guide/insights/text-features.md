---
title: 文本功能
description: 了解GenStudio for Performance Marketing中使用的属性类别的文本功能。
feature: Insights, Attributes, Generative AI
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: 5cff6d1dd097b18e4fa3d286afddc1db553a415d
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 1%

---

# 文本功能

文本特征包括某些文本元素的计数，如词语、句子、表情符号，以及用于通过[!DNL Insights]进行分析的语义、情感和色调的分类。 文本也可以接收可读性分数。

GenStudio for Performance Marketing使用Adobe的AI和机器学习功能来学习文本，并根据关联的文本音调和营销叙述应用[!UICONTROL 资产属性]。 该过程验证输入文本以确保它包含字母数字字符，去除多余的空格和不可打印的字符，并将文本截断到最大允许的1500个单词。 在应用检测到的属性标记之前，AI预测流行色调。

## 语调

语调代表通过语言展现的一般性格、态度或气氛。 选择简单的字词和标点、句子结构和样式可以改变消息的语调。 例如，考虑以下使用三个基本音调级别的紧急消息：

- `Formal`

  ```
  Take advantage of this distinctive and exceptional opportunity!
  ```

- `Conversational`

  ```
  Don't miss out on this great opportunity!
  ```

- `Direct`

  ```
  Don't miss the chance!
  ```

AI进一步检测更细微的音调。 使用前一个示例中的同一紧急语句，以下版本使用异想天开的`poetic`语调：

- `Poetic`

  ```
  Embrace the moment, without delay, for this occasion won't always stay.
  ```

音调的其他次要值包括： `Enthusiastic`、`Assertive`、`Humorous/Witty`、`Inspirational`、`Empathetic`、`Sensory`、`Storytelling`、`Poetic`、`Quantitative`、`Personal`

## 叙述

叙述属性可帮助您识别传达与目标受众产生共鸣的值、目的或身份的资产。

| 叙述 | 描述 | 示例 |
| ----------------- | ----------- | ------- |
| `Authenticity` |             |         |
| `Celebration` |             |         |
| `Community` |             |         |
| `Convenience` |             |         |
| `Empowerment` |             |         |
| `Exploration` |             |         |
| `Futuristic` |             |         |
| `Hype` |             |         |
| `Indulgence` |             |         |
| `Peace of mind` |             |         |
| `Personalization` |             |         |
| `Prestige` |             |         |
| `Timelessness` |             |         |
| `Versatility` |             |         |
| `Well-being` |             |         |

## 可读性评分

可读性评分评估文本阅读和理解的难易程度。 它有助于确保您的内容适合您的目标受众。 得分基于各种因素，包括句子长度和单词复杂度。

| 分数 | 学校级别 | 注释 |
| ----------- | ------------------ | ------------------------------------------------------------------------- |
| 100.00-90.00 | 五年级 | 非常易于阅读。 普通的11岁学生容易理解。 |
| 90.0-80.0 | 6年级 | 易于阅读。 面向消费者的对话式英语。 |
| 80.0-70.0 | 七年级 | 读起来相当容易。 |
| 70.0-60.0 | 八年级和九年级 | 纯正的英语。 13至15岁的学生容易理解。 |
| 60.0-50.0 | 10至12年级 | 读起来相当困难。 |
| 50.0-30.0 | 大学 | 难以阅读。 |
| 30.0-0.0 | 大学毕业生 | 很难读。 大学毕业生最能理解这一点。 |

## 字数

待定

下表列出了GenStudio for Performance Marketing AI识别的图像功能类别。

| 类别 | 描述 | 示例 |
| -------------------- | ------------- | --------------------- |
| 表情符号计数 |             |        |
| HashTags计数 |             |        |
| 关键字 |             |        |
| 营销情感 | 在营销消息中，情绪是目标性的，以唤起观众的特定感受和反应，这可能会增强与品牌的参与度和联系。 | `Aspiration`，`Challenge`，`Curiosity`，`Exclusivity`，`Fascination`，`Gratification`，`Recognition`，`Trust`，`Urgency` |
| 说服策略 | 用于影响消费者行为和推动所需操作的技术。 这些策略针对特定的心理触发器和客户群体，以提高营销消息的有效性。 | `Social identity`，`Social proof`，`Endorsement`，`Concreteness`，`Foot in the door`，`Overcoming reactance`，`Reciprocity`，`Comparison`，`Social impact`，`Scarcity`，`Anthropomorphism` |
| 语调 | 营销消息中通过单词选择、标点、句子结构和样式传递的一般字符、态度或气氛。 | `Enthusiastic`，`Assertive`，`Humorous/Witty`，`Inspirational`，`Empathetic`，`Sensory`，`Storytelling`，`Poetic`，`Quantitative`，`Personal` |
