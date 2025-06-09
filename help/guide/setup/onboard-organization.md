---
title: 载入和管理组织
description: 了解如何在Real-Time CDP Collaboration中载入和管理组织的各个方面
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: a95e932a-9681-48f2-bf34-6fe5a50597d7
source-git-commit: fda414120decc0c76712616ff85b83febede53e9
workflow-type: tm+mt
source-wordcount: '861'
ht-degree: 16%

---

# 载入并管理您的组织

{{limited-availability-release-note}}

了解如何将您的组织载入Real-Time CDP Collaboration并管理公司的各个方面。 本页概述了将组织载入Adobe Real-Time CDP Collaboration的步骤，包括设置匹配键、首选身份和更多选项。

![组织的设置工作区显示其当前设置。](/help/assets/setup/manage-organization/my-organization.png){zoomable="yes"}

## 初始组织设置

您必须首先设置组织和组织详细信息。 如果这是您的第一个组织，则会立即引导您完成入门流程，从设置您的[帐户详细信息](#set-up-details)开始。

要添加其他组织，请导航到左边栏中的&#x200B;**[!UICONTROL 设置]**，然后选择添加图标（![添加图标）。](/help/assets/icons/plus.png))。 接下来，选择&#x200B;**[!UICONTROL 帐户]**。

![突出显示“帐户”选项的设置工作区。](/help/assets/setup/manage-organization/add-new-account.png){zoomable="yes"}

### 设置详细信息 {#set-up-details}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_setup_contact_email"
>title="联系电子邮件"
>abstract="请提供一个基于团队或角色的电子邮件地址，例如 `collaboration@yourcompany.com`。不应使用私人或个人的电子邮件地址。"

要开始载入您的组织，您必须首先设置组织详细信息。 这要求您添加以下信息：

* 为您的公司添加&#x200B;**[!UICONTROL 组织名称]**。
* 添加有关您公司的&#x200B;**[!UICONTROL 描述]**。
* 选择您的&#x200B;**[!UICONTROL 公司角色]**。 您可以选择介于&#x200B;**[!UICONTROL 广告商]**&#x200B;和&#x200B;**[!UICONTROL 发布者]**&#x200B;之间。 请阅读[端到端工作流文档](/help/guide/end-to-end-workflow.md)以了解两种组织角色类型之间工作流的相似之处和细微差异。
* 为您的组织选择&#x200B;**[!UICONTROL 行业]**。 某些示例包括&#x200B;**[!UICONTROL 零售业]**、**[!UICONTROL 电信]**&#x200B;或&#x200B;**[!UICONTROL 金融服务]**。
* 为您的组织选择&#x200B;**[!UICONTROL 区域]**。 在产品的当前版本中，**[!UICONTROL 北美洲]**&#x200B;是预设的默认选择。
* 为您的组织添加&#x200B;**[!UICONTROL 联系人电子邮件]**。 这应该是基于团队或角色的电子邮件地址。 不应提供个人电子邮件地址。
* 为您的公司上传&#x200B;**[!UICONTROL 徽标]**。 目前，支持SVG类型的图像。
* 选择公司标题图片的图像。

>[!NOTE]
>
>虽然您可以随时编辑这些详细信息中的大部分内容，但在初始设置后，**[!UICONTROL 角色]**&#x200B;和&#x200B;**[!UICONTROL 区域]**&#x200B;不可编辑。

![显示了“详细信息”部分的“设置组织”工作区。](/help/assets/setup/manage-organization/add-organization-details.png){zoomable="yes"}

完成后，使用&#x200B;**[!UICONTROL 下一步]**&#x200B;进入下一页，选择贵组织将使用的所需匹配密钥。

### 设置匹配键 {#set-up-match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_matchkeys"
>title="匹配键"
>abstract="匹配键是用于协调来自不同数据源的受众成员的标识符。包括您的公司可以使用的任何匹配键。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_peopleIDs"
>title="第一方人员 ID"
>abstract="第一方人员 ID（例如经过哈希处理的电子邮件地址或电话号码）直接与个人轮廓相关联。目前支持的 ID 是经过哈希处理的电子邮件和电话号码。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_deviceIDs"
>title="第一方设备 ID"
>abstract="第一方设备 ID（例如 ECID 或 IP 地址）直接与设备相关联，这些设备可以由多个人共享。IPv4 是目前唯一受支持的第一方设备 ID。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_partnerIDs"
>title="支持的合作伙伴 ID"
>abstract="与轮廓关联的合作伙伴 ID 可扩大对特定轮廓的覆盖范围。"

>[!IMPORTANT]
>
>您在组织设置期间选择的匹配键将确定您与其他组织创建的连接的可用匹配键。 虽然可以在连接设置期间删除匹配键，但以后无法添加新的匹配键。 在组织设置期间，请务必选择您计划在未来营销活动中使用的所有匹配键。

匹配键（如电子邮件地址、设备ID或客户ID）通过实现准确且以隐私为中心的数据同步，帮助广告商和出版商开展合作，从而实现更准确的受众定位和测量。

![幻灯片显示Real-Time CDP Collaboration第一版本的可用标识符。](/help/assets/setup/manage-organization/available-identifiers.png)

选择在协调发布者和广告商受众的成员时要使用的任何匹配键。 包括您的公司可以使用的任何匹配键。 规划未来并选择您预计将在未来的发布者 — 广告商营销活动中使用的匹配键。 如果您确实需要为您的组织选择其他匹配键，则以后还可以在[编辑组织](#edit-organization)工作流中执行该操作。

![显示“设置组织”工作区的“匹配键”部分。](/help/assets/setup/manage-organization/add-organization-match-keys.png){zoomable="yes"}

最多选择五个您计划使用的匹配键。 稍后，在设置连接时，您可以删除不需要的匹配键，但无法添加新匹配键。

Real-Time CDP Collaboration中可用的匹配键可以是三种类型：

* 第一方人员 ID
* 第一方设备 ID
* 合作伙伴 ID

Real-Time CDP Collaboration第一个版本的可用匹配键包括：

* 哈希电子邮件

准备就绪后，选择&#x200B;**[!UICONTROL 完成]**&#x200B;以完成组织设置工作流。

## 编辑组织 {#edit-organization}

最初设置组织后，您可以随时编辑组织的某些方面和详细信息。 要编辑您的组织，请在&#x200B;**[!UICONTROL 设置]工作区**&#x200B;的&#x200B;**[!UICONTROL 我的组织]**&#x200B;部分中选择&#x200B;**[!UICONTROL 编辑]**。

![突出显示了“我的组织”选项卡和“编辑”选项的“设置”工作区。](/help/assets/setup/manage-organization/edit-organization.png){zoomable="yes"}

您现在可以编辑组织详细信息，但&#x200B;**[!UICONTROL 角色]**&#x200B;和&#x200B;**[!UICONTROL 区域]**&#x200B;除外。

![编辑组织详细信息对话框。](/help/assets/setup/manage-organization/editable-options.png){zoomable="yes"}

您还可以更新在加入组织时最初选择的匹配密钥。 在&#x200B;**[!UICONTROL 匹配键]**&#x200B;部分中选择&#x200B;**[!UICONTROL 编辑]**&#x200B;以添加任何其他所需的匹配键。

![在组织的“匹配键”部分中，突出显示具有“编辑”选项的“设置”工作区。](/help/assets/setup/manage-organization/edit-match-keys.png){zoomable="yes"}

## 后续步骤

设置组织后，您便可以[将受众](/help/guide/setup/onboard-audiences.md)导入Real-Time CDP Collaboration。
