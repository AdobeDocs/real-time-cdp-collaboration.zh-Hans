---
title: 激活受众
description: 了解如何将受众发送给协作者，并将收到的受众手动激活到Adobe Real-Time CDP Collaboration中的目标。
audience: admin, publisher, advertiser
exl-id: fd82fcbf-ab39-48e0-9438-0a9046693431
TQID: https://experienceleague.adobe.com/bfPHtcW8Mf6RhIlg5fKcJmPSEKDyAODjbNRJ5D3SMkQ
product_v2: id: fdddec33-c9cb-4459-b8b6-2664395a6f10
feature_v2: id: ba929a52-9339-4154-9487-317dc875a3c7
topic_v2: id: c2be0313-b3ae-45e0-b454-d20bf54b23f2id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 5d12a5004a6854392c130fd6b93a841fb22cf6ab
workflow-type: tm+mt
source-wordcount: 1565
ht-degree: 2%

---

# 激活受众

使用项目中的&#x200B;**[!UICONTROL 激活]**&#x200B;选项卡将受众发送到协作者，审查从协作者处收到的受众，并激活收到的受众以发送到配置的目标。 要从顶级&#x200B;**[!UICONTROL 激活]**&#x200B;工作区配置和管理目标，请参阅[目标概述](../destinations/overview.md)。

>[!IMPORTANT]
>
>**[!UICONTROL 激活]**&#x200B;选项卡仅在连接进程](../connect/establishing-connections.md#connection-settings)期间[启用了&#x200B;**受众激活**&#x200B;用例时才可用。 有关用例的更多信息，请参阅[管理项目](./manage-projects.md#project-use-cases)。

使用[发现选项卡](./discover.md)确定与您的活动最匹配的受众，然后将其发送给您的协作者。 接收协作者选择配置的目标并安排接收受众进行激活。

发送和激活是独立的操作。 发送可让您的协作者访问受众。 然后，接收协作者选择一个目标并手动激活接收的受众。

您可用的部分和操作取决于您的组织是在项目中发送还是接收受众。 **[!UICONTROL 激活]**&#x200B;选项卡包含以下部分：

| 部分 | 描述 |
|---|---|
| **[!UICONTROL 将受众发送至[协作者]]** | 已发送给协作者的受众。 |
| **[!UICONTROL 已接收受众]** | 您的协作者已发送给您且可供激活的受众。 |
| **[!UICONTROL 激活的受众]** | 已收到您激活到目标的受众。 |

![项目级别的“激活”选项卡，其摘要计数位于顶部，并展开“已发送受众”、“已接收受众”和“已激活受众”部分。 每个部分都显示状态计数和受众详细信息表。](/help/assets/collaborate/activate/activate-dashboard.png)

## 先决条件 {#prerequisites}

在发送或激活受众之前，请确保：

- 受众是来源受众并可用于发送。 有关详细信息，请参阅[Source和管理受众](../setup/onboard-audiences.md)。
- 如果您需要激活收到的受众，则至少会配置一个目标。 有关详细信息，请参阅[目标概述](../destinations/overview.md)。

## 发送受众 {#send-audiences}

发送受众以授予您的协作者对其进行访问的权限。 发送受众后，该受众会显示在您的&#x200B;**[!UICONTROL 将受众发送到[协作者]]**&#x200B;分区以及协作者的&#x200B;**[!UICONTROL 已接收受众]**&#x200B;分区中。

导航到&#x200B;**[!UICONTROL 协作]**，打开一个项目，然后选择&#x200B;**[!UICONTROL 激活]**&#x200B;选项卡。

在&#x200B;**[!UICONTROL 将受众发送到[协作者]]**&#x200B;部分中，选择添加图标（![添加图标。](/help/assets/icons/plus.png)）。 如果未发送任何受众，请改为从空显示中选择&#x200B;**[!UICONTROL 发送受众]**。

![未发送受众时，使用项目级别的“激活”选项卡。 显示消息为空说明您尚未发送受众，并显示“发送受众”按钮。](/help/assets/collaborate/activate/activate-new-audiences.png)

将打开&#x200B;**[!UICONTROL 发送受众]**&#x200B;工作流。 使用受众选择器查找受众，或选择&#x200B;**[!UICONTROL 浏览受众]**&#x200B;来比较可用受众。

![包含受众选择器和浏览受众按钮的“发送受众”工作流。 工作流允许发件人在配置匹配密钥和访问设置之前选择受众。](/help/assets/collaborate/activate/audience-activation.png)

在&#x200B;**[!UICONTROL 浏览受众]**&#x200B;对话框中，查看每个受众的&#x200B;**[!UICONTROL 身份计数]**、**[!UICONTROL 重叠身份]**&#x200B;和&#x200B;**[!UICONTROL 重叠%]**。

![浏览受众对话框列出了可用受众及其身份计数、重叠身份计数和重叠百分比。](/help/assets/collaborate/activate/browse-audiences.png)

>[!IMPORTANT]
>
>如果受众使用多个匹配键，则每个选定的匹配键都必须满足所需的重叠阈值。 使用[发现选项卡](./discover.md)在发送受众之前确认受众满足重叠要求。

选择要发送的受众，然后选择&#x200B;**[!UICONTROL 保存]**。

所选受众会显示在工作流中，其中包含其标识和重叠信息。

![发送受众工作流中的选定受众显示其身份计数、重叠身份计数、重叠百分比、匹配键和编辑匹配键选项。](/help/assets/collaborate/activate/audience-selected.png)

### 编辑匹配键 {#edit-match-keys}

使用为Collaborator连接配置的匹配键，或删除任何不适用于受众的匹配键。

在所选受众中选择&#x200B;**[!UICONTROL 编辑匹配键]**。

![在“发送受众”工作流中选择的受众中突出显示“编辑匹配键”选项。](/help/assets/collaborate/activate/edit-match-keys.png)

出现&#x200B;**[!UICONTROL 编辑匹配键]**&#x200B;对话框。 关闭任何您不想使用的匹配键，然后选择&#x200B;**[!UICONTROL 保存]**。

>[!NOTE]
>
>必须至少保留一个匹配键。

![“编辑匹配键”对话框，其中包含通过Collaborator连接和“保存”按钮提供的匹配键的切换控件。](/help/assets/collaborate/activate/edit-match-keys-selection.png)

### 配置受众访问 {#configure-audience-access}

配置受众的发送方式以及协作者可以对其进行访问的时长。

使用&#x200B;**[!UICONTROL 访问持续时间]**&#x200B;控件选择以下选项之一：

- **[!UICONTROL 立即发送（一次性）]**：将受众发送一次。 接收协作者可以将其激活一次。
- **[!UICONTROL 计划定期受众发送]**：在指定的访问期间刷新受众。 使用&#x200B;**[!UICONTROL 日期范围]**&#x200B;控件选择开始日期和结束日期。

![发送受众工作流中的访问持续时间步骤，其中包含选项可用于发送受众一次，或计划定期发送受众。 定期选项显示用于定义访问时段的日期控件。](/help/assets/collaborate/activate/activation-frequency.png)

完成受众和访问设置后，选择&#x200B;**[!UICONTROL 发送]**。

受众显示在您的&#x200B;**[!UICONTROL 将受众发送到[协作者]]**&#x200B;部分中。 您的协作者可以在其&#x200B;**[!UICONTROL 已接收受众]**&#x200B;分区中查看它。

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

![发送的受众部分，其删除图标显示在受众行的旁边。](/help/assets/collaborate/activate/delete-sent-audiences.png)

将显示确认对话框。 选择&#x200B;**[!UICONTROL 删除]**&#x200B;以确认。

![已发送受众删除确认对话框，其中说明将删除受众，协作者将失去访问权限，并显示“取消”和“删除”按钮。](/help/assets/collaborate/activate/delete-sent-audiences-confirmation.png)

受众将从部分中删除，您的协作者将无法访问它。

## 查看收到的受众 {#received-audiences}

使用&#x200B;**[!UICONTROL 接收的受众]**&#x200B;部分查看您的协作者发送给您的受众。 在将数据发送到目标之前，必须手动激活接收到的受众。

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

![包含活动受众和已过期受众规模的“已接收受众”部分。 每个受众行会显示其名称、状态、身份信息、上次数据流运行、访问持续时间、匹配键以及用于开始激活的添加图标。](/help/assets/collaborate/activate/received-audiences-section.png)

### 激活已接收的受众 {#activate-received-audience}

激活已接收的受众，将其数据发送到其中一个已配置的目标。

在&#x200B;**[!UICONTROL 接收的受众]**&#x200B;部分中，选择添加图标（![添加图标。](/help/assets/icons/plus.png)） ，位于要激活的受众旁。

出现&#x200B;**[!UICONTROL 激活受众]**&#x200B;对话框。

使用&#x200B;**[!UICONTROL 目标]**&#x200B;选择接收受众数据的目标。 如果目标列表为空，请在继续之前配置目标。 有关说明，请参阅[目标概述](../destinations/overview.md)。

使用&#x200B;**[!UICONTROL 日期]**&#x200B;选择激活运行的日期，然后选择&#x200B;**[!UICONTROL 激活]**。

![从收到的受众中打开“激活受众”对话框。 该对话框包含用于选择已配置目标的“目标”下拉列表、带有日历控件的“日期”字段以及“取消”和“激活”按钮。](/help/assets/collaborate/activate/activate-received-audience.png)

对话框关闭，激活显示在&#x200B;**[!UICONTROL 激活的受众]**&#x200B;部分。 接收到的受众在&#x200B;**[!UICONTROL 接收到的受众]**&#x200B;部分中仍然可用，但其访问权限仍保持活动状态。

## 查看激活的受众 {#activated-audiences}

使用&#x200B;**[!UICONTROL 激活的受众]**&#x200B;部分确认哪些接收的受众已激活，并查看其目标和投放状态。

每个激活的受众都会显示以下信息：

| 列 | 描述 |
|---|---|
| **[!UICONTROL 受众名称]** | 已激活受众的名称。 |
| **[!UICONTROL 状态]** | 当前的激活状态。 |
| **[!UICONTROL 激活计数]** | 激活到目标的身份数。 |
| **[!UICONTROL 上次刷新时间]** | 激活的受众最近刷新的日期和时间。 |
| **[!UICONTROL 目标]** | 接收受众数据的目标。 |
| **[!UICONTROL 频率]** | 激活频率。 手动激活显示&#x200B;**[!UICONTROL 一次]**。 |
| **[!UICONTROL 日期]** | 运行激活的日期。 |
| **[!UICONTROL 匹配键]** | 激活的受众中包含的匹配键。 |

![激活受众部分具有活动、已存档和已暂停的激活计数。 每行显示受众名称、状态、激活计数、上次刷新日期、目标、频率、激活日期、匹配键和删除图标。](/help/assets/collaborate/activate/activated-audiences-section.png)

### 删除激活的受众 {#delete-activated-audience}

删除激活的受众，以从&#x200B;**[!UICONTROL 激活的受众]**&#x200B;分区中删除该激活。

选择删除图标（![删除图标。](/help/assets/icons/delete.png)） ，位于已激活受众的旁边。

将显示确认对话框。 选择&#x200B;**[!UICONTROL 删除]**&#x200B;以确认。

![激活的受众删除确认对话框，说明受众将从激活的受众列表中删除，稍后可以使用“取消”和“删除”按钮再次激活。](/help/assets/collaborate/activate/delete-activated-audience-confirmation.png)

激活将从列表中删除。 您可以再次激活已接收的受众，同时保持其访问权限处于活动状态。

## 后续步骤 {#next-steps}

发送或激活受众后，在&#x200B;**[!UICONTROL 将受众发送到[协作者]]**&#x200B;和&#x200B;**[!UICONTROL 激活的受众]**&#x200B;部分中监视其状态。 营销活动完成后，请与Adobe启用和工程团队合作，上传测量数据并查看相应的[测量报告](./measure.md)。
