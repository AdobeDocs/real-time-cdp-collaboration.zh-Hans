---
title: 跟踪您的额度使用情况
description: 了解如何在Real-Time CDP Collaboration中查看贵组织的信用电子钱包和跟踪信用消耗活动。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: b24d63e7-60f4-4cdb-ab1b-77c284543486
TQID: https://experienceleague.adobe.com/hDvkKFUCBYvsX8wntcYFrL6qZTxOo5CZOWAbxNwk7mw
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 681f4af47a58a2ce66b25b09d793d0b5b127df39
workflow-type: tm+mt
source-wordcount: 726
ht-degree: 4%

---

# 跟踪您的额度使用情况 {#track-credit-consumption-activity}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_my_activity"
>title="了解更多信息"
>abstract=""

{{limited-availability-release-note}}

>[!BEGINSHADEBOX]

**90天无超额期限**：符合条件的地区的客户将从其地区的可用性日期起享有90天无超额期限。 在此期间，客户不会因超出其信贷额度而产生超额费用。

>[!ENDSHADEBOX]

要访问您的信用电子钱包和信用消耗活动，请在主导航中导航到&#x200B;**[!UICONTROL 设置]**，然后选择&#x200B;**[!UICONTROL 我的活动]**&#x200B;选项卡。

![显示“信用钱包”的“我的活动”选项卡，其中包含已设置的信用额、已使用的信用额、可用的信用额以及信用额使用活动表。](/help/assets/setup/my-activity-credits/activity-dashboard.png)

>[!TIP]
>
>**[!UICONTROL 我的活动]**&#x200B;视图不包括来自Real-Time CDP Collaboration界面其他区域的用户操作。 使用[审核日志](/help/guide/setup/audit-logs.md)功能获取该信息。

## 了解“我的活动”视图 {#understand-dashboard}

使用&#x200B;**[!UICONTROL 我的活动]**&#x200B;视图监视信用使用情况，并审查使用信用额的活动。 该视图包括信用Wallet和活动表。

Credit Wallet显示您配置的信用额、已用信用额和可用信用额。

| 量度 | 描述 |
|---------|-------------|
| 已设置&#x200B;**[!UICONTROL 积分]** | 为您的帐户配置的积分数。 |
| 已使用&#x200B;**[!UICONTROL 积分]** | 截至最近每日刷新时，您的帐户使用的积分数。 |
| **[!UICONTROL 可用积分]** | 您的帐户可用的贷项数，从已设置的贷项减去已冲销的贷项进行计算。 |

{style="table-layout:auto"}

活动表按日期、活动类型、处理的输入和使用的贷项列出了每日贷项冲减记录：

>[!NOTE]
>
>**[!UICONTROL 受众管理]**&#x200B;活动未与另一个协作者关联，因此这些活动类型的&#x200B;**[!UICONTROL 连接ID]**&#x200B;和&#x200B;**[!UICONTROL 连接名称]**&#x200B;列显示一个&#x200B;**[!UICONTROL -]**&#x200B;值。

| 列 | 描述 |
|------------|--------------|
| **[!UICONTROL 日期]** | 活动发生的日期，以YYYY/MM/DD格式显示。 |
| **[!UICONTROL 连接ID]** | 与信贷消费活动关联的每个连接的唯一标识符，以字母数字字符串表示。 |
| **[!UICONTROL 连接名称]** | 与连接和信贷消费活动关联的协作者的名称。 |
| **[!UICONTROL 活动]** | 执行的活动类型，如&#x200B;**[!UICONTROL 激活 — Audience Access （一次）]**、**[!UICONTROL 激活 — Audience Access （定期）]**、**[!UICONTROL 激活 — Audience Egress （一次）]**、**[!UICONTROL 激活 — Audience Egress （定期）]**&#x200B;或&#x200B;**[!UICONTROL Audience Management]**。 |
| **[!UICONTROL 输入已处理]** | 为活动处理的输入总数（例如，ID或行）。 |
| **[!UICONTROL 已使用的积分总数]** | 活动消耗的总积分。 |
| **[!UICONTROL 我的信用共享]** | 您的帐户中用于活动的积分部分。 |

{style="table-layout:auto"}

## 活动类型 {#types-of-activities}

**[!UICONTROL Activity]**&#x200B;列显示不同类型的信贷消耗操作。

* **[!UICONTROL 受众管理]**：当受众源于Collaboration时使用了积分。 积分是根据Collaboration中所有受众编制索引的ID数量以及该索引的频率来消耗的，例如每天、每三天或每周。 要了解更多信息，请阅读[采购和管理受众](/help/guide/setup/onboard-audiences.md)指南。
* **[!UICONTROL 激活 — Audience Access （一次）]**：通过激活工作流处理一次受众访问时，使用积分。 若要了解详细信息，请阅读[激活受众](/help/guide/collaborate/activate.md)指南。
* **[!UICONTROL 激活 — 受众访问（循环）]**：通过激活工作流按循环计划处理受众访问时，将消耗积分。 若要了解详细信息，请阅读[激活受众](/help/guide/collaborate/activate.md)指南。
* **[!UICONTROL 激活 — 受众出口（一次）]**：当通过激活工作流处理一次受众出口到目标时，将消耗积分。 此活动费用由接收受众的协作者支付。 若要了解详细信息，请阅读[激活受众](/help/guide/collaborate/activate.md)指南。
* **[!UICONTROL 激活 — 受众出口（循环）]**：通过激活工作流按循环计划处理受众出口到目标时，将消耗积分。 此活动费用由接收受众的协作者支付。 若要了解详细信息，请阅读[激活受众](/help/guide/collaborate/activate.md)指南。
* **[!UICONTROL 测量]**：在Collaboration中生成营销活动效果报表和分析时使用积分。 积分根据所有营销活动的营销活动报表中的行数以及报表的频率来使用，例如每天、每三天或每周。

## 管理您的信用使用情况 {#manage-credit-consumption}

要有效地管理您的信用消费，请执行以下操作：

1. **了解**&#x200B;与每个活动关联的信用消耗量。 检查[Collaboration产品描述](https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html){target=_blank}以了解每个活动使用的积分表。
2. **定期监视使用情况**：查看可用信用和活动表，以了解受众管理、受众访问、受众出口和测量活动中的使用模式。
3. **按连接跟踪**：使用连接名称识别哪些连接占用最多积分。
