---
title: 为Collaboration [!DNL Starter] 载入配置权限控制
description: 了解如何使用Adobe Experience Cloud中的权限配置Adobe Real-Time CDP Collaboration [!DNL Starter] 的权限。
audience: users invited to Real-Time CDP Collaboration [!DNL Starter]
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 4e50b6cc-58f7-4a0c-8b6d-f5aa4f092e9f
source-git-commit: 147fd5847bc5074e4b4f8a05a9a1c3afc089be56
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 4%

---

# 为Collaboration [!DNL Starter]载入配置权限控制

在设置管理员和用户对Adobe Experience Platform产品的访问权限后，您需要为自己分配对Real-Time CDP Collaboration具有适当权限的角色。 阅读本指南，了解如何通过Experience Cloud权限界面向您的帐户添加正确的角色，以便您可以访问和管理用户对Collaboration功能的访问权限。

有关Collaboration资源中包含的标准角色和可用权限的详细信息，请参阅[如何管理角色指南](../permissions/manage-roles.md)。

## 先决条件 {#prerequisites}

确保您同时具有Adobe Experience Platform产品的&#x200B;**管理员权限**&#x200B;和&#x200B;**用户访问权限**。 如果您尚未设置这些访问级别，请参阅[管理员访问指南](./starter-admin-access.md)以了解分步说明。

## 设置权限 {#setup-permissions}

请按照以下步骤设置Collaboration所需的权限。 首先，使用您的凭据登录到[Adobe Experience Cloud](https://experience.adobe.com/)。

### 访问权限 {#access-permissions}

登录后，导航到&#x200B;**[!UICONTROL 快速访问]**&#x200B;部分并选择&#x200B;**[!UICONTROL 权限]**。 这将打开“权限”功能板，您可以在其中为您自己分配必要的角色。

![Experience Cloud主页，其“快速访问”部分中的权限突出显示。](../../assets/setup/starter/access-permissions.png){zoomable="yes"}

### 选择用户 {#select-user}

在&#x200B;**[!UICONTROL 权限]**&#x200B;仪表板中，从左侧面板中选择&#x200B;**[!UICONTROL 用户]**。 然后，从“用户”表中选择您的帐户。

>[!NOTE]
>
> 如果您是贵组织中第一个访问Experience Platform的用户，则您可能是&#x200B;**用户**&#x200B;表中列出的唯一用户。 若要邀请其他团队成员，请按照[用户访问配置指南](../permissions/manage-user-access.md#administrators-configure-user-access-to-experience-platform)中的步骤操作。

![权限仪表板显示突出显示用户帐户的“用户”表。](../../assets/setup/starter/select-user.png){zoomable="yes"}

### 分配角色 {#assign-roles}

在对应&#x200B;**[!UICONTROL 用户]**&#x200B;工作区中，导航到&#x200B;**[!UICONTROL 角色]**&#x200B;选项卡。 然后选择&#x200B;**[!UICONTROL 添加角色]**。

![相应的用户工作区显示“角色”选项卡，其中突出显示“添加角色”选项。](../../assets/setup/starter/add-roles.png){zoomable="yes"}

此时将显示&#x200B;**[!UICONTROL 添加角色]**&#x200B;对话框，其中包含可用角色的表。 表中的每一行代表一个角色，其信息如下：

| **列** | **描述** |
|---------------|--------------------------------------------------------|
| **名称** | 角色的名称。 |
| **描述** | 概述角色功能的简短摘要。 请注意，无法自定义“只读”角色。 |
| **沙盒** | 指定角色提供访问权限的沙箱（例如，`Prod`）。 |
| **已修改** | 上次更新角色的日期。 |

{style="table-layout:auto"}

有关特定角色及其权限的深入概述，请参阅[管理角色的权限](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/abac/permissions-ui/permissions)指南。

查看信息并选择要分配给帐户的角色。 完成后，选择&#x200B;**[!UICONTROL 保存]**。

![“添加角色”对话框显示选定的角色，并突出显示“保存”选项。](../../assets/setup/starter/add-roles-dialog.png){zoomable="yes"}

确认对话框用于确认新角色是否已成功添加。

为确保您的权限设置正确，请返回[Experience Cloud](https://experience.adobe.com/)主页。 在&#x200B;**[!UICONTROL 快速访问]**&#x200B;中选择&#x200B;**[!UICONTROL Real-Time CDP Collaboration]**。 您应该能够访问Collaboration工作区，并开始使用您的[!DNL Starter]帐户可用的功能。

## 后续步骤 {#next-steps}

设置好权限后，您便可以访问Collaboration。 接下来，您可以：

* [创建具有特定权限的自定义角色以管理不同的访问级别](../permissions/manage-roles.md#create-specific-access-roles)。
* [在权限](../permissions/manage-user-access.md#assign-a-role)中将多个用户分配给一个角色。
* [设置Collaboration帐户并与邀请的协作者建立连接](../overview/starter-overview.md#set-up-connections)。
* [在Collaboration中了解有关信用使用情况和消费情况的更多信息 [!DNL Starter]](./starter-credit-usage.md)。

要全面了解Real-Time CDP Collaboration及其主要功能，请阅读[概述指南](../home.md)。
