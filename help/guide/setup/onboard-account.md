---
title: 配置和管理您的帐户
description: 了解如何在Real-Time CDP Collaboration中配置和管理帐户的各个方面
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/cn/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: a95e932a-9681-48f2-bf34-6fe5a50597d7
source-git-commit: 873af5b0ef5e4e0c937c540de4697ec314624669
workflow-type: tm+mt
source-wordcount: '1373'
ht-degree: 11%

---

# 配置和管理您的帐户

{{limited-availability-release-note}}

了解如何在Real-Time CDP Collaboration中设置帐户，为与其他协作者建立连接做好准备。 本指南涵盖帐户的初始设置，包括添加帐户详细信息、选择匹配密钥和管理帐户设置。

![显示已配置帐户的安装工作区。](/help/assets/setup/manage-account/my-account.png){zoomable="yes"}

## 设置您的帐户 {#set-up-account}

首次访问Collaboration时，系统会提示您设置帐户。 这是一个一次性流程，允许您配置帐户详细信息和匹配密钥。 如果这是您组织的第一个帐户，则会立即引导您完成入门流程，从设置您的[帐户详细信息](#set-up-details)开始。

要添加其他组织，请导航到左边栏中的&#x200B;**[!UICONTROL 设置]**，然后选择添加图标（![添加图标）。](/help/assets/icons/plus.png))。 接下来，选择&#x200B;**[!UICONTROL 帐户]**。

![突出显示了“我的帐户”选项卡和“帐户”选项的设置工作区。](/help/assets/setup/manage-account/add-new-account.png){zoomable="yes"}

### 设置详细信息 {#set-up-details}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_setup_contact_email"
>title="联系电子邮件"
>abstract="请提供一个基于团队或角色的电子邮件地址，例如 **collaboration@yourcompany.com**。不应使用私人或个人的电子邮件地址。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_setup_connect_code"
>title="连接代码"
>abstract="连接代码是您帐户的唯一标识符。它用于在 Real-Time CDP Collaboration 中与其他协作者建立连接。"

要开始配置帐户，必须首先设置帐户详细信息。 这要求您添加以下信息：

* 添加明确代表您品牌的&#x200B;**[!UICONTROL 帐户名称]**。
* 添加有关您品牌的&#x200B;**[!UICONTROL 描述]**。 虽然这是一项可选操作，但它有助于其他协作者更好地了解您的品牌。
* 选择您的&#x200B;**[!UICONTROL 角色]**。 您可以选择介于&#x200B;**[!UICONTROL 广告商]**&#x200B;和&#x200B;**[!UICONTROL 发布者]**&#x200B;之间。 阅读[角色](/help/guide/overview/roles.md)指南以了解两种帐户角色类型在工作流中的相似之处和细微差异。
* 为您的帐户选择&#x200B;**[!UICONTROL 行业]**。 某些示例包括&#x200B;**[!UICONTROL 零售业]**、**[!UICONTROL 电信]**&#x200B;或&#x200B;**[!UICONTROL 金融服务]**。
* 已根据您的Adobe Experience Cloud帐户自动设置&#x200B;**[!UICONTROL 地区]**。 此更改随时无法更改。
* 为您的帐户添加&#x200B;**[!UICONTROL 联系人电子邮件]**。 这应该是基于团队或角色的电子邮件地址。 不应提供个人电子邮件地址。
* 为您的帐户上传&#x200B;**[!UICONTROL 徽标]**。 目前，支持SVG类型的图像。 这是可选操作，但上传徽标有助于在Collaboration界面中直观地展示您的品牌
* 选择帐户标题图片的图像。

>[!NOTE]
>
>虽然您可以随时编辑这些详细信息中的大部分内容，但在初始设置后，**[!UICONTROL 角色]**&#x200B;将不可编辑。 完成后，使用&#x200B;**[!UICONTROL 下一步]**&#x200B;进入下一页，选择贵组织将使用的所需匹配密钥。

![设置帐户工作区，其中显示了“详细信息”部分，并突出显示了“下一步”选项。](/help/assets/setup/manage-account/add-account-details.png){zoomable="yes"}

### 设置匹配键 {#set-up-match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_matchkeys"
>title="匹配键"
>abstract="匹配键是一种用于协调来自不同数据源的受众轮廓的标识符。包括您的品牌可以使用的任何匹配键。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_setup_match_keys"
>title="匹配键"
>abstract=""

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_peopleIDs"
>title="第一方人员 ID"
>abstract="第一方人员 ID（例如经过哈希处理的电子邮件地址和电话号码，或者 CRM ID）直接与个人轮廓连接。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_deviceIDs"
>title="第一方设备 ID"
>abstract="第一方设备ID（如ECID或IP地址）直接连接到可能在多个人之间共享的设备。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_partnerIDs"
>title="支持的合作伙伴 ID"
>abstract="合作伙伴 ID 是一种外部合作伙伴提供的用于协调受众的标识符。合作伙伴 ID 不与个人轮廓直接连接。"

![支持的匹配键。](/help/assets/setup/manage-account/match-keys.png){zoomable="yes"}

>[!IMPORTANT]
>
>您在帐户设置期间选择的匹配键将决定您的连接中可用的匹配键。 虽然在连接设置过程中可以[删除不需要的匹配键](../connect/establishing-connections.md#connection-settings)，但在建立连接后无法添加匹配键。 在帐户设置过程中，选择您计划在未来营销活动中使用的&#x200B;**所有**&#x200B;匹配键，这一点很重要。

匹配关键有助于协作者通过实现准确且以隐私为中心的数据同步来展开协作，进而实现更准确的受众定位和测量。 在帐户设置期间选择的匹配键将确定哪些匹配键在未来的连接中可用。 在获取受众时，它们还用于将[数据连接中的字段](./onboard-audiences.md#map-fields)映射到Collaboration中的目标字段。

选择要在协调受众配置文件时使用的任何匹配键。 针对未来进行规划，并包含您可以使用的任何匹配键，以及预计将在未来营销活动中使用的匹配键。 如果以后确实需要为您的帐户选择其他匹配密钥，则可以在[编辑帐户](#edit-account)工作流中执行此操作。 但是，在初始设置之后添加的任何匹配键将不可用于现有连接。

#### 支持的匹配键 {#supported-match-keys}

Collaboration支持三种类型的匹配键：第一方人员ID、第一方设备ID和合作伙伴ID。 所有匹配键必须满足以下要求：

* 匹配键必须是&#x200B;**修剪**，**小写**
* 哈希匹配键必须为&#x200B;**SHA256-hashed**。
* 如果您提供的哈希值使用大写字符，Collaboration会自动将其转换为小写。
* 如果源包含&#x200B;**纯文本标识符**，请在&#x200B;**[!UICONTROL 数据连接设置]**&#x200B;期间使用[应用转换](./manage-data-connection.md#match-keys)选项来应用散列。 仅当从Experience Platform获取受众时，此选项才可用，而基于云的源不支持此选项。

##### 第一方人员 ID

第一方人员ID直接关联到个人资料。 当前支持的ID包括：

* **[!UICONTROL 散列电子邮件]**
* **[!UICONTROL 散列电话]**
* **[!UICONTROL CRM ID]**
* **[!UICONTROL 忠诚度ID]**
<!-- * **[!UICONTROL Custom ID]**: Custom identifiers -->

##### 第一方设备 ID

第一方设备ID是连接到特定设备的标识符。 当前支持的ID包括：

* **[!UICONTROL 哈希IPv4]**：哈希IPv4地址
* **[!UICONTROL IDFA]**： Apple iOS设备中使用的广告商标识符(IDFA)
* **[!UICONTROL GAID]**： Android设备中使用的Google广告商ID

##### 合作伙伴 ID

合作伙伴 ID 是一种外部合作伙伴提供的用于协调受众的标识符。当前支持的ID包括：

* **[!UICONTROL AdFixus ID]**

>[!NOTE]
>
>Adobe与[!DNL AdFixus]的集成将每个帐户的唯一[!UICONTROL AdFixus ID]映射到通用的Adobe编码格式。 这些映射用于标识协作者之间的重叠。 使用&#x200B;**[!UICONTROL AdFixus ID]**&#x200B;激活受众时，将使用原始ID。 Adobe编码的格式永远不会离开Collaboration。

选择&#x200B;**[!UICONTROL AdFixus ID]**&#x200B;时，您需要在&#x200B;**[!UICONTROL 帐户凭据]**&#x200B;部分提供来自外部合作伙伴的对应ID。 此选项仅在&#x200B;*AdFixus ID*&#x200B;上切换&#x200B;**[!UICONTROL 后]**&#x200B;可用。 在&#x200B;**[!UICONTROL 帐户ID]**&#x200B;字段中输入您的AdFixus ID，并确保仔细检查该值是否准确。

![已打开AdFixus ID的“匹配密钥”对话框，并突出显示了“帐户凭据”部分。](/help/assets/setup/manage-account/adfixus-settings.png){zoomable="yes"}

选择所有所需的匹配键后，选择&#x200B;**[!UICONTROL 完成]**&#x200B;以完成帐户设置工作流。

![显示了“设置帐户工作区”的“匹配键”部分。](/help/assets/setup/manage-account/add-account-match-keys.png){zoomable="yes"}

## 编辑帐户 {#edit-account}

设置帐户后，您可以随时编辑详细信息和匹配密钥。

### 编辑详细信息 {#edit-details}

您可以随时编辑帐户的大多数详细信息，但&#x200B;**[!UICONTROL 角色]**&#x200B;除外。 地区是根据您的Adobe Experience Cloud帐户自动设置的，无法更改。

要编辑您的帐户，请在&#x200B;**[!UICONTROL 设置]**&#x200B;工作区的&#x200B;**[!UICONTROL 我的帐户]**&#x200B;部分中选择&#x200B;**[!UICONTROL 编辑]**。

![突出显示了“我的帐户”选项卡和“编辑”选项的“设置”工作区。](/help/assets/setup/manage-account/edit-account.png){zoomable="yes"}

您现在可以编辑帐户详细信息。 更新您要更改的任何字段，然后选择&#x200B;**[!UICONTROL 保存]**&#x200B;以确认更改。

![编辑帐户详细信息对话框。](/help/assets/setup/manage-account/editable-options.png){zoomable="yes"}

### 编辑匹配键 {#edit-match-keys}

>[!IMPORTANT]
>
>编辑匹配键不会影响现有连接。 建立连接后，在连接设置期间选择的匹配键将被固定。 在帐户设置过程中，选择您计划在未来营销活动中使用的&#x200B;**所有**&#x200B;匹配键，这一点很重要。

您还可以更新在创建帐户时最初选择的匹配键。 这些匹配键将确定可用于将来连接的匹配键。

在&#x200B;**[!UICONTROL 匹配键]**&#x200B;部分中选择&#x200B;**[!UICONTROL 编辑]**。

![在帐户的“匹配密钥”部分中，突出显示具有“编辑”选项的“设置”工作区。](/help/assets/setup/manage-account/edit-match-keys.png){zoomable="yes"}

出现&#x200B;**[!UICONTROL 匹配键]**&#x200B;对话框。 打开和关闭任何匹配的密钥，或者更新&#x200B;**[!UICONTROL AdFixus ID]**&#x200B;的[!UICONTROL 帐户ID]，然后选择&#x200B;**[!UICONTROL 保存]**&#x200B;以确认更改。

>[!IMPORTANT]
>
>更改您的[!UICONTROL AdFixus ID]不会使用匹配键触发现有数据连接的[数据草图](../glossary.md#sketches)刷新。 草图数据后，对您的[!UICONTROL AdFixus ID]所做的任何更改都不会反映在下一个受众刷新之前，该刷新操作将遵循[数据连接计划](./manage-data-connection.md#scheduling)设置。 如果在下次刷新之前需要进行更改，可以删除并重新创建数据连接。

![突出显示了“保存”选项的“匹配键”对话框。](/help/assets/setup/manage-account/match-key-dialog.png){zoomable="yes"}

## 后续步骤

设置帐户后，您便可以[将受众](/help/guide/setup/onboard-audiences.md)源到Real-Time CDP Collaboration中。
