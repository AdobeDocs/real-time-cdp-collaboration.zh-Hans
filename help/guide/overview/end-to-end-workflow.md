---
title: 端到端工作流程
description: 了解根据您的协作模式使用Real-Time CDP Collaboration的端到端工作流程。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/cn/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 90f9341e-5dd7-4521-a602-edb0263838c5
source-git-commit: 36f43d9d34ce7851a1c7093e0891f9c87e56387c
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 0%

---

# 端到端工作流程

{{limited-availability-release-note}}

在Adobe Real-Time CDP Collaboration中，端到端工作流会因您选择的协作模式而异。 该工作流概述了设置和执行协作项目所涉及的各个步骤，从创建帐户和采购受众到建立连接和创建项目。 了解此工作流对于有效利用平台的功能来实现营销目标至关重要。

## 快速入门

在开始之前，请确保您对这些关键概念有深入的了解：

- **Collaboration模式**：这些模式定义了协作者如何协作。 有两种不同的模式：[广告商对发布商](./collaboration-patterns.md#advertiser-to-publisher)和[品牌对品牌](./collaboration-patterns.md#brand-to-brand)。
- **帐户角色**：帐户角色决定您在平台中的功能。 它们应与贵组织的目标、品牌和目标相一致。 有两种帐户角色：[广告商](./roles.md#advertiser)和[发布者](./roles.md#publisher)。
- **用例**：用例定义了利用Collaboration实现营销目标的方法。 存在三个协作用例：[发现](./use-cases.md#discover)、[激活](./use-cases.md#activate)和[度量](./use-cases.md#measure)。

本指南将使用三个模拟的协作者来说明端到端工作流程：

- **[!UICONTROL Luma]**：运动服装品牌。 他们是一家希望通过有针对性的营销活动触及特定受众的广告商。
- **[!UICONTROL TV Tube]**：数字流提供商。 它们是发布者，提供受众数据供广告商使用。
- **[!UICONTROL 适合服装]**：另一个运动服装品牌。 他们是第二个希望进行协作以共享受众数据和洞察信息的广告商，以便加强营销工作。

## 广告商到发布商工作流程 {#advertiser-to-publisher-workflow}

[!UICONTROL Luma]，一家体育零售公司，想要与数字流媒体提供商[!UICONTROL TV Tube]建立连接，以便通过有针对性的营销活动触及特定受众。

若要开始，[!UICONTROL Luma]需要使用广告商角色[创建帐户](../setup/onboard-account.md)，而[!UICONTROL TV Tube]使用发布者角色创建帐户。

建立帐户后，[!UICONTROL Luma]和[!UICONTROL TV Tube]都必须[创建数据连接和源受众](../setup/onboard-audiences.md)。 只有[!UICONTROL TV Tube]会激活营销活动的受众，因此他们需要[配置目标](../setup/manage-destinations.md)。

一旦两个协作者都设置了帐户，他们就准备好[在平台内建立连接](../connect/establishing-connections.md)。 [!UICONTROL Luma]使用[发现协作者](../connect/discover-collaborators.md)功能查找[!UICONTROL TV Tube]并启动连接请求。 在[!UICONTROL TV Tube]接受连接请求后，[!UICONTROL Luma]将配置连接设置以定义协作方式。 [!UICONTROL TV Tube]接受连接请求，以便在两个品牌之间建立安全链接。

建立连接后，[!UICONTROL Luma] [创建一个项目](../collaborate/manage-projects.md)以开始他们与[!UICONTROL TV Tube]的协作。 在项目设置过程中，他们选择最符合其目标的协作用例：[发现](../collaborate/discover.md)、[激活](../collaborate/activate.md)和[度量](../collaborate/measure.md)。

[!UICONTROL Luma]利用[Discover](../collaborate/discover.md)用例来分析[!UICONTROL TV Tube]的受众数据。 在[!UICONTROL Luma]识别目标受众区段后，他们[激活](../collaborate/activate.md)这些受众。

激活受众后，[!UICONTROL TV Tube]运行目标营销活动，并将数据上传到[衡量](../collaborate/measure.md)结果，以评估其营销活动的有效性。

## 品牌到品牌工作流程 {#brand-to-brand-workflow}

[!UICONTROL Fit Apparel]是一个运动服装品牌，它希望与另一个运动服装品牌[!UICONTROL Luma]合作，以共享受众数据和见解，从而加强营销工作。

建立帐户后，[!UICONTROL 适合服装]和[!UICONTROL Luma]都需要[创建数据连接和源受众](../setup/onboard-audiences.md)。 [!UICONTROL 适合服装]和[!UICONTROL Luma]都将激活营销活动的受众，因此它们都需要[配置目标](../setup/manage-destinations.md)。

在获取受众后，[!UICONTROL Fit Apparel]和[!UICONTROL Luma][在平台内形成连接](../connect/establishing-connections.md)以安全地共享受众数据。 为此，他们必须使用[专用连接邀请](../connect/establishing-connections.md#private-connection-invite)功能。 [!UICONTROL Luma]与[!UICONTROL Fit服装]共享其连接代码，后者随后使用它来启动连接请求。 在[!UICONTROL Luma]接受连接请求后，[!UICONTROL Fit Apparel]将配置连接设置以定义他们将如何协作。 在配置中，[!UICONTROL Fit Apparel]指定两个协作者都可以激活营销活动的受众。 为了完成连接，[!UICONTROL Luma]接受在两个品牌之间建立安全链接的请求。

建立连接后，[!UICONTROL Fit Apparel] [创建一个项目](../collaborate/manage-projects.md)以开始他们与[!UICONTROL Luma]的协作。 在项目设置过程中，他们选择最符合其目标的协作用例：[发现](../collaborate/discover.md)、[激活](../collaborate/activate.md)和[度量](../collaborate/measure.md)。

[!UICONTROL Fit服装]和[!UICONTROL Luma]都可以使用[发现](../collaborate/discover.md)用例来深入了解彼此的受众数据。 确定有价值的受众区段后，他们[激活](../collaborate/activate.md)为营销活动选择的受众。

最后，在执行其促销活动后，两个品牌都会将数据上传到[度量](../collaborate/measure.md)结果并评估其协作的有效性。
