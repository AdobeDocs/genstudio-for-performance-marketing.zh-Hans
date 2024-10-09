---
title: “连接到 [!DNL AEM Assets Content Hub] 存储库”
description: 了解如何将Adobe GenStudio for Performance Marketing连接到Adobe Experience Manager (AEM) [!DNL Content Hub] 存储库并利用现有的已批准内容。
level: Experienced
feature: Assets, Content
source-git-commit: 82ac164cb852305fce206845d15f04c4b4395387
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 0%

---

# 连接到[!DNL AEM Assets Content Hub]存储库

如果您在Adobe Experience Manager (AEM)中具有资源，则可以按照以下步骤在GenStudio for Performance Marketing中访问它们。

>[!BEGINSHADEBOX]

**先决条件**：

以下步骤需要对Admin Console和AEM Assetsas a Cloud Service具有管理访问权限。

>[!ENDSHADEBOX]

## 步骤1：启用[!DNL AEM Assets Content Hub]

请按照&#x200B;**部署Content Hub**&#x200B;自助服务流程，在Cloud Manager中为现有AEM Assets启用[!DNL Content Hub]。 请参阅&#x200B;_AEM as a Cloud Service_&#x200B;文档中的[部署 [!DNL Content Hub]](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub)。

启用[!DNL AEM Assets Content Hub]后，您在Admin Console的[!DNL AEM Assets as a Cloud Service]内有一个后缀为`contenthub`的新实例。

>[!IMPORTANT]
>
>管理员应验证[!DNL AEM Assets Content Hub]存储库是否与GenStudio for Performance Marketing位于同一组织内。

## 步骤2：载入GenStudio用户

在[!DNL Admin Console]中，将GenStudio for Performance Marketing用户或用户组添加到[!DNL AEM Assets Content Hub]产品配置文件。 如果内容查看者无权访问与[!DNL AEM Assets Content Hub]存储库相同的组织，则他们可能会在查看和批准内容时遇到困难。

- [板载 [!DNL Content Hub] 管理员](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub#onboard-content-hub-administrator)
- [板载 [!DNL Content Hub] 用户](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub#onboard-content-hub-users)

## 步骤3：批准资源

批准资源以在[!DNL AEM Assets Content Hub]中使用，这使其在GenStudio for Performance Marketing中可用。

请参阅&#x200B;_AEM as a Cloud Service_&#x200B;文档中的[批准Experience Manager](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/dynamicmedia/dynamic-media-open-apis/approve-assets)中的资源。

## 步骤4：配置资源可见性

在&#x200B;_[!DNL AEM Assets Content Hub]_配置选项中，查看筛选条件、资产详细信息、搜索和品牌推广的每组配置选项。

请参阅&#x200B;_Content Hub_&#x200B;文档中的[配置AEM as a Cloud Service用户界面](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/configure-content-hub-ui-options)。

## 步骤5：验证连接

在GenStudio for Performance Marketing内容中，_[!UICONTROL 位置]_&#x200B;列表位于图库的右上方。 如果您没有访问权限，或者您的组织尚未部署和连接[!DNL AEM Assets Content Hub]存储库，则列表不可用。
