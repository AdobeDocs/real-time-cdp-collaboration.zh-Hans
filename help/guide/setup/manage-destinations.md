---
title: 配置和管理目标
description: 了解如何在Real-Time CDP Collaboration中配置和管理目标。
audience: admin, publisher
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/cn/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: b4b26761-46ac-420f-b9f7-6e829d67aec9
source-git-commit: a7215d453021be578a32ce1af4d659845c3b8493
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 1%

---

# 配置和管理目标

{{limited-availability-release-note}}

目标是指用于将目标受众发送到外部平台的集成。 通过这些集成，您可以跨各种营销渠道和平台激活受众，以用于营销活动和客户参与。

协作者可以配置目标以将受众发送到外部平台，例如Adobe Experience Platform，以用于营销活动。 协作者随后可以[激活项目](../collaborate/activate.md)中的受众，这些受众将发送到其连接的配置目标。 根据连接[中配置的受众激活设置](/help/guide/connect/establishing-connections.md#configure-connection-settings)，激活可由协作者完成。

![安装工作区中的“我的目标”选项卡显示活动的Adobe Experience Platform目标。](/help/assets/setup/manage-destinations/my-destinations-overview.png)

要了解有关目标的更多信息，请参阅[目标概述](../destinations/overview.md)指南。

## 配置目标 {#configure-destinations}

在Collaboration的&#x200B;**[!UICONTROL 设置]**&#x200B;部分中配置了目标。 要配置目标，请导航到&#x200B;**[!UICONTROL 设置]**，然后选择&#x200B;**[!UICONTROL 我的目标]**&#x200B;选项卡。 在这里，您可以查看所有可用的目标。

>[!IMPORTANT]
>
>要配置和管理目标，您的用户必须具有分配了&#x200B;**管理受众数据**&#x200B;权限的角色。 有关管理角色的更多信息，请参阅[管理角色](../permissions/manage-roles.md)指南。

![设置工作区中的“我的目标”选项卡显示可用的目标。](/help/assets/setup/manage-destinations/my-destinations.png)

目标的设置过程取决于您配置的目标。 请参阅[可用目标](../destinations/overview.md#available-destinations)目录以查看可用目标及其配置指南。

>[!NOTE]
>
>目前，只有Adobe Experience Platform可作为Real-Time CDP Collaboration中的自助服务目标。 如果您有兴趣配置其他目标，请联系您的Adobe代表。

## 删除目标 {#delete-destinations}

删除目标会将其从您的帐户中删除，会从目标中删除以前发送的任何受众，并阻止将来将任何受众发送到该目标。

要删除目标，请导航到&#x200B;**[!UICONTROL 设置]**&#x200B;部分中的&#x200B;**[!UICONTROL 我的目标]**&#x200B;选项卡。 为要删除的目标选择&#x200B;**[!UICONTROL 删除]**&#x200B;选项。

![为Adobe Experience Platform目标突出显示了包含“删除”选项的“我的目标”工作区。](/help/assets/setup/manage-destinations/delete-destination.png)

此时将显示一个确认对话框，您可以在该对话框中确认要删除目标。 选择&#x200B;**[!UICONTROL 删除]**&#x200B;以删除目标。

![突出显示了“删除”选项的“删除目标”对话框。](/help/assets/setup/manage-destinations/delete-destination-confirmation.png)

## 后续步骤

配置目标后，您可以在连接内开始协作以激活项目中的[目标受众](../collaborate/activate.md)。
