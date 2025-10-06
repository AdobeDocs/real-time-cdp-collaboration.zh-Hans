---
title: 连接概述
description: 了解Real-Time CDP Collaboration中的连接。
audience: publisher, advertiser
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
source-git-commit: 5c08738cdc8e1e208203ee1f9a1cf1891b5b07cb
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 0%

---

# 连接概述

{{limited-availability-release-note}}

协作者必须先建立连接，然后才能一起处理营销活动。 利用此连接，他们可以激活受众、创建项目并运行营销活动效果报表。

连接是根据您选择的协作模式建立的。 Collaboration支持三种关键协作模式：广告商到发布商、品牌到品牌和广告商到广告平台。 要了解有关这些模式的更多信息，请参阅[协作模式](/help/guide/overview/collaboration-patterns.md)指南。

要了解如何建立连接，请阅读以下与您的协作模式对应的部分：

- [广告商与发布商的连接](#advertiser-to-publisher-connection)
- [品牌到品牌连接](#brand-to-brand-connection)
- [广告商到广告平台的连接](#advertiser-to-advertising-platform-connection)

## 广告商与发布商的连接 {#advertiser-to-publisher-connection}

![广告商 — 发布商连接过程的高级图表。](/help/assets/connect/establish-connection/advertiser-publisher-flow.png){zoomable="yes"}

在广告商对发布商模式中，广告商通过&#x200B;**[!UICONTROL Discover publishers]**&#x200B;工作区发现要与之合作的发布商，并发送连接邀请。 然后，发布者会审核并接受邀请，从而允许广告商提出连接设置。 一旦发布者接受连接设置，连接就会建立，两个协作者就可以开始一起处理项目。

### 高级概述

要在广告商和发布商之间建立连接，需要执行以下步骤：

1. [发现发布者](./discover-collaborators.md)：广告商标识要与之协作的潜在发布者。
2. [发送邀请](./establishing-connections.md#send-invite)：广告商向选定的发布者发送连接邀请。
3. [接受邀请](./establishing-connections.md#accept-invite)：发布者审核并接受邀请。
4. [配置连接设置](./establishing-connections.md#configure-connection-settings)：广告商配置连接设置并将它们发送给发布者以供审阅。
5. [确认连接设置](./establishing-connections.md#review-connection-settings)：发布者查看连接设置并接受或拒绝它们。 如果接受，则建立连接。 如果被拒绝，发布者可以为产品之外的修订提供反馈。 然后，广告商可以修改设置并重新发送这些设置以供审阅。

接受连接设置后，即建立连接，协作者已准备[创建项目](/help/guide/collaborate/manage-projects.md#create-project)以开始协作营销活动。

## 品牌到品牌连接 {#brand-to-brand-connection}

![品牌到品牌连接过程的高级图表。](/help/assets/connect/establish-connection/brand-to-brand-flow.png){zoomable="yes"}

>[!TIP]
>
>术语&#x200B;**brand**&#x200B;用于引用Collaboration之外的公司或品牌。 术语&#x200B;**协作者**&#x200B;是指可在Collaboration中建立连接的任何帐户，无论它们是广告商还是发布者。

在品牌到品牌模式中，在产品外部沟通的两个品牌可以使用[私有连接邀请](#private-connection-invite)直接在Collaboration中连接。 品牌既可以是广告商，也可以是发布者。 此模式对于可能不符合传统广告商 — 出版商模式的品牌特别有用，例如两个广告商或两个出版商。

首先，协作者向另一个协作者发送专用连接邀请。 收件人会查看并接受邀请，从而允许所有者建议连接设置。 收件人接受连接设置后，即可建立连接，两个协作者可以开始一起处理项目。

### 高级概述

>[!TIP]
>
>在讨论连接过程时，**所有者**&#x200B;和&#x200B;**收件人**&#x200B;之间存在区别。 所有者是通过发送邀请来启动连接的协作者，而收件人则是接收并审阅邀请的协作者。

两个品牌之间的连接过程包括几个步骤。 在连接过程开始之前，必须满足几个先决条件：

1. 两个品牌在产品之外沟通，讨论潜在的联系。
1. 品牌[在Collaboration中创建帐户](/help/guide/setup/onboard-account.md)（如果尚未创建），请确保选择适当的角色类型（广告商或发布商）。

满足前提条件后，即可开始连接过程。 以下步骤概述了该过程：

1. [发送专用连接邀请](./establishing-connections.md#private-connection-invite)：一个协作者向另一个协作者发送专用连接邀请。
2. [接受专用连接邀请](./establishing-connections.md#accept-invite)：收件人审阅并接受专用连接邀请。
3. [配置连接设置](./establishing-connections.md#configure-connection-settings)：所有者配置连接设置并将它们发送给收件人进行审查和接受。
4. [确认连接设置](./establishing-connections.md#review-connection-settings)：收件人查看连接设置并接受或拒绝它们。

接受连接设置后，即建立连接，协作者已准备[创建项目](/help/guide/collaborate/manage-projects.md#create-project)以开始协作营销活动。

## 广告商到广告平台的连接 {#advertiser-to-advertising-platform-connection}

广告商到广告平台的连接过程允许广告商与第三方广告平台(如Amazon Marketing Cloud (AMC))连接，以增强其营销功能。

### 高级概述

广告商和广告平台之间的连接过程包括几个步骤。 在连接过程开始之前，请确保您在广告平台中拥有活动帐户，并且已批准您使用其服务。 以下步骤概述了连接过程：

1. [发现广告平台](./discover-collaborators.md)：广告商标识要与之协作的潜在广告平台。
2. [连接到广告平台](./advertising-platforms/overview.md#advertising-platforms-overview)：广告商通过选择要连接的广告平台来启动连接过程，并按照提示验证和授权连接。
