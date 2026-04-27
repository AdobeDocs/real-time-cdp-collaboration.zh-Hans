---
title: Manage roles through Permissions
description: Understand all available role resources that provide access to different components within the Real-Time CDP Collaboration UI.
audience: admin
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 59cf5bf2-421b-4ebc-beab-30eafb098649
TQID: https://experienceleague.adobe.com/dB7nEQtEGG8PvCSE7eDDelH-ml2EhKOQ8ovvGXG1Ejg
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
feature_v2:
  - id: ba929a52-9339-4154-9487-317dc875a3c7
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 3ce7e66b31332836fd6cc6137c94622436505cc9
workflow-type: tm+mt
source-wordcount: 623
ht-degree: 3%

---

# 管理角色 {#manage-roles}

{{limited-availability-release-note}}

To manage user access to different components of the Adobe Real-Time CDP Collaboration UI, an [administrator](./manage-user-access.md#system-admin-gain-access) can define and assign roles. Roles define the access that an administrator or user has to [resources](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/home#permissions){target="_blank"} in your organization. This guide will provide information on the standard roles provided in Real-Time CDP Collaboration, as well as the individual permissions you that can be assign to custom roles.

To begin managing roles, an administrator will need access to the Experience Platform product. For information on gaining administrative access, or on gaining access to Experience Platform, read the [manage user access](./manage-user-access.md#manage-user-access-through-permissions) guide.

## Standard roles {#standard-roles}

There are two standard roles provided to you that fill two common access control use cases. These are &quot;read only&quot; roles meaning they cannot be customized.

| 角色名称 | Role description | 权限 |
| --- | --- | --- |
| Collaboration Managers | This is all-access permission, containing all 15 permissions. This allows the user to read, create, and edit all data. It also provides access to the **[!UICONTROL Prod]** sandbox in Experience Platform, allowing you to import audiences into Real-Time CDP Collaboration. | All from the table below. |
| Collaboration Viewers | This is a read-only access permission. A user can read and discover data, activities, connections, and more. It also provides access to the **[!UICONTROL Prod]** sandbox in Experience Platform, allowing you to import audiences into Real-Time CDP Collaboration. | All read permissions from the table below. |

{style="table-layout:auto"}

## Create specific access roles {#specific-access-roles}

您可能需要创建其他角色，以便为不同用户提供不同级别的访问权限。 创建角色时，您可以通过选择&#x200B;**[!UICONTROL 协作]**&#x200B;资源中的特定权限来管理不同的访问级别。 要了解如何创建和管理角色，请参阅[角色](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/abac/permissions-ui/roles#create-new-role){target="_blank"}指南。

>[!NOTE]
> 要访问Collaboration，用户必须有权访问Adobe Experience Platform中的&#x200B;**[!UICONTROL Prod]**&#x200B;沙盒。 要授予用户访问此沙盒的权限，必须将他们分配给&#x200B;**[!UICONTROL 沙盒]**&#x200B;资源中包含&#x200B;**[!UICONTROL Prod]**&#x200B;权限的角色。

协作资源中的可用权限列表如下：

| 高级权限 | 描述 |
| --- | --- |
| 管理Collaboration实例 | 查看、创建、更新和删除组织的协作实例。 发现其他组织的协作实例。 |
| 读取Collaboration实例 | 读取组织的协作实例并发现其他组织的协作实例。 |
| 管理连接邀请 | 查看、创建和删除您的组织发起的连接邀请。 接受和拒绝其他组织发起的连接邀请。 |
| 读取连接邀请 | 查看连接邀请。 |
| 管理Collaboration连接 | 协作者可以查看、创建和更新设置以及提交和删除连接。 |
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

在创建定义Collaboration访问权限的角色后，您需要将角色[分配给管理员和用户](./manage-user-access.md#assign-a-role)。 有关管理角色的完整概述，请参阅[角色的管理权限](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/abac/permissions-ui/permissions)指南。
