---
title: 管理连接
description: 了解如何在Real-Time CDP Collaboration中管理您的连接。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/cn/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 50120839-4a20-4ec1-8887-9342bd17c52d
source-git-commit: 46d2596bd0ccdc5da32067493968945c61f8acc4
workflow-type: tm+mt
source-wordcount: '1079'
ht-degree: 1%

---

# 管理连接 {#manage-connections}

{{limited-availability-release-note}}

**[!UICONTROL 我的连接]**&#x200B;工作区提供了一个管理连接的集中位置。 您可以在&#x200B;**[!UICONTROL 现有连接]**&#x200B;部分中查看现有连接，并在&#x200B;**[!UICONTROL 需要操作]**&#x200B;部分中查看任何需要操作的连接。

## 查看连接 {#view-connection}

要查看现有连接，请导航到&#x200B;**[!UICONTROL 连接]**&#x200B;工作区。 作为发布者，将显示您现有的连接。 作为广告商，您应该导航到&#x200B;**[!UICONTROL 我的连接]**。

![在“我的连接”工作区中，为某个连接突出显示了“查看连接”选项。](/help/assets/connect/manage-connections/view-connection.png){zoomable="yes"}

此时会出现连接概述工作区，其中显示有关连接及其活动项目的详细信息。 选择&#x200B;**[!UICONTROL 连接设置]**&#x200B;以查看连接设置。

![连接概述工作区中突出显示的连接设置选项。](/help/assets/connect/manage-connections/connection-overview.png){zoomable="yes"}

此时会出现连接设置工作区，其中显示您与协作者之间的连接详细信息。 在这里，您可以查看在连接过程中选择的所有设置、连接的当前状态、连接所有者和协作者的联系信息。 有关特定连接设置的信息，请参阅[连接设置](/help/guide/connect/establishing-connections.md#connection-settings)指南。

![连接设置工作区显示连接详细信息。](/help/assets/connect/manage-connections/connection-settings.png){zoomable="yes"}

## 删除连接 {#delete-connection}

您可以删除与协作者之间不希望继续使用的任何连接。 要删除连接，请导航到要删除的连接，然后在连接工作区中选择删除图标![删除图标](/help/assets/common/delete.svg)。

![连接工作区中突出显示的删除图标。](/help/assets/connect/establish-connection/delete-option.png){zoomable="yes"}

将出现一个确认对话框，要求您确认删除连接。 选择&#x200B;**[!UICONTROL 删除]**&#x200B;以确认删除。

![用于删除连接的确认对话框。](/help/assets/connect/establish-connection/delete-confirmation-dialog.png){zoomable="yes"}

>[!WARNING]
>
>删除连接后，协作中的所有现有项目将被永久删除且无法恢复。 在&#x200B;**[!UICONTROL 我的连接]**&#x200B;的&#x200B;**[!UICONTROL 需要操作]**&#x200B;部分中，连接请求将保持挂起状态，但连接及其配置将不再处于活动状态。 如果要再次与协作者连接，则需要重新建立连接。

## 编辑连接 {#edit-connection}

作为协作连接的所有者，您可以在建立连接后编辑与协作者的连接设置。 您可以：

* 添加用例
* 添加匹配键。 以后将支持删除匹配键。
* 更新受众激活权限
* 更新信用拆分设置

>[!IMPORTANT]
>
>将用例或匹配键添加到连接后，便无法将其删除。

>[!TIP]
>
>**所有者**&#x200B;是通过向&#x200B;**收件人**&#x200B;发送邀请来启动连接的协作者。 有关详细信息，请参阅[与协作者建立连接文档](./establishing-connections.md)。

要编辑连接设置，请导航到连接设置工作区。 选择三点图标（![三点图标）。](/help/assets/icons/more.png))以查看可用的操作，然后选择&#x200B;**[!UICONTROL 编辑]**。

![突出显示了“编辑”选项的连接设置工作区。](/help/assets/connect/manage-connections/edit-connection.png){zoomable="yes"}

此时会出现一个对话框，提示您编辑并提交设置更改以供协作者审阅。 选择&#x200B;**[!UICONTROL 编辑]**。

![突出显示了“编辑”选项的“编辑连接设置”对话框。](/help/assets/connect/manage-connections/edit-connection-settings-dialog.png){zoomable="yes"}

### 编辑受众激活 {#edit-audience-activation}

受众激活设置确定连接中的哪个协作者可以将受众激活到目标。 要更改这些设置，请在&#x200B;**[!UICONTROL 受众激活]**&#x200B;分区中选择&#x200B;**[!UICONTROL 编辑]**。

![编辑连接设置屏幕显示“受众激活”部分和“编辑”选项。](/help/assets/connect/manage-connections/edit-audience-activation.png){zoomable="yes"}

在&#x200B;**[!UICONTROL 受众激活]**&#x200B;对话框中，使用下拉菜单更新受众激活权限。 您可以选择单个协作者或允许两个协作者激活受众。

![为更新受众激活权限而扩展的“受众激活对话框突出显示”下拉菜单。](/help/assets/connect/manage-connections/audience-activation-dropdown-menu.png){zoomable="yes"}

完成后，选择&#x200B;**[!UICONTROL 保存]**。

![显示新受众激活权限和“保存”选项的“受众激活”对话框。](/help/assets/connect/manage-connections/audience-activation-dialog.png){zoomable="yes"}

### 添加用例 {#add-use-cases}

在Collaboration中，“发现”、“激活”和“测量”等用例决定了可以与协作者一起使用的项目部分和功能。 您可以将其他用例添加到未来项目的现有连接中。 有关详细信息，请参阅[协作用例](../overview/use-cases.md)。

要添加新用例，请在&#x200B;**[!UICONTROL 用例]**&#x200B;部分中选择&#x200B;**[!UICONTROL 编辑]**。

![编辑连接设置屏幕突出显示“用例”部分和“编辑”选项。](/help/assets/connect/manage-connections/edit-use-cases.png){zoomable="yes"}

在&#x200B;**[!UICONTROL 用例]**&#x200B;对话框中，打开要添加的新用例，然后打开&#x200B;**[!UICONTROL 保存]**。

![显示“保存”选项的“用例”对话框突出显示。](/help/assets/connect/manage-connections/use-cases-dialog.png){zoomable="yes"}

>[!NOTE]
>
>当您[添加新的用例](#add-use-cases)（如“Audience Activation”或“Measurement”）时，编辑连接设置屏幕将更新为包含&#x200B;**[!UICONTROL Audience Activation]**&#x200B;和&#x200B;**[!UICONTROL 信用拆分]**&#x200B;部分。 您必须为这些新用例配置相应的设置。 有关更多详细信息，请参阅[受众激活](../connect/establishing-connections.md#audience-activation)和[信用分摊](../connect/establishing-connections.md#credit-split)指南。
>
>![添加新用例后，编辑连接设置屏幕显示“受众激活”和“信用拆分”部分。](/help/assets/connect/manage-connections/setup-audience-activation-credit-split.png){zoomable="yes"}

### 添加匹配键 {#add-match-keys}

只有匹配您在帐户中配置并由协作者选择的密钥才可用于连接。 当您[向您的帐户](../setup/onboard-account.md#edit-match-keys)添加新的匹配密钥，并且您的协作者也选择相同的密钥后，您便可以在现有连接中启用它们。

在“编辑连接设置”屏幕中，选择&#x200B;**[!UICONTROL 匹配键]**&#x200B;部分中的&#x200B;**[!UICONTROL 编辑]**。

![编辑连接设置屏幕突出显示“匹配键”部分和“编辑”选项。](/help/assets/connect/manage-connections/edit-connection-match-keys.png){zoomable="yes"}

出现&#x200B;**[!UICONTROL 匹配键]**&#x200B;对话框，显示为连接配置的现有匹配键。 选择要添加的匹配键，然后选择&#x200B;**[!UICONTROL 保存]**。

![“匹配键”对话框显示所选的新匹配键和“保存”选项。](/help/assets/connect/manage-connections/connection-match-keys-dialog.png){zoomable="yes"}

### 编辑信用拆分 {#edit-credit-split}

信用分摊设置指定由哪个协作者负责与连接中的每个用例关联的成本。 要更新这些设置，请在&#x200B;**[!UICONTROL 信用拆分]**&#x200B;分区中选择&#x200B;**[!UICONTROL 编辑]**。

![编辑连接设置屏幕突出显示“信用拆分”部分和“编辑”选项。](/help/assets/connect/manage-connections/edit-credit-split.png){zoomable="yes"}

在&#x200B;**[!UICONTROL 信用拆分]**&#x200B;对话框中，选择[!UICONTROL 激活匹配]和[!UICONTROL 测量]的首选设置。 然后，选择&#x200B;**[!UICONTROL 保存]**&#x200B;以进行确认。

![显示信用拆分设置和“保存”选项的“信用拆分”对话框。](/help/assets/connect/manage-connections/credit-split-dialog.png){zoomable="yes"}

### 审核并提交更改 {#review-and-submit-changes}

完成编辑连接设置后，查看并选择&#x200B;**[!UICONTROL 提交更改]**。 连接设置更新将发送给您的协作者以供审查。

![编辑连接设置屏幕显示更新和“提交更改”选项。](/help/assets/connect/manage-connections/review-and-submit-changes.png){zoomable="yes"}

#### 将连接设置更改另存为草稿

您可以将连接设置更改另存为草稿，并随时返回以完成连接设置的更新。

要将更改另存为草稿，请选择&#x200B;**[!UICONTROL 提交更改]**&#x200B;旁边的&#x200B;**[!UICONTROL 取消]**。 然后，在&#x200B;**[!UICONTROL 未提交的更改]**&#x200B;对话框中，选择&#x200B;**[!UICONTROL 稍后继续]**&#x200B;以进行确认。

![编辑连接设置屏幕。](/help/assets/connect/manage-connections/unsubmitted-changes-dialog.png){zoomable="yes"}

现在，您的更改将另存为草稿。 在连接设置工作区中，您可以看到一条通知，指示存在未提交的更改。 若要进行进一步的更新，请选择&#x200B;**[!UICONTROL 继续编辑]**。

![连接设置工作区中的通知，显示有未提交的更改等待审核和提交。](/help/assets/connect/manage-connections/continue-editing-connection.png){zoomable="yes"}
