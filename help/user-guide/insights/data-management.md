---
title: 数据管理
description: 了解GenStudio for Performance Marketing中 [!DNL Insights] 的数据引入和存储。
feature: Insights
level: Experienced
role: Admin
last-substantial-update: 2025-1-7
exl-id: a5ab44d6-75c0-405b-82ad-9c65f6094bd6
source-git-commit: 5cff6d1dd097b18e4fa3d286afddc1db553a415d
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---

# 数据管理

GenStudio for Performance Marketing使用Adobe Experience Platform (AEP)进行数据摄取和存储支持[!DNL Insights]的指标和元数据。 AEP使用&#x200B;_架构_&#x200B;定义数据结构以及用于存储和管理数据集合的&#x200B;_数据集_。

## 数据连接

GenStudio for Performance Marketing使用Customer Journey Analytics (CJA)通过创建与一个或多个AEP数据集的连接来聚合多个数据源。 CJA使用这些数据连接创建用于分析具有[!DNL Insights]的指标的数据视图。

>[!BEGINSHADEBOX]

**有关数据连接的重要信息**

如果您是[Adobe系统管理员](/help/user-guide/user-roles.md#adobe-system-administrator-vs-genstudio-system-manager)，则您可能有权访问支持GenStudio for Performance Marketing的AEP沙盒管理和数据湖组件。

>[!WARNING]
>
>在AEP中重置生产沙盒会删除所有数据连接并导致[!DNL Insights]停止工作。

请务必小心，不要删除GenStudio for Performance Marketing可靠运行所需的以下数据连接：

- 以`GS Insights`为前缀的AEP数据集
- 以`GS Insights`为前缀的AEP架构、类和字段组
- 自定义字段组`timestamp for metadata`
- AEP连接：以`GS Insights`为前缀的数据流
- AEP连接： GS Insights帐户

在删除AEP中的任何数据组件之前，请参阅&#x200B;_Customer Journey Analytics_&#x200B;指南中的[删除含义](https://experienceleague.adobe.com/en/docs/analytics-platform/using/technotes/deletion)。

>[!ENDSHADEBOX]

## 数据保留策略

GenStudio for Performance Marketing会将渠道数据保留13个月。 此保留策略包括在初始连接期间摄取的6个月的数据，从而确保全面的历史数据分析和报告。

请参阅[连接渠道广告帐户](/help/user-guide/insights/connect-channel.md)。
