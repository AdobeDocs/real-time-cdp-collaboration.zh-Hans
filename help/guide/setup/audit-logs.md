---
title: 审核日志
description: Learn how to use the Audit Logs functionality in Real-Time CDP Collaboration to track user activities and changes.
audience: admin
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 3af1ac47-dc3d-4f19-a6b9-9e4e835977c0
TQID: https://experienceleague.adobe.com/zb09-bUpxJ2VPDknETHeayMuLpNRCaQ2VTnV9QnTRgE
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 3ce7e66b31332836fd6cc6137c94622436505cc9
workflow-type: tm+mt
source-wordcount: 950
ht-degree: 2%

---

# 审核日志

{{limited-availability-release-note}}

In order to increase the transparency and visibility of activities performed in the system, you can audit user activity for various services and capabilities in the form of audit logs in Adobe Experience Platform. These logs form an audit trail that can help with troubleshooting issues in Adobe Real-Time CDP Collaboration, and help your business effectively comply with corporate data stewardship policies and regulatory requirements.

In a basic sense, an audit log tells *who* performed *what* action, and *when*. Each action recorded in a log contains metadata that indicates the action type, date and time, the email ID of the user who performed the action, and additional attributes relevant to the action type.

Use the audit logs functionality in Collaboration to track user activities and changes within the platform. This feature is integrated with the Experience Platform audit service, and the UI for this functionality resides in Experience Platform.

![High-level overview screen of the audit logs functionality.](/help/assets/setup/audit-logs/audit-logs-overview.png)

For more comprehensive information about audit logs, visit the [Experience Platform audit logs documentation](https://experienceleague.adobe.com/en/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview){target="_blank"}.

## Access audit logs

You can access audit logs in two ways, as described in the sections below. Both options display a list of audit logs capturing various activities performed within Collaboration.

### Access audit logs from the Collaboration user interface

1. Navigate to the **[!UICONTROL My Activity]** tab in **[!UICONTROL Setup]** workspace in Collaboration.
2. Select the Experience Platform link in the text at the top of the page.

![Access audit logs from the My activity tab in Collaboration.](/help/assets/setup/audit-logs/access-from-collaboration-ui.png)

### Access audit logs directly in the Experience Platform user interface

1. Navigate to [Experience Platform](https://platform.adobe.com/) and select the **[!UICONTROL Audits]** section from the left-hand menu. Reach out to your organization&#39;s system administrators to obtain the necessary permissions if you cannot view audit logs.

![Access audit logs from Experience Platform.](/help/assets/setup/audit-logs/access-from-experience-platform-ui.png)

## View and use audit logs

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

这些日志可全面跟踪Collaboration实例中的所有活动，这对数据治理和法规遵从性非常有用。 阅读有关[在UI](https://experienceleague.adobe.com/en/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview#managing-audit-logs-in-the-ui)中管理审核日志的更多信息。

### 筛选审核日志 {#filter-audit-logs}

审核日志UI提供了多个过滤器来帮助您搜索特定日志：

* **类别**：对其执行操作的资源类型，如Collaboration实例或Collaboration连接邀请。
* **操作**：执行的操作类型。 可用操作取决于所选类别。 例如，Collaboration实例的操作包括创建、更新和删除。
* **请求ID**：请求的唯一标识符。
* **用户**：执行操作的用户的电子邮件地址。
* **状态**：操作的状态，如允许或拒绝。
* **日期范围**：要查看其日志的日期范围。

阅读有关[筛选审核日志](https://experienceleague.adobe.com/en/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview#filter-audit-logs)的详细信息。

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
