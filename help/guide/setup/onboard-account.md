---
title: 配置和管理您的帐户
description: 了解如何在Real-Time CDP Collaboration中配置和管理帐户的各个方面
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: a95e932a-9681-48f2-bf34-6fe5a50597d7
source-git-commit: 608706d00124372ac59209478ab551a3a6ce0226
workflow-type: tm+mt
source-wordcount: '937'
ht-degree: 13%

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
>abstract="请提供基于团队或角色的电子邮件，如&#x200B;**collaboration@yourcompany.com**。 不应使用私人或个人的电子邮件地址。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_setup_connect_code"
>title="连接代码"
>abstract="连接代码是您帐户的唯一标识符。 它用于与Real-Time CDP Collaboration中的其他协作者建立连接。"

<!-- Move the above popover to new section for invite on this page when its created -->

要开始配置帐户，必须首先设置帐户详细信息。 这要求您添加以下信息：

* 添加明确代表您品牌的&#x200B;**[!UICONTROL 帐户名称]**。
* 添加有关您品牌的&#x200B;**[!UICONTROL 描述]**。 虽然这是一项可选操作，但它有助于其他协作者更好地了解您的品牌。
* 选择您的&#x200B;**[!UICONTROL 角色]**。 您可以选择介于&#x200B;**[!UICONTROL 广告商]**&#x200B;和&#x200B;**[!UICONTROL 发布者]**&#x200B;之间。 请阅读[端到端工作流文档](/help/guide/end-to-end-workflow.md)以了解两种组织角色类型之间工作流的相似之处和细微差异。
<!-- The above will need to be updated when I update things for B2B -->
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
>abstract="匹配键是用于协调来自不同数据源的受众成员的标识符。包含您的品牌可以使用的任何匹配键。"

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
>您在帐户设置期间选择的匹配键将决定您与其他协作者创建的连接的可用匹配键。 虽然可以在连接设置期间删除匹配键，但无法添加新的匹配键。 选择您计划在帐户设置期间在未来的营销活动中使用的&#x200B;**所有**&#x200B;匹配键很重要。

匹配键（如电子邮件地址、设备ID或客户ID）通过实现准确且以隐私为中心的数据同步，帮助协作者进行合作，从而实现更准确的受众定位和测量。

![幻灯片显示Collaboration第一版本的可用标识符。](/help/assets/setup/manage-account/available-identifiers.png)

<!-- Eventually replace this image above to match branding better. -->

选择要在协调受众配置文件时使用的任何匹配键。 包括您可以使用的任何匹配键。 规划未来并选择您预计将在未来营销活动中使用的匹配键。 如果以后确实需要为您的帐户选择其他匹配密钥，则可以在[编辑帐户](#edit-account)工作流中执行此操作。

最多选择五个您计划使用的匹配键。 稍后，在设置连接时，您可以删除不需要的匹配键，但无法添加新匹配键。

可用的匹配键有三种：

* 第一方人员 ID
* 第一方设备 ID
* 合作伙伴 ID

>[!IMPORTANT]
>
>目前，唯一支持的匹配键是哈希电子邮件。

准备就绪后，选择&#x200B;**[!UICONTROL 完成]**&#x200B;以完成组织设置工作流。

![显示“设置组织”工作区的“匹配键”部分。](/help/assets/setup/manage-account/add-account-match-keys.png){zoomable="yes"}

## 编辑帐户 {#edit-account}

设置帐户后，您可以随时编辑帐户的某些方面和详细信息。 要编辑您的帐户，请在&#x200B;**[!UICONTROL 设置]**&#x200B;工作区&#x200B;**[!UICONTROL 的]**&#x200B;我的帐户&#x200B;**[!UICONTROL 部分中选择]编辑**。

![突出显示了“我的帐户”选项卡和“编辑”选项的“设置”工作区。](/help/assets/setup/manage-account/edit-account.png){zoomable="yes"}

您现在可以编辑帐户详细信息，但&#x200B;**[!UICONTROL 角色]**&#x200B;除外。 请注意，区域是根据您的Adobe Experience Cloud帐户自动设置的，无法随时更改。

![编辑帐户详细信息对话框。](/help/assets/setup/manage-account/editable-options.png){zoomable="yes"}

您还可以更新在加入组织时最初选择的匹配密钥。 在&#x200B;**[!UICONTROL 匹配键]**&#x200B;部分中选择&#x200B;**[!UICONTROL 编辑]**&#x200B;以添加任何其他所需的匹配键。

![在帐户的“匹配密钥”部分中，突出显示具有“编辑”选项的“设置”工作区。](/help/assets/setup/manage-account/edit-match-keys.png){zoomable="yes"}

## 后续步骤

设置帐户后，您便可以[将受众](/help/guide/setup/onboard-audiences.md)源到Real-Time CDP Collaboration中。
