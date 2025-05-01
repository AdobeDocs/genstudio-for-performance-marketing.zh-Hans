---
title: 创建App Builder应用程序以扩展GenStudio for Performance Marketing
description: 开始构建应用程序或加载项。
feature: Extensibility
exl-id: 4e757dd4-a02d-472c-bc13-6f27dffa48f2
source-git-commit: 89b7f477310326755a6b34cb97d5ad5664e98dec
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 0%

---

# 开发App Builder应用程序

扩展GenStudio for Performance Marketing本机功能的开发人员使用[Adobe App Builder](https://developer.adobe.com/app-builder/)创建、提交和部署其可扩展应用程序或加载项。

>[!BEGINSHADEBOX]

**先决条件**：

* Node.js（版本20.x或更高版本）

* npm（与Node.js打包）

* Adobe Developer命令行界面(CLI)。 要安装： `npm install -g @adobe/aio-cli`

>[!ENDSHADEBOX]

## 应用程序结构

GenStudio for Performance Marketing加载项是App Builder应用程序，包含与其他App Builder应用程序相同的基本组件。

### 生成和配置文件

App Builder应用程序的关键组件包括这些内部版本和配置文件。 此列表未包含所有内部版本和配置文件。

* `README.md`：包含有关应用程序的一般信息。

* TS应用程序文件：

   * `package.json`
   * `package-lock.json`
   * `eslint`
   * `tsconfig`
   * `jest test up`

* App Builder配置文件：

   * `app.config.yaml`
   * `ext.config.yaml`：加载项的配置文件
   * `app.config.yaml`：加载项的配置文件(包括将应用程序定义为GenStudio for Performance Marketing加载项)
   * `.aio`
   * `.env`：不将`.env`文件提交到源代码管理

### Source代码

```
- src/
    - genstudiopem/
        - web-src/
            - src/
                - components/
                - utils/
                - Constants.ts
                - index.tsx
                - index.css
                - utils.ts
        - index.html
```

### Source代码组件

* `ExtensionRegistration.tsx`：定义主机应用程序(GenStudio for Performance Marketing)加载和显示加载项所需的必要API。

* `App.tsx`：定义路由到其他组件的主应用程序组件。

* `AdditionalContextDialog.tsx`：用于显示其他上下文加载项的对话框组件。

* `RightPanel.tsx`：验证加载项的对话框组件。

* `Helper`组件：包含`ClaimsChecker`。

## 从现有应用程序创建App Builder应用程序

您可以使用示例应用程序快速开始创建加载项。

**要从现有应用程序创建App Builder应用程序**：

1. 从[GenStudio UIX示例](https://github.com/adobe/genstudio-uix-examples)存储库下载示例应用程序。

1. 从[Adobe Developer Console](https://developer.adobe.com/console/)上的App Builder项目工作区中，选择&#x200B;**[!UICONTROL 全部下载]**&#x200B;以下载项目详细信息。

1. 在首选的集成开发环境(IDE)中本地打开示例应用程序。

1. 使用Adobe Developer命令行界面进行身份验证：

   ```bash
   aio login
   ```

1. 下载您的JSON文件，然后创建您的应用程序：

   ```bash
   aio app use '/path/to/your/downloaded/app-builder/project/details/config.json'
   ```

## 将自定义代码添加到加载项

您在`AdditionalContextDialog.tsx`和`RightPanel.tsx`文件中定义加载项代码。 这两个文件定义用户访问加载项时的弹出窗口外观和行为。

* `AdditionalContextDialog.tsx`：如果您计划使用&#x200B;_添加上下文_&#x200B;加载项，请定义此组件。 用户在[!DNL Create]的提示抽屉中单击&#x200B;_加载项_&#x200B;时与此组件交互。

* `RightPanel.tsx`：如果您计划使用&#x200B;_右侧面板_&#x200B;加载项（体验验证），请定义此组件。 用户在[!DNL Create]体验草稿中单击右侧面板中的验证加载项时与此组件交互。

您现在已准备好[部署您的应用程序](deploy-app.md)

## 应用程序开发的最佳实践

维护开发环境可以帮助您避免应用程序开发和部署错误：

* 如果您使用的是示例应用程序的旧版本，请通过重新安装这些依赖项来升级它们：

  ```bash
  rm -rf node_modules package-lock.json && npm i
  ```

* 升级GenStudio UIX SDK。 确认您使用的是最新版本的[GenStudio UIX SDK](https://github.com/adobe/genstudio-uix-sdk)。 请参阅[GenStudio UIX示例存储库](https://github.com/adobe/genstudio-uix-examples)，了解如何使用最新的SDK更改。
