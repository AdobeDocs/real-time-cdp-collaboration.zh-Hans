---
title: 端到端工作流程
description: Understand the end-to-end workflow of using Real-Time CDP Collaboration based on your collaboration pattern.
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 90f9341e-5dd7-4521-a602-edb0263838c5
TQID: https://experienceleague.adobe.com/9edtg5tMbnB3BrdLrDkcHQ-AjBNOqMFGojAja3NCwCs
product_v2: id: fdddec33-c9cb-4459-b8b6-2664395a6f10
feature_v2: id: ba929a52-9339-4154-9487-317dc875a3c7
topic_v2: id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 3ce7e66b31332836fd6cc6137c94622436505cc9
workflow-type: tm+mt
source-wordcount: 1738
ht-degree: 0%

---

# 端到端工作流程

{{limited-availability-release-note}}

In Adobe Real-Time CDP Collaboration, the end-to-end workflow varies based on the collaboration pattern you choose. The workflow outlines the steps involved in setting up and executing a collaboration project, from creating accounts and sourcing audiences to forming connections and creating projects. Understanding this workflow is essential for effectively leveraging the platform&#39;s capabilities to achieve your marketing goals.

## 快速入门

Before you begin, ensure you have a solid understanding of these key concepts:

- **Collaboration patterns**: These patterns define how collaborators work together. There are five distinct patterns:
   - [advertiser-to-publisher](./collaboration-patterns.md#advertiser-to-publisher)
   - [brand-to-brand](./collaboration-patterns.md#brand-to-brand)
   - [advertiser-to-data partner](./collaboration-patterns.md#advertiser-to-data-partner)
   - [agency-to-publisher](./collaboration-patterns.md#agency-to-publisher)
   - [advertiser-to-agency platform](./collaboration-patterns.md#advertiser-to-agency-platform)
- **Account roles**: Account roles determine your capabilities within the platform. They should align with your organization&#39;s objectives, brand, and goals. There are four account roles: [advertiser](./roles.md#advertiser), [publisher](./roles.md#publisher), [agency](./roles.md#agency) and [data partner](./roles.md#data-partner).
- **Use cases**: Uses cases define the ways you can leverage Collaboration to achieve your marketing objectives. There are three collaboration use cases: [Discover](./use-cases.md#discover), [Activate](./use-cases.md#activate), and [Measure](./use-cases.md#measure).

This guide will use three mock collaborators to illustrate the end-to-end workflow:

- **[!UICONTROL Luma]**: An athletic apparel brand. They are an advertiser that wants to reach specific audiences through targeted marketing campaigns.
- **[!UICONTROL TV Tube]**: A digital streaming provider. They are a publisher that provides audience data for use by advertisers.
- **[!UICONTROL Fit Apparel]**: Another athletic apparel brand. 他们是第二个希望进行协作以共享受众数据和洞察信息的广告商，以便加强营销工作。
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

[!UICONTROL Luma], an athletic retail company, wants to collaborate with [!UICONTROL DataM8], a third-party data provider, to enrich customer profiles and improve audience targeting.

To begin, [!UICONTROL Luma] needs to [create an account](../setup/onboard-account.md) with the advertiser role, while [!UICONTROL DataM8] creates an account with the data partner role.

After establishing their accounts, both [!UICONTROL Luma] and [!UICONTROL DataM8] must [create a data connection and source audiences](../setup/onboard-audiences.md). Both collaborators may activate audiences for marketing campaigns, so they each need to [configure a destination](../setup/manage-destinations.md).

Once both collaborators have their accounts set up, they&#39;re ready to [form a connection](../connect/establishing-connections.md) within the platform. [!UICONTROL Luma] uses the [discover collaborators](../collaborate/discover.md) feature to find [!UICONTROL DataM8] and initiate a connection request. After [!UICONTROL DataM8] accepts the connection request, [!UICONTROL Luma] configures the connection settings to define how they will collaborate. [!UICONTROL DataM8] accepts the connection request to establish a secure link between the two collaborators.

After the connection is established, [!UICONTROL Luma] [creates a project](../collaborate/manage-projects.md) to kick off their collaboration with [!UICONTROL DataM8]. During the project setup, they choose the collaboration use cases that best fit their objectives: [Discover](../collaborate/discover.md), [Activate](../collaborate/activate.md), and [Measure](../collaborate/measure.md).

[!UICONTROL Luma] leverages the [Discover](../collaborate/discover.md) use case to gain insights into [!UICONTROL DataM8]&#39;s audience data. Once [!UICONTROL Luma] has identified the target audience segments, they [activate](../collaborate/activate.md) these audiences.

[!UICONTROL DataM8] can also [activate](../collaborate/activate.md) their audiences to [!UICONTROL Luma]. [!UICONTROL Luma] uses these capabilities to append third-party attributes to its customer profiles and analyze audience composition. With enriched data available directly in its CDP, [!UICONTROL Luma] can build more precise audiences and activate them to paid media destinations without moving data outside its governed environment.

## Agency-to-publisher workflow {#agency-to-publisher-workflow}

[!UICONTROL Agency99], a media agency, wants to collaborate with [!UICONTROL TV Tube], a digital streaming provider, to reach specific audiences through targeted marketing campaigns.

To begin, [!UICONTROL Agency99] needs to [create an account](../setup/onboard-account.md) with the agency role, while [!UICONTROL TV Tube] creates an account with the publisher role.

After establishing their accounts, both [!UICONTROL Agency99] and [!UICONTROL TV Tube] must [create a data connection and source audiences](../setup/onboard-audiences.md). [!UICONTROL Agency99] will set up client sub-accounts and source client data within its workspace. Only [!UICONTROL TV Tube] will activate audiences for marketing campaigns, so they need to [configure a destination](../setup/manage-destinations.md).

Once both collaborators have their accounts set up, they&#39;re ready to [form a connection](../connect/establishing-connections.md) within the platform. [!UICONTROL Agency99] uses the [discover collaborators](../collaborate/discover.md) feature to find [!UICONTROL TV Tube] and initiate a connection request. [!UICONTROL Agency99] will do this for one or multiple clients that want to collaborate with [!UICONTROL TV Tube]. After [!UICONTROL TV Tube] accepts the connection request(s), [!UICONTROL Agency99] configures the connection settings to define how each collaboration. [!UICONTROL TV Tube]接受连接请求，以便在两个品牌之间建立安全链接。

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
