---
title: '为受众源配置 [!DNL Snowflake] '
description: 了解如何将 [!DNL Snowflake Secure Data Share] 配置为自助数据源并将其连接，以将受众数据摄取到Real-Time CDP Collaboration。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 11a73116-4919-48a3-bf44-de2a10c102c1
source-git-commit: 19a516b472b1ddde68990f98b57667dd302f1fbc
workflow-type: tm+mt
source-wordcount: '1229'
ht-degree: 21%

---

# 为受众源配置[!DNL Snowflake]

了解如何在Adobe Real-Time CDP Collaboration UI中配置您的[!DNL Snowflake Secure Data Share]并将其连接到受众数据以进行激活和重叠分析。

## 概述 {#overview}

[!DNL Snowflake]是支持将第一方受众数据获取到Collaboration中的选项之一。 其他可用方法包括从[Experience Platform](./onboard-audiences.md)获取受众、连接[[!DNL AWS S3] 存储桶](./configure-aws-s3-audience-sourcing.md)或上传[CSV文件](./upload-csv-audience-sourcing.md)。

按照以下步骤连接您的[!DNL Snowflake Secure Data Share]并将受众数据来源到Collaboration。 设置完成后，您可以审核、激活和管理协作项目的来源受众。

## 先决条件 {#prerequisites}

在配置[!DNL Snowflake]连接之前，请确保满足以下先决条件：

* 您已创建一个[!DNL Snowflake Share]并在您的[!DNL Snowflake]帐户中设置必要的权限来授予对您的[!DNL Snowflake Secure Data Share]的Adobe访问权限。
* 您已准备好[!DNL Snowflake Share]个值：

   * **共享名称**
   * **帐户标识符**
   * **架构**
   * **视图**

* [!DNL Snowflake Secure Data Share]中的受众数据必须符合[受众源规格(v1.2)](../../assets/quick-start/RTCDP_Collaboration_Audience_Sourcing_Spec_v1.2.pdf)指南中所述的格式要求。
* 还必须为您的Collaboration帐户启用[!DNL Snowflake]受众文件中的所有匹配键。 了解如何[启用匹配键](./onboard-account.md#set-up-match-keys)或[将新的匹配键](./onboard-account.md#edit-match-keys)添加到您的帐户。

## 配置您的[!DNL Snowflake]连接 {#configure-snowflake-connection}

从&#x200B;**[!UICONTROL 设置]**&#x200B;工作区的&#x200B;**[!UICONTROL 我的受众]**&#x200B;选项卡中，选择添加图标（![添加图标。](/help/assets/icons/plus.png)） 然后选择&#x200B;**[!UICONTROL 受众]**。

如果这是您的第一个受众，您还可以选择&#x200B;**[!UICONTROL 添加受众]**&#x200B;选项。

![在“设置”工作区中显示的“我的受众”选项卡，其中显示了“添加”图标和“添加受众”选项。](../../assets/setup/snowflake-audience-sourcing/add-audience.png)

此时会显示添加受众工作流。 选择&#x200B;**[!UICONTROL 添加新数据连接]**，然后选择&#x200B;**[!UICONTROL 下一步]**。

![突出显示了“添加新数据连接”选项的“添加受众”工作区。](../../assets/setup/snowflake-audience-sourcing/add-data-connection.png){zoomable="yes"}

### 选择[!DNL Snowflake]作为数据连接 {#select-snowflake}

接下来，选择&#x200B;**[!UICONTROL Snowflake]**&#x200B;作为数据连接，然后选择&#x200B;**[!UICONTROL 下一步]**。

![具有[!DNL Snowflake]的数据连接选择屏幕可用作可选选项。](../../assets/setup/snowflake-audience-sourcing/select-snowflake-data-connection.png)

### 查看受众文件 {#review-audience-file}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_audience_sourcing_specifications_snowflake"
>title="请为加入过程准备好您的数据"
>abstract="请参阅《受众源规格指南》，了解如何设置和构建适用于Collaboration的Snowflake中的受众数据。"
>additional-url="https://www.adobe.com/go/rtcdp-collaboration-audience-sourcing" text="查看指南"

此时会出现一个对话框，说明在开始获取之前[!DNL Snowflake Share]和[!DNL Snowflake]受众文件的要求。 确保使用正确的共享名、帐户标识符、架构和视图创建您的[!DNL Snowflake Share]。 要确认受众数据的格式和结构正确无误，以便在Collaboration中使用，请查看&#x200B;**[[!UICONTROL 受众源规格]](../../assets/quick-start/RTCDP_Collaboration_Audience_Sourcing_Spec_v1.2.pdf)**&#x200B;指南。

完成后，选择&#x200B;**[!UICONTROL 开始载入]**。

![使用指向受众源规范的链接准备[!DNL Snowflake Share]以加入对话框。](../../assets/setup/snowflake-audience-sourcing/prepare-snowflake-share-onboarding-dialog.png)

### 验证[!DNL Snowflake Share]连接 {#authenticate-snowflake-share-connection}

在此步骤中，您需要提供将您的[!DNL Snowflake Share]连接到Collaboration所需的[!DNL Snowflake Share]凭据：

| 字段 | 描述 | 示例 |
|--------------------|-------------|------------------------------|
| 共享名称 | [!DNL Snowflake Share]的名称。 | `ADOBE_DATA_SHARE` |
| 帐户标识符 | Snowflake帐户的唯一标识符。 | `CUSTOMER_ORG.CUSTOMER_SNOWFLAKE_ACCOUNT` |
| 架构 | [!DNL Snowflake Share]中包含受众数据的架构。 | `CUSTOMER_SCHEMA` |
| 视图 | Collaboration拉入受众数据的实际数据集。 | `SECURE_VIEW_FOR_ADOBE` |

{style="table-layout:auto"}

输入所有必需的凭据后，选择&#x200B;**[!UICONTROL 下一步]**。

![已填写[!DNL Snowflake Share]连接表单，其中的“共享名称”、“帐户标识符”、“架构”和“视图”字段已填写，并且“下一步”按钮已突出显示。](../../assets/setup/snowflake-audience-sourcing/snowflake-authentication-credentials-form.png)

下一页底部会显示一个确认对话框，用于确认您的[!DNL Snowflake Share]已成功连接到Collaboration。

![确认对话框确认您的[!DNL Snowflake Share]连接已成功建立。](../../assets/setup/snowflake-audience-sourcing/snowflake-share-connection-established.png)

### 提供名称和描述 {#provide-name-description}

在&#x200B;**[!UICONTROL 提供详细信息]**&#x200B;视图中，为您的[!DNL Snowflake]数据连接输入描述性名称和可选描述。 完成后，选择&#x200B;**[!UICONTROL 下一步]**。

![提供详细信息屏幕显示数据连接的名称和描述，并突出显示“下一步”按钮。](../../assets/setup/snowflake-audience-sourcing/provide-name-description.png)

### 映射字段 {#map-fields}

**[!UICONTROL 映射]**&#x200B;屏幕当前为只读。 不能添加、删除或应用转换。 Collaboration根据&#x200B;**[受众源规格(v1.2)](../../assets/quick-start/RTCDP_Collaboration_Audience_Sourcing_Spec_v1.2.pdf)**&#x200B;自动将源标识字段从[!DNL Snowflake Share]数据映射到目标字段。

以可视方式确认映射的字段并选择&#x200B;**[!UICONTROL 下一步]**&#x200B;以继续。 您还可以使用&#x200B;**[!UICONTROL 预览源数据]**&#x200B;选项预览[!DNL Snowflake Share]中的示例数据。

![映射字段屏幕显示自动映射的源字段和目标字段，并突出显示“预览源数据”和“下一步”选项。](../../assets/setup/snowflake-audience-sourcing/map-fields-screen.png)

当您选择预览时，将显示&#x200B;**[!UICONTROL [!DNL Snowflake Share]数据预览]**&#x200B;对话框，其中以表格格式显示样本数据。 查看此内容，然后选择&#x200B;**[!UICONTROL 关闭]**。

![[!DNL Snowflake Share]数据预览对话框显示[!DNL Snowflake Share]中的示例数据，并且突出显示了“关闭”选项。](../../assets/setup/snowflake-audience-sourcing/preview-source-data.png)

<!-- NOTE: Manual mapping will be available in the future. -->
<!-- In the **[!UICONTROL Map fields]** screen, you can use the **[!UICONTROL Source field]** and **[!UICONTROL Target field]** dropdowns to update the auto-mapped fields, or include additional fields with the **[!UICONTROL Add field]** option. Once finished, select **[!UICONTROL Next]**. -->

<!-- ![The Map fields screen showing the mapped fields with the Next option highlighted.](../../assets/setup/snowflake-audience-sourcing/map-fields.png) -->

### 计划刷新频率和日期范围 {#refresh-frequency-date-range}

接下来，在&#x200B;**[!UICONTROL 计划]**&#x200B;视图中，使用下拉菜单选择一到六天之间的刷新频率。 然后，使用日历图标指定来源受众的开始和结束日期。

>[!IMPORTANT]
>
>要有效地管理Collaboration积分，请将刷新频率设置为匹配或不超过基础[!DNL Snowflake]数据的更新频率。 支持的最低刷新间隔为每6天一次。

![计划屏幕突出显示刷新频率和日期范围配置，以及下一个选项。](../../assets/setup/snowflake-audience-sourcing/refresh-frequency-date-range.png)

### 查看并完成连接 {#review-and-complete}

最后，在摘要屏幕中查看配置设置。 此视图包含以下部分的摘要：

* **[!UICONTROL 数据连接]**：显示[!DNL Snowflake Share]的共享名、帐户标识符、方案和视图。
* **[!UICONTROL 详细信息]**：显示数据连接的名称和可选说明，以便帮助以后识别它。
* **[!UICONTROL 映射]**：显示受众文件中的源字段如何映射到Collaboration中使用的目标字段。
* **[!UICONTROL 计划]**：显示连接刷新受众数据的频率以及来源的有效日期范围。

如果需要编辑节，请选择铅笔图标（![编辑图标](/help/assets/icons/edit.png)）。 选择&#x200B;**[!UICONTROL 完成]**&#x200B;以确认所有节。

![查看屏幕显示数据连接、详细信息、映射和计划设置的摘要，并突出显示“完成”选项。](../../assets/setup/snowflake-audience-sourcing/review-settings.png)

确认对话框用于确认数据连接是否已成功创建以及受众获取是否正在进行中。

## 审查源受众 {#review-sourced-audiences}

设置完成后，Collaboration开始从您的[!DNL Snowflake Share]中获取受众。 如果受众源正在进行，则会在视图顶部显示横幅。

![我的受众选项卡显示正在采购的受众横幅。](../../assets/setup/snowflake-audience-sourcing/audience-sourcing-in-progress.png)

>[!TIP]
>
>受众源获取时间因[!DNL Snowflake]数据的大小和您配置的刷新频率而异。 较大的数据集或不太频繁的刷新计划可能需要更长的时间才能显示在&#x200B;**[!UICONTROL 我的受众]**&#x200B;工作区中。

采购完成后，您的受众将位于&#x200B;**[!UICONTROL 我的受众]**&#x200B;选项卡中，其功能和信息与源自Experience Platform的受众相同。

![我的受众选项卡以表格视图显示来源受众列表。](../../assets/setup/snowflake-audience-sourcing/snowflake-audience-list.png)

在网格视图或表格视图中，选择行项或&#x200B;**[!UICONTROL 查看受众]**&#x200B;以查看特定受众的概述。 它显示受众的状态、源和数据连接名称，以及&#x200B;**[!UICONTROL 身份]**、**[!UICONTROL 类别]**、**[!UICONTROL 连接访问]**&#x200B;和&#x200B;**[!UICONTROL 元数据可见性]**&#x200B;的详细面板。 有关详细信息，请参阅[如何查看单个受众](./onboard-audiences.md#view-individual-audiences)。

在协作项目中使用受众之前，请使用此视图确认受众配置和可见性设置。

## 查看您的[!DNL Snowflake]数据连接 {#view-snowflake-connection}

您新添加的[!DNL Snowflake]连接在&#x200B;**[!UICONTROL 我的数据连接]**&#x200B;选项卡中立即可用。 受众源显示为[!UICONTROL [!DNL Snowflake]]。

您的[!DNL Snowflake]数据连接包含与其他受众数据连接相同的功能和详细信息。 详细了解[如何查看和管理数据连接](../setup/manage-data-connection.md)。

![我的数据连接选项卡显示与源状态信息的[!DNL Snowflake]数据连接。](../../assets/setup/snowflake-audience-sourcing/data-connection-tab-snowflake.png)

## 后续步骤 {#next-steps}

您现在已成功将您的[!DNL Snowflake]配置为Collaboration中的数据源并将其连接。 完成源获取后，您可以[创建协作项目](../collaborate/manage-projects.md)、[激活受众](../collaborate/activate.md)、[查看重叠和见解](../collaborate/measure.md)以及[管理受众设置和可见性](./onboard-audiences.md)。

有关其他受众来源补充方法的信息，请参阅以下文档：

* [为受众源配置 [!DNL Amazon S3] &#x200B;](./configure-aws-s3-audience-sourcing.md)
* [来自Experience Platform的Source受众](./onboard-audiences.md)
* [上传CSV文件以进行受众源](./upload-csv-audience-sourcing.md)
