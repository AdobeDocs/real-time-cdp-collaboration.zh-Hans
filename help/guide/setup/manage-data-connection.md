---
title: 管理数据连接
description: 了解如何在Real-Time CDP Collaboration中管理数据连接，包括匹配键、计划、用例和受众筛选
audience: administrator, data engineer
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: d142d3ed-f56a-4150-a885-571728a73ac8
source-git-commit: acaaaa1e1fab981d874210639c16e76e48fc3394
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 17%

---

# 管理数据连接

{{limited-availability-release-note}}

## 概述

在Real-Time CDP Collaboration中使用数据连接从各种源导入受众。 了解如何管理匹配键以及计划现有数据连接的数据导入。 此外，您还可以按不同属性过滤受众，以获得更精细的见解。

在此处管理数据连接之前，您应在[受众入门工作流](./onboard-audiences.md)期间首先对其进行设置。 这将确保连接正确的数据源以供在Real-Time CDP Collaboration中使用。

## 查看数据连接

>[!IMPORTANT]
>
>Real-Time CDP Collaboration用户界面当前不支持删除数据连接。 要删除数据连接，请联系您的Adobe代表或[创建客户支持工单](https://experienceleague.adobe.com/home?lang=en&amp;support-tab=open-ticket#support){target="_blank"}。

要查看现有的数据连接，请导航到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 我的受众]**，然后选择&#x200B;**[!UICONTROL 管理数据连接]**。

![设置工作区，突出显示管理数据连接。](/help/assets/setup/manage-data-connection/manage-data-connection-highlighted.png){zoomable="yes"}

这会显示您当前设置的所有数据连接，以及有关每个连接中的受众数量、数据连接来源等的信息。 选择&#x200B;**[!UICONTROL 查看数据连接]**&#x200B;可查看有关匹配键、计划以及属于此数据连接的受众的信息。

![管理具有连接的数据连接工作区查看突出显示的数据连接。](/help/assets/setup/manage-data-connection/view-data-connection-highlighted.png){zoomable="yes"}

### 匹配键 {#match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_matchkeys"
>title="匹配键"
>abstract="匹配键决定如何匹配来自不同来源的数据。选择与您的用例和隐私准则最相关的匹配键。"

匹配键是用于协调来自不同数据源的受众成员的标识符。可用的匹配键包括：

- **散列电子邮件**

您无法编辑此数据连接中使用的匹配键。

![突出显示匹配键部分的数据连接工作区。](/help/assets/setup/manage-data-connection/view-data-connection-match-keys.png){zoomable="yes"}

### 日程安排 {#scheduling}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_scheduling"
>title="日程安排"
>abstract="此视图显示您最初为数据连接选择的调度选项。"

您无法编辑最初为数据连接选择的计划选项。 有关计划选项的详细信息，请查看受众导入工作流文档中的[计划部分](/help/guide/setup/onboard-audiences.md#schedule)。

![突出显示了“计划”部分的数据连接工作区。](/help/assets/setup/manage-data-connection/view-data-connection-scheduling.png){zoomable="yes"}

## 管理受众 {#manage-audiences}

在数据连接中查看受众列表时，您可以选择查看受众、编辑其类别或从数据连接中删除受众。

![突出显示受众的数据连接工作区。](/help/assets/setup/manage-data-connection/view-data-connection-manage-audiences.png){zoomable="yes"}

## 后续步骤

管理数据连接后，您可以[发现受众与协作者已使其可发现的受众之间的重叠](/help/guide/collaborate/discover.md)。
