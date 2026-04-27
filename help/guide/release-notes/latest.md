---
title: Latest Real-Time CDP Collaboration Release Notes
description: Follow the latest releases for Real-Time CDP Collaboration
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/cn/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
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
source-git-commit: 3ce7e66b31332836fd6cc6137c94622436505cc9
workflow-type: tm+mt
source-wordcount: 1461
ht-degree: 3%

---

# Latest Real-Time CDP Collaboration Release Notes

{{limited-availability-release-note}}

**Last update**: January 2026.

These release notes cover the functionality released in Adobe Real-Time CDP Collaboration. Collaboration releases operate on a continuous delivery model, which allows for an approximate monthly release cadence. These release notes get updated often, so be sure to check them regularly.

## 2026 年 1 月 {#january-2026}

Real-Time CDP Collaboration now supports CSV file upload as a new method for sourcing audiences, as well as new mobile match keys (IDFA and GAID) for enhanced audience matching and measurement.

**新增功能或更新后的功能**

| 功能 | 描述 |
| ------- | ----------- |
| CSV upload for Audience Sourcing | Upload CSV files to source audiences into Collaboration directly from the UI. Ideal for onboarding first-party data for short-term collaboration projects. For more information, see the [upload CSV file for audience sourcing guide](../setup/upload-csv-audience-sourcing.md). |
| Mobile Match Key Support | Collaboration now supports mobile match keys, including IDFA and GAID, for audience matching and measurement. These match keys are selected during account setup and can then be used when configuring connection settings for new connections and in downstream collaboration workflows. See the [Match keys setup guide](../setup/onboard-account.md#set-up-match-keys) for more details. |

{style="table-layout:auto"}

## 2025 年 12 月 {#december-2025}

Real-Time CDP Collaboration is now available to customers in **Europe, the Middle East, and Africa (EMEA))**. It is automatically available to Real-Time CDP Prime and Ultimate customers in these regions.

## 2025 年 8 月 {#august-2025}

Real-Time CDP Collaboration is now available to customers in **Canada**. It is automatically available to Real-Time CDP Prime and Ultimate customers in these regions.

* Collaboration now supports the following [match keys](../setup/onboard-account.md#supported-match-keys):
   * 哈希电子邮件
   * Hashed phone number
   * CRM ID
   * 忠诚度 ID
   * 哈希 IPv4
   * AdFixus ID
* Multiple match keys are now available across Collaboration, giving you the ability to expand your audience size and improve match rates. Multiple match keys can be used when sourcing audiences, establishing connections, and activating audiences. To learn more about using multiple match keys, read the [set up match keys](../setup/onboard-account.md) and [sourcing audiences](../setup/onboard-audiences.md#map-fields) guides.

>[!IMPORTANT]
>
>在激活使用了多个匹配键的受众时，如果一个（或多个）匹配键没有重叠、没有受众规模或低于阈值，则整个激活将失败。 在激活之前，请确保您的受众有足够的重叠，并满足所有匹配键中1000个ID的最低阈值。

* The Adobe Experience Platform destination now supports activating audiences with multiple match keys. Additionally, you can now used a linked key when configuring your destination&#39;s mapping to specify which match key is sent during activation. To learn more, read the [Experience Platform destination](../destinations/experience-platform.md#linked-keys) guide.
* Collaborators can now edit multiple audiences at once. You can now edit audience metadata, connection access, names, descriptions, and categories for multiple audiences using the bulk edit tool. To learn more about editing audiences, read the [manage audiences](../setup/onboard-audiences.md#edit-audiences) guide.

## 2025 年 7 月 {#july-2025}

Real-time CDP Collaboration now supports brand-to-brand collaboration. Collaborators can now form connections, regardless of whether they are an advertiser or publisher. This allows for more flexible collaboration opportunities and enables brands to leverage each other&#39;s data and insights. To learn more about the differences between brand-to-brand collaboration and advertiser-to-publisher collaboration, read the [collaboration patterns](../overview/collaboration-patterns.md) guide.

* Collaborators can now connect to each other using [private connection invites](../connect/establishing-connections.md#private-connection-invites). Share your account&#39;s unique connect code with a collaborator who can then use it to connect with you directly. This is a core feature of brand-to-brand collaboration, allowing collaborators to establish connections beyond advertisers exploring the **[!UICONTROL Discover collaborators]** directory.
* [Self-serve destinations](../setup/manage-destinations.md) are now available to both advertisers and publishers.
* Audience activation is now available for both collaborators in a connection, regardless of their [account role](../overview/roles.md). Audience activation settings are configured while [establishing connections](../connect/establishing-connections.md#configure-connection-settings), allowing you to specify which collaborator can activate audiences. To learn more about audience activation, read the [activate audiences](../collaborate/activate.md) guide.
* The **[!UICONTROL Activate]** use case has been reconfigured to support brand-to-brand collaboration. The **[!UICONTROL Activate]** tab within a project now displays the audiences that have been sent to your collaborator, and the audiences activated to your destination by your collaborator. To learn more, read the [activate audiences](../collaborate/activate.md) guide. <br> ![The Activate dashboard with the Audiences sent to and Audiences activated sections.](/help/assets/release-notes/2025/activate-dashboard.png){zoomable="yes"}
* 受众索引分数现在可在项目的&#x200B;**[!UICONTROL 发现]**&#x200B;选项卡中获得。 受众索引得分用于衡量受众与协作者受众的匹配程度。 此得分根据基础受众规模和重叠情况计算。 若要了解有关受众索引分数的详细信息，请阅读[受众索引分数](../collaborate/discover.md#audience-index-score)指南。

## 2025 年 5 月 {#may-2025}

* Real-Time CDP Collaboration现在可供&#x200B;**澳大利亚**&#x200B;和&#x200B;**新西兰**&#x200B;的客户使用。 它自动提供给这些地区的Real-Time CDP Prime和Ultimate客户。
* Real-Time CDP Collaboration现在通过&#x200B;**[!UICONTROL 设置]**&#x200B;部分中的&#x200B;**[!UICONTROL 我的目标]**&#x200B;选项卡提供[自助目标](../setup/manage-destinations.md)。 目标允许您在第三方平台（如广告网络或数据管理平台）中激活受众，以通过各种渠道触及您的客户。 目前，仅支持Adobe Experience Platform目标。 如果您有兴趣配置其他目标，请联系您的Adobe代表。 若要了解有关目标的更多信息，请阅读[目标概述](../destinations/overview.md)指南。
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
4. **发现并激活**：创建项目以识别要在营销活动中激活的有价值受众。 To learn more about creating projects, read the [manage projects](/help/guide/collaborate/manage-projects.md) guide.

### 可用性

* Adobe Real-Time CDP Collaboration is currently available to US customers only.
* It is automatically available to Adobe Real-Time CDP Prime and Ultimate customers

For more information, read the:

* [Collaboration overview](/help/guide/home.md)
* [End-to-End workflow](/help/guide/overview/end-to-end-workflow.md)
* [Permissions overview](/help/guide/permissions/overview.md)
