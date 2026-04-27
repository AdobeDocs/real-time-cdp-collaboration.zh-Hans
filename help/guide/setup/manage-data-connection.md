---
title: 管理数据连接
description: 了解如何在Real-Time CDP Collaboration中管理数据连接，包括匹配键、计划、用例和受众筛选
audience: administrator, data engineer
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: d142d3ed-f56a-4150-a885-571728a73ac8
TQID: https://experienceleague.adobe.com/QvkEpR1fJMZ5BXrucAzEtxFNSfSMS-2hIZvMSg63ySE
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
feature_v2:
  - id: ba929a52-9339-4154-9487-317dc875a3c7
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 3ce7e66b31332836fd6cc6137c94622436505cc9
workflow-type: tm+mt
source-wordcount: 1179
ht-degree: 37%

---

# 管理数据连接

{{limited-availability-release-note}}

## 概述

在Real-Time CDP Collaboration中使用数据连接从各种平台获取受众。 了解如何管理匹配键并为现有数据连接计划数据刷新。 此外，您还可以按不同属性过滤受众，以获得更精细的见解。

>[!NOTE]
>
>要创建新的数据连接，请参阅[添加和管理受众](./onboard-audiences.md)。

## 查看数据连接

要查看现有的数据连接，请导航到&#x200B;**[!UICONTROL 安装程序]**，然后选择&#x200B;**[!UICONTROL 我的数据连接]**&#x200B;选项卡。 此时将显示您当前的所有数据连接，其中显示每个连接的简短概述。 要完整查看数据连接的信息（包括其匹配键、计划详细信息和受众），请选择相应连接上的&#x200B;**[!UICONTROL 查看数据连接]**。

![显示并突出显示“我的数据连接”选项卡视图的设置工作区。](/help/assets/setup/manage-data-connection/my-data-connections.png){zoomable="yes"}

### 匹配键 {#match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_matchkeys"
>title="匹配键"
>abstract="匹配键决定如何匹配来自不同来源的数据。 下面显示的匹配键是您将源字段映射到那里的目标字段。"

匹配键是您[将源字段映射到](./onboard-audiences.md#map-fields)的目标字段。 要了解有关匹配键如何工作的更多信息，请参阅[匹配键](./onboard-account.md#set-up-match-keys)指南。

![突出显示匹配键部分的数据连接工作区。](/help/assets/setup/manage-data-connection/view-data-connection-match-keys.png){zoomable="yes"}

### 日程计划 {#scheduling}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_scheduling"
>title="日程计划"
>abstract="查看数据连接的计划详情，并在需要时编辑相关配置。"

查看和管理数据连接的计划设置。 计划决定了刷新受众的频率。

创建数据连接后，可以直接从数据连接工作区的&#x200B;**[!UICONTROL 计划]**&#x200B;部分更新其刷新频率、开始日期和结束日期。

>[!NOTE]
>
>从Adobe Experience Platform获取受众后，受众将在数据连接建立后的24小时内可用。 在初始来源补充后，受众数据会根据定义的频率进行刷新。

有关计划的详细信息，请参阅配置受众指南中的[计划部分](/help/guide/setup/onboard-audiences.md#schedule)。

![突出显示计划部分的数据连接的工作区。](/help/assets/setup/manage-data-connection/view-data-connection-scheduling.png){zoomable="yes"}

## 编辑数据连接 {#edit-data-connection}

请阅读以下部分，了解如何更新匹配键以及现有数据连接的计划设置。

### 编辑匹配键 {#edit-match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_edit_measurement_data_connection_enrichment"
>title="扩充"
>abstract="不支持关闭扩充。 您可以改为更改扩充连接键。"
>additional-url="https://www.adobe.com/go/rtcdp-collaboration-manage-dataconnections_cn" text="扩充"

>[!IMPORTANT]
>
>在编辑数据连接的匹配键之前，请注意以下事项：
>
>* 只有为您的帐户配置的匹配键才能用于数据连接。
>* 此时，您可以向数据连接添加其他匹配键，但一旦启用了匹配键，就无法将其删除。

从&#x200B;**[!UICONTROL 匹配键]**&#x200B;部分中选择&#x200B;**[!UICONTROL 编辑]**。

![突出显示了“编辑”选项的“匹配键”部分。](/help/assets/setup/manage-data-connection/edit-match-keys.png){zoomable="yes"}

此时将显示确认对话框，其中说明对数据连接所做的任何更改都将应用于所有关联受众。 选择&#x200B;**[!UICONTROL 确定]**&#x200B;确认。 You can choose to skip this confirmation in the future.

![Confirmation dialog showing that any changes to the data connection will apply to all associated audiences.](/help/assets/setup/manage-data-connection/confirm-data-connection-changes.png){zoomable="yes"}

在&#x200B;**[!UICONTROL 匹配键]**&#x200B;对话框中，可以查看源字段与其对应的目标字段（匹配键）之间的现有映射。 您可以通过更新映射的源字段来编辑匹配键，或者添加其他映射字段行以填充新的匹配键。

![The Match keys dialog showing the existing mappings between source fields and the corresponding target fields.](/help/assets/setup/manage-data-connection/match-keys-dialog.png){zoomable="yes"}

#### Add match keys {#add-match-keys}

Select **[!UICONTROL Add field]** to add a new field row.

![选择“添加字段”后，“匹配键”对话框将显示一个空的新映射字段可供输入。](/help/assets/setup/manage-data-connection/add-new-field.png){zoomable="yes"}

Next, select the empty source field. 将显示&#x200B;**[!UICONTROL 选择源字段]**&#x200B;对话框，其中包含&#x200B;**[!UICONTROL 身份命名空间]**&#x200B;和&#x200B;**[!UICONTROL 配置文件属性]**&#x200B;选项。 您可以筛选列表并使用搜索选项查找所需的源字段。

选择所需的源字段，然后选择&#x200B;**[!UICONTROL 选择]**。

![已选择GAID选项的“选择源字段”对话框。](/help/assets/setup/manage-data-connection/select-source-field.png){zoomable="yes"}

在&#x200B;**[!UICONTROL 匹配键]**&#x200B;对话框中，使用下拉菜单将新的源字段映射到目标字段。 所有可用的目标字段都是为Collaborator帐户配置的匹配键。 如果未看到所需的目标字段，请[编辑帐户的匹配键](./onboard-account.md#edit-match-keys)以添加它。

如果您要将非哈希字段源到哈希目标字段，例如将纯文本电子邮件源字段映射到&#x200B;**[!UICONTROL 哈希电子邮件]**&#x200B;目标字段，请使用&#x200B;**[!UICONTROL 应用转换]**&#x200B;选项。

![下拉菜单显示所有可用目标字段以与新的源字段映射。](/help/assets/setup/manage-data-connection/select-target-field.png){zoomable="yes"}

完成字段映射后，查看更新并选择&#x200B;**[!UICONTROL 确认]**&#x200B;以应用更改。

![The Match keys dialog showing the updated field mapping with the Confirm option highlighted.](/help/assets/setup/manage-data-connection/review-and-confirm.png){zoomable="yes"}

A confirmation dialog confirms that the match keys were updated successfully.

### Edit scheduling {#edit-scheduling}

创建数据连接后，可以直接从数据连接工作区的&#x200B;**[!UICONTROL 计划]**&#x200B;部分更新其刷新频率、开始日期和结束日期。

You can edit the frequency of an existing data connection to better control how often audiences are refreshed. To edit the schedule, select **[!UICONTROL Edit]** from within the data connection in the scheduling card.

![The Scheduling section with the Edit option highlighted.](/help/assets/setup/manage-data-connection/edit-scheduling.png){zoomable="yes"}

此时将显示确认对话框，其中说明对数据连接所做的任何更改都将应用于所有关联受众。 选择&#x200B;**[!UICONTROL 确定]**&#x200B;确认。 You can choose to skip this confirmation in the future.

![Confirmation dialog showing that any changes to the data connection will apply to all associated audiences.](/help/assets/setup/manage-data-connection/confirm-data-connection-changes.png){zoomable="yes"}

In the **[!UICONTROL Scheduling]** dialog, select the dropdown menu to update the **[!UICONTROL Frequency]**. Set the refresh frequency to run daily or every two to six days.

![The Scheduling dialog with the Frequency dropdown expanded to display audience refresh frequency options.](../../assets/setup/manage-data-connection/edit-frequency.png){zoomable="yes"}

Next, select **[!UICONTROL Date range]** if you want to update the period during which audiences are populated and refreshed.

![The Scheduling dialog showing the Date range dropdown expanded to edit the start and end dates for audience population and refresh.](../../assets/setup/manage-data-connection/edit-date-range.png){zoomable="yes"}

When you&#39;re done, review the updates and select **[!UICONTROL Save]** to apply your changes.

![The Scheduling dialog highlighting the updates and Save option.](../../assets/setup/manage-data-connection/scheduling-dialog.png){zoomable="yes"}

## 删除数据连接

Deleting a data connection will remove all underlying audiences, associated settings, and usage across Collaboration. 无法撤消此操作。

To delete an existing data connection, select the delete icon (![Delete icon](/help/assets/common/delete.svg)) within an individual data connection&#39;s workspace.

![A data connections workspace with the delete option highlighted.](/help/assets/setup/manage-data-connection/delete-data-connection.png){zoomable="yes"}

A confirmation dialogue will appear. Select **[!UICONTROL Delete]** to finish deleting the data connection.

![The Delete data connection dialog with the Delete option highlighted.](/help/assets/setup/manage-data-connection/delete-data-connection-confirm.png){zoomable="yes"}

## Manage audiences {#manage-audiences}

附加到数据连接的受众列表将显示在工作区底部。 该列表显示每个受众的简要概述，包括其状态、来源和连接访问。 To edit an audience&#39;s categories, connection access, or metadata visbility, select the audience&#39;s name. 有关管理受众的完整指南，请参阅[查看各个受众](./onboard-audiences.md#view-individual-audiences)指南。

![A data connections workspace with the audiences highlighted.](/help/assets/setup/manage-data-connection/view-data-connection-manage-audiences.png){zoomable="yes"}

## 后续步骤

管理数据连接后，您可以[发现受众与协作者已使其可发现的受众之间的重叠](/help/guide/collaborate/discover.md)。
