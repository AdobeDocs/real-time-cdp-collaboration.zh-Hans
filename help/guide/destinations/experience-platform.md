---
title: 将Adobe Experience Platform配置为目标
description: 了解如何在Real-Time CDP Collaboration中配置和管理Adobe Experience Platform作为目标。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 594610a0-9102-448a-b59b-ec162ef9dd57
source-git-commit: 6acf936f50b412147578a70e2369b06c53260f06
workflow-type: tm+mt
source-wordcount: '1487'
ht-degree: 11%

---

# 将Adobe Experience Platform配置为目标

{{limited-availability-release-note}}

配置此目标以将受众从您的项目激活到Adobe Experience Platform。 在Adobe Experience Platform中激活受众可让您利用该平台的功能在各种营销渠道中进行受众分段、分析和激活。 要了解有关Adobe Experience Platform的更多信息，请参阅[Experience Platform概述](https://experienceleague.adobe.com/en/docs/experience-platform/landing/home){target="_blank"}。

>[!WARNING]
>
>创建目标后，无法更新该目标。 如果需要更改任何设置，则必须删除现有目标并创建新目标。

## 配置目标 {#configure-destination}

要将Adobe Experience Platform配置为目标，请导航到&#x200B;**[!UICONTROL 设置]**，然后选择&#x200B;**[!UICONTROL 我的目标]**&#x200B;选项卡。 为Adobe Experience Platform选择&#x200B;**[!UICONTROL 设置]**。

![为Adobe Experience Platform目标突出显示具有“设置”选项的“我的目标”工作区。](/help/assets/destinations/adobe-experience-platform/setup-aep.png)

出现&#x200B;**[!UICONTROL 创建目标]**&#x200B;工作流。

![Adobe Experience Platform的“创建目标”工作流。](/help/assets/destinations/adobe-experience-platform/create-destination.png)

### 配置沙盒 {#configure-sandbox}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_audience_expiration"
>title="受众过期"
>abstract="受众在 Adobe Experience Platform 中不再可用的时间期限。默认过期时间为 30 天，但您可以将其设置为 1 至 30 天之间的任意值。"

首先，您必须选择将发送受众数据的沙盒。

>[!IMPORTANT]
>
>您只能选择用户有权访问的沙盒。 默认情况下，所有Collaboration用户都有权访问&#x200B;**Prod**&#x200B;沙盒。 要获得对其他沙盒的访问权限，管理员必须将其他沙盒添加到分配给用户的角色。 有关管理角色的更多信息，请参阅[管理角色](../permissions/manage-roles.md)指南。

在&#x200B;**[!UICONTROL 配置沙盒]**&#x200B;部分中，选择&#x200B;**[!UICONTROL 沙盒]**&#x200B;下拉列表，或键入沙盒的名称。

![在创建目标工作流中突出显示的沙盒下拉列表。](/help/assets/destinations/adobe-experience-platform/select-sandbox.png)

或者，您可以选择&#x200B;**[!UICONTROL 浏览沙盒]**&#x200B;以查看所有可用的沙盒以及它们的&#x200B;**[!UICONTROL 类型]**、**[!UICONTROL 状态]**&#x200B;和&#x200B;**[!UICONTROL 区域]**。 选择要使用的沙盒，然后选择&#x200B;**[!UICONTROL 保存]**。

接下来，配置&#x200B;**[!UICONTROL 受众过期]**。 默认情况下，受众过期时间设置为30天。 您可以选择将过期时间设置为1到30天。 过期日期后，该受众将无法在Adobe Experience Platform中使用。

![创建目标工作流中突出显示的受众过期部分。](/help/assets/destinations/adobe-experience-platform/audience-expiration.png)

### 创建激活映射 {#create-activation-mapping}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_activation_matchkeys"
>title="激活匹配键"
>abstract="激活匹配键会根据您在创建组织时所选择的匹配键进行显示。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_target_namespaces"
>title="目标命名空间"
>abstract="目标命名空间用于指定匹配键在 Adobe Experience Platform 中将映射到的身份标识命名空间。经过哈希处理的匹配键必须映射到支持哈希值的目标命名空间。"

默认情况下，为您的帐户启用的所有匹配密钥都包含在激活映射中。 如果不希望将匹配键直接映射到目标命名空间，则可以使用链接键选项将其替换为其他匹配键。 有关链接键的更多信息，请参阅下面的[部分](#linked-keys)。

#### 映射目标命名空间 {#map-target-namespaces}

要将每个匹配键映射到目标命名空间，请选择匹配键旁边的&#x200B;**[!UICONTROL 目标命名空间]**&#x200B;字段。 出现&#x200B;**[!UICONTROL 选择源字段]**&#x200B;对话框。 在列表中查找目标命名空间，或搜索特定命名空间。 选择要用于匹配键的目标命名空间，然后选择&#x200B;**[!UICONTROL 选择]**。

>[!IMPORTANT]
>
>哈希匹配键必须映射到支持哈希值的目标命名空间。 例如，**[!UICONTROL 哈希电子邮件]**&#x200B;匹配键必须映射到Adobe Experience Platform中的&#x200B;**[!UICONTROL Email（SHA256，小写）]**&#x200B;身份命名空间。 您无法将&#x200B;**[!UICONTROL 哈希电子邮件]**&#x200B;匹配键映射到&#x200B;**[!UICONTROL 电子邮件]**&#x200B;身份命名空间，因为此命名空间不支持哈希值。

![突出显示了“选择”选项的“选择源字段”对话框……](/help/assets/destinations/adobe-experience-platform/select-target-namespace.png)

对要包含在激活映射中的每个匹配键重复此过程。 如果您不想包含匹配键，则可以将其删除，或者使用链接键选项将其替换为其他匹配键。

#### 关联的键 {#linked-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_linked_key"
>title="关联的键"
>abstract="关联的键允许您指定在激活期间使用不同的匹配键取代原始匹配键。要激活一个轮廓，它必须同时具有原始匹配键和关联匹配键的两个值。"

关联的键允许您指定在激活期间使用不同的匹配键取代原始匹配键。要更好地了解链接键的工作方式，请考虑以下示例：

retailer希望将激活到Experience Platform的数据发送到其CRM系统。 retailer启用了将IP作为匹配键的哈希，以便其帐户在激活受众时提高匹配率。 但是，retailer的CRM系统不支持将哈希IP作为身份命名空间，因此他们希望在将受众激活到Experience Platform时改用CRM ID匹配键。 retailer可以使用链接键选项，通过CRM ID而不是哈希IP将受众激活到Experience Platform。

>[!NOTE]
>
>对于要激活的配置文件，它必须具有原始匹配键和链接的匹配键的值。 例如，如果哈希ID链接到CRM ID，则配置文件必须具有哈希ID和CRM ID的值才能激活。 如果缺少任一值，则不会激活配置文件。

若要使用链接键，请打开要在其位置使用的匹配键旁边的&#x200B;**[!UICONTROL 链接键]**&#x200B;选项。 出现&#x200B;**[!UICONTROL 链接键]**&#x200B;部分，要求您创建映射。

![创建目标工作流中突出显示的链接键选项和部分。](/help/assets/destinations/adobe-experience-platform/linked-key.png)

从下拉菜单中选择要使用的&#x200B;**[!UICONTROL 链接键]**。 按照上述示例，retailer将选择&#x200B;**[!UICONTROL CRM ID]**&#x200B;作为链接键。

![在创建目标工作流中突出显示的链接键下拉列表。](/help/assets/destinations/adobe-experience-platform/select-linked-key.png)

接下来，要为链接键指定目标命名空间（如果尚未指定）。 如果您已在&#x200B;**[!UICONTROL 创建激活映射]**&#x200B;部分中选择了匹配密钥的目标命名空间，则将自动填充该命名空间。 如果您尚未为链接键选择目标命名空间，现在可以这样做。

选择链接键旁边的&#x200B;**[!UICONTROL 目标命名空间]**&#x200B;字段。 出现&#x200B;**[!UICONTROL 选择源字段]**&#x200B;对话框。 在列表中查找目标命名空间，或搜索特定命名空间。 选择要用于链接键的目标命名空间，然后选择&#x200B;**[!UICONTROL 选择]**。

![选择源字段对话框。](/help/assets/destinations/adobe-experience-platform/select-linked-key-target-namespace.png)

现已配置链接密钥。

>[!NOTE]
>
>每个激活映射只能使用一个链接密钥目标命名空间。 例如，如果您将哈希ID链接到CRM ID，则切换其他字段的链接键选项也会将其链接到CRM ID。

完成所有匹配键的映射后，请查看设置。 **[!UICONTROL 预览]**&#x200B;部分提供了配置摘要。

![创建目标工作流中的“预览”部分。](/help/assets/destinations/adobe-experience-platform/preview.png)

>[!IMPORTANT]
>
>目前，每个匹配键都会作为单独的受众激活到Experience Platform。 例如，如果您将[!UICONTROL 哈希电子邮件]和[!UICONTROL 哈希电话]作为匹配键，则激活受众后，将在Audience Portal中创建两个单独的受众。

如果对配置满意，请选择&#x200B;**[!UICONTROL 创建目标]**。 将显示一条确认消息，指示已成功创建目标。

## 使用Adobe Experience Platform作为目标

将Experience Platform配置为目标后，即可开始[通过项目将受众](../collaborate/activate.md)激活到平台。 目前，激活过程是由协作者启动的单步流程。 例如，当广告商激活受众时，该受众将发送到发布者的预配置目标(Experience Platform)。 发布者无需执行任何其他步骤即可将受众发送到目标。 品牌到品牌的协作模式也是如此。

>[!IMPORTANT]
>
>您&#x200B;**必须**&#x200B;将Experience Platform配置为目标&#x200B;*，然后*&#x200B;您的协作者才能激活受众。 如果未配置目标，则将会向您发送该受众，并在项目的&#x200B;**[!UICONTROL 激活]**&#x200B;选项卡中显示，但不会激活到Experience Platform。

在激活受众后，该受众将在Experience Platform的[受众门户](#audience-portal)中可用，其来源为Real-Time CDP Collaboration。  这些受众随后可用于营销活动和客户参与。

### 受众门户 {#audience-portal}

现在，您已将Adobe Experience Platform配置为目标，接下来可以在受众门户中查看激活的受众。 Audience Portal是Adobe Experience Platform中的一个中心枢纽，您可以通过该中心查看和管理受众。 现在，Audience Portal在筛选受众时将Real-Time CDP Collaboration作为源提供。

>[!IMPORTANT]
>
>您负责将任何必要的数据使用标签应用于您激活到Adobe Experience Platform的受众。 有关详细信息，请参阅[数据使用标签](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/data-governance/labels/overview){target="_blank"}指南。

![筛选选项中将Real-Time CDP Collaboration作为源的受众门户。](/help/assets/destinations/adobe-experience-platform/audience-portal.png)

要了解有关受众门户的更多信息，请参阅[受众门户概述](https://experienceleague.adobe.com/en/docs/experience-platform/segmentation/ui/audience-portal#manage-audiences){target="_blank"}指南。
