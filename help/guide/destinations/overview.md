---
title: 设计概述
description: 了解Real-Time CDP Collaboration中的目标。
audience: admin, publisher
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 5cbbf5c4-4caa-40da-97be-690d95c1201c
source-git-commit: eed99cfafd5ffad5a468741f7258c162454769b7
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 6%

---

# 目标概述

{{limited-availability-release-note}}

目标是指用于将目标受众发送到外部平台的集成。 通过这些集成，您可以跨各种营销渠道和平台激活受众，以用于营销活动和客户参与。

目前，目标仅适用于Adobe Real-Time CDP Collaboration中的发布者。 发布者可以配置目标以将受众发送到外部平台，例如Adobe Experience Platform，以用于营销活动。 然后，广告商可以[激活项目](../collaborate/activate.md)中的受众，这些受众将发送到发布者的配置目标。

>[!IMPORTANT]
>
>目前，当广告商激活您项目中的受众时，它们会自动发送到发布者配置的目标。 作为发布者，您&#x200B;**必须**&#x200B;在&#x200B;*您的协作者激活受众之前，先配置目标*。 如果未配置目标，则受众将会发送给您，并显示在项目的&#x200B;**[!UICONTROL 激活]**&#x200B;选项卡中，但不会激活。

## 配置目标 {#configure-destinations}

要配置目标，请导航到&#x200B;**[!UICONTROL 安装程序]**，然后选择&#x200B;**[!UICONTROL 我的目标]**&#x200B;选项卡。 在这里，您可以查看所有可用的目标。

>[!NOTE]
>
> 目前，只有Adobe Experience Platform可作为Collaboration中的自助服务目标。 如果您有兴趣配置Amazon S3或Snowflake等目标，请联系您的Adobe代表。

![设置工作区中的“我的目标”选项卡显示可用的目标。](/help/assets/destinations/overview/my-destinations-overview.png)

要开始配置目标，请选择所选目标中的&#x200B;**[!UICONTROL 设置]**&#x200B;选项。 有关配置特定目标的信息，请参阅[可用目标](#available-destinations)表中的指南。

![为Adobe Experience Platform目标突出显示具有“设置”选项的“我的目标”工作区。](/help/assets/destinations/overview/my-destinations-set-up.png)

### 可用目标 {#available-destinations}

可以在Collaboration中配置以下目标。 要查看该目标的配置指南，请在下表中选择目标名称。 如果您有兴趣配置当前不可用的目标，请联系您的Adobe代表。

| 目标 | 可用性 |
| --- | --- |
| [Adobe Experience Platform](./experience-platform.md) | 可用 |
| Amazon S3 | 即将推出。 |
| Snowflake | 即将推出。 |
| Google 云存储 | 即将推出。 |
| Azure Blob Storage | 即将推出。 |

## 后续步骤

配置目标后，即可开始[激活项目中的目标受众](../collaborate/activate.md)。
