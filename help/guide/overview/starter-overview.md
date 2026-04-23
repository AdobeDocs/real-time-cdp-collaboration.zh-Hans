---
title: RTCDP Collaboration Starter Overview
description: Learn how Adobe Real-Time CDP Collaboration Starter helps you to expand and enhance privacy-centric collaboration with a licensed partner without requiring your own full Real-Time CDP license.
audience: publisher, advertiser, invited users to Real-Time CDP Collaboration Starter
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/cn/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 7ae0bd3d-eee9-48c0-9f18-a56033fee52d
source-git-commit: 3d29985d88e6370b4a0e8cd3d56358e85bb91e06
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 4%

---

# Adobe Real-Time CDP Collaboration [!DNL Starter] Overview

Use Adobe Real-Time CDP Collaboration [!DNL Starter] to collaborate with a licensed partner on privacy-centric data projects. You do not need your own Collaboration license to participate.

Your licensed partner invites you into Collaboration and uses their credits to fund your joint workflows, across both advertiser-to-publisher and brand-to-brand patterns. To learn more about these patterns and how they work, read the [collaboration patterns](./collaboration-patterns.md) and [end-to-end workflow](./end-to-end-workflow.md) guides.

As an invited [!DNL Starter] user, you can:

* Onboard and manage collaboration data in a [!DNL Starter] account.
* Source and maintain audiences for use in joint projects.
* Gain insights into audience overlaps with your partner to support effective targeting and campaign measurement.
* Activate audiences and share them back to your partner for joint campaign activation and engagement.

## 先决条件 {#prerequisites}

To get started with Collaboration [!DNL Starter], ensure that both your organization and your licensed partner are located in the same region. You must be invited by a partner who holds a Real-Time CDP Prime, Ultimate, or Collaboration license.

To initiate the invitation, provide the following information to your licensed partner:

* Contact name
* 联系电子邮件
* Company
* Role (Advertiser/Publisher): Advertiser
* 行业

After you receive and accept the invitation, your organization must review and sign a no-cost Sales Order with Adobe to access Collaboration [!DNL Starter]. For more details on the invitation process, see the [inviting a collaborator to Collaboration [!DNL Starter]](../connect/establishing-connections.md#invite-collaborator-to-starter) guide.

## 护栏 {#guardrails}

Read the following table to understand the key guardrails that apply to your [!DNL Starter] account. These include limits on audience sourcing, data volume, refresh frequency, audience overlaps and activation capabilities.

| Guardrail | 描述 |
|----------| ------------|
| 受众来源 | You can bring audience data into Collaboration with **[!DNL Amazon S3]** as your source. For step-by-step instructions, see [how to configure [!DNL Amazon S3] for audience sourcing](../setup/configure-aws-s3-audience-sourcing.md). |
| 受众 | 您的[!DNL Starter]帐户有权使用的最大值为：<ul><li>来自[!DNL AWS S3]存储段的10个受众</li><li>总身份数5,000万（由受众数据中的行数计算）</li><li>每个受众每6天刷新1次</li></ul> |
| 受众重叠和见解 | 您的受众可以运行受众重叠和分析的频率没有使用限制。 了解如何[发现重叠和比较受众](../collaborate/discover.md)。 |
| 激活 | 作为[!DNL Starter]用户，您只能激活受众并与邀请您的合作伙伴共享受众。 目标到外部平台的配置不可用。 了解有关[激活受众的详细信息](../collaborate/activate.md)。 |

{style="table-layout:auto"}

## 快速入门 {#getting-started}

在您[接受邀请并同意条款](../connect/establishing-connections.md#accept-invitation-sign-terms)后，请使用您的凭据登录[Adobe Experience Cloud](https://experience.adobe.com/){target="_blank"}。 在使用Collaboration之前，必须向您的帐户授予适当的访问权限和角色。

使用此工作流设置您的[!DNL Starter]帐户并开始与合作伙伴协作。

### 设置管理员访问权限 {#setup-admin-access}

首先，使用&#x200B;**管理员访问权限**&#x200B;工作区授予您自己必要的访问权限。 这可以确保您同时具有Experience Platform产品的管理权限和用户访问权限。 有关如何设置初始访问的详细步骤，请参阅[管理员访问说明](../setup/starter-admin-access.md)。

完成后，您应会在[Experience Platform](https://experience.adobe.com/){target="_blank"}主页上的&#x200B;**[!UICONTROL 快速访问]**&#x200B;部分中看到&#x200B;**[!UICONTROL 权限]**、**[!UICONTROL Adobe Experience Cloud]**&#x200B;和&#x200B;**[!UICONTROL Real-Time CDP Collaboration]**。

![Adobe Experience Cloud工作区在产品管理员访问设置后显示权限、Experience Platform和Real-Time CDP Collaboration。](/help/assets/overview/starter/setup-admin-access.png){zoomable="yes"}

有关访问角色和其他Adobe Experience Cloud产品的更多详细信息，请阅读[访问控制概述](../permissions/overview.md)。

### 配置权限 {#configure-permissions}

现在您拥有管理员权限，可以为自己以及组织中的其他用户分配角色和权限。 在访问Real-Time CDP Collaboration或允许其他人使用它之前，需要执行此步骤。 有关详细说明，请参阅[如何配置权限](../setup/starter-permission-controls.md)。 有关Collaboration中可用的各种角色和权限的更多信息，请参阅[管理角色](../permissions/manage-roles.md)文档。

Once roles and permissions have been assigned, confirm that you can access Collaboration. Navigate to [Adobe Experience Cloud](https://experience.adobe.com/){target="_blank"}, and select **[!UICONTROL Real-Time CDP Collaboration]** within the **[!UICONTROL Quick access]** section. This opens the **[!UICONTROL Adobe Real-Time CDP Collaboration]** workspace, where you can begin using Collaboration features.

### Set up connections {#set-up-connections}

Next, follow steps in the following guides to set up connection and start collaborating with your partner:

* [Set up your Collaboration account](../setup/onboard-account.md)
* [Establish a connection with your inviting collaborator](../connect/overview.md)
* [Create a new project and begin collaborating with your partner](../collaborate/overview.md)

### Understand credit usage {#understand-credit-usage}

All Collaboration [!DNL Starter] activities use credits. However, as an invited user, you do not need to purchase or manage these credits. The collaborator who invited you covers all credit usage associated with your activities. To learn more, see the [credit usage and consumption in Collaboration [!DNL Starter]](../setup/starter-credit-usage.md) documentation.

## 后续步骤 {#next-steps}

You&#39;ve now completed initial setup and configured your organization for secure collaboration. Next, explore the following resources to learn about audience sourcing and different project use cases  within Collaboration:

* [Source和管理受众](../setup/onboard-audiences.md)
* [Project use cases](../collaborate/overview.md#project-use-cases):
   * [Discover overlaps and compare audiences](../collaborate/discover.md)
   * [激活受众](../collaborate/activate.md)
   * [Measure campaign performance](../collaborate/measure.md)
