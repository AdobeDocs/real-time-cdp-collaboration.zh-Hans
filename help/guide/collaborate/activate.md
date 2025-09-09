---
title: 激活受众
description: 了解如何在Adobe Real-Time CDP Collaboration中激活受众。
audience: admin, publisher
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/cn/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: fd82fcbf-ab39-48e0-9438-0a9046693431
source-git-commit: afe8560a12017c6b993f93cde8636288aa6e4991
workflow-type: tm+mt
source-wordcount: '1003'
ht-degree: 2%

---

# 激活受众

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>**[!UICONTROL 激活]**&#x200B;工作区仅在连接进程&#x200B;**期间**&#x200B;启用[受众激活](../connect/establishing-connections.md#connection-settings)用例时才可用。 有关用例的更多信息，请参阅[管理项目](./manage-projects.md#project-use-cases)指南。

Audience Activation允许您激活受众，以便在营销活动中使用。 根据连接[中配置的受众激活设置](/help/guide/connect/establishing-connections.md#configure-connection-settings)，激活可由协作者完成。 在您[发现营销活动的最佳受众](./discover.md)后，激活这些受众以使其可用。 激活受众后，该受众会发送到协作者的预配置目标，例如Adobe Experience Platform，可在其中用于营销活动。 有关设置目标的详细信息，请参阅[目标概述](../destinations/overview.md)指南。

## 激活新受众 {#activate-new-audiences}

要开始激活受众，请导航到项目工作区中的&#x200B;**[!UICONTROL 激活]**&#x200B;选项卡。

>[!IMPORTANT]
>
>**在**&#x200B;可以激活受众之前，协作者&#x200B;**必须**&#x200B;配置目标。 激活受众后，该受众会自动发送到协作者配置的目标位置。 如果未设置目标，则无法激活受众。
>
>![当协作者未配置目标时激活工作区。](/help/assets/collaborate/activate/no-destination-configured.png)

选择添加图标（![添加图标）。](/help/assets/icons/plus.png))或&#x200B;**[!UICONTROL 激活受众]**&#x200B;选项（如果未发送以前的受众进行激活）。

![未添加受众的项目中的激活工作区。](/help/assets/collaborate/activate/activate-new-audiences.png)

激活受众工作流将打开，您可以在其中选择要发送给协作者受众。 使用下拉菜单选择受众，或搜索特定受众。 要在进行选择之前查看有关受众的详细信息，请选择&#x200B;**[!UICONTROL 浏览受众]**

![突出显示了下拉列表和浏览受众选项的Audience激活工作流。](/help/assets/collaborate/activate/audience-activation.png)

在&#x200B;**[!UICONTROL 浏览受众]**&#x200B;中，您可以看到每个受众的&#x200B;**[!UICONTROL 身份计数]**、**[!UICONTROL 重叠身份]**&#x200B;和&#x200B;**[!UICONTROL 重叠%]**。

![显示可用受众的“浏览受众”对话框。](/help/assets/collaborate/activate/browse-audiences.png)

>[!IMPORTANT]
>
>在激活使用了多个匹配键的受众时，如果一个（或多个）匹配键没有重叠、没有受众计数或低于阈值，则整个激活将失败。 在激活之前，请确保您的受众有足够的重叠，并满足所有匹配键中1000个ID的最低阈值。

选择要在营销活动中激活的受众，然后选择&#x200B;**[!UICONTROL 保存]**。 该受众现在显示出来，您可以看到所选受众的&#x200B;**[!UICONTROL 身份计数]**、**[!UICONTROL 重叠身份]**&#x200B;和&#x200B;**[!UICONTROL 重叠%]**。

![显示具有选定受众的受众激活工作流。](/help/assets/collaborate/activate/audience-selected.png)

### 编辑匹配键 {#edit-match-keys}

接下来，您可以通过选择受众中的&#x200B;**[!UICONTROL 编辑匹配键]**&#x200B;来编辑受众的匹配键。 最初设置协作者之间的连接时，这些选项继承自匹配的键选择。 如果所选匹配键不适用于特定营销活动，则可以将其删除，但无法添加新的匹配键。

![突出显示了“编辑匹配键”选项的Audience激活工作流。](/help/assets/collaborate/activate/edit-match-keys.png)

**[!UICONTROL 编辑匹配键]**&#x200B;对话框打开，您可以在其中关闭不想使用的匹配键。 选择&#x200B;**[!UICONTROL 保存]**&#x200B;以保存更改。

>[!NOTE]
>
>必须至少选择一个匹配键。 在当前版本中，唯一可用的匹配密钥是&#x200B;**[!UICONTROL 哈希电子邮件]**，因此您不能删除此匹配密钥。

![受众激活工作流中的“编辑匹配密钥”对话框。](/help/assets/collaborate/activate/edit-match-keys-selection.png)

### 设置受众刷新频率 {#set-audience-refresh-frequency}

最后，设置受众刷新的所需频率和日期范围。 在当前版本中，唯一支持的频率选项是&#x200B;**[!UICONTROL 一次]**。 **[!UICONTROL 一次]**&#x200B;频率表示只激活一次受众，不刷新受众。 **[!UICONTROL Date]**&#x200B;选项自动填充了当前日期。

![已突出显示“频率”部分的Audience激活工作流。](/help/assets/collaborate/activate/audience-frequency.png)

如果对您的选择满意，请选择&#x200B;**[!UICONTROL 激活]**&#x200B;以完成工作流。

## 激活仪表板 {#activate-dashboard}

在&#x200B;**[!UICONTROL 激活]**&#x200B;选项卡中，可以查看发送给协作者的所有受众，以及协作者激活到目标的所有受众。

![显示“已发送受众”和“已激活受众”部分的“激活”仪表板。](/help/assets/collaborate/activate/activate-dashboard.png)

## 查看已发送受众 {#view-sent-audiences}

在&#x200B;**[!UICONTROL 将受众发送到]**&#x200B;协作者部分中，将列出您发送的所有受众。 目前，在发送受众后，受众会自动发送到协作者的配置目标。 在协作者的视图中，这些受众显示在&#x200B;**[!UICONTROL 激活的受众]**&#x200B;部分中。

在每个已发送受众中，您可以看到以下量度：

| 量度 | 描述 |
|---------|----------|
| **[!UICONTROL 名称]** | 受众的名称。 |
| **[!UICONTROL 状态]** | 已发送受众的状态。 |
| **[!UICONTROL 身份计数]** | 受众中的身份数。 |
| **[!UICONTROL 身份重叠]** | 此受众与协作者库存中的配置文件总数之间的重叠身份数。 |
| **[!UICONTROL 已创建]** | 最初发送受众的日期。 |
| **[!UICONTROL 上次发送]** | 上次将受众发送给协作者时的日期。 |
| **[!UICONTROL 匹配键]** | 指示用于受众的匹配键。 |

## 查看激活的受众 {#view-activated-audiences}

在&#x200B;**[!UICONTROL 激活的受众]**&#x200B;部分中，您可以看到已激活到目标的所有受众。

在每个激活的受众中，您可以看到以下量度：

| 量度 | 描述 |
|---------|----------|
| **[!UICONTROL 名称]** | 受众的名称。 |
| **[!UICONTROL 状态]** | 已激活受众的状态。 |
| **[!UICONTROL 身份计数]** | 根据协作者发送受众时的重叠身份激活的身份数。 |
| **[!UICONTROL 已创建]** | 激活受众的日期。 |
| **[!UICONTROL 上次刷新时间]** | 根据激活期间选择的刷新计划，上次刷新受众的日期。 |
| **[!UICONTROL 目标]** | 受众激活到的目标。 |
| **[!UICONTROL 匹配键]** | 指示用于受众的匹配键。 |

## 删除已发送受众 {#delete-sent-audiences}

您可以删除不再想要激活的已发送受众。 当您删除已发送受众时，该受众将会从&#x200B;**[!UICONTROL 已发送受众至]**&#x200B;分区中删除，并且不会再激活到您的协作者的目标。

要删除已发送受众，请选择&#x200B;**[!UICONTROL 删除]**&#x200B;图标（![删除图标）。](/help/assets/icons/delete.png)将受众发送到&#x200B;**[!UICONTROL 分区中的受众旁边的]**。

![“将受众发送至”部分中的“删除”选项。](/help/assets/collaborate/activate/delete-sent-audiences.png)

这将打开一个确认对话框，要求您确认删除。 选择&#x200B;**[!UICONTROL 删除]**&#x200B;以确认。

![删除确认对话框。](/help/assets/collaborate/activate/delete-sent-audiences-confirmation.png)

## 后续步骤 {#next-steps}

在激活受众并运行营销活动后，与Adobe启用和工程团队合作，上传测量数据并查看相应的[测量报表](/help/guide/collaborate/measure.md)。
