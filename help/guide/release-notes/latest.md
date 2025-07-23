---
title: 最新Real-Time CDP Collaboration发行说明
description: 遵循Real-Time CDP Collaboration的最新版本
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/cn/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 8513c648-1cc1-4544-b86d-2ee3193ab60f
source-git-commit: eed99cfafd5ffad5a468741f7258c162454769b7
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 2%

---

# 最新Real-Time CDP Collaboration发行说明

{{limited-availability-release-note}}

**上次更新**：2025年5月。

以下发行说明介绍了Adobe Real-Time CDP Collaboration中发布的功能。 Collaboration版本在持续交付模型上运行，该模型允许大约每月一次的发布。 这些发行说明会经常更新，因此请务必定期检查。

## 2025 年 5 月 {#may-2025}

* Real-Time CDP Collaboration现在可供&#x200B;**澳大利亚**&#x200B;和&#x200B;**新西兰**&#x200B;的客户使用。 它自动提供给这些地区的Real-Time CDP Prime和Ultimate客户。
* Real-Time CDP Collaboration现在通过[设置](../setup/manage-destinations.md)部分中的&#x200B;**[!UICONTROL 我的目标]**&#x200B;选项卡提供&#x200B;**[!UICONTROL 自助目标]**。 目标允许您在第三方平台（如广告网络或数据管理平台）中激活受众，以通过各种渠道触及您的客户。 目前，仅支持Adobe Experience Platform目标。 如果您有兴趣配置其他目标，请联系您的Adobe代表。 若要了解有关目标的更多信息，请阅读[目标概述](../destinations/overview.md)指南。
   * 目标还添加了对在[Collaboration受众门户](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/segmentation/ui/audience-portal.md#manage-audiences)中查看Adobe Experience Platform受众的支持。
* 您现在可以在Collaboration中编辑现有数据连接的受众刷新频率。 目前，您可以选择每天或每两到六天刷新一次受众。 要了解有关如何编辑受众刷新频率的更多信息，请阅读[管理数据连接](../setup/manage-data-connection.md#scheduling)指南。
* 现在，系统会为连接内选择的每个用例设置协作者之间的信用拆分。 您可以为每个用例设置不同的信用冲减规则，以更好地控制信用额的使用方式。 要了解有关信用拆分功能的更多信息，请阅读[连接设置](../connect/establishing-connections.md#connection-settings)指南。 若要了解有关如何使用积分的更多信息，请阅读[积分活动类型](../setup/my-activity.md#types-of-activities)指南。<br> ![显示信用拆分功能的连接设置屏幕。](/help/assets/release-notes/2025/credit-split.png){zoomable="yes"}
* 发布者现在可以在接受来自广告商的连接设置之前设置广告商名称和ID。 发布者可以设置与其内部系统一致的名称和ID，这可能与广告商的名称和ID不同。 要了解有关添加广告商名称和ID的详细信息，请阅读[连接设置](../connect/establishing-connections.md#connection-settings.md)指南。<br> ![连接设置屏幕，显示发布者设置广告商名称和ID。](/help/assets/release-notes/2025/add-advertiser-names-modal.png){zoomable="yes"}

## 2025 年 4 月 {#april-2025}

* 新的&#x200B;**[!UICONTROL 已处理的输入数]**&#x200B;列已添加到信用消耗活动表中。 此列显示为每个活动处理的输入总数（例如，ID或行）。 [阅读更多](/help/guide/setup/my-activity.md#inputs-processed)。<br> ![输入我的活动视图中突出显示的已处理列。](/help/assets/release-notes/2025/inputs-processed-column.png){zoomable="yes"}
* 在帐户创建中添加了新的联系人电子邮件选项。 这有助于合作伙伴协作者在连接过程中根据需要与您联系。 [了解详情](../setup/onboard-account.md)。

## 2025 年 3 月 {#march-2025}

* 现在，当[将受众](/help/guide/setup/onboard-audiences.md)收集到Collaboration中时，您可以将受众刷新频率设置为每&#x200B;**天到每六天**，以便更好地管理[受众管理点数活动](/help/guide/setup/my-activity.md#types-of-activities)。 有关详细信息，请阅读[管理受众](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/segmentation/ui/audience-portal.md#manage-audiences)指南。<br> ![计划屏幕，其中显示更新受众成员资格的不同频率间隔。](/help/assets/setup/add-manage-audiences/audience-scheduling-frequency.png "计划屏幕，其中显示更新受众成员资格的不同频率间隔。"){width="250" align="center" zoomable="yes"}
* 与协作者建立连接时，您现在可以从预定义的&#x200B;**用例**&#x200B;中进行选择。 所选用例确定哪些项目部分和产品功能可用。 有关详细信息，请阅读[管理项目](/help/guide/collaborate/manage-projects.md#project-use-cases)指南。
   * *度量*&#x200B;启用&#x200B;**度量**&#x200B;项目节。
   * *受众发现*&#x200B;启用&#x200B;**发现**&#x200B;项目部分。
   * *受众激活*&#x200B;启用&#x200B;**激活**&#x200B;项目部分<br>
* 现在，您可以删除与不希望再使用的协作者建立的连接。 要了解如何删除连接，请阅读[删除连接](/help/guide/connect/establishing-connections.md#delete-connections)指南。

## 2025 年 2 月 {#february-2025}

Adobe Real-Time CDP Collaboration目前在美国正式推出，其专门构建旨在使广告商和出版商能够发现、激活和测量没有第三方Cookie的高价值受众。

### 快速入门

1. **访问安装程序**：系统管理员为用户配置访问权限。 要了解有关配置访问权限的更多信息，请阅读[管理用户访问权限](/help/guide/permissions/manage-user-access.md#RTCDP-collaboration-access)指南。
2. **连接数据源**：要在Collaboration中使用的Source受众。 要开始采购受众，请阅读[来源和管理受众](/help/guide/setup/onboard-audiences.md)指南。
3. **建立连接**：开始与受信任的广告商或发布者协作。 若要了解有关建立连接的更多信息，请阅读[建立连接](/help/guide/connect/establishing-connections.md)指南。
4. **发现并激活**：创建项目以识别要在营销活动中激活的有价值受众。 要了解有关创建项目的更多信息，请阅读[管理项目](/help/guide/collaborate/manage-projects.md)指南。

### 可用性

* Adobe Real-Time CDP Collaboration目前仅向美国客户提供。
* Adobe Real-Time CDP Prime和Ultimate客户可自动使用此功能

有关详细信息，请阅读：

* [Collaboration概述](/help/guide/home.md)
* [端到端工作流](/help/guide/end-to-end-workflow.md)
* [权限概述](/help/guide/permissions/overview.md)
