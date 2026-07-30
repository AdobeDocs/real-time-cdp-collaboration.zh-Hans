---
title: 配置和管理云存储目标
description: 了解如何在Real-Time CDP Collaboration中配置、查看和删除Cloud Storage目标。
audience: admin, publisher
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
topic_v2:
  - id: b5520579-b31f-4df7-9281-f0d9f91e2edc
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 60124235569ca9b17b3bb1cef502d57d39e82e1f
workflow-type: tm+mt
source-wordcount: 885
ht-degree: 2%

---

# 配置和管理云存储目标

使用本指南可以从&#x200B;**[!UICONTROL 激活]**&#x200B;工作区中配置、查看和删除云存储目标。 使用&#x200B;**[!UICONTROL 目录]**&#x200B;选项卡配置目标，使用&#x200B;**[!UICONTROL 目标]**&#x200B;选项卡管理目标，使用&#x200B;**[!UICONTROL 激活的受众]**&#x200B;选项卡查看激活到目标的受众。

配置目标后，该目标将在激活受众时变得可用。 要查看支持的目标的完整列表，请参阅[可用目标](./overview.md#available-destinations)表。

>[!NOTE]
>
> 本指南以&#x200B;**[!DNL Amazon S3]**&#x200B;目标为例。 引导式配置工作流在支持的云存储目标类型之间共享，但身份验证方法、必填字段和连接器功能可能会有所不同。 在配置目标之前，请查看[云存储目标要求](./cloud-storage-destination-requirements.md)，该要求链接到相应的Adobe Experience Platform目标文档。
>
> Adobe Experience Platform在Real-Time CDP Collaboration中具有单独的配置工作流。 要对其进行配置，请参阅[将Adobe Experience Platform配置为目标](./experience-platform.md)。

## 先决条件 {#prerequisites}

在配置目标之前，请确保：

* 您有权访问&#x200B;**[!UICONTROL 激活]**&#x200B;工作区。
* 您拥有云存储提供商所需的连接信息。
* 如果您需要创建帐户，则您拥有所需的凭据或权限。
* 您已查看云存储目标[&#128279;](./cloud-storage-destination-requirements.md)的要求。

## 配置目标 {#configure-destination}

配置目标时，您需要将云存储帐户连接到Real-Time CDP Collaboration并定义如何将受众数据导出到其中。

导航到&#x200B;**[!UICONTROL 激活]** > **[!UICONTROL 目录]**。

**[!UICONTROL 目录]**&#x200B;选项卡显示可用的目标提供程序。 每个目标都显示为卡片。 根据目标的不同，其信息卡可以显示已配置的帐户和操作以查看其他信息。

![显示目标提供商卡的“目录”选项卡。](/help/assets/destinations/manage-destinations/destination-provider-catalog.png)

找到要配置的目标提供程序，然后选择&#x200B;**[!UICONTROL 设置]**。

目标配置引导式安装程序将打开并指导您完成四个步骤：**[!UICONTROL 身份验证]**、**[!UICONTROL 创建目标]**、**[!UICONTROL 映射字段]**&#x200B;和&#x200B;**[!UICONTROL 审核]**。

### 身份验证 {#authenticate}

**[!UICONTROL 身份验证]**&#x200B;步骤在Real-Time CDP Collaboration与目标帐户之间建立连接。

如果现有帐户可用，请从帐户选择器中选择它。 若要创建帐户，请选择&#x200B;**[!UICONTROL 新建帐户]**。

选择身份验证方法并提供所需的帐户信息。 可用的身份验证方法和字段取决于所选的目标提供程序。 有关连接器特定的要求，请参阅[云存储目标要求](./cloud-storage-destination-requirements.md)。

选择&#x200B;**[!UICONTROL 连接到Amazon S3]**。 对于其他目标提供程序，该按钮显示相应的提供程序名称。

成功验证帐户后，选择&#x200B;**[!UICONTROL 下一步]**。

![身份验证步骤显示帐户选择和新帐户创建。](/help/assets/destinations/manage-destinations/authenticate-destination-account.png)

### 创建目标 {#create-destination}

**[!UICONTROL 创建目标]**&#x200B;步骤定义受众导出文件的交付位置和方式。

输入目标名称，并完成所需的存储和导出设置。 可用字段取决于所选的目标提供商。 有关定义和连接器特定的要求，请参阅从[云存储目标要求](./cloud-storage-destination-requirements.md)链接的目标文档。

完成所有必填字段后，选择&#x200B;**[!UICONTROL 下一步]**。 引导式设置前进到字段映射步骤。

![显示目标配置字段的“创建目标”步骤。](/help/assets/destinations/manage-destinations/configure-new-destination.png)

### 映射字段 {#map-fields}

**[!UICONTROL 映射字段]**&#x200B;步骤定义如何将受众匹配键映射到目标所需的标识字段。

与标准Real-Time CDP目标工作流不同，Real-Time CDP Collaboration在创建目标时配置这些映射。 受众匹配键显示为源字段。 将每个源字段映射到相应的目标标识，以便目标可以识别导出的标识符并将它们与预期用户相关联。

选择&#x200B;**[!UICONTROL 添加字段]**&#x200B;以添加其他匹配键映射，或选择删除图标以删除映射。 查看和配置所有必需的映射。

映射完成后，选择&#x200B;**[!UICONTROL 下一步]**。 引导式设置前进到审核步骤。

![显示激活匹配键映射配置的映射字段步骤。](/help/assets/destinations/manage-destinations/map-destination-fields.png)

### 审阅 {#review-destination}

**[!UICONTROL 审核]**&#x200B;步骤在创建目标配置之前对该配置进行了汇总。

查看目标设置。 要进行更改，请选择铅笔图标![铅笔图标。](../../assets/icons/edit.png) 以了解适用的部分，并更新配置。

当配置正确时，选择&#x200B;**[!UICONTROL 完成]**。 将创建目标，并使其可用于受众激活。

![查看步骤在完成前显示目标配置摘要。](/help/assets/destinations/manage-destinations/review-destination-configuration.png)

## 查看已配置的目标 {#view-configured-destinations}

配置目标后，该目标会显示在目标清单中。 在清单中，您可以查看其状态和激活它的受众。

导航到&#x200B;**[!UICONTROL 激活]** > **[!UICONTROL 目标]**。 **[!UICONTROL 目标]**&#x200B;选项卡显示已配置目标的表。

![显示已配置目标的“目标”选项卡。](/help/assets/destinations/manage-destinations/configured-destinations-list.png)

## 删除目标 {#delete-destination}

当受众激活不再需要某个目标时将其删除。 删除目标会将其从目标清单中删除，并阻止将来将受众激活到该目标。

>[!IMPORTANT]
>
>删除目标不会删除之前导出到该目标的受众数据。 直接从目标数据存储中删除之前导出的数据。

导航到&#x200B;**[!UICONTROL 激活]** > **[!UICONTROL 目标]**。

找到要删除的目标，在&#x200B;**[!UICONTROL 操作]**&#x200B;列中选择省略号图标，然后选择&#x200B;**[!UICONTROL 删除]**。

![激活工作区的“目标”选项卡，突出显示省略号图标和删除操作。](/help/assets/destinations/manage-destinations/delete-configured-destination.png)

将显示确认对话框。 查看将要删除的目标，然后选择&#x200B;**[!UICONTROL 删除]**&#x200B;进行确认。

目标将从目标库存中删除，并且不再可用于受众激活。

## 后续步骤 {#next-steps}

配置目标后，您可以开始[激活项目中的受众](../collaborate/activate.md)。
