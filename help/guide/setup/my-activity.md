---
title: 跟踪您的信用消耗活动
description: 了解如何在Real-Time CDP Collaboration中跟踪贵组织的信用消耗活动。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: b24d63e7-60f4-4cdb-ab1b-77c284543486
source-git-commit: b253588d8960757ed2023031bc95a7e3e0a0f65b
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 0%

---

# 跟踪您的信用消耗活动

{{limited-availability-release-note}}

>[!BEGINSHADEBOX]

**90天无超额期限**：符合条件的地区的客户将从其地区的可用性日期起享有90天无超额期限。 在此期间，客户不会因超出其信贷额度而产生超额费用。

>[!ENDSHADEBOX]

>[!IMPORTANT]
>
>信用消耗量表会按天进行舍入和汇总，以便进行监控。 **[!UICONTROL 我的活动]**&#x200B;仪表板中的数字表示预计的&#x200B;*信用消耗*。 用于计费的&#x200B;*实际*&#x200B;信用消耗在内部系统中进行跟踪，可应请求供您使用。 请联系您的Adobe代表以获取该信息。

要访问您的预计信用消耗活动，请在主导航中导航到&#x200B;**[!UICONTROL 设置]**，然后选择&#x200B;**[!UICONTROL 我的活动]**&#x200B;选项卡。

![我的活动信息板显示信用消耗详细信息](/help/assets/setup/my-activity-credits/activity-dashboard.png)

>[!TIP]
>
>**[!UICONTROL 我的活动]**&#x200B;视图不包括有关Real-Time Collaboration CDP用户界面不同部分中的用户操作的信息。 使用[审核日志](/help/guide/setup/audit-logs.md)功能获取该信息。

## 了解您的活动信息板 {#understand-dashboard}

活动仪表板显示贵组织内所有信贷消费操作的完整列表。 每一行表示一个不同的活动，并提供有关信用使用的关键信息：

>[!NOTE]
>
>**[!UICONTROL 受众管理]**&#x200B;活动未与另一个协作者关联，因此这些活动类型的&#x200B;**[!UICONTROL 连接ID]**&#x200B;和&#x200B;**[!UICONTROL 连接名称]**&#x200B;列指示了&#x200B;**[!UICONTROL N/A]**&#x200B;值。

| 列 | 描述 |
|------------|--------------|
| **[!UICONTROL 日期]** | 活动发生的日期，以YYYY/MM/DD格式显示。 |
| **[!UICONTROL 连接ID]** | 与信贷消费活动关联的每个连接的唯一标识符，以字母数字字符串表示。 |
| **[!UICONTROL 连接名称]** | 与连接和信贷消费活动关联的协作者的名称。 |
| **[!UICONTROL 活动]** | 执行的活动类型，如&#x200B;**激活 — 共享**、**激活 — 出口**&#x200B;或&#x200B;**受众管理**。 |
| **[!UICONTROL 输入已处理]** | 为活动处理的输入总数（例如，ID或行）。 |
| **[!UICONTROL 已使用的积分总数]** | 活动消耗的积分总数。 |
| **[!UICONTROL 我的信用共享]** | 贵组织用于活动的积分部分。 |

{style="table-layout:auto"}

## 活动类型 {#types-of-activities}

**[!UICONTROL Activity]**&#x200B;列显示不同类型的信贷消耗操作。

* **[!UICONTROL 受众管理]**：当受众源于Real-Time CDP Collaboration时使用了积分。 积分的使用取决于在Real-Time CDP Collaboration内为所有受众编制索引的ID数量（以百万为单位）以及该索引的频率（每天、每三天或每周）。 若要了解详细信息，请阅读[导入和管理受众](/help/guide/setup/onboard-audiences.md)指南。
* **[!UICONTROL 激活 — 匹配]** — 积分是作为匹配并准备激活的ID数量的函数而使用的。 若要了解详细信息，请阅读[激活受众](/help/guide/collaborate/activate.md)指南。
* **[!UICONTROL 激活 — 出口]** — 积分的使用情况与发送到目标的ID数量有关。 此费用始终由接收受众的协作者支付。 若要了解详细信息，请阅读[激活受众](/help/guide/collaborate/activate.md)指南。
* **[!UICONTROL 受众测量]** — 在Real-Time CDP Collaboration中执行活动以生成营销活动效果报表和见解。 积分根据所有营销活动的营销活动报表中的行数以及报表的频率（每天、每三天或每周）来使用。

## 管理您的信用使用情况 {#manage-credit-consumption}

要有效地管理您的信用消费，请执行以下操作：

1. **了解**&#x200B;与每个活动关联的点数消耗。 检查[Real-Time CDP Collaboration产品描述](https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html){target=_blank}以了解每个活动使用的协作积分表。
2. **定期监控**：请经常查看您的活动仪表板以了解使用模式。
3. **按连接跟踪**：使用连接名称识别哪些伙伴关系占用最多积分。

<!--

## Pagination and navigation

The activity list is paginated to improve performance and readability. Use the navigation controls at the bottom of the table to move between pages and adjust how many records you can view at once.

-->
