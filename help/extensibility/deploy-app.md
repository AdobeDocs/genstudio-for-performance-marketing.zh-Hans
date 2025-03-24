---
title: 部署您的App Builder应用程序
description: 部署适用于GenStudio for Performance Marketing的App Builder应用程序或加载项。
feature: Extensibility
exl-id: 51888ab7-7772-4ac8-838d-26db3019e9b0
source-git-commit: 52e8e078bc013fe686b5cc2105089f7098cce575
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---

# 部署您的应用程序

运行应用程序可在部署加载项行为之前提供加载项行为的初步快照。 此信息有助于调试。 您可以强制构建和部署已部署的应用程序，而无需重新提交它以供审批。


**要运行应用程序**：

在`https://localhost:9080`中运行应用程序：

```bash
aio app run
```

**要部署应用程序**：

1. 导航到您的部署工作区。 例如，要导航到生产工作区，请执行以下操作：

   ```bash
   aio app use -w Production
   ```

1. 部署应用程序：

   ```bash
   aio app deploy
   ```

**强制重新部署**：

>[!NOTE]
>
>强制构建和部署会覆盖现有部署。 首先在测试环境中彻底测试您的应用程序。

```bash
aio app build --force-build
```

```bash
aio app deploy --force-deploy
```

**要同时生成和部署**：

```bash
aio app deploy --force-build --force-deploy
```

**要查看应用程序**：

部署后，您可以通过向GenStudio for Performance Marketing URL添加`query`参数在GenStudio for Performance Marketing中查看应用程序：

`https://experience.adobe.com/?ext=https://<my-deployed-add-on>.adobeio-static.net/index.html#/@<ims-org>/genstudio/create`

如果您对加载项感到满意，则可以将其分发而不使用`query`参数。

您现在可以[分发您的应用程序](distribute-app.md)。
