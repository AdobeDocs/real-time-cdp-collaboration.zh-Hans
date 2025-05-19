---
title: 载入和管理组织
description: 了解如何在Real-Time CDP Collaboration中载入和管理组织的各个方面
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/cn/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: a95e932a-9681-48f2-bf34-6fe5a50597d7
source-git-commit: 12e73a9bf64f5746748d1a8c81827c50000a6428
workflow-type: tm+mt
source-wordcount: '842'
ht-degree: 19%

---

# 载入和管理组织

{{limited-availability-release-note}}

了解如何将您的组织载入Real-Time CDP Collaboration并管理公司的各个方面。 本页概述了将组织载入Adobe Real-Time CDP Collaboration的步骤，包括设置匹配键、首选身份和更多选项。

![设置页面](/help/assets/setup/manage-organization/my-organization.png){zoomable="yes"}

## 初始组织设置

您必须首先设置组织和组织详细信息。 导航到左边栏中的&#x200B;**[!UICONTROL 设置]**，选择右上角的&#x200B;**+**&#x200B;符号，然后选择&#x200B;**[!UICONTROL 帐户]**。

>[!TIP]
>
>设置要使用的初始帐户后，您可以使用同一工作流在同一组织内设置其他帐户。

![选择帐户以向Real-Time CDP Collaboration添加新组织](/help/assets/setup/manage-organization/add-new-account.png){zoomable="yes"}

设置组织的工作流包括以下两个页面：

* [设置详细信息](#set-up-details)
* [设置匹配键](#set-up-match-keys)

>[!IMPORTANT]
>
>在广告商和发布商之间的协作中，您在组织级别选择的任何&#x200B;*匹配键*&#x200B;都将向下渗透到[项目级别](/help/guide/collaborate/manage-projects.md)。 在项目级别，您可以删除任何匹配的键，但您&#x200B;*无法*&#x200B;添加此屏幕中组织级别未选择的任何其他键。

### 设置详细信息 {#set-up-details}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_setup_contact_email"
>title="联系电子邮件"
>abstract="请提供一个基于团队或角色的电子邮件地址，例如 `collaboration@yourcompany.com`。不应使用私人或个人的电子邮件地址。"

![设置组织的详细信息和用例步骤](/help/assets/setup/manage-organization/add-organization-details.png){zoomable="yes"}

1. 为您的公司添加&#x200B;**[!UICONTROL 组织名称]**。
2. 添加有关您公司的&#x200B;**[!UICONTROL 描述]**。
3. 选择您的&#x200B;**[!UICONTROL 公司角色]**。 您可以选择介于&#x200B;**[!UICONTROL 广告商]**&#x200B;和&#x200B;**[!UICONTROL 发布者]**&#x200B;之间。 请阅读[端到端工作流文档](/help/guide/end-to-end-workflow.md)以了解两种组织角色类型之间工作流的相似之处和细微差异。
4. 为您的组织选择&#x200B;**[!UICONTROL 行业]**。 某些示例包括&#x200B;**[!UICONTROL 零售业]**、**[!UICONTROL 电信]**&#x200B;或&#x200B;**[!UICONTROL 金融服务]**。
5. 为您的组织选择&#x200B;**[!UICONTROL 区域]**。 在产品的当前版本中，**[!UICONTROL 北美洲]**&#x200B;是预设的默认选择。
6. 为您的组织添加&#x200B;**[!UICONTROL 联系人电子邮件]**。 这应该是基于团队或角色的电子邮件地址。 不应提供个人电子邮件地址。
7. 为您的公司上传&#x200B;**[!UICONTROL 徽标]**。 目前，支持SVG类型的图像。
8. 选择公司标题图片的图像。

对您的选择感到满意后，使用&#x200B;**[!UICONTROL 下一步]**&#x200B;进入下一页，并选择贵组织应使用的所需匹配键。

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

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_activation_matchkeys"
>title="激活匹配键"
>abstract="根据您组织选择的匹配键显示激活匹配键。"

匹配键（如电子邮件地址、设备ID或客户ID）通过实现准确且以隐私为中心的数据同步，帮助广告商和出版商开展合作，从而实现更准确的受众定位和测量。

![幻灯片显示Real-Time CDP Collaboration第一版本的可用标识符。](/help/assets/setup/manage-organization/available-identifiers.png)

选择在协调发布者和广告商受众的成员时要使用的任何匹配键。 包括您的公司可以使用的任何匹配键。 规划未来并选择您预计将在未来的发布者 — 广告商营销活动中使用的匹配键。 如果您确实需要为您的组织选择其他匹配键，则以后还可以在[编辑组织](#edit-organization)工作流中执行该操作。

![匹配键选择步骤。](/help/assets/setup/manage-organization/add-organization-match-keys.png){zoomable="yes"}

最多选择五个您计划使用的匹配键。 稍后，在设置连接时，您可以删除不需要的匹配键，但无法添加新匹配键。

Real-Time CDP Collaboration中可用的匹配键可以是三种类型：

* 第一方人员 ID
* 第一方设备 ID
* 合作伙伴 ID

Real-Time CDP Collaboration第一个版本的可用匹配键包括：

* 哈希电子邮件

<!--

not available in the Limited GA release

* Hashed phone
* IPv4

-->

准备就绪后，选择&#x200B;**[!UICONTROL 完成]**&#x200B;以完成组织设置工作流。

## 编辑组织 {#edit-organization}

最初设置组织后，您可以随时编辑组织的某些方面和详细信息。 要编辑您的组织，请在&#x200B;**[!UICONTROL 我的组织]**&#x200B;视图中选择&#x200B;**[!UICONTROL 编辑]**。

![已突出显示编辑组织控件。](/help/assets/setup/manage-organization/edit-organization.png){zoomable="yes"}

此时，您可以更新组织名称、描述、徽标和组织配置文件图片。

![组织的可编辑选项。](/help/assets/setup/manage-organization/editable-options.png){zoomable="yes"}

您还可以更新在加入组织时最初选择的匹配键，以及与匹配键对应的身份的最低阈值，以在受众重叠和其他产品区域可见和可用。 在&#x200B;**[!UICONTROL 匹配键]**&#x200B;选项卡中选择&#x200B;**[!UICONTROL 编辑]**&#x200B;以添加任何其他所需的匹配键或更新身份阈值。

![编辑匹配键](/help/assets/setup/manage-organization/edit-match-keys.png){zoomable="yes"}

## 后续步骤

设置组织后，您便可以[将受众](/help/guide/setup/onboard-audiences.md)导入Real-Time CDP Collaboration。
