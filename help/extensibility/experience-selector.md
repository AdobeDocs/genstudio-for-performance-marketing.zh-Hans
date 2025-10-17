---
title: GenStudio Experience Selector MFE
description: 了解并为GenStudio应用程序和加载项实施Experience Selector微前端。
feature: Extensibility, Extensions, Experiences
source-git-commit: d9d6d3825cd953245049de119c66f54274f20fd9
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 6%

---

# GenStudio Experience Selector MFE

Experience Selector是一个微型前端(MFE)，它提供了用于选择GenStudio体验的`ExperienceSelectorDialog`组件。 通过从独立的JavaScript捆绑包导入`renderExperienceSelectorWithSUSI`函数在应用程序中使用组件，该捆绑包会自动加载最新部署的Micro Frontend并呈现自然的组件接口。

GenStudio Experience Selector MFE允许用户执行以下操作：

- 浏览并选择GenStudio体验
- 按各种标准筛选体验
- 支持单一选择模式和多重选择模式
- 通过SUSI（注册登录）集成处理身份验证
- 在不同的框架中提供一致的UI

## 集成选项

MFE可通过两种不同的方法集成：

### ESM （ES模块） — 推荐

```javascript
import { renderExperienceSelectorWithSUSI } from 'https://experience-stage.adobe.com/solutions/GenStudio-experience-selector-mfe/static-assets/resources/@genstudio/experience-selector/esm/standalone.js';
```

### UMD（通用模块定义）

```html
<script src="https://experience-stage.adobe.com/solutions/GenStudio-experience-selector-mfe/static-assets/resources/@genstudio/experience-selector/umd/standalone.js"></script>
```

## 配置属性

`renderExperienceSelectorWithSUSI`函数接受具有以下属性的配置对象：

| 属性 | 类型 | 必需 | 描述 |
|----------|------|----------|-------------|
| `apiKey` | 字符串 | 是 | GenStudio服务的API密钥 |
| `imsOrg` | 字符串 | 是 | IMS组织ID |
| `env` | 字符串 | 是 | 环境(`stage`， `prod`) |
| `susiConfig` | 对象 | 是 | [SUSI身份验证配置](#susi-configuration) |
| `onSelectionConfirmed` | 函数 | 是 | 确认选择后回调 |
| `onDismiss` | 函数 | 是 | 关闭对话框时的回调 |
| `locale` | 字符串 | 否 | 语言区域设置（例如，`en-US`） |
| `isOpen` | 布尔型 | 否 | 初始对话框状态 |
| `selectionType` | 字符串 | 否 | 选择模式（`single`或`multiple`） |
| `customFilters` | 数组 | 否 | 自定义筛选条件 |
| `dialogTitle` | 字符串 | 否 | 自定义对话框标题 |

### SUSI配置

`susiConfig`对象可能包括：

```javascript
{
  clientId: 'genstudio',
  environment: 'stg1', // or 'prod'
  scope: 'additional_info.projectedProductContext,additional_info.ownerOrg,AdobeID,openid,session,read_organizations,ab.manage',
  locale: 'en_US',
  modalSettings: {
    width: 500,
    height: 700
  }
}
```

## 快速启动

1. **从以下可用示例中选择您的框架**
1. **导航到示例目录**
1. **安装依赖项**（用于React/Vue示例）
1. **使用您的API密钥和IMS组织更新配置**：

   ```javascript
   const experienceSelectorProps = {
     locale: 'en-US',
     apiKey: 'exc_app',           
     imsOrg: 'your-ims-org@AdobeOrg',  // Replace with your IMS Org
     env: 'stage', // or 'prod'
     susiConfig: {
        clientId: 'genstudio',
        environment: 'stg1', // or 'prod'
        scope: 'additional_info.projectedProductContext,additional_info.ownerOrg,AdobeID,openid,session,read_organizations,ab.manage',
        locale: 'en_US',
        modalSettings: {
          width: 500,
          height: 700,
        },
     },
     customFilters: ['genstudio-channel:email'],
     selectionType: 'single', // or 'multiple'
     dialogTitle: 'Select Email Templates'
   };
   ```

1. **运行开发服务器**

### 实施示例

此存储库包含不同框架的工作示例：

- [一个&#x200B;**完整的React应用程序**，演示与Vite生成系统](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/react-js)的集成。

- [具有组合API集成的&#x200B;**Vue 3应用程序**](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vue-js)。

- [两个&#x200B;**Vanilla JavaScript实施**](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vanilla-js)：

   - [此&#x200B;**Vanilla ESM**&#x200B;版本使用ES6模块和现代JavaScript](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vanilla-js/vanilla-esm)。

   - [此&#x200B;**Vanilla UMD**&#x200B;版本使用通过脚本标记](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vanilla-js/vanilla-umd-global-var)加载的UMD捆绑包。

## 身份验证流程

Experience Selector通过SUSI自动处理身份验证：

1. 对话框打开时，将检查是否存在现有的身份验证。
1. 如果未经过身份验证，则会打开SUSI登录流程。
1. 成功验证后，将显示体验选择器。
1. 用户可以浏览并选择体验。
1. 选定的体验通过`onSelectionConfirmed`回调返回。
