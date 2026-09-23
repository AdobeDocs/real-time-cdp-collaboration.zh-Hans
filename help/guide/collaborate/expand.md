---
title: 在展开中创建展开受众
description: 了解如何使用Adobe Real-Time CDP Collaboration中的协作者受众群体，从种子受众创建扩展受众。
source-git-commit: 88cd685742a4d85850cbf732ef93ab215287c22a
workflow-type: tm+mt
source-wordcount: '871'
ht-degree: 1%
---
# 在展开中创建展开受众

使用项目中的&#x200B;**[!UICONTROL 展开]**&#x200B;选项卡从某个受众创建展开受众。 Collaboration使用协作者的受众群体来查找与种子受众相似的用户档案，这样可帮助您在不暴露协作者基础受众数据的情况下接触新的潜在客户。 生成的扩展受众将发送给您的协作者进行激活。

## 先决条件 {#prerequisites}

在使用&#x200B;**[!UICONTROL 展开]**&#x200B;选项卡之前，您应具有：

* [来源](/help/guide/setup/onboard-audiences.md)至少一个受众用作种子受众
* [已连接](/help/guide/connect/establishing-connections.md)协作者
* [已使用该协作者创建项目](/help/guide/collaborate/manage-projects.md)
* 如果您正在接收扩展受众，则将[目标](/help/guide/destinations/overview.md)配置为接收激活的受众

## 展开概述 {#expand-overview}

导航到&#x200B;**[!UICONTROL 协作]** > **[!UICONTROL 我的项目]**，打开一个项目，然后选择&#x200B;**[!UICONTROL 展开]**&#x200B;选项卡。

**[!UICONTROL 展开]**&#x200B;页面显示为此协作者创建的展开受众以及创建新受众的选项。

![显示“扩展”受众表的“扩展”选项卡，其中包含“名称”、“状态”、“模型大小”、“受众范围”和“上次更新时间”列。](/help/assets/collaborate/expand/expand-overview.png){zoomable="yes"}

**[!UICONTROL 扩展受众]**&#x200B;表列出了项目中创建的每个扩展受众：

| 列 | 描述 |
|---|---|
| **[!UICONTROL 名称]** | 扩展受众的名称。 默认使用种子受众名称，直到编辑为止。 |
| **[!UICONTROL 状态]** | 扩展受众的当前状态。 有关详细信息，请参阅[扩展受众状态](#expansion-audience-status)。 |
| **[!UICONTROL 模型大小]** | 生成的扩展受众的大小。 在模型完成处理之前不可用。 |
| **[!UICONTROL 受众范围]** | 用于扩展受众的“受众范围”设置。 |
| **[!UICONTROL 上次更新时间]** | 上次更新扩展受众的日期和时间。 |

{style="table-layout:auto"}

### 扩展受众状态 {#expansion-audience-status}

扩展受众会经历以下状态：

| 状态 | 描述 |
|---|---|
| **[!UICONTROL 正在处理]** | 扩展模型仍在生成扩展受众。 |
| **[!UICONTROL 草稿]** | 模型已完成，扩展受众已准备好供您查看并发送给您的协作者。 |
| **[!UICONTROL 活动]** | 您已向协作者发送扩展受众。 |

{style="table-layout:auto"}

>[!NOTE]
>
>状态不会实时更新。 重新打开或刷新&#x200B;**[!UICONTROL 展开]**&#x200B;选项卡以查看最新状态。

## 创建扩展受众 {#create-expansion-audience}

要创建新的扩展受众，请选择添加图标（![添加图标。](/help/assets/icons/plus.png)） 在&#x200B;**[!UICONTROL 展开]**&#x200B;页面上，然后选择&#x200B;**[!UICONTROL 创建展开的受众]**。


出现&#x200B;**[!UICONTROL 生成扩展受众]**&#x200B;对话框。 填写每个字段以生成扩展受众。

![包含种子受众、受众范围、匹配键和种子受众成员字段的“生成受众扩展”对话框。](/help/assets/collaborate/expand/generate-expansion-audience-dialog.png){zoomable="yes"}

### 选择您的种子受众 {#select-seed-audience}

从&#x200B;**[!UICONTROL 选择种子受众]**&#x200B;下拉列表中选择您自己的受众之一。 Collaboration使用此受众作为在协作者群体中查找相似用户档案的基础。

![生成受众扩展对话框中的种子受众字段。](/help/assets/collaborate/expand/select-seed-audience.png){zoomable="yes"}

### 选择匹配键 {#select-match-key}

为扩展受众启用一个匹配键。 不能启用多个扩展。

| 人员 ID | 设备 ID |
|---|---|
| **[!UICONTROL 散列电子邮件]** | **[!UICONTROL 散列IPv4]** |
| **[!UICONTROL 散列电话]** | **[!UICONTROL GAID]** |
| **[!UICONTROL 忠诚度ID]** | **[!UICONTROL IDFA]** |
| **[!UICONTROL CRM ID]** | **[!UICONTROL Demdex ID]** |

{style="table-layout:auto"}

>[!NOTE]
>
>如果您的种子受众不包括给定的匹配键，则该选项显示为禁用状态，无法选择。

![“生成受众扩展”对话框中的“匹配键”部分，其中包含可用的匹配键选项。](/help/assets/collaborate/expand/select-match-key.png){zoomable="yes"}

### 选择您的受众范围 {#select-audience-reach}

使用&#x200B;**[!UICONTROL 受众范围]**&#x200B;下拉菜单以平衡与种子受众的相似性和整体范围。 选择&#x200B;**[!UICONTROL Balanced]**&#x200B;作为与您的种子受众的相似性和整体覆盖范围之间的中间位置。

![在“生成受众扩展”对话框中，选择了“平衡”选项及其下方的描述文本的“受众范围”字段。](/help/assets/collaborate/expand/select-audience-reach.png){zoomable="yes"}

### 包含或排除您的种子受众 {#include-exclude-seed-audience}

使用&#x200B;**[!UICONTROL 种子受众]**&#x200B;单选按钮选择您的原始种子受众是包含在最终扩展受众中还是从最终扩展受众中排除。

![使用“是”和“否”单选按钮的“生成受众扩展”对话框中的“种子受众成员”字段。](/help/assets/collaborate/expand/include-exclude-seed-audience.png){zoomable="yes"}

### 生成扩展受众 {#generate-expansion-audience}

完成所有字段后，选择&#x200B;**[!UICONTROL 生成扩展受众]**。 一条确认消息确认Collaboration正在创建扩展受众，并且您可以在&#x200B;**[!UICONTROL 扩展]**&#x200B;页面上跟踪其进度。

## 审阅并发送扩展受众 {#review-send-expansion-audience}

扩展受众的状态更新为&#x200B;**[!UICONTROL 草稿]**&#x200B;后，从&#x200B;**[!UICONTROL 扩展受众]**&#x200B;表中选择其名称以将其打开。

![扩展受众显示受众元数据、模型大小、种子受众大小和发送按钮的详细信息页面。](/help/assets/collaborate/expand/expansion-audience-detail.png){zoomable="yes"}

从该视图中，您可以：

* 编辑扩展受众名称
* 查看创建日期和时间
* 比较种子受众规模与生成的扩展受众规模
* 查看用于生成受众的匹配键

准备就绪后，选择&#x200B;**[!UICONTROL 发送给合作伙伴]**&#x200B;以将扩展受众发送给您的协作者。 在发送受众之前，该受众将保持在&#x200B;**[!UICONTROL 草稿]**&#x200B;状态，然后更新为&#x200B;**[!UICONTROL 活动]**。

>[!NOTE]
>
>如果协作者未配置目标，则&#x200B;**[!UICONTROL 发送到合作伙伴]**&#x200B;不可用。 有一条消息说明您的协作者需要首先设置一个目标。

>[!IMPORTANT]
>
>如果未发送给您的协作者，则扩展受众将在生成后7天过期。

## 接收和激活扩展受众 {#receive-activate-expansion-audience}

当您发送扩展受众时，Collaboration会根据为连接配置的激活设置将其交付给协作者：

* 如果启用了&#x200B;**自动激活**，Collaboration会自动将扩展受众激活到协作者的配置目标，该受众将显示在其[激活选项卡](./activate.md#activated-audiences)中。
<!-- Beta release: automatic activation is the only available activation setting. Uncomment the manual activation guidance below when manual activation is introduced with the GA release. -->
<!-- * If **manual activation** is enabled, the expansion audience appears in your collaborator's [Received audiences](./activate.md#received-audiences) section of the **[!UICONTROL Activate]** tab, and your collaborator must manually activate it. -->

## 后续步骤

发送扩展受众后，请使用[发现选项卡](./discover.md)将其与其他受众进行比较，或者使用[激活选项卡](./activate.md)跟踪其激活。
