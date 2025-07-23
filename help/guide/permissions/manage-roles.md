---
title: 通过权限管理角色
description: 了解提供对Real-Time CDP Collaboration UI中不同组件的访问权限的所有可用角色资源。
audience: admin
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/cn/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 59cf5bf2-421b-4ebc-beab-30eafb098649
source-git-commit: eed99cfafd5ffad5a468741f7258c162454769b7
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 1%

---

# 管理角色 {#manage-roles}

{{limited-availability-release-note}}

要管理用户对Adobe Real-Time CDP Collaboration UI其他组件的访问权限，[管理员](./manage-user-access.md#system-admin-gain-access)可以定义和分配角色。 角色定义管理员或用户对您组织中的[资源](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/access-control/home#permissions){target="_blank"}的访问权限。 本指南将介绍Real-Time CDP Collaboration中提供的标准角色，以及可分配给自定义角色的各个权限。

要开始管理角色，管理员需要访问Experience Platform产品。 有关获取管理访问权限或获取Experience Platform访问权限的信息，请参阅[管理用户访问权限](./manage-user-access.md#manage-user-access-through-permissions)指南。

## 标准角色 {#standard-roles}

为您提供的两个标准角色填写了两个常见的访问控制用例。 这些是“只读”角色，这意味着无法对其进行自定义。

| 角色名称 | 角色描述 | 权限 |
| --- | --- | --- | 
| Collaboration Managers | 这是完全访问权限，包含所有15个权限。 这允许用户读取、创建和编辑所有数据。 它还提供对Experience Platform中&#x200B;**[!UICONTROL Prod]**&#x200B;沙盒的访问权限，从而允许您将受众导入Real-Time CDP Collaboration。 | 下表显示全部内容。 |
| Collaboration查看器 | 这是只读访问权限。 用户可以读取和发现数据、活动、连接等。 它还提供对Experience Platform中&#x200B;**[!UICONTROL Prod]**&#x200B;沙盒的访问权限，从而允许您将受众导入Real-Time CDP Collaboration。 | 下表中的所有读取权限。 |

{style="table-layout:auto"}

## 创建特定的访问角色 {#specific-access-roles}

您可能需要创建其他角色，以便为不同用户提供不同级别的访问权限。 创建角色时，您可以通过选择&#x200B;**[!UICONTROL 协作]**&#x200B;资源中的特定权限来管理不同的访问级别。 要了解如何创建和管理角色，请参阅[角色](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/access-control/abac/permissions-ui/roles#create-new-role){target="_blank"}指南。

>[!NOTE]
> 要访问Collaboration，用户必须有权访问Adobe Experience Platform中的&#x200B;**[!UICONTROL Prod]**&#x200B;沙盒。 要授予用户访问此沙盒的权限，必须将他们分配给&#x200B;**[!UICONTROL 沙盒]**&#x200B;资源中包含&#x200B;**[!UICONTROL Prod]**&#x200B;权限的角色。

协作资源中的可用权限列表如下：

| 高级权限 | 描述 |
| --- | --- |
| 管理Collaboration实例 | 查看、创建、更新和删除组织的协作实例。 发现其他组织的协作实例。 |
| 读取Collaboration实例 | 读取组织的协作实例并发现其他组织的协作实例。 |
| 管理连接邀请 | 查看、创建和删除您的组织发起的连接邀请。 接受和拒绝其他组织发起的连接邀请。 |
| 读取连接邀请 | 查看连接邀请。 |
| 管理Collaboration连接 | 广告商可以查看、创建和更新设置，以及提交和删除连接。 发布者可以查看、接受或拒绝连接。 |
| 读取Collaboration连接 | 查看连接。 |
| 管理受众数据 | 载入和发现受众。 更新公共、私有和自定义受众，并管理受众清单元数据设置。 |
| 读取受众数据 | 阅读和发现受众。 |
| 管理测量数据 | 载入、更新和删除测量数据。 |
| 读取测量数据 | 读取测量数据。 |
| 管理项目 | 查看、创建、更新和删除任何发现、激活和测量活动的项目。 |
| 读取项目 | 查看任何发现、激活和测量活动的项目。 |
| 读取用户活动 | 读取用户活动。 |
| 导出用户活动 | 导出用户活动。 |
| 阅读Collaboration信用监控 | 组织和实例层的信用监控。 |

{style="table-layout:auto"}

## 后续步骤

在创建定义Collaboration访问权限的角色后，您需要将角色[分配给管理员和用户](./manage-user-access.md#assign-a-role)。 有关管理角色的完整概述，请参阅[角色的管理权限](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/access-control/abac/permissions-ui/permissions)指南。
