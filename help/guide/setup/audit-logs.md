---
title: 审核日志
description: 了解如何使用Real-Time CDP Collaboration中的审核日志功能来跟踪用户活动和更改。
audience: admin
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/cn/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 3af1ac47-dc3d-4f19-a6b9-9e4e835977c0
source-git-commit: eed99cfafd5ffad5a468741f7258c162454769b7
workflow-type: tm+mt
source-wordcount: '888'
ht-degree: 1%

---

# 审核日志

{{limited-availability-release-note}}

为了提高系统中所执行活动的透明度和可见性，您可以在Adobe Experience Platform中以审核日志的形式审核各种服务和功能的用户活动。 这些日志形成审核跟踪，可以帮助对Adobe Real-Time CDP Collaboration中的问题进行故障诊断，并帮助您的企业有效地遵守公司数据管理政策和法规要求。

从基本意义上说，审核日志可告知&#x200B;*谁*&#x200B;执行了&#x200B;*什么*&#x200B;操作，以及&#x200B;*何时*。 日志中记录的每个操作都包含元数据，这些元数据指示操作类型、日期和时间、执行操作的用户的电子邮件ID以及与操作类型相关的其他属性。

使用Collaboration中的审核日志功能来跟踪平台中的用户活动和更改。 此功能与Experience Platform审核服务集成，并且此功能的UI驻留在Experience Platform中。

![审核日志功能的高级概览屏幕。](/help/assets/setup/audit-logs/audit-logs-overview.png)

有关审核日志的更全面信息，请访问[Experience Platform审核日志文档](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview){target="_blank"}。

## 访问审核日志

您可以通过两种方式访问审核日志，如下节所述。 这两个选项都会显示一个审核日志列表，其中捕获了在Collaboration内执行的各种活动。

### 从Collaboration用户界面访问审核日志

1. 导航到Collaboration中&#x200B;**[!UICONTROL 设置]**&#x200B;工作区的&#x200B;**[!UICONTROL 我的活动]**&#x200B;选项卡。
2. 在页面顶部的文本中选择Experience Platform链接。

![从Collaboration的“我的活动”选项卡访问审核日志。](/help/assets/setup/audit-logs/access-from-collaboration-ui.png)

### 直接在Experience Platform用户界面中访问审核日志

1. 导航到[Experience Platform](https://platform.adobe.com/)，然后从左侧菜单中选择&#x200B;**[!UICONTROL 审核]**&#x200B;部分。 如果您无法查看审核日志，请联系贵组织的系统管理员以获取必要权限。

![从Experience Platform访问审核日志。](/help/assets/setup/audit-logs/access-from-experience-platform-ui.png)

## 查看和使用审核日志

要查看审核日志，请执行以下操作：

1. 导航到Experience Platform中的&#x200B;**[!UICONTROL 审核]**&#x200B;部分。
2. 使用[筛选器](#filter-audit-logs)根据您的条件缩小日志范围。
3. 选择一个日志条目以查看详细信息，包括时间戳、请求ID、资源详细信息和操作状态。

![详细的审核日志](/help/assets/setup/audit-logs/filters-and-detailed-view.png)

### 捕获的活动

审核日志可捕获有关用户活动的详细信息，包括：

* **时间戳**：以月/日/年/小时:minute上午/下午格式执行的操作的确切日期和时间。
* **资源名称**：对其执行操作的资源的名称。
* **类别**：执行操作的资源类型。
* **操作**：执行的特定操作，如创建或删除。
* **用户**：执行操作的用户的电子邮件地址。

这些日志可全面跟踪Collaboration实例中的所有活动，这对数据治理和法规遵从性非常有用。 阅读有关[在UI](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview#managing-audit-logs-in-the-ui)中管理审核日志的更多信息。

### 筛选审核日志 {#filter-audit-logs}

审核日志UI提供了多个过滤器来帮助您搜索特定日志：

* **类别**：对其执行操作的资源类型，如Collaboration实例或Collaboration连接邀请。
* **操作**：执行的操作类型。 可用操作取决于所选类别。 例如，Collaboration实例的操作包括创建、更新和删除。
* **请求ID**：请求的唯一标识符。
* **用户**：执行操作的用户的电子邮件地址。
* **状态**：操作的状态，如允许或拒绝。
* **日期范围**：要查看其日志的日期范围。

阅读有关[筛选审核日志](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview#filter-audit-logs)的详细信息。

## 优点

审核日志为使用Collaboration的组织提供了以下几个好处：

* **数据管理**：使用审核日志，确保平台内的所有活动都受到跟踪且可审核。
* **法规遵从性**：此功能提供了用户活动跟踪以满足法规要求。
* **疑难解答**：审核日志通过提供用户操作的详细日志，帮助识别和解决问题。

## 类别和操作参考

下表提供了Real-Time CDP Collaboration所有类别和操作的参考。

![Real-Time CDP Collaboration审核日志中突出显示的可用类别。](/help/assets/setup/audit-logs/available-categories.png)

| 类别 | 操作 | 描述 |
|-------------------------------|------------------------------------------|-------------|
| **[!UICONTROL Collaboration实例]** | 创建、更新、删除 | 管理帐户，包括创建、更新和删除帐户。 要了解更多信息，请阅读[配置您的帐户](/help/guide/setup/onboard-account.md)指南。 |
| **[!UICONTROL Collaboration连接邀请]** | 创建、更新、删除、批准、拒绝 | 管理连接邀请，包括创建、更新、删除、批准和拒绝邀请。 有关详细信息，请参阅[建立连接](/help/guide/connect/establishing-connections.md)指南。 |
| **[!UICONTROL Collaboration连接]** | 创建、更新、删除、批准、拒绝、请求审批 | 管理连接，包括创建、更新、删除、批准、拒绝和请求审批连接。 |
| **[!UICONTROL Collaboration数据连接]** | 创建、更新、删除 | 管理从中获取和管理受众的数据连接，包括创建、更新和删除数据连接。 有关详细信息，请阅读[管理数据连接](/help/guide/setup/manage-data-connection.md)指南。 |
| **[!UICONTROL Collaboration数据实体]** | 创建、更新、删除 | 管理Collaboration的数据实体，包括创建、更新和删除数据实体。 此上下文中的数据实体是指受众。 有关详细信息，请参阅[采购和管理受众](/help/guide/setup/onboard-audiences.md)指南。 |
| **[!UICONTROL Collaboration项目]** | 创建、更新、删除 | 在Collaboration中管理项目，包括创建、更新和删除项目。 有关详细信息，请阅读[管理项目](/help/guide/collaborate/manage-projects.md)指南。 |
| **[!UICONTROL Collaboration模块]** | 创建、更新、删除 | 管理项目中的不同模块，包括在UI中创建、更新和删除各种模块。 例如，能够[激活受众](/help/guide/collaborate/activate.md)。 |

{style="table-layout:auto"}

利用审核日志功能，您可以对Collaboration中的所有活动进行清晰而详细的记录，从而确保透明度和可问责性。
