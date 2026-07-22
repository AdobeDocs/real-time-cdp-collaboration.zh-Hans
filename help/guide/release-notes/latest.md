---
title: 最新Real-Time CDP Collaboration发行说明
description: 遵循Real-Time CDP Collaboration的最新版本
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 8513c648-1cc1-4544-b86d-2ee3193ab60f
TQID: https://experienceleague.adobe.com/re4oFblCLiZpspWIS7D4EEYNh36EDhULEOd2-ccXH28
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
feature_v2:
  - id: ba929a52-9339-4154-9487-317dc875a3c7
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
source-git-commit: e6156a39107edb0e15e2115db0762f6a86801ed6
workflow-type: tm+mt
source-wordcount: 1968
ht-degree: 4%

---

# 最新Real-Time CDP Collaboration发行说明

{{limited-availability-release-note}}

**上次更新时间**：2026年7月。

以下发行说明介绍了Adobe Real-Time CDP Collaboration中发布的功能。 Collaboration版本在持续交付模型上运行，该模型允许大约每月一次的发布。 这些发行说明会经常更新，因此请务必定期检查。

## 2026年7月 {#july-2026}

Real-Time CDP Collaboration现在支持其他自助受众源选项。

**新增功能或更新后的功能**

| 功能 | 描述 |
| ------- | ----------- |
| 来自[!DNL Databricks Delta Share]和Adobe Audience Manager的自助受众源 | 您现在可以直接从[!DNL Databricks Delta Share]获取第一方受众，或将符合条件的Adobe Audience Manager区段引入Collaboration。 有关设置说明，请参阅以下指南： <ul><li>[为受众源配置 [!DNL Databricks Delta Share] &#x200B;](../setup/configure-databricks-audience-sourcing.md)</li><li>[为受众源配置Adobe Audience Manager](../setup/configure-aam-audience-sourcing.md)</li></ul> |

{style="table-layout:auto"}

## 2026 年 4 月 {#april-2026}

Real-Time CDP Collaboration中现在提供了新功能。 其中包括用于邀请合作伙伴的Collaboration [!DNL Starter]、从[!DNL Snowflake]和[!DNL Google Cloud Storage]扩展的受众源、支持[!DNL Demdex ID (ECID)]作为匹配键，以及两个新的协作者角色：代理和数据合作伙伴。

**新增功能或更新后的功能**

| 功能 | 描述 |
| ------- | ----------- |
| Real-Time CDP Collaboration [!DNL Starter] | 您现在可以邀请没有Collaboration许可证的合作伙伴通过Collaboration [!DNL Starter]与您协作。 受邀合作伙伴可以在共享连接中获取受众、发现重叠并激活受众。 请参阅[Collaboration [!DNL Starter] 概述](../overview/starter-overview.md)以开始操作。 |
| 来自[!DNL Snowflake]和[!DNL Google Cloud Storage]的自助受众源 | 您现在可以直接从[!DNL Snowflake Secure Data Share]或[!DNL Google Cloud Storage]存储段向Collaboration中获取第一方受众。 有关设置说明，请参阅以下指南： <ul><li>[为受众源配置 [!DNL Snowflake] &#x200B;](../setup/configure-snowflake-audience-sourcing.md) </li><li> [为受众源配置 [!DNL Google Cloud Storage] &#x200B;](../setup/configure-gcs-audience-sourcing.md) </li></ul> |
| [!DNL Demdex ID]匹配键 | 现在支持[!DNL Demdex ID] (ECID)作为匹配键，以跨平台匹配基于Cookie的匿名身份。 它提高了受众重叠的准确性，而无需依赖经过身份验证的用户数据。 有关详细信息，请参阅[支持的匹配键](../setup/onboard-account.md#supported-match-keys)。 |
| 新协作者角色 | Collaboration现在支持另外两个协作者角色，包括&#x200B;**代理**&#x200B;和&#x200B;**数据合作伙伴**。 这些角色将扩展不同组织在该平台中参与和协同工作的方式。 详细了解： <ul><li>[协作者帐户角色](../overview/roles.md)</li><li>[Collaboration模式](../overview/collaboration-patterns.md)</li><li>[端到端工作流](../overview/end-to-end-workflow.md)</li></ul> |

{style="table-layout:auto"}

## 2026年3月 {#march-2026}

您现在可以在Real-Time CDP Collaboration中生成营销活动测量报告并管理测量数据。

**新增功能或更新后的功能**

| 功能 | 描述 |
| ------- | ----------- |
| 测量正式发布 | 测量报表现在通常在Collaboration中可用。 现在，您可以输入与营销活动关联的促销活动ID作为发布者，输入源转化数据作为广告商，并生成两种类型的报表：针对整体促销活动结果的&#x200B;**促销活动摘要**&#x200B;以及针对促销活动效果分析的&#x200B;**归因**。 要开始操作，请参阅以下指南： <ul><li>[输入营销活动ID](../collaborate/manage-projects.md#manage-campaign-id)</li><li>[Source转化数据](../setup/onboard-measurement-data.md)</li><li>[创建和查看测量报告](../collaborate/measure.md)</li></ul> |
| 测量生命周期管理 | Collaboration还支持测量管理：<ul><li> 广告商现在可以编辑或删除测量数据连接和关联的转化事件，以确保准确且最新的促销活动分析。 有关更多详细信息，请参阅[管理测量数据连接](../setup/manage-measurement-data-connection.md)和[管理转换事件](../setup/onboard-measurement-data.md#edit-measurement-data)。</li><li>您还可以直接从任何协作项目中的&#x200B;**[!UICONTROL 度量]**&#x200B;选项卡编辑或删除计划的度量报表。 这适用于所有用户。 有关详细信息，请参阅[管理测量报告指南](../collaborate/measure.md)。</li></ul> |

{style="table-layout:auto"}

## 2026 年 2 月 {#february-2026}

Real-Time CDP Collaboration现在支持直接在界面中编辑现有连接和数据连接设置。

**新增或更新功能**

| 功能 | 描述 |
| ------- | ----------- |
| 编辑连接设置 | 建立连接后，连接所有者现在可以更新用例、匹配键、激活权限和点数拆分。 有关分步说明，请参阅[编辑连接](../connect/manage-connections.md#edit-connection)。 |
| 编辑数据连接 | 直接在Collaboration中更新现有数据连接的匹配键和计划配置。 有关分步说明，请参阅[编辑数据连接](../setup/manage-data-connection.md#edit-data-connection)。 |

## 2026 年 1 月 {#january-2026}

Real-Time CDP Collaboration现在支持CSV文件上传作为获取受众的新方法，以及新的移动匹配键（IDFA和GAID）用于增强受众匹配和测量。

**新增功能或更新后的功能**

| 功能 | 描述 |
| ------- | ----------- |
| 为受众源上传CSV | 直接从UI将CSV文件上传到源受众中的Collaboration。 非常适合于为短期协作项目载入第一方数据。 有关详细信息，请参阅受众源指南[&#128279;](../setup/upload-csv-audience-sourcing.md)的上传CSV文件。 |
| 移动设备匹配密钥支持 | Collaboration现在支持移动匹配键（包括IDFA和GAID），以进行受众匹配和测量。 这些匹配键是在帐户设置期间选择的，然后可以在为新连接配置连接设置时以及下游协作工作流中使用。 有关详细信息，请参阅[匹配键设置指南](../setup/onboard-account.md#set-up-match-keys)。 |

{style="table-layout:auto"}

## 2025 年 12 月 {#december-2025}

Real-Time CDP Collaboration现在可供&#x200B;**欧洲、中东和非洲(EMEA)**&#x200B;的客户使用。 它自动提供给这些地区的Real-Time CDP Prime和Ultimate客户。

## 2025 年 8 月 {#august-2025}

Real-Time CDP Collaboration现在可供&#x200B;**加拿大**&#x200B;的客户使用。 它自动提供给这些地区的Real-Time CDP Prime和Ultimate客户。

* Collaboration现在支持以下[个匹配的键](../setup/onboard-account.md#supported-match-keys)：
  * 哈希电子邮件
  * 散列电话号码
  * CRM ID
  * 忠诚度 ID
  * 哈希 IPv4
  * AdFixus ID
* 现在，Collaboration中提供了多个匹配键，使您能够扩展受众规模并提高匹配率。 在获取受众、建立连接和激活受众时，可以使用多个匹配键。 要了解有关使用多个匹配键的更多信息，请阅读[设置匹配键](../setup/onboard-account.md)和[来源受众](../setup/onboard-audiences.md#map-fields)指南。

>[!IMPORTANT]
>
>在激活使用了多个匹配键的受众时，如果一个（或多个）匹配键没有重叠、没有受众规模或低于阈值，则整个激活将失败。 在激活之前，请确保您的受众有足够的重叠，并满足所有匹配键中1000个ID的最低阈值。

* Adobe Experience Platform目标现在支持使用多个匹配键激活受众。 此外，您现在可以在配置目标的映射时使用链接密钥，以指定在激活期间发送匹配密钥。 若要了解详细信息，请阅读[Experience Platform目标](../destinations/experience-platform.md#linked-keys)指南。
* 协作者现在可以同时编辑多个受众。 您现在可以使用批量编辑工具编辑多个受众的受众元数据、连接访问权限、名称、描述和类别。 要了解有关编辑受众的更多信息，请阅读[管理受众](../setup/onboard-audiences.md#edit-audiences)指南。

## 2025 年 7 月 {#july-2025}

Real-time CDP Collaboration现在支持品牌到品牌协作。 协作者现在可以建立连接，无论他们是广告商还是发布者。 这提供了更灵活的协作机会，并使品牌能够利用彼此的数据和见解。 要了解有关品牌到品牌协作和广告商到发布商协作之间的差异的更多信息，请阅读[协作模式](../overview/collaboration-patterns.md)指南。

* 协作者现在可以使用[专用连接邀请](../connect/establishing-connections.md#private-connection-invites)相互连接。 与协作者共享您帐户的唯一连接代码，协作者随后可以使用该代码直接与您连接。 这是品牌到品牌协作的核心功能，它允许协作者在探索&#x200B;**[!UICONTROL 发现协作者目录]**&#x200B;的广告商之外建立连接。
* [自助服务目标](../setup/manage-destinations.md)现在可供广告商和出版商使用。
* 现在，Audience Activation可用于连接中的两个协作者，无论他们的[帐户角色](../overview/roles.md)如何。 在[建立连接](../connect/establishing-connections.md#configure-connection-settings)时配置受众激活设置，允许您指定哪个协作者可以激活受众。 要了解有关受众激活的更多信息，请阅读[激活受众](../collaborate/activate.md)指南。
* **[!UICONTROL 激活]**&#x200B;用例已重新配置为支持品牌到品牌协作。 项目中的&#x200B;**[!UICONTROL 激活]**&#x200B;选项卡现在显示已发送给协作者的受众，以及由协作者激活到目标的受众。 若要了解详细信息，请阅读[激活受众](../collaborate/activate.md)指南。<br> ![“激活”仪表板，其中的“受众”部分已发送至，而“受众”部分已激活。](/help/assets/release-notes/2025/activate-dashboard.png){zoomable="yes"}
* 受众索引分数现在可在项目的&#x200B;**[!UICONTROL 发现]**&#x200B;选项卡中获得。 受众索引得分用于衡量受众与协作者受众的匹配程度。 此得分根据基础受众规模和重叠情况计算。 若要了解有关受众索引分数的详细信息，请阅读[受众索引分数](../collaborate/discover.md#audience-index-score)指南。

## 2025 年 5 月 {#may-2025}

* Real-Time CDP Collaboration现在可供&#x200B;**澳大利亚**&#x200B;和&#x200B;**新西兰**&#x200B;的客户使用。 它自动提供给这些地区的Real-Time CDP Prime和Ultimate客户。
* Real-Time CDP Collaboration现在通过&#x200B;**[!UICONTROL 设置]**&#x200B;部分中的&#x200B;**[!UICONTROL 我的目标]**&#x200B;选项卡提供[自助目标](../setup/manage-destinations.md)。 目标允许您在第三方平台（如广告网络或数据管理平台）中激活受众，以通过各种渠道触及您的客户。 目前，仅支持Adobe Experience Platform目标。 如果您有兴趣配置其他目标，请联系您的Adobe代表。 若要了解有关目标的更多信息，请阅读[目标概述](../destinations/overview.md)指南。
  * 目标还添加了对在[Collaboration受众门户](https://experienceleague.adobe.com/en/docs/experience-platform/segmentation/ui/audience-portal.md#manage-audiences)中查看Adobe Experience Platform受众的支持。
* 您现在可以在Collaboration中编辑现有数据连接的受众刷新频率。 目前，您可以选择每天或每两到六天刷新一次受众。 要了解有关如何编辑受众刷新频率的更多信息，请阅读[管理数据连接](../setup/manage-data-connection.md#scheduling)指南。
* 现在，系统会为连接内选择的每个用例设置协作者之间的信用拆分。 您可以为每个用例设置不同的信用冲减规则，以更好地控制信用额的使用方式。 要了解有关信用拆分功能的更多信息，请阅读[连接设置](../connect/establishing-connections.md#connection-settings)指南。 若要了解有关如何使用积分的更多信息，请阅读[积分活动类型](../setup/my-activity.md#types-of-activities)指南。<br> ![显示信用拆分功能的连接设置屏幕。](/help/assets/release-notes/2025/credit-split.png){zoomable="yes"}
* 发布者现在可以在接受来自广告商的连接设置之前设置广告商名称和ID。 发布者可以设置与其内部系统一致的名称和ID，这可能与广告商的名称和ID不同。 要了解有关添加广告商名称和ID的详细信息，请阅读[连接设置](../connect/establishing-connections.md#connection-settings.md)指南。<br> ![连接设置屏幕，显示发布者设置广告商名称和ID。](/help/assets/release-notes/2025/add-advertiser-names-modal.png){zoomable="yes"}

## 2025 年 4 月 {#april-2025}

* 新的&#x200B;**[!UICONTROL 已处理的输入数]**&#x200B;列已添加到信用消耗活动表中。 此列显示为每个活动处理的输入总数（例如，ID或行）。 [阅读更多](/help/guide/setup/my-activity.md#inputs-processed)。<br> ![输入我的活动视图中突出显示的已处理列。](/help/assets/release-notes/2025/inputs-processed-column.png){zoomable="yes"}
* 在帐户创建中添加了新的联系人电子邮件选项。 这有助于合作伙伴协作者在连接过程中根据需要与您联系。 [了解详情](../setup/onboard-account.md)。

## 2025 年 3 月 {#march-2025}

* 现在，当[将受众](/help/guide/setup/onboard-audiences.md)收集到Collaboration中时，您可以将受众刷新频率设置为每&#x200B;**天到每六天**，以便更好地管理[受众管理点数活动](/help/guide/setup/my-activity.md#types-of-activities)。 有关详细信息，请阅读[管理受众](https://experienceleague.adobe.com/en/docs/experience-platform/segmentation/ui/audience-portal.md#manage-audiences)指南。<br> ![计划屏幕，其中显示更新受众成员资格的不同频率间隔。](/help/assets/setup/add-manage-audiences/audience-scheduling-frequency.png "计划屏幕，其中显示更新受众成员资格的不同频率间隔。"){width="250" align="center" zoomable="yes"}
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
* [端到端工作流](/help/guide/overview/end-to-end-workflow.md)
* [权限概述](/help/guide/permissions/overview.md)
