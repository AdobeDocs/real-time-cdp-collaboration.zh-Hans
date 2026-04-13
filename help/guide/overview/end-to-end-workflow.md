---
title: 端到端工作流程
description: 了解根据您的协作模式使用Real-Time CDP Collaboration的端到端工作流程。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 90f9341e-5dd7-4521-a602-edb0263838c5
source-git-commit: 901b17c7493e76b17e780b6f7b05a69fa22303d2
workflow-type: tm+mt
source-wordcount: '1738'
ht-degree: 0%

---

# 端到端工作流程

{{limited-availability-release-note}}

在Adobe Real-Time CDP Collaboration中，端到端工作流会因您选择的协作模式而异。 该工作流概述了设置和执行协作项目所涉及的各个步骤，从创建帐户和采购受众到建立连接和创建项目。 了解此工作流对于有效利用平台的功能来实现营销目标至关重要。

## 快速入门

在开始之前，请确保您对这些关键概念有深入的了解：

- **Collaboration模式**：这些模式定义了协作者如何协作。 有五种不同的模式：
   - [广告商对发布商](./collaboration-patterns.md#advertiser-to-publisher)
   - [品牌到品牌](./collaboration-patterns.md#brand-to-brand)
   - [广告商到数据合作伙伴](./collaboration-patterns.md#advertiser-to-data-partner)
   - [代理到发布者](./collaboration-patterns.md#agency-to-publisher)
   - [广告商到代理平台](./collaboration-patterns.md#advertiser-to-agency-platform)
- **帐户角色**：帐户角色决定您在平台中的功能。 它们应与贵组织的目标、品牌和目标相一致。 有四个帐户角色： [广告商](./roles.md#advertiser)、[发布者](./roles.md#publisher)、[代理](./roles.md#agency)和[数据合作伙伴](./roles.md#data-partner)。
- **用例**：用例定义了利用Collaboration实现营销目标的方法。 存在三个协作用例：[发现](./use-cases.md#discover)、[激活](./use-cases.md#activate)和[度量](./use-cases.md#measure)。

本指南将使用三个模拟的协作者来说明端到端工作流程：

- **[!UICONTROL Luma]**：运动服装品牌。 他们是一家希望通过有针对性的营销活动触及特定受众的广告商。
- **[!UICONTROL TV Tube]**：数字流提供商。 它们是发布者，提供受众数据供广告商使用。
- **[!UICONTROL 适合服装]**：另一个运动服装品牌。 他们是第二个希望进行协作以共享受众数据和洞察信息的广告商，以便加强营销工作。
- **[!UICONTROL 代理99]**：媒体代理。 他们在其工作区中管理多个客户帐户，并与发布者和广告商联系。
- **[!UICONTROL DataM8]**：第三方数据提供程序。 它们提供受众数据供广告商使用。
- **[!UICONTROL Holdco]**：一个代理公司营销和广告服务平台，内部代理团队使用该平台来管理客户营销活动。

## 广告商到发布商工作流程 {#advertiser-to-publisher-workflow}

[!UICONTROL Luma]，一家体育零售公司，想要与数字流媒体提供商[!UICONTROL TV Tube]建立连接，以便通过有针对性的营销活动触及特定受众。

若要开始，[!UICONTROL Luma]需要使用广告商角色[创建帐户](../setup/onboard-account.md)，而[!UICONTROL TV Tube]使用发布者角色创建帐户。

建立帐户后，[!UICONTROL Luma]和[!UICONTROL TV Tube]都必须[创建数据连接和源受众](../setup/onboard-audiences.md)。 只有[!UICONTROL TV Tube]会激活营销活动的受众，因此他们需要[配置目标](../setup/manage-destinations.md)。

一旦两个协作者都设置了帐户，他们就准备好[在平台内建立连接](../connect/establishing-connections.md)。 [!UICONTROL Luma]使用[发现协作者](../connect/discover-collaborators.md)功能查找[!UICONTROL TV Tube]并启动连接请求。 在[!UICONTROL TV Tube]接受连接请求后，[!UICONTROL Luma]将配置连接设置以定义他们将如何协作。 [!UICONTROL TV Tube]接受连接请求，以便在两个品牌之间建立安全链接。

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

## 广告商到广告平台的工作流程 {#advertiser-to-advertising-platform-workflow}

[!UICONTROL Luma]，一家体育零售公司，想要与[!DNL Amazon Marketing Cloud] ([!DNL AMC])联系，以利用[!DNL AMC]的标识解析和定位工具来增强其营销能力。 Luma已具有活动的[!DNL Amazon Advertising]帐户，并且已批准使用[!DNL AMC]。

若要开始，[!UICONTROL Luma]需要使用广告商角色[创建帐户](../setup/onboard-account.md)。 建立帐户后，[!UICONTROL Luma]必须[创建数据连接和源受众](../setup/onboard-audiences.md)。 由于[!UICONTROL Luma]将激活营销活动的受众，因此他们需要[配置目标](../setup/manage-destinations.md)。

在[!UICONTROL Luma]设置好帐户后，他们便已准备好在平台中[与[!DNL AMC]建立连接](../connect/establishing-connections.md)。 [!UICONTROL Luma]使用[发现协作者](../connect/discover-collaborators.md)功能查找[!UICONTROL Amazon Marketing Cloud]和[启动连接请求](../connect/advertising-platforms/amc.md)。 在通过[!DNL Amazon]登录页面验证并授权连接后，已建立与[!DNL AMC]的连接。

建立连接后，[!UICONTROL Luma] [创建一个项目](../collaborate/manage-projects.md)以开始他们与[!DNL AMC]的协作。 连接设置（包括用例）会根据广告平台进行预配置。 对于[!DNL AMC]，可用的用例是[发现](../collaborate/advertising-platforms/amc.md#discover)。

[!UICONTROL Luma]利用[发现](../collaborate/advertising-platforms/amc.md#discover)用例从[!DNL AMC]获取见解和受众数据。 利用这些见解，[!UICONTROL Luma]可以优化其营销策略并提高促销活动有效性。

## 广告商到数据合作伙伴工作流程 {#advertiser-to-data-partner-workflow}

[!UICONTROL Luma]（一家体育零售公司）希望与第三方数据提供商[!UICONTROL DataM8]协作，以丰富客户配置文件并改进受众定位。

若要开始，[!UICONTROL Luma]需要使用广告商角色[创建帐户](../setup/onboard-account.md)，而[!UICONTROL DataM8]使用数据合作伙伴角色创建帐户。

建立帐户后，[!UICONTROL Luma]和[!UICONTROL DataM8]都必须[创建数据连接和源受众](../setup/onboard-audiences.md)。 两个协作者都可以为营销活动激活受众，因此他们各自需要[配置目标](../setup/manage-destinations.md)。

一旦两个协作者都设置了帐户，他们就准备好[在平台内建立连接](../connect/establishing-connections.md)。 [!UICONTROL Luma]使用[发现协作者](../collaborate/discover.md)功能查找[!UICONTROL DataM8]并启动连接请求。 在[!UICONTROL DataM8]接受连接请求后，[!UICONTROL Luma]将配置连接设置以定义他们将如何协作。 [!UICONTROL DataM8]接受连接请求，以便在两个协作者之间建立安全链接。

建立连接后，[!UICONTROL Luma] [创建一个项目](../collaborate/manage-projects.md)以开始他们与[!UICONTROL DataM8]的协作。 在项目设置过程中，他们选择最符合其目标的协作用例：[发现](../collaborate/discover.md)、[激活](../collaborate/activate.md)和[度量](../collaborate/measure.md)。

[!UICONTROL Luma]利用[Discover](../collaborate/discover.md)用例来分析[!UICONTROL DataM8]的受众数据。 在[!UICONTROL Luma]识别目标受众区段后，他们[激活](../collaborate/activate.md)这些受众。

[!UICONTROL DataM8]还可以[将其受众](../collaborate/activate.md)激活到[!UICONTROL Luma]。 [!UICONTROL Luma]使用这些功能将第三方属性附加到其客户配置文件并分析受众构成。 利用其CDP中直接提供的丰富数据，[!UICONTROL Luma]可以构建更准确的受众并将他们激活到付费媒体目标，而无需将数据移动到其控制的环境之外。

## 机构到发布者工作流程 {#agency-to-publisher-workflow}

[!UICONTROL Agency99]是一家媒体代理商，它希望与数字流媒体提供商[!UICONTROL TV Tube]合作，通过有针对性的营销活动来吸引特定受众。

若要开始，[!UICONTROL Agency99]需要[使用代理角色](../setup/onboard-account.md)创建帐户，而[!UICONTROL TV Tube]使用发布者角色创建帐户。

建立帐户后，[!UICONTROL Agency99]和[!UICONTROL TV Tube]都必须[创建数据连接和源受众](../setup/onboard-audiences.md)。 [!UICONTROL Agency99]将在其工作区中设置客户端子帐户和源客户端数据。 只有[!UICONTROL TV Tube]会激活营销活动的受众，因此他们需要[配置目标](../setup/manage-destinations.md)。

一旦两个协作者都设置了帐户，他们就准备好[在平台内建立连接](../connect/establishing-connections.md)。 [!UICONTROL Agency99]使用[发现协作者](../collaborate/discover.md)功能来查找[!UICONTROL TV Tube]并启动连接请求。 [!UICONTROL Agency99]将为一个或多个希望与[!UICONTROL TV Tube]协作的用户执行此操作。 在[!UICONTROL TV Tube]接受连接请求后，[!UICONTROL Agency99]将配置连接设置以定义每次协作的方式。 [!UICONTROL TV Tube]接受连接请求，以便在两个品牌之间建立安全链接。

建立连接后，[!UICONTROL Agency99] [创建一个项目](../collaborate/manage-projects.md)以开始与每个客户端子帐户中的[!UICONTROL TV Tube]合作。 在项目设置过程中，他们选择最符合其目标的协作用例：[发现](../collaborate/discover.md)、[激活](../collaborate/activate.md)和[度量](../collaborate/measure.md)。

[!UICONTROL Agency99]利用[Discover](../collaborate/discover.md)用例深入了解[!UICONTROL TV Tube]的受众数据。 一旦[!UICONTROL Agency99]识别出目标受众区段，他们[激活](../collaborate/activate.md)这些受众。

激活受众后，[!UICONTROL TV Tube]运行目标营销活动，并将数据上传到[衡量](../collaborate/measure.md)结果，以评估其营销活动的有效性。

## 广告商到代理平台工作流程 {#advertiser-to-agency-platform-workflow}

[!UICONTROL Luma]是一家体育零售公司，它希望与代理平台[!UICONTROL Holdco]合作，以共享数据并接收付费媒体分析。

若要开始，[!UICONTROL Luma]需要使用广告商角色[创建帐户](../setup/onboard-account.md)，而[!UICONTROL Holdco]使用代理角色创建帐户。 

建立帐户后，[!UICONTROL Luma]和[!UICONTROL Holdco]都必须[创建数据连接和源受众](../setup/onboard-audiences.md)。 两个协作者都可以为营销活动激活受众，因此他们各自需要[配置目标](../setup/manage-destinations.md)。 

一旦两个协作者都设置了帐户，他们就准备好[在平台内建立连接](../connect/establishing-connections.md)。 [!UICONTROL Luma]使用[发现协作者](../collaborate/discover.md)功能查找[!UICONTROL Holdco]并启动连接请求。 在[!UICONTROL Holdco]接受连接请求后，[!UICONTROL Luma]将配置连接设置以定义他们将如何协作。

[!UICONTROL Holdco]接受连接请求，以便在两个协作者之间建立安全链接。

建立连接后，[!UICONTROL Luma] [创建一个项目](../collaborate/manage-projects.md)以开始他们与[!UICONTROL Holdco]的协作。 在项目设置过程中，他们选择最符合其目标的协作用例：[发现](../collaborate/discover.md)、[激活](../collaborate/activate.md)和[度量](../collaborate/measure.md)。

[!UICONTROL Luma]利用[Discover](../collaborate/discover.md)用例来分析[!UICONTROL Holdco]的受众数据。 在[!UICONTROL Luma]识别目标受众区段后，他们[激活](../collaborate/activate.md)这些受众。

[!UICONTROL Holdco]还可以[激活其受众](../collaborate/activate.md)以[!UICONTROL Luma]。 [!UICONTROL Luma]使用这些功能接收机构运行的营销活动的付费媒体分析，以获取见解、CDP个人资料附加和自有媒体编排。
