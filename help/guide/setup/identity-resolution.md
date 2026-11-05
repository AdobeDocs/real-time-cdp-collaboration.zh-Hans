---
title: 设置和管理身份解析
description: 了解如何在Real-Time CDP Collaboration中配置和管理身份解析。
audience: admin, publisher, advertiser, agency
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
    internal-label: Real-Time Customer Data Platform
source-git-commit: ff233017fb78a63b2e911dc0dc94d67f2b18af04
workflow-type: tm+mt
source-wordcount: '1110'
ht-degree: 2%
---
# 设置和管理身份解析

{{limited-availability-release-note}}

身份解析可帮助您识别与协作者共有的客户，即使您的组织使用不同的标识符也是如此。 在Real-Time CDP Collaboration中使用受支持的身份提供程序配置和管理身份解析，而无需为每个合作伙伴构建自定义集成。

>[!NOTE]
>
>本指南中的步骤和屏幕截图以[!DNL Epsilon Core ID]为例。 要求和可用选项可能因您的身份提供者而异。

>[!AVAILABILITY]
>
>启动时，只有[!DNL Epsilon Core ID]可用于配置。 Epsilon核心ID身份解析仅适用于在美国设置的Real-Time CDP Collaboration帐户。

## 先决条件 {#prerequisites}

在开始之前，请确保您具有：

* **帐户管理权限。** 您必须具有&#x200B;**[!UICONTROL 管理帐户]**&#x200B;和&#x200B;**[!UICONTROL 管理Collaboration实例]**&#x200B;权限。
* **至少一个受众数据连接。** 您需要一个现有的受众数据连接来配置身份解析。 [根据需要设置受众源](./source-overview.md)。 不支持测量数据连接。
* **支持的匹配键和字段。** 要用于标识解析的每个受众数据连接都必须包含您的标识提供者支持的字段。 对于Epsilon Core ID，您可以使用经过哈希处理的电子邮件、经过哈希处理的手机或结合邮政地址使用的姓名。

  必须为您的帐户启用帐户级别的匹配键（例如经过哈希处理的电子邮件和手机），并将其映射到您的受众数据。 名称和邮政地址字段在设置受众数据连接期间映射，不需要帐户级别启用。

  如果使用姓名和邮政地址，请映射每个组中的至少一个字段：

  * **姓名：**&#x200B;名字、姓氏或全名。
  * **邮政地址：**&#x200B;街道地址、城市、邮政编码、州或国家/地区。

  名称和邮政地址值未进行哈希处理。 有关启用帐户级别匹配键（如散列电子邮件和散列电话）的说明，请参阅[编辑匹配键](./onboard-account.md#edit-match-keys)。 要将受支持的匹配键或名称和邮政地址字段映射到您的受众数据，请参阅[映射字段](./onboard-audiences.md#map-fields)。
* **Epsilon帐号。** 从您的Epsilon客户代表处获取您的Epsilon帐号。

## 配置身份解析 {#configure-identity-resolution}

选择身份提供程序以开始配置身份解析。 在此[!DNL Epsilon Core ID]示例中，您将通过提供商的身份验证、选择受众数据连接、设置日期范围并在确认之前查看配置。

若要开始，请在左侧导航中选择&#x200B;**[!UICONTROL 设置]**，然后选择&#x200B;**[!UICONTROL 身份解析]**&#x200B;选项卡以查看可用的身份提供程序。

### 选择身份提供者 {#select-identity-provider}

找到您的身份提供者的卡，并查看其支持的区域并匹配键。 选择&#x200B;**[!UICONTROL 安装程序]**&#x200B;以开始。

![包含Epsilon核心ID卡的身份提供程序目录及其设置操作。](../../assets/setup/identity-resolution/select-an-identity-provider.png){zoomable="yes"}

在启动配置工作流之前，Collaboration会检查是否存在数据连接和兼容的匹配键。 如果缺少要求，将显示一个对话框来指导该过程。 按照对话框中的操作进行操作：

* **[!UICONTROL 需要数据连接]：**&#x200B;选择&#x200B;**[!UICONTROL 设置数据连接]**&#x200B;以配置受众数据连接。 请参阅[连接源](./source-overview.md#connect-a-source)。
* **[!UICONTROL 需要匹配键]：**&#x200B;选择&#x200B;**[!UICONTROL 编辑匹配键]**&#x200B;以启用支持的键。 请参阅[编辑匹配键](./onboard-account.md#edit-match-keys)。

如果两者都丢失，则首先出现数据连接对话框。 修复先决条件后，返回到&#x200B;**[!UICONTROL 身份解析]**&#x200B;并再次选择&#x200B;**[!UICONTROL 设置]**。

### 向您的身份提供程序进行身份验证 {#authenticate-with-provider}

在&#x200B;**[!UICONTROL 身份验证]**&#x200B;步骤中，提供您的身份提供程序所需的信息。 对于Epsilon Core ID，请在&#x200B;**[!UICONTROL Epsilon帐号]**&#x200B;字段中输入您的Epsilon代表提供的帐号。 选择&#x200B;**[!UICONTROL 下一步]**&#x200B;以继续。

![显示Epsilon帐号字段的身份验证步骤。](../../assets/setup/identity-resolution/authenticate.png){zoomable="yes"}

### 选择数据连接 {#select-data-connections}

接下来，选择要用于身份解析的受众数据连接。 这会确定将哪些受众数据用于将您的客户身份与您的身份提供商进行匹配。 标识解析会自动使用每个选定连接中映射的受支持标识符。
接下来，选择要用于身份解析的受众数据连接。 选定的连接决定了哪些受众数据和映射的字段可用于身份解析。

标识解析适用于每个选定数据连接内的所有受众，包括稍后添加的任何受众。 此时无法选择单个受众。

如果未列出您想要的连接，请在继续之前[设置受众数据连接](./source-overview.md)。

在&#x200B;**[!UICONTROL 数据源]**&#x200B;下，选中要包含在&#x200B;**[!UICONTROL 受众源]**&#x200B;中的每个连接的复选框。 您必须至少选择一个连接。 选择&#x200B;**[!UICONTROL 下一步]**&#x200B;以继续。

![显示选定和未选定数据连接的受众源卡片。](../../assets/setup/identity-resolution/source-selection.png){zoomable="yes"}

### 设置身份解析计划 {#set-schedule}

选择开始和结束日期，以定义Adobe刷新合作伙伴ID的时段。 刷新频率由所选受众数据连接决定，因此无法为身份解析配置单独的刷新频率。

在&#x200B;**[!UICONTROL 计划]**&#x200B;步骤中，选择&#x200B;**[!UICONTROL 日期范围]**&#x200B;下的日历控件并选择您的日期。 选择&#x200B;**[!UICONTROL 下一步]**&#x200B;以继续。

![计划包含Epsilon核心ID标识解析日期范围的步骤。](../../assets/setup/identity-resolution/schedule-identity-resolution-job.png){zoomable="yes"}

### 查看并确认配置 {#review-and-confirm}

在&#x200B;**[!UICONTROL 审核]**&#x200B;步骤中，检查您的身份验证详细信息、选定的受众数据连接和计划。 要进行更改，请选择相关部分旁边的&#x200B;**[!UICONTROL 编辑]**。

安装后无法编辑配置。 要稍后进行更改，您必须删除它并重新进行设置。 在您满意您的选择后，请选择&#x200B;**[!UICONTROL 确认并计划]**。

![显示身份验证、数据源和计划摘要的审核步骤。](../../assets/setup/identity-resolution/review-and-confirm.png){zoomable="yes"}

确认对话框指示已成功配置身份解析。

<!-- [Question: Does the first identity resolution run happen immediately after setup, or at the next scheduled audience data connection refresh?] -->

## 管理身份解析 {#manage-identity-resolution}

确认设置后，您将自动返回到&#x200B;**[!UICONTROL 身份解析]**&#x200B;选项卡，您可以在其中查看或删除配置。

### 查看配置详细信息 {#view-configuration-details}

要查看您的配置，请在您配置的身份提供程序卡上选择&#x200B;**[!UICONTROL 查看详细信息]**。

查看身份验证详细信息、选定的受众数据连接和日期范围。 您还可以查看配置详细信息中显示的匹配键，以及配置状态和创建和更新信息。

![身份解析配置详细信息，显示状态、匹配键、计划和关联的受众连接。](../../assets/setup/identity-resolution/view-connection-details.png){zoomable="yes"}

### 更改现有配置 {#edit-configuration}

安装后，您无法编辑核心ID配置。 若要更改Epsilon帐号、所选的数据连接或日期范围，请[删除配置](#delete-configuration)并再次完成[设置工作流](#configure-identity-resolution)。

<!-- Question: Do other providers have the same limitation? -->

### 删除身份解析配置 {#delete-configuration}

要删除配置，请导航到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 身份解析]**，然后在您配置的身份提供程序的卡中选择&#x200B;**[!UICONTROL 删除]**。 查看确认对话框，然后选择&#x200B;**[!UICONTROL 删除]**&#x200B;以进行确认。

如果要再次使用此身份提供程序，您需要[设置新配置](#configure-identity-resolution)。

<!-- [UNVERIFIED: Does deletion affect previously resolved identifiers, future processing, or both? Confirm before publication.] -->

## 设置问题疑难解答 {#troubleshoot}

如果由于缺少数据连接或匹配键而无法开始安装，请按照[选择身份提供程序](#select-identity-provider)下的说明操作。

对于Epsilon核心ID，请检查以下内容：

* **在您的地区不可用：** Epsilon核心ID仅适用于在美国设置的Collaboration帐户。
* **Epsilon帐号不可用：**&#x200B;请与Epsilon代表联系以获取您的帐号。
