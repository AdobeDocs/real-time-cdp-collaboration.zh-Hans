---
title: 激活受众
description: 了解如何发送受众，以及在Adobe Real-Time CDP Collaboration中自动或手动将收到的受众激活到目标。
audience: admin, publisher, advertiser
exl-id: fd82fcbf-ab39-48e0-9438-0a9046693431
TQID: https://experienceleague.adobe.com/bfPHtcW8Mf6RhIlg5fKcJmPSEKDyAODjbNRJ5D3SMkQ
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
    internal-label: Real-Time Customer Data Platform
feature_v2:
  - id: ba929a52-9339-4154-9487-317dc875a3c7
    internal-label: Use cases
topic_v2:
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
    internal-label: Measurement
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: df0c7fe0d09203a02a192931135abaa1715e593f
workflow-type: tm+mt
source-wordcount: '2043'
ht-degree: 1%
---
# 激活受众

使用项目中的&#x200B;**[!UICONTROL 激活]**&#x200B;选项卡将受众发送到协作者，审查从协作者处收到的受众，并激活收到的受众以发送到配置的目标。 接收受众时，会自动创建激活，或由接收协作者手动创建。 要从顶级&#x200B;**[!UICONTROL 激活]**&#x200B;工作区配置和管理目标，请参阅[目标概述](../destinations/overview.md)。

>[!IMPORTANT]
>
>**[!UICONTROL 激活]**&#x200B;选项卡仅在连接进程[&#128279;](../connect/establishing-connections.md#connection-settings)期间启用了&#x200B;**受众激活**&#x200B;用例时才可用。 有关用例的更多信息，请参阅[管理项目](./manage-projects.md#project-use-cases)。

使用[发现选项卡](./discover.md)确定与您的活动最匹配的受众，然后将其发送给您的协作者。

如果接收者在连接设置中配置了自动激活目标，则发送者在发送受众时选择激活计划。 对于发件人，目标为只读。 接收受众后，受众会按照发件人的激活计划，自动激活到接收者配置的目的地。 有关连接设置说明，请参阅[配置自动激活目标](../connect/manage-connections.md#configure-auto-activation-destination)。

如果接收方未配置自动激活目标，则发送和激活操作将保持分离。 发送功能允许接收者访问受众，接收者在手动激活受众时选择目标和计划。 在项目中，只能选择预配置的目标进行激活。 有关目标配置说明，请参阅[管理目标](../destinations/manage-destinations.md)。

您可用的部分和操作取决于您的组织是在项目中发送还是接收受众。 **[!UICONTROL 激活]**&#x200B;选项卡包含以下部分：

| 部分 | 描述 |
|---|---|
| **[!UICONTROL 将受众发送至[协作者]]** | 已发送给协作者的受众。 |
| **[!UICONTROL 已接收受众]** | 您的协作者已发送给您且可供激活的受众。 |
| **[!UICONTROL 激活的受众]** | 通过自动或手动创建的激活接收的受众。 |

![项目级别的“激活”选项卡，其摘要计数位于顶部，并展开“已发送受众”、“已接收受众”和“已激活受众”部分。 每个部分都显示状态计数和受众详细信息表。](/help/assets/collaborate/activate/activate-dashboard.png){zoomable="yes"}

## 先决条件 {#prerequisites}

在发送或激活受众之前，请确保：

- 受众是来源受众并可用于发送。 有关详细信息，请参阅[Source和管理受众](../setup/onboard-audiences.md)。
- 受众满足发送和激活所需的最低1,000个身份重叠阈值。
- 使用多匹配键受众时，会使用所需的匹配键配置受众。
- 如果您需要激活收到的受众，则至少会配置一个目标。 有关详细信息，请参阅[目标概述](../destinations/overview.md)。
- 对于自动激活，接收方拥有活动目标并将其选为连接的[自动激活目标](../connect/manage-connections.md#configure-auto-activation-destination)。

## 发送受众 {#send-audiences}

发送受众以授予您的协作者对其进行访问的权限。 发送受众后，该受众会显示在您的&#x200B;**[!UICONTROL 将受众发送到[协作者]]**&#x200B;分区以及协作者的&#x200B;**[!UICONTROL 已接收受众]**&#x200B;分区中。

导航到&#x200B;**[!UICONTROL 协作]**，打开一个项目，然后选择&#x200B;**[!UICONTROL 激活]**&#x200B;选项卡。

在&#x200B;**[!UICONTROL 将受众发送到[协作者]]**&#x200B;部分中，选择添加图标（![添加图标。](/help/assets/icons/plus.png)）。 如果未发送任何受众，请改为从空显示中选择&#x200B;**[!UICONTROL 发送受众]**。

![未发送受众时，使用项目级别的“激活”选项卡。 显示消息为空说明您尚未发送受众，并显示“发送受众”按钮。](/help/assets/collaborate/activate/activate-new-audiences.png){zoomable="yes"}

将打开&#x200B;**[!UICONTROL 发送受众]**&#x200B;工作流。 使用受众选择器查找受众，或选择&#x200B;**[!UICONTROL 浏览受众]**&#x200B;来比较可用受众。

>[!IMPORTANT]
>
>只有重叠身份数超过1000的受众才可供激活。 如果受众重叠接近于1000身份阈值，则激活可能会失败。

![包含受众选择器和浏览受众按钮的“发送受众”工作流。 工作流允许发件人在配置匹配密钥和访问设置之前选择受众。](/help/assets/collaborate/activate/audience-activation.png){zoomable="yes"}

在&#x200B;**[!UICONTROL 浏览受众]**&#x200B;对话框中，查看每个受众的&#x200B;**[!UICONTROL 身份计数]**、**[!UICONTROL 重叠身份]**&#x200B;和&#x200B;**[!UICONTROL 重叠%]**。

![浏览受众对话框列出了可用受众及其身份计数、重叠身份计数和重叠百分比。](/help/assets/collaborate/activate/browse-audiences.png){zoomable="yes"}

>[!IMPORTANT]
>
>如果受众使用多个匹配键，则每个选定的匹配键都必须满足所需的重叠阈值。 使用[发现选项卡](./discover.md)在发送受众之前确认受众满足重叠要求。

选择要发送的受众，然后选择&#x200B;**[!UICONTROL 保存]**。

所选受众会显示在工作流中，其中包含其标识和重叠信息。

![发送受众工作流中的选定受众显示其身份计数、重叠身份计数、重叠百分比、匹配键和编辑匹配键选项。](/help/assets/collaborate/activate/audience-selected.png){zoomable="yes"}

### 编辑匹配键 {#edit-match-keys}

使用为Collaborator连接配置的匹配键，或删除任何不适用于受众的匹配键。

在所选受众中选择&#x200B;**[!UICONTROL 编辑匹配键]**。

![在“发送受众”工作流中选择的受众中突出显示“编辑匹配键”选项。](/help/assets/collaborate/activate/edit-match-keys.png){zoomable="yes"}

出现&#x200B;**[!UICONTROL 编辑匹配键]**&#x200B;对话框。 关闭任何您不想使用的匹配键，然后选择&#x200B;**[!UICONTROL 保存]**。

>[!NOTE]
>
>必须至少保留一个匹配键。

![“编辑匹配键”对话框，其中包含通过Collaborator连接和“保存”按钮提供的匹配键的切换控件。](/help/assets/collaborate/activate/edit-match-keys-selection.png){zoomable="yes"}

### 配置受众访问 {#configure-audience-access}

配置受众的发送方式以及协作者可以对其进行访问的时长。

使用&#x200B;**[!UICONTROL 访问持续时间]**&#x200B;控件选择以下选项之一：

- **[!UICONTROL 立即发送（一次性）]**：将受众发送一次。 接收协作者可以将其激活一次。
- **[!UICONTROL 计划定期受众发送]**：在指定的访问期间刷新受众。 使用&#x200B;**[!UICONTROL 日期范围]**&#x200B;控件选择开始日期和结束日期。

![发送受众工作流中的访问持续时间步骤，其中包含选项可用于发送受众一次，或计划定期发送受众。 定期选项显示用于定义访问时段的日期控件。](/help/assets/collaborate/activate/activation-frequency.png)

### 选择自动激活计划 {#auto-activation-schedule}

如果您的协作者为连接配置了自动激活目标，则&#x200B;**[!UICONTROL 激活]**&#x200B;部分指示已启用&#x200B;**[!UICONTROL 自动激活]**。 接收方选择的目的地显示为只读。 作为发件人，请使用&#x200B;**[!UICONTROL Frequency]**&#x200B;选择激活运行的时间：

- **[!UICONTROL 立即激活（一次性）]**：收到受众后运行激活一次。
- **[!UICONTROL 安排一次受众激活]**：在您选择的将来日期和时间运行一次激活。
- **[!UICONTROL 计划定期激活]**：按您在所选日期范围内配置的计划运行激活。

![启用了自动激活的“发送受众”工作流以及“频率”菜单，其中显示立即、将来的一次性和循环激活选项。](/help/assets/collaborate/activate/choose-auto-activation-schedule.png){zoomable="yes"}

对于定期激活，请配置激活计划、开始时间和日期范围。 自动激活支持立即、将来的一次性或定期计划；不需要定期激活。

![使用每日定期激活计划、开始时间和日期范围配置的“发送受众”工作流。](/help/assets/collaborate/activate/configure-recurring-auto-activation.png){zoomable="yes"}

完成受众和访问设置后，选择&#x200B;**[!UICONTROL 发送]**。

受众显示在您的&#x200B;**[!UICONTROL 将受众发送到[协作者]]**&#x200B;部分中。 您的协作者可以在其&#x200B;**[!UICONTROL 已接收受众]**&#x200B;分区中查看它。 如果启用了自动激活，则Collaboration还会为接收方创建激活，并根据您选择的计划运行激活。

## 查看已发送受众 {#view-sent-audiences}

使用&#x200B;**[!UICONTROL 将受众发送到[collaborator]]**&#x200B;部分查看您已发送的受众，并监视其当前访问状态。

每个已发送受众都会显示以下信息：

| 列 | 描述 |
|---|---|
| **[!UICONTROL 受众名称]** | 已发送受众的名称。 |
| **[!UICONTROL 状态]** | 受众的当前访问状态。 |
| **[!UICONTROL 身份计数]** | 受众中的身份数。 |
| **[!UICONTROL 身份重叠]** | 与协作者清单重叠的身份数。 |
| **[!UICONTROL 已创建]** | 首次发送受众的日期和时间。 |
| **[!UICONTROL 上次发送]** | 最近将受众数据发送到协作者时的日期和时间。 |
| **[!UICONTROL 访问持续时间]** | 发送受众时配置的访问设置。 |
| **[!UICONTROL 匹配键]** | 发送受众时使用的匹配键。 |

### 删除已发送受众 {#delete-sent-audience}

删除已发送受众，以将其从已发送受众列表中删除，并撤销协作者的访问权限。

选择删除图标（![删除图标。](/help/assets/icons/delete.png)） 在&#x200B;**[!UICONTROL 将受众发送到[协作者]]**&#x200B;分区中的受众旁边。

![发送的受众部分，其删除图标显示在受众行的旁边。](/help/assets/collaborate/activate/delete-sent-audiences.png){zoomable="yes"}

将显示确认对话框。 选择&#x200B;**[!UICONTROL 删除]**&#x200B;以确认。

![已发送受众删除确认对话框，其中说明将删除受众，协作者将失去访问权限，并显示“取消”和“删除”按钮。](/help/assets/collaborate/activate/delete-sent-audiences-confirmation.png)

受众将从部分中删除，您的协作者将无法访问它。

## 查看收到的受众 {#received-audiences}

使用&#x200B;**[!UICONTROL 接收的受众]**&#x200B;部分查看您的协作者发送给您的受众。 如果在发送受众之前配置了自动激活目标，则Collaboration会在收到受众时自动创建激活。 对于循环自动激活，您还可以创建对其他目标的额外手动激活。 有关详细信息，请参阅[手动激活接收的受众](#activate-received-audience)。 如果未配置自动激活目标，请手动激活受众。

每个收到的受众都会显示以下信息：

| 列 | 描述 |
|---|---|
| **[!UICONTROL 受众名称]** | 接收受众的名称。 |
| **[!UICONTROL 状态]** | 受众的当前访问状态。 |
| **[!UICONTROL 身份计数]** | 受众中的身份数。 |
| **[!UICONTROL 身份重叠]** | 与您的清单重叠的标识数。 |
| **[!UICONTROL 上次数据流运行]** | 受众最近运行数据流的日期和时间。 |
| **[!UICONTROL 访问持续时间]** | 由发送受众的协作者配置的访问设置。 |
| **[!UICONTROL 匹配键]** | 用于受众的匹配键。 |

![包含活动受众和已过期受众规模的“已接收受众”部分。 每个受众行会显示其名称、状态、身份信息、上次数据流运行、访问持续时间、匹配键以及用于开始激活的添加图标。](/help/assets/collaborate/activate/received-audiences-section.png){zoomable="yes"}

### 手动激活已接收的受众 {#activate-received-audience}

手动激活已接收的受众，以将其数据发送到您配置的目标之一。

在&#x200B;**[!UICONTROL 接收的受众]**&#x200B;部分中，选择添加图标（![添加图标。](/help/assets/icons/plus.png)） ，位于要激活的受众旁。

出现&#x200B;**[!UICONTROL 激活受众]**&#x200B;对话框。

使用&#x200B;**[!UICONTROL 目标]**&#x200B;选择接收受众数据的目标。 如果目标列表为空，请在继续之前配置目标。 有关说明，请参阅[目标概述](../destinations/overview.md)。

配置&#x200B;**[!UICONTROL 频率]**&#x200B;和可用的计划控件以选择激活运行的时间和频率。 然后选择&#x200B;**[!UICONTROL 激活]**。

以下示例显示了选择&#x200B;**[!UICONTROL Northstar Audience Exports]**&#x200B;作为目标的手动激活工作流。

![手动激活Northstar Fall Campaign客户受众对话框示例，已选择Northstar受众导出并配置每日计划、开始时间和日期范围。](/help/assets/collaborate/activate/manually-activate-received-audience.png){zoomable="yes"}

>[!NOTE]
>
>对于通过定期自动激活接收的受众，您可以手动为该受众创建对其他目标的额外激活。 循环自动激活可独立继续。

对话框关闭，激活显示在&#x200B;**[!UICONTROL 激活的受众]**&#x200B;部分。 接收到的受众在&#x200B;**[!UICONTROL 接收到的受众]**&#x200B;部分中仍然可用，但其访问权限仍保持活动状态。

## 查看激活的受众 {#activated-audiences}

使用&#x200B;**[!UICONTROL 激活的受众]**&#x200B;部分确认哪些接收的受众已自动或手动创建激活并查看其目标和投放状态。 此处显示自动创建的激活，无需接收者完成手动激活工作流。

![显示“已接收”受众中Northstar Fall Campaign客户的“激活”选项卡，以及它自动创建的对“已激活”受众中Northstar受众导出的每日激活。](/help/assets/collaborate/activate/view-auto-activated-audience.png){zoomable="yes"}

每个激活的受众都会显示以下信息：

| 列 | 描述 |
|---|---|
| **[!UICONTROL 受众名称]** | 已激活受众的名称。 |
| **[!UICONTROL 状态]** | 当前的激活状态。 |
| **[!UICONTROL 激活计数]** | 激活到目标的身份数。 |
| **[!UICONTROL 上次刷新时间]** | 激活的受众最近刷新的日期和时间。 |
| **[!UICONTROL 目标]** | 接收受众数据的目标。 |
| **[!UICONTROL 频率]** | 激活频率，如一次性计划或定期计划。 |
| **[!UICONTROL 日期]** | 激活运行的日期或日期范围。 |
| **[!UICONTROL 匹配键]** | 激活的受众中包含的匹配键。 |

![激活受众部分具有活动、已存档和已暂停的激活计数。 每行显示受众名称、状态、激活计数、上次刷新日期、目标、频率、激活日期、匹配键和删除图标。](/help/assets/collaborate/activate/activated-audiences-section.png){zoomable="yes"}

### 删除激活的受众 {#delete-activated-audience}

删除激活的受众，以从&#x200B;**[!UICONTROL 激活的受众]**&#x200B;分区中删除该激活。

选择删除图标（![删除图标。](/help/assets/icons/delete.png)） ，位于已激活受众的旁边。

将显示确认对话框。 选择&#x200B;**[!UICONTROL 删除]**&#x200B;以确认。

![激活的受众删除确认对话框，说明受众将从激活的受众列表中删除，稍后可以使用“取消”和“删除”按钮再次激活。](/help/assets/collaborate/activate/delete-activated-audience-confirmation.png)

激活将从列表中删除。 您可以再次激活已接收的受众，同时保持其访问权限处于活动状态。

## 后续步骤 {#next-steps}

发送或激活受众后，在&#x200B;**[!UICONTROL 将受众发送到[协作者]]**&#x200B;和&#x200B;**[!UICONTROL 激活的受众]**&#x200B;部分中监视其状态。 营销活动完成后，请与Adobe启用和工程团队合作，上传测量数据并查看相应的[测量报告](./measure.md)。
