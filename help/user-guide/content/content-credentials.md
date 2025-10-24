---
title: Content Credentials组织版
description: 了解如何在GenStudio for Performance Marketing中应用和查看Content Credentials。
level: Intermediate
feature: Content Management, Content Attributes
source-git-commit: b7e3d1c3b20149eee85670098ddd100b41e27f2c
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 0%

---

# Content Credentials组织版

了解用于证明品牌真实性并促进合规性的内容的防篡改凭据如何直接嵌入您的营销工作流程中。

>[!WARNING]
>
>此功能当前为测试版，仅适用于已被授予访问权限的组织。 如有兴趣，请联系您的Adobe客户团队代表进行注册。


## Content Credentials入门

在Admin Console中激活Content Credentials后，GenStudio for Performance Marketing用户可以在应用程序中全局启用所有资产的Content Credentials。 如果应用凭据的全局选项处于关闭状态，则用户可以选择为每个单独的资源应用Content Credentials。

发布内容后，Content Credentials将显示在外部平台上，如LinkedIn。

管理员负责在Admin Console中上传有效的X.509证书。 此步骤可确保企业的数字签名配置正确，并可在支持的Adobe DX应用程序中使用。

>[!NOTE]
>
>控制此设置可能会在将来过渡到Admin Console，从而简化跨应用程序的Content Credentials管理并增强行政监督。

## 什么是Content Credentials？ 

Content Credentials是一种持久的行业标准元数据类型，其中包含有关如何制作内容的详细信息以及有关创建者的身份信息。 当内容在线发布到支持平台时，或者使用诸如[Adobe的Inspect tool](https://contentauthenticity.adobe.com/inspect)或[Adobe Content Authenticity Chrome浏览器扩展](https://helpx.adobe.com/creative-cloud/help/cai/adobe-content-authenticity-chrome-browser-extension.html)之类的工具时，可以查看Content Credentials。  

应用Content Credentials有助于提高内容制作方式的透明度，并且可帮助您的用户将自己连接到其内容。

在Adobe上[了解有关Content Credentials的更多信息](https://helpx.adobe.com/cn/creative-cloud/help/content-credentials.html)。

## 品牌签名和资产跟踪

品牌签署内容在促进品牌完整性和用户信任方面起着重要作用。 如果在Admin Console中正确配置了组织证书，则组织可以使用Adobe应用程序中的独特品牌签名对内容进行签名。 使用不可见水印和指纹技术维护这种真实性保证，这有助于在内容的整个生命周期中保持签名的持久性。

除了品牌签名之外，企业还可以直接将资产ID附加到其内容。 这有助于有效跟踪资产，尤其是当资产在社交媒体平台上共享或发布时。 通过整合资产ID，组织可以跟踪其内容的来源和分发路径，从而加强监督和问责。

## 营销工作流中的Content Credentials

可以直接在GenStudio for Performance Marketing中在整个营销工作流程中应用Content Credentials，从导入和内容发现到激活和导出。 您还可以在内容上找到显示的凭据，以供在整个应用程序中查看。

### 导入和发现

在内容库中，凭据将显示在导入的资产上。

缩略图右上角的Content Credential徽章表示“Brand signed”内容。

![已导入具有凭据的资产](./images/import-discovery1.png){width="350"}

选择已签署的内容会显示详细的元数据：已发布的品牌、录制器、使用的工具、时间戳。

可按凭据状态筛选内容。

![资产上的凭据数据](./images/import-discovery2.png)

### 创建和选择

Content Credential徽章将显示在画布资源选择器中。

在为体验选择资产以在编辑过程中维护来源链时，会保留凭据元数据。

画布资源选择器中的![Content Credential徽章](./images/creation-selection1.png)

### 编辑和转换

在从草稿导出期间，修改后的资产会自动重新签名，并且新凭据将链接到原始凭据。

![已导出资产的凭据数据](./images/edit-and-transformation1.png){width="300"}

### 审阅和批准

在“审核并批准”预览中，将在右边栏中显示资产的凭据状态。

![已批准资产上的凭据数据](./images/review-and-approve1.png){width="300"}

当审阅者检查资产时，会显示每个变体的凭据详细信息。 当用户单击“保存到内容”****&#x200B;时，已批准的体验将被重新签名。

![已批准资产上的凭据数据](./images/review-and-approve2.png)

### 激活和导出

在激活期间，体验选择器中会显示凭据状态。

![已激活资产的凭据数据](./images/activate-export1.png){width="350"}

导出的文件将嵌入符合C2PA的凭据。

凭据完整性在所有支持的格式(JPEG、PNG、MP4)中得到了维护。

![已导出资产的凭据数据](./images/activate-export2.png)

