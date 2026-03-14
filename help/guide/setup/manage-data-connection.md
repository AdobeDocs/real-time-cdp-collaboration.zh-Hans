---
title: 管理数据连接
description: 了解如何在Real-Time CDP Collaboration中管理数据连接，包括匹配键、计划、用例和受众筛选
audience: administrator, data engineer
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: d142d3ed-f56a-4150-a885-571728a73ac8
source-git-commit: 4bfa57ba36336dd835551fb846f1d567d6830bf9
workflow-type: tm+mt
source-wordcount: '1168'
ht-degree: 6%

---

# 管理数据连接

{{limited-availability-release-note}}

## 概述

在Real-Time CDP Collaboration中使用数据连接从各种平台获取受众。 了解如何管理匹配键并为现有数据连接计划数据刷新。 此外，您还可以按不同属性过滤受众，以获得更精细的见解。

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
>additional-url="https://www.adobe.com/go/rtcdp-collaboration-manage-dataconnections" text="扩充"

>[!IMPORTANT]
>
>在编辑数据连接的匹配键之前，请注意以下事项：
>
>* 只有为您的帐户配置的匹配密钥才能用于数据连接。
>* 此时，您可以向数据连接添加其他匹配密钥，但启用匹配密钥后，将无法将其删除。

从&#x200B;**[!UICONTROL 匹配项]**&#x200B;部分中选择&#x200B;**[!UICONTROL 编辑]**。

![突出显示了“编辑”选项的“匹配键”部分。](/help/assets/setup/manage-data-connection/edit-match-keys.png){zoomable="yes"}

此时会显示确认对话框，说明对数据连接所做的任何更改都将应用于所有关联的访问群体。 选择“**[!UICONTROL 确定]**”进行确认。 您以后可以选择跳过此确认。

![确认对话框，其中显示对数据连接所做的任何更改都将应用于所有关联的受众。](/help/assets/setup/manage-data-connection/confirm-data-connection-changes.png){zoomable="yes"}

在&#x200B;**[!UICONTROL 匹配键]**&#x200B;对话框中，可以查看源字段与其相应目标字段（匹配键）之间的现有映射。 您可以通过更新映射的源字段来编辑匹配键，或添加其他映射字段行以填充新的匹配键。

![显示源字段和相应目标字段之间现有映射的“匹配键”对话框。](/help/assets/setup/manage-data-connection/match-keys-dialog.png){zoomable="yes"}

#### 添加匹配键 {#add-match-keys}

选择&#x200B;**[!UICONTROL 添加字段]**&#x200B;以添加新字段行。

![选择“添加字段”后，“匹配键”对话框会显示一个空的新映射字段，此字段已准备好输入。](/help/assets/setup/manage-data-connection/add-new-field.png){zoomable="yes"}

接下来，选择空的源字段。 显示&#x200B;**[!UICONTROL 选择源字段]**&#x200B;对话框，其中包含&#x200B;**[!UICONTROL 标识命名空间]**&#x200B;和&#x200B;**[!UICONTROL 配置文件属性]**&#x200B;选项。 您可以筛选列表，并使用搜索选项查找所需的源字段。

选择所需的源字段，然后进行&#x200B;**[!UICONTROL 选择]**。

![选择了GAID选项的“选择源字段”对话框。](/help/assets/setup/manage-data-connection/select-source-field.png){zoomable="yes"}

在&#x200B;**[!UICONTROL 匹配键]**&#x200B;对话框中，使用下拉菜单将新源字段映射到目标字段。 所有可用目标字段都是为Collaborator帐户配置的匹配密钥。 如果未看到所需的目标字段，请[编辑帐户的匹配密钥](./onboard-account.md#edit-match-keys)以添加该字段。

如果您要将非哈希域作为哈希目标域的源，例如，将纯文本电子邮件源域映射到&#x200B;**[!UICONTROL 哈希电子邮件]**&#x200B;目标域时，请使用&#x200B;**[!UICONTROL 应用转换]**&#x200B;选项。

![下拉菜单显示所有可用目标字段，以使用新的源字段进行映射。](/help/assets/setup/manage-data-connection/select-target-field.png){zoomable="yes"}

完成映射字段后，请查看更新并选择&#x200B;**[!UICONTROL 确认]**&#x200B;以应用更改。

![显示更新字段映射的“匹配键”对话框突出显示“确认”选项。](/help/assets/setup/manage-data-connection/review-and-confirm.png){zoomable="yes"}

确认对话框用于确认匹配键已成功更新。

### 编辑计划 {#edit-scheduling}

创建数据连接后，可以直接从数据连接工作区的&#x200B;**[!UICONTROL 计划]**&#x200B;部分更新其刷新频率、开始日期和结束日期。

您可以编辑现有数据连接的频率，以更好地控制刷新受众的频率。 要编辑计划，请在计划卡片的数据连接中选择&#x200B;**[!UICONTROL 编辑]**。

![突出显示了“编辑”选项的“计划”部分。](/help/assets/setup/manage-data-connection/edit-scheduling.png){zoomable="yes"}

此时将显示确认对话框，其中说明对数据连接所做的任何更改都将应用于所有关联受众。 选择&#x200B;**[!UICONTROL 确定]**&#x200B;确认。 您可以选择以后跳过此确认。

![确认对话框，其中显示对数据连接所做的任何更改都将应用于所有关联的受众。](/help/assets/setup/manage-data-connection/confirm-data-connection-changes.png){zoomable="yes"}

在&#x200B;**[!UICONTROL 计划]**&#x200B;对话框中，选择下拉菜单以更新&#x200B;**[!UICONTROL 频率]**。 将刷新频率设置为每天或每两到六天运行一次。

![展开了“计划”对话框，其中的“频率”下拉菜单显示受众刷新频率选项。](../../assets/setup/manage-data-connection/edit-frequency.png){zoomable="yes"}

接下来，如果要更新填充和刷新受众的时段，请选择&#x200B;**[!UICONTROL 日期范围]**。

![显示“日期范围”下拉列表的“计划”对话框已展开，可编辑受众填充和刷新的开始和结束日期。](../../assets/setup/manage-data-connection/edit-date-range.png){zoomable="yes"}

完成后，查看更新并选择&#x200B;**[!UICONTROL 保存]**&#x200B;以应用更改。

![“计划”对话框突出显示“更新和保存”选项。](../../assets/setup/manage-data-connection/scheduling-dialog.png){zoomable="yes"}

## 删除数据连接

删除数据连接将会删除整个Collaboration中的所有基础受众、关联设置和使用情况。 无法撤消此操作。

要删除现有的数据连接，请选择单个数据连接工作区中的删除图标（![删除图标](/help/assets/common/delete.svg)）。

![突出显示删除选项的数据连接工作区。](/help/assets/setup/manage-data-connection/delete-data-connection.png){zoomable="yes"}

将出现一个确认对话框。 选择&#x200B;**[!UICONTROL 删除]**&#x200B;以完成数据连接的删除。

![突出显示带有“删除”选项的“删除数据连接”对话框。](/help/assets/setup/manage-data-connection/delete-data-connection-confirm.png){zoomable="yes"}

## 管理受众 {#manage-audiences}

附加到数据连接的访问群体列表会显示在工作区的底部。 该列表显示了每个受众的简要概述，包括其状态、来源和连接访问。 要编辑受众的类别、连接访问权限或元数据可见性，请选择受众的名称。 有关管理受众的完整指南，请参阅[查看个人受众](./onboard-audiences.md#view-individual-audiences)指南。

![突出显示受众的数据连接工作区。](/help/assets/setup/manage-data-connection/view-data-connection-manage-audiences.png){zoomable="yes"}

## 后续步骤

管理数据连接后，您可以[发现受众与协作者发现的受众之间的重叠](/help/guide/collaborate/discover.md)。
