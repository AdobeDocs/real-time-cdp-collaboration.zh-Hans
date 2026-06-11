---
title: RTCDP Collaboration入门概述
description: 了解Adobe Real-Time CDP Collaboration Starter如何帮助您与许可合作伙伴扩展和增强以隐私为中心的协作，而无需您自己的完整Real-Time CDP许可证。
audience: publisher, advertiser, invited users to Real-Time CDP Collaboration Starter
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/cn/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 7ae0bd3d-eee9-48c0-9f18-a56033fee52d
source-git-commit: d0d854f73fa835984e5cff5207ce3e01297c8deb
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 4%

---

# Adobe Real-Time CDP Collaboration [!DNL Starter]概述

使用Adobe Real-Time CDP Collaboration [!DNL Starter]与许可合作伙伴协作，实施以隐私为中心的数据项目。 您无需自己的Collaboration许可证即可参与。

您的许可合作伙伴邀请您加入Collaboration，并使用他们的信用在广告商到出版商和品牌到品牌模式中为您联合的工作流提供资金。 要了解有关这些模式及其工作方式的更多信息，请阅读[协作模式](./collaboration-patterns.md)和[端到端工作流程](./end-to-end-workflow.md)指南。

作为受邀的[!DNL Starter]用户，您可以：

* 在[!DNL Starter]帐户中载入和管理协作数据。
* Source和维护用于联合项目的受众。
* 深入了解与您的合作伙伴之间的受众重叠，从而支持有效的定位和促销活动测量。
* 激活受众并将其共享给您的合作伙伴，以便联合激活和参与营销活动。

## 先决条件 {#prerequisites}

要开始使用Collaboration [!DNL Starter]，请确保您的组织和许可合作伙伴都位于同一地区。 您必须受到拥有Real-Time CDP Prime、Ultimate或Collaboration许可证的合作伙伴的邀请。

要启动邀请，请向您的许可合作伙伴提供以下信息：

* 联系人姓名
* 联系电子邮件
* 公司
* 角色（广告商/发布商）：广告商
* 行业

收到并接受邀请后，贵组织必须通过Adobe查看和签署免费销售订单才能访问Collaboration [!DNL Starter]。 有关邀请流程的更多详细信息，请参阅[邀请协作者加入Collaboration [!DNL Starter]](../connect/establishing-connections.md#invite-non-licensed-collaborator)指南。

## 护栏 {#guardrails}

请阅读下表，了解适用于您的[!DNL Starter]帐户的关键护栏。 其中包括对受众源、数据量、刷新频率、受众重叠和激活功能的限制。

| 护栏 | 描述 |
|----------| ------------|
| 受众来源 | 您可以将&#x200B;**[!DNL Amazon S3]**&#x200B;作为源，将受众数据引入Collaboration。 有关分步说明，请参阅[如何为受众源配置 [!DNL Amazon S3] &#x200B;](../setup/configure-aws-s3-audience-sourcing.md)。 |
| 受众 | 您的[!DNL Starter]帐户有权使用的最大值为：<ul><li>来自[!DNL AWS S3]存储段的10个受众</li><li>总身份数5,000万（由受众数据中的行数计算）</li><li>每个受众每6天刷新1次</li></ul> |
| 受众重叠和见解 | 您的受众可以运行受众重叠和分析的频率没有使用限制。 了解如何[发现重叠和比较受众](../collaborate/discover.md)。 |
| 激活 | 作为[!DNL Starter]用户，您只能激活受众并与邀请您的合作伙伴共享受众。 目标到外部平台的配置不可用。 了解有关[激活受众的详细信息](../collaborate/activate.md)。 |

{style="table-layout:auto"}

## 快速入门 {#getting-started}

在您[接受邀请并同意条款](../connect/establishing-connections.md#accept-invitation-sign-terms)后，请使用您的凭据登录[Adobe Experience Cloud](https://experience.adobe.com/){target="_blank"}。 在使用Collaboration之前，必须向您的帐户授予适当的访问权限和角色。

使用此工作流设置您的[!DNL Starter]帐户并开始与合作伙伴协作。

### 设置管理员访问权限 {#setup-admin-access}

首先，使用&#x200B;**管理员访问权限**&#x200B;工作区授予您自己必要的访问权限。 这可以确保您同时具有Experience Platform产品的管理权限和用户访问权限。 有关如何设置初始访问的详细步骤，请参阅[管理员访问说明](../setup/starter-admin-access.md)。

完成后，您应会在[Adobe Experience Cloud](https://experience.adobe.com/){target="_blank"}主页上的&#x200B;**[!UICONTROL 快速访问]**&#x200B;部分中看到&#x200B;**[!UICONTROL 权限]**、**[!UICONTROL Experience Platform]**&#x200B;和&#x200B;**[!UICONTROL Real-Time CDP Collaboration]**。

![在产品管理员访问设置后，Adobe Experience Cloud工作区显示权限、Experience Platform和Real-Time CDP Collaboration。](/help/assets/overview/starter/setup-admin-access.png){zoomable="yes"}

有关访问角色和不同Adobe Experience Cloud产品的更多详细信息，请阅读[访问控制概述](../permissions/overview.md)。

### 配置权限 {#configure-permissions}

现在您拥有管理员权限，可以为自己以及组织中的其他用户分配角色和权限。 在访问Real-Time CDP Collaboration或允许其他人使用它之前，需要执行此步骤。 有关详细说明，请参阅[如何配置权限](../setup/starter-permission-controls.md)。 有关Collaboration中可用的各种角色和权限的更多信息，请参阅[管理角色](../permissions/manage-roles.md)文档。

分配角色和权限后，请确认您可以访问Collaboration。 导航到[Adobe Experience Cloud](https://experience.adobe.com/){target="_blank"}，然后在&#x200B;**[!UICONTROL 快速访问]**&#x200B;部分中选择&#x200B;**[!UICONTROL Real-Time CDP Collaboration]**。 这将打开&#x200B;**[!UICONTROL Adobe Real-Time CDP Collaboration]**&#x200B;工作区，您可以在其中开始使用Collaboration功能。

### 设置连接 {#set-up-connections}

接下来，请按照以下指南中的步骤来设置连接，并开始与合作伙伴协作：

* [设置您的Collaboration帐户](../setup/onboard-account.md)
* [建立与邀请协作者之间的连接](../connect/overview.md)
* [创建新项目并开始与合作伙伴协作](../collaborate/overview.md)

### 了解信用使用情况 {#understand-credit-usage}

所有Collaboration [!DNL Starter]活动都使用积分。 但是，作为受邀用户，您无需购买或管理这些积分。 邀请您的协作者涵盖与您的活动关联的所有信用使用情况。 若要了解更多信息，请参阅Collaboration [!DNL Starter][&#128279;](../setup/starter-credit-usage.md)文档中的信用使用情况和使用情况。

## 后续步骤 {#next-steps}

您现在已完成初始设置并配置您的组织以进行安全协作。 接下来，探索以下资源，了解受众源以及Collaboration中的各种项目用例：

* [Source和管理受众](../setup/onboard-audiences.md)
* [项目用例](../collaborate/overview.md#project-use-cases)：
   * [发现重叠并比较受众](../collaborate/discover.md)
   * [激活受众](../collaborate/activate.md)
   * [衡量促销活动效果](../collaborate/measure.md)
