---
title: 数据管理
description: 了解GenStudio for Performance Marketing中 [!DNL Insights] 的数据引入和存储。
feature: Reporting and Insights
level: Experienced
role: Admin, Developer
last-substantial-update: 2025-1-7
exl-id: a5ab44d6-75c0-405b-82ad-9c65f6094bd6
TQID: https://experienceleague.adobe.com/HM2e0Yq2uwTpKtK-z8gHs0hDFrsJS6koQBqoNoKJK0Y
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: c95c94c1-727b-457a-9184-a4dda4c95ab2id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: e0aa398c-6185-4e77-8cf7-2561c578c181
subfeature_v2: id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: d3cdead0-685a-4489-9250-4bb709942f66id: e1e0219c-f879-479f-8427-888ed2a6e9c2id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 249
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

请参阅[连接付费媒体帐户](/help/user-guide/connectors/connect-channel.md)。
