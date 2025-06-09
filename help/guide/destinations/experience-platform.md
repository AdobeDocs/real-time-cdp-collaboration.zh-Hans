---
title: 将Adobe Experience Platform配置为目标
description: 了解如何在Real-Time CDP Collaboration中配置和管理Adobe Experience Platform作为目标。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
source-git-commit: f19aff1b7d10a446dd209721e7a6fdf537c9d63e
workflow-type: tm+mt
source-wordcount: '766'
ht-degree: 1%

---

# 将Adobe Experience Platform配置为目标

{{limited-availability-release-note}}

配置此目标以将受众从您的项目激活到Adobe Experience Platform。 在Adobe Experience Platform中激活受众可让您利用该平台的功能在各种营销渠道中进行受众分段、分析和激活。 要了解有关Adobe Experience Platform的更多信息，请参阅[Experience Platform概述](https://experienceleague.adobe.com/en/docs/experience-platform/landing/home){target="_blank"}。

>[!NOTE]
>
>目前，只有发布者才能在Real-Time CDP Collaboration中配置目标。

## 配置目标 {#configure-destination}

要将Adobe Experience Platform配置为目标，请导航到&#x200B;**[!UICONTROL 设置]**，然后选择&#x200B;**[!UICONTROL 目标]**&#x200B;选项卡。 为Adobe Experience Platform选择&#x200B;**[!UICONTROL 设置]**。

![为Adobe Experience Platform目标突出显示具有“设置”选项的“我的目标”工作区。](/help/assets/destinations/adobe-experience-platform/setup-aep.png)

出现&#x200B;**[!UICONTROL 创建目标]**&#x200B;工作流。

![Adobe Experience Platform的“创建目标”工作流。](/help/assets/destinations/adobe-experience-platform/create-destination.png)

### 配置沙盒 {#configure-sandbox}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_audience_expiration"
>title="受众过期"
>abstract="受众在Adobe Experience Platform中将不再可用的时段。 默认到期时间为30天，但您可以将其设置为1到30天之间的任何值。"

首先，您必须选择将发送受众数据的沙盒。

>
>
>您只能选择用户有权访问的沙盒。 默认情况下，所有Real-Time CDP Collaboration用户都有权访问&#x200B;**Prod**&#x200B;沙盒。 要获得对其他沙盒的访问权限，管理员必须将其他沙盒添加到分配给用户的角色。 有关管理角色的更多信息，请参阅[管理角色](../permissions/manage-roles.md)指南。

在&#x200B;**[!UICONTROL 配置沙盒]**&#x200B;部分中，选择&#x200B;**[!UICONTROL 沙盒]**&#x200B;下拉列表，或键入沙盒的名称。

![在创建目标工作流中突出显示的沙盒下拉列表。](/help/assets/destinations/adobe-experience-platform/select-sandbox.png)

或者，您可以选择&#x200B;**[!UICONTROL 浏览沙盒]**&#x200B;以查看所有可用的沙盒以及它们的&#x200B;**[!UICONTROL 类型]**、**[!UICONTROL 状态]**&#x200B;和&#x200B;**[!UICONTROL 区域]**。 选择要使用的沙盒，然后选择&#x200B;**[!UICONTROL 保存]**。

接下来，配置&#x200B;**[!UICONTROL 受众过期]**。 默认情况下，受众过期时间设置为30天。 您可以选择将过期时间设置为1到30天。 过期日期后，该受众将无法在Adobe Experience Platform中使用。

![创建目标工作流中突出显示的受众过期部分。](/help/assets/destinations/adobe-experience-platform/audience-expiration.png)

### 创建激活映射 {#create-activation-mapping}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_activation_matchkeys"
>title="激活匹配键"
>abstract="激活匹配密钥根据您在创建组织时选择的匹配密钥显示。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_target_namespaces"
>title="Target 命名空间"
>abstract="Target命名空间指定匹配键将在Adobe Experience Platform中映射到的身份命名空间。 哈希匹配键必须映射到支持哈希值的目标命名空间。"

接下来，您必须创建一个激活映射来定义将受众数据发送到Adobe Experience Platform的方式。 您可以将创建组织时选择的每个[匹配键](../setup/onboard-organization.md#set-up-match-keys)映射到目标命名空间。 目标命名空间指定匹配键将在Adobe Experience Platform中映射到哪个[身份命名空间](https://experienceleague.adobe.com/en/docs/experience-platform/identity/features/namespaces#standard){target="_blank"}。

>
>
>哈希匹配键必须映射到支持哈希值的目标命名空间。 例如，**[!UICONTROL 哈希电子邮件]**&#x200B;匹配键必须映射到Adobe Experience Platform中的&#x200B;**[!UICONTROL Email（SHA256，小写）]**&#x200B;身份命名空间。 您无法将&#x200B;**[!UICONTROL 哈希电子邮件]**&#x200B;匹配键映射到&#x200B;**[!UICONTROL 电子邮件]**&#x200B;身份命名空间，因为此命名空间不支持哈希值。

选择每个匹配键旁边的&#x200B;**[!UICONTROL 目标命名空间]**&#x200B;字段。 出现&#x200B;**[!UICONTROL 选择源字段]**&#x200B;对话框。 在列表中查找目标命名空间，或搜索特定命名空间。 选择要用于匹配键的目标命名空间，然后选择&#x200B;**[!UICONTROL 选择]**。

![突出显示了“选择”选项的“选择源字段”对话框……](/help/assets/destinations/adobe-experience-platform/select-target-namespace.png)

完成映射所有匹配键后，请检查设置，然后选择&#x200B;**[!UICONTROL 创建]**&#x200B;以完成创建目标。

## 使用Adobe Experience Platform作为目标

将Adobe Experience Platform配置为目标后，即可开始[通过项目将受众](../collaborate/activate.md)激活到平台。 目前，激活过程是由广告商启动的单步流程。 当广告商激活受众时，该受众将发送到发布者的预配置目标(在本例中为Adobe Experience Platform)。 发布者无需执行任何其他步骤即可将受众发送到目标。

>[!IMPORTANT]
>
>您&#x200B;**必须**&#x200B;将Adobe Experience Platform配置为目标&#x200B;*，然后*&#x200B;您的协作者才能激活受众。 如果未配置目标，则将会向您发送该受众，并在项目的&#x200B;**[!UICONTROL 激活]**&#x200B;选项卡中显示，但不会激活到Adobe Experience Platform。

在激活受众后，该受众将在Experience Platform的[受众门户](#audience-portal)中可用，其来源为Real-Time CDP Collaboration。  这些受众随后可用于营销活动和客户参与。

### 受众门户 {#audience-portal}
