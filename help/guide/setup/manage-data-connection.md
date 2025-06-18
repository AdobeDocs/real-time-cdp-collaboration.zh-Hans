---
title: 管理数据连接
description: 了解如何在Real-Time CDP Collaboration中管理数据连接，包括匹配键、计划、用例和受众筛选
audience: administrator, data engineer
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: d142d3ed-f56a-4150-a885-571728a73ac8
source-git-commit: b28bb5037c25f630059e6e8bc375ce28e0967ac7
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 12%

---

# 管理数据连接

{{limited-availability-release-note}}

## 概述

在Real-Time CDP Collaboration中使用数据连接从各种源导入受众。 了解如何管理匹配键以及计划现有数据连接的数据导入。 此外，您还可以按不同属性过滤受众，以获得更精细的见解。

## 查看数据连接

要查看现有的数据连接，请导航到&#x200B;**[!UICONTROL 安装程序]**，然后选择&#x200B;**[!UICONTROL 我的数据连接]**&#x200B;选项卡。 此时将显示您当前的所有数据连接，其中显示每个连接的简短概述。 要完整查看数据连接的信息（包括其匹配键、计划详细信息和受众），请选择相应连接上的&#x200B;**[!UICONTROL 查看数据连接]**。

![显示并突出显示“我的数据连接”选项卡视图的设置工作区。](/help/assets/setup/manage-data-connection/my-data-connections.png){zoomable="yes"}

### 匹配键 {#match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_matchkeys"
>title="匹配键"
>abstract="匹配键决定如何匹配来自不同来源的数据。选择与您的用例和隐私准则最相关的匹配键。"

匹配键是用于协调来自不同数据源的受众成员的标识符。您无法编辑最初为数据连接选择的匹配键。

>[!IMPORTANT]
> 
>创建数据连接后，无法编辑匹配键。 要更新匹配键，必须创建新的数据连接。

可用的匹配键包括：

- **散列电子邮件**

![突出显示匹配键部分的数据连接工作区。](/help/assets/setup/manage-data-connection/view-data-connection-match-keys.png){zoomable="yes"}

### 日程计划 {#scheduling}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_scheduling"
>title="日程计划"
>abstract="查看数据连接的调度详细信息，并在需要时编辑刷新频率。"

查看和管理数据连接的计划设置。 计划决定了刷新受众的频率。

创建数据连接后，可以直接从数据连接工作区的&#x200B;**[!UICONTROL 计划]**&#x200B;部分更新其刷新频率。

>[!NOTE]
>
>从Adobe Experience Platform获取受众后，受众将在数据连接建立后的24小时内可用。 首次导入后，受众数据会根据定义的频率进行刷新。

有关计划的更多信息，请参阅入门受众指南中的[计划部分](/help/guide/setup/onboard-audiences.md#schedule)。

![突出显示计划部分的数据连接的工作区。](/help/assets/setup/manage-data-connection/view-data-connection-scheduling.png){zoomable="yes"}

#### 编辑计划 {#edit-scheduling}

您可以编辑现有数据连接的频率，以更好地控制刷新受众的频率。 要编辑计划，请在计划卡片的数据连接中选择&#x200B;**[!UICONTROL 编辑]**。

在&#x200B;**[!UICONTROL 计划]**&#x200B;对话框中，选择下拉菜单以更新&#x200B;**[!UICONTROL 频率]**。 将刷新频率设置为每天或每两到六天运行一次。 完成后，选择&#x200B;**[!UICONTROL 保存]**&#x200B;以应用更改。

![计划对话框，显示用于设置频率和日期范围的选项。](../../assets/setup/manage-data-connection/scheduling-dialog.png){zoomable="yes" alt="The Scheduling dialog with editable fields for frequency."}

## 删除数据连接

删除数据连接将会删除整个平台中的所有底层受众、关联设置和使用情况。 此操作无法撤消。

要删除现有的数据连接，请选择单个数据连接工作区中的删除图标（![删除图标](/help/assets/common/delete.svg)）。

![突出显示删除选项的数据连接工作区。](/help/assets/setup/manage-data-connection/delete-data-connection.png){zoomable="yes"}

将出现一个确认对话框。 选择&#x200B;**[!UICONTROL 删除]**&#x200B;以完成数据连接的删除。

![突出显示带有“删除”选项的“删除数据连接”对话框。](/help/assets/setup/manage-data-connection/delete-data-connection-confirm.png){zoomable="yes"}

## 管理受众 {#manage-audiences}

附加到数据连接的受众列表将显示在工作区底部。 该列表显示每个受众的简要概述，包括其状态、来源和连接访问。 要编辑受众的类别、连接访问权限或元数据可见性，请选择受众的名称。 有关管理受众的完整指南，请参阅[查看各个受众](./onboard-audiences.md#view-individual-audiences)指南。

![突出显示受众的数据连接工作区。](/help/assets/setup/manage-data-connection/view-data-connection-manage-audiences.png){zoomable="yes"}

## 后续步骤

管理数据连接后，您可以[发现受众与协作者已使其可发现的受众之间的重叠](/help/guide/collaborate/discover.md)。
