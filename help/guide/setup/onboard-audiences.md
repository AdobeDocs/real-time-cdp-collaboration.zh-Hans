---
title: Source和管理受众
description: 了解如何在Adobe Real-Time CDP Collaboration中获取和管理受众
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/cn/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 0a5158fa-73d3-4406-af20-2b6c7be9934e
source-git-commit: f14b5d2f49f20f229c4f474c31e22c008827a09b
workflow-type: tm+mt
source-wordcount: '3512'
ht-degree: 16%

---

# Source和管理受众

{{limited-availability-release-note}}

受众是根据各种属性划分的特定用户或客户组。 通过这些功能，协作者可共同创作有针对性的营销和个性化体验，从而更有效地开展广告促销活动。 本指南介绍如何在Real-Time CDP Collaboration中获取受众、查看受众仪表板以及管理单个受众。

## 将Source受众引入Collaboration {#source-audiences}

>[!IMPORTANT]
>
>要获取受众源，需要将您的用户分配到包含两个配置文件管理权限的角色 — **[!UICONTROL 查看配置文件]**&#x200B;和&#x200B;**[!UICONTROL 查看区段]**。 有关分配必要权限的信息，请参阅权限中的[受众源](../permissions/overview.md#audience-sourcing)指南。

您需要将受众来源添加到Collaboration，然后才能通过协作者激活受众并运行重叠计算。 要获取受众，请按照以下部分中的工作流步骤进行操作。

从&#x200B;**[!UICONTROL 设置]**&#x200B;工作区的&#x200B;**[!UICONTROL 我的受众]**&#x200B;选项卡中，选择添加图标（![添加图标）。](/help/assets/icons/plus.png))，然后选择&#x200B;**[!UICONTROL 受众]**。 如果这是您的第一个受众，您还可以选择&#x200B;**[!UICONTROL 添加]选项**。

![突出显示了“添加”选项和“受众”选项的“我的受众”工作区。](/help/assets/setup/add-manage-audiences/add-audiences.png){zoomable="yes"}

### 选择数据连接 {#select-data-connection}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_marketing_actions"
>title="营销操作"
>abstract="<p>使用营销操作来控制从 Experience Platform 向 Real-Time CDP Collaboration 导入哪些受众数据。<strong>数据协作</strong>营销操作支持 C4、C5 和 C9 数据使用标签。<strong>数据科学</strong>营销操作支持 C9 数据使用标签。</p> <p> <ul><li> <em>启用</em>该复选框后，Experience Platform 中标有上述标签的任何数据都会被排除，并且<strong>不</strong>被纳入 Real-Time CDP Collaboration。</li><li> <em>禁用</em>该复选框后，从 Experience Platform 引入 Real-Time CDP Collaboration 的数据不受限制。</li></ul></p>"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/data-governance/labels/overview.html?lang=zh-Hans" text="数据使用标签概述"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/data-governance/labels/reference.html?lang=zh-Hans" text="数据使用标签词汇表"

>[!IMPORTANT]
>
>在建立您的第一个数据连接并获取您的第一个受众后，您可以从现有数据连接获取多个受众。 添加其他受众时，您将从[选择受众](#select-audiences)步骤开始，因为数据连接已建立。

数据连接是从中获取受众的数据源。 目前，唯一支持的数据连接是Adobe Experience Platform。

您为数据连接配置的任何设置都将应用于来自此数据连接的所有受众。

>[!TIP]
>
>您可以在一个单独的工作流中查看和编辑数据连接。 有关详细信息，请遵循[管理数据连接](/help/guide/setup/manage-data-connection.md)指南。

要开始添加数据连接，请选择&#x200B;**[!UICONTROL 添加新数据连接]**，然后选择&#x200B;**[!UICONTROL 下一步]**。

![突出显示了“添加新数据连接”选项的“添加受众”工作区。](/help/assets/setup/add-manage-audiences/add-data-connection.png){zoomable="yes"}

#### 选择数据源

接下来，您将选择数据连接的源。 可用的源包括：

* **Adobe Experience Platform**：选择此选项可从Adobe Experience Platform引入受众。
* **CSV文件**（未来版本）：上载包含受众数据的CSV文件以快速而直接地摄取数据。
* **Amazon Web Services**：直接从S3存储桶连接到Amazon S3存储以源受众数据。 有关分步说明，请参阅[为受众源配置AWS S3](./configure-aws-s3-audience-sourcing.md)指南。
* **Snowflake**（未来版本）：使用Snowflake数据仓库无缝提取受众数据。
* **Google Cloud Platform**（未来版本）：连接到Google Cloud Storage，以直接从GCS存储桶获取受众数据。

选择数据源，然后选择&#x200B;**[!UICONTROL 下一步]**。

![突出显示了Adobe Experience Platform选项的“添加受众”工作区。](/help/assets/setup/add-manage-audiences/select-data-connection-source.png){zoomable="yes"}

#### 选择沙盒

选择数据源后，必须选择沙盒，其中包含要用于Collaboration的受众。 从可用沙盒列表中选择沙盒，然后选择&#x200B;**[!UICONTROL 下一步]**

![已选中沙盒的“添加受众”工作区。](/help/assets/setup/add-manage-audiences/select-sandbox.png){zoomable="yes"}

#### 治理策略和执行操作 {#governance-policy-and-enforcement-actions}

接下来，您必须确保对来源数据设置了正确的营销操作。 对于源自Experience Platform的数据要用于数据协作，您还需要提供同意。

使用营销操作可以控制要将哪些受众数据从Experience Platform引入Collaboration。 **[!UICONTROL 数据协作]**&#x200B;营销操作支持 C4、C5 和 C9 数据使用标签。**[!UICONTROL 数据科学]**&#x200B;营销操作支持 C9 数据使用标签。

详细了解[C4、C5和C9数据使用标签](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/data-governance/labels/reference#contract){target="_blank"}。

* 当复选框为&#x200B;***已启用***&#x200B;时，Experience Platform中标记如上所述的任何数据都将被排除，**不会**&#x200B;引入Collaboration。
* 禁用复选框&#x200B;***后***，对来自Experience Platform的数据没有限制。

有关数据使用标签的更多信息，请参阅Experience Platform文档：

* [数据使用标签概述](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/data-governance/labels/overview){target="_blank"}
* [数据使用标签术语表](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/data-governance/labels/reference){target="_blank"}

此外，您还需要选择同意规则以应用于源自Collaboration的数据。

![位于治理策略和执行操作部分的“添加受众”工作区。](/help/assets/setup/add-manage-audiences/data-collaboration-consent.png){zoomable="yes"}

选择营销操作和同意规则后，选择&#x200B;**[!UICONTROL 下一步]**&#x200B;以继续执行下一步。 将出现一个确认对话框，要求您接受条款。 选中该复选框，然后选择&#x200B;**[!UICONTROL 确定]**&#x200B;进行确认。

![选中了复选框和“确定”选项的“治理策略和执行操作”对话框。](/help/assets/setup/add-manage-audiences/data-collaboration-consent-confirmation.png){zoomable="yes"}

### 提供详细信息

接下来，提供数据连接的名称和描述。 此信息将帮助您以后识别数据连接。

![添加受众工作区，可选择提供名称和描述。](/help/assets/setup/add-manage-audiences/data-connection-details.png){zoomable="yes"}

### 映射字段 {#map-fields}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_source_fields"
>title="源字段"
>abstract="源字段是来自您的 Experience Platform 实施的身份标识命名空间和属性。您可以将它们映射到 Collaboration 中定义的目标字段。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_target_fields"
>title="目标字段"
>abstract="目标字段是在帐户设置过程中选择的匹配键。默认情况下，您选择的所有匹配键均可用。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_apply_transformation"
>title="应用转换"
>abstract="从来源获取&#x200B;*非哈希*&#x200B;字段时，使用此选项可让 Collaboration 应用哈希算法，将纯文本字段转换为哈希字段。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_identity_namespaces"
>title="身份标识命名空间"
>abstract="从 Experience Platform 组织中可用的标准的及自定义的身份标识命名空间中选择一个身份标识命名空间。"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/identity/features/namespaces.html?lang=zh-Hans#standard" text="Experience Platform 中的标准和身份标识命名空间"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_profile_attributes"
>title="轮廓属性"
>abstract="从 Experience Platform 中的轮廓类的并集架构中选择属性。此视图显示并集架构中存在的属于 XDM 个人轮廓类的属性。"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/profile/union-schemas/union-schema.html?lang=zh-Hans" text="Experience Platform 中的联合架构"

接下来，您将选择要映射到Collaboration中目标字段的源字段。 可用的目标字段将基于您在帐户设置期间选择的匹配键。

>[!IMPORTANT]
>
>目前，您无法编辑数据连接以包含新的映射字段。 如果在创建数据连接后向帐户中添加新的匹配键，则需要创建新数据连接以映射到它们。

![添加受众工作区，可选择将源字段映射到目标字段。](/help/assets/setup/add-manage-audiences/add-map-fields.png){zoomable="yes"}

>[!TIP]
>
>您可以将多个源字段映射到同一个目标字段。 例如，如果您在Experience Platform中的两个单独字段中包含电子邮件地址，则可以将每个地址映射到&#x200B;**[!UICONTROL 哈希电子邮件]**&#x200B;目标字段，作为两个单独的行。 使用&#x200B;**[!UICONTROL 添加字段]**&#x200B;选项添加其他映射行。

>[!BEGINSHADEBOX]

**[!UICONTROL Source字段]**&#x200B;是Experience Platform中的身份命名空间和属性。 这些命名空间包括[标准](https://experienceleague.adobe.com/docs/experience-platform/identity/features/namespaces.html?lang=zh-Hans#standard){target="_blank"}和[自定义](https://experienceleague.adobe.com/docs/experience-platform/identity/features/namespaces.html?lang=zh-Hans#create-namespaces){target="_blank"}身份命名空间。 它们还包含[联合架构](https://experienceleague.adobe.com/docs/experience-platform/profile/union-schemas/union-schema.html?lang=zh-Hans){target="_blank"}中存在的属于XDM个人资料类的个人资料属性。

Source字段会被映射到Collaboration中定义的目标字段。

**[!UICONTROL 目标字段]**&#x200B;指示标识在Collaboration中的引用方式。 目标字段是在帐户设置过程中选择的匹配键。默认情况下，您选择的所有匹配键均可用。

当您将&#x200B;**[!UICONTROL 非哈希]**&#x200B;字段获取到哈希字段时，请使用&#x200B;*应用转换*&#x200B;选项。 Collaboration将应用哈希处理并转换字段。 Adobe使用的哈希算法是SHA256。

>[!ENDSHADEBOX]

要开始映射字段，请选择目标字段旁边的空源字段。 将显示&#x200B;**[!UICONTROL 选择源字段]**&#x200B;对话框。 在&#x200B;**[!UICONTROL 身份命名空间]**&#x200B;和&#x200B;**[!UICONTROL 配置文件属性]**&#x200B;选项之间选择以查找所需的源字段，然后从列表中选择该字段。 您还可以使用搜索选项查找所需字段。

![显示电子邮件选项的“选择源字段”对话框。](/help/assets/setup/add-manage-audiences/select-source-field.png){zoomable="yes"}

若要处理将非哈希字段源补充到哈希目标字段，请使用&#x200B;**[!UICONTROL 应用转换]**&#x200B;选项。 例如，要添加第二个电子邮件字段，请选择&#x200B;**[!UICONTROL 添加字段]**&#x200B;选项以添加新行，然后为目标字段选择&#x200B;**[!UICONTROL 散列电子邮件]**。 选择一个非散列电子邮件源字段，然后选择&#x200B;**[!UICONTROL 应用转换]**。

![将电子邮件源字段映射到目标字段的“添加受众”工作区中的“应用”转换打开。](/help/assets/setup/add-manage-audiences/apply-transformation.png){zoomable="yes"}

继续为每个目标字段添加映射对。 如果您不想使用匹配键，可以使用字段旁边的删除（![删除图标](/help/assets/icons/delete.png)）图标将其删除。 如果删除了匹配键，则在从连接采购任何受众时，您将无法使用该匹配键。

![添加受众工作区，在突出显示的目标字段旁边具有删除选项。](/help/assets/setup/add-manage-audiences/remove-target-field.png){zoomable="yes"}

完成字段映射后，选择&#x200B;**[!UICONTROL 下一步]**&#x200B;以继续。

![“添加受众”工作区中填写了映射字段，并且突出显示了“下一步”选项。](/help/assets/setup/add-manage-audiences/confirm-field-mapping.png){zoomable="yes"}

### 计划 {#schedule}

接下来，安排何时开始和结束填充受众。 受众将按照此计划进行刷新。

![显示计划选项的“添加受众”工作区。](/help/assets/setup/add-manage-audiences/audience-scheduling.png){zoomable="yes"}

>[!IMPORTANT]
>
>调整受众更新的频率将有助于管理[受众管理信用活动](/help/guide/setup/my-activity.md#types-of-activities)，该活动是按受众刷新计算的。 选择更高的频率可能会影响可用于受众发现报告和受众激活的数据的刷新率。

从&#x200B;**[!UICONTROL 频率]**&#x200B;下拉列表中选择受众刷新频率。

![打开“频率”下拉菜单的“添加受众计划”工作区。](/help/assets/setup/add-manage-audiences/audience-scheduling-frequency.png){zoomable="yes"}

接下来，选择&#x200B;**[!UICONTROL 日期范围]**。 开始日期是受众开始填充用户档案的日期，结束日期是受众停止刷新时的日期。

![显示了“添加受众计划工作区”中的“日期范围”选项。](/help/assets/setup/add-manage-audiences/audience-scheduling-date-range.png){zoomable="yes"}

>[!IMPORTANT]
>
>在日期范围内的结束日期之后，来自此数据连接的所有受众将停止刷新。 要续订连接，请按照[管理数据连接](/help/guide/setup/manage-data-connection.md)指南操作。

### 选择受众 {#select-audiences}

选择受众源后，您将选择要包含的特定受众。 使用搜索和筛选选项从数据连接中查找相关受众。 选择所需的受众，然后选择&#x200B;**[!UICONTROL 下一步]**。

![包含可用受众列表的添加受众工作区。](/help/assets/setup/add-manage-audiences/select-audience.png){zoomable="yes"}

### 审查

在最终确定受众添加之前，请查看所有配置和设置。 确保所有详细信息正确，然后选择&#x200B;**[!UICONTROL 完成]**&#x200B;以完成创建数据连接。

![显示所有选定配置的“添加受众”工作区。](/help/assets/setup/add-manage-audiences/review-connection.png){zoomable="yes"}

## 查看受众仪表板 {#view-audiences-dashboard}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_missing_identities"
>title="缺少身份标识"
>abstract="按照配置的计划，身份标识计数将在下一次数据连接刷新后可用。初始刷新通常发生在数据连接建立后的 24 小时内。正在进行的刷新将遵循配置的计划。"

在来源补充受众后，**[!UICONTROL 我的受众]**&#x200B;工作区会显示当前来源于Collaboration的所有受众。

![我的受众工作区显示所有来源受众。](/help/assets/setup/add-manage-audiences/audiences-workspace.png)

每个受众都包含以下信息的概述：

| 项目 | 描述 |
|----------|---------|
| **[!UICONTROL 名称]** | 受众的名称。 |
| **[!UICONTROL 标识]** | 指示此受众中存在的身份数。 请注意，如果同一配置文件具有两个或更多身份，并且这些身份在项目中被用作匹配键，则该配置文件将在计数中显示两次。 |
| **[!UICONTROL 状态]** | 指示受众是否处于活动状态以及是否可以在项目中使用。 **[!UICONTROL Pending]**&#x200B;状态表示受众最近刚获得来源，并且身份尚未填充。 初次刷新后（通常在数据连接设置后的24小时内刷新），源受众将填充用户档案。 |
| **[!UICONTROL Source]** | 指示受众源自何处。 在Collaboration的当前版本中，Experience Platform是唯一受支持的源。 |
| **[!UICONTROL 数据连接]** | 受众来源的数据连接。 您可以选择名称以查看数据连接。 |
| **[!UICONTROL 连接访问]** | 定义受众是私有还是公共。 公共受众可在重叠报表中找到，并可在项目中激活。 |
| **[!UICONTROL 已创建]** | 指示受众最初来源于Collaboration的时间。 |
| **[!UICONTROL 上次更新时间]** | 指示在Collaboration中更新受众的最后日期和时间。 这并非指上次刷新受众的时间，而是指上次更改受众配置或元数据的时间。 |

![我的受众工作区显示所有来源受众。](/help/assets/setup/add-manage-audiences/audiences-workspace.png){zoomable="yes"}

要对受众执行快速操作，请选择受众名称旁边的省略号&#x200B;**...**。 可以使用以下选项：

* **[!UICONTROL 编辑类别]**&#x200B;允许您向受众添加不同的类别标记。 有关详细信息，请参阅下面的[类别](#categories)部分。
* **[!UICONTROL 删除]**&#x200B;将从数据连接中删除受众。

![我的受众工作区中打开了省略号菜单，并突出显示了“编辑类别”和“删除”选项。](/help/assets/setup/add-manage-audiences/audiences-ellipsis-menu.png){zoomable="yes"}

## 查看单个受众 {#view-individual-audiences}

要查看和更新单个受众的信息，请从&#x200B;**[!UICONTROL 我的受众]**&#x200B;工作区中选择受众。 受众工作区显示有关所选受众的详细信息，包括其详细信息、标识、类别、连接访问和元数据可见性设置。

### 受众详情

将显示每个受众的以下信息：

| 项目 | 描述 |
|----------|---------|
| **[!UICONTROL 状态]** | 指示受众是否处于活动状态以及是否可以在项目中使用。 |
| **[!UICONTROL Source]** | 指示受众源自何处。 在Collaboration的当前版本中，Experience Platform是唯一受支持的源。 |
| **[!UICONTROL 数据连接]** | 受众来源的数据连接。 |
| **[!UICONTROL 上次更新时间]** | 指示在Collaboration中更新受众的最后日期和时间。 这并非指上次刷新受众的时间，而是指上次更改受众配置或元数据的时间 |
| **[!UICONTROL 上次更新者]** | 指示上次更新受众的用户。 |
| **[!UICONTROL 已创建]** | 指示受众最初来源于Collaboration的时间。 |
| **[!UICONTROL 创建者]** | 指示将受众来源于Collaboration的用户。 |

![单个受众的工作区。](/help/assets/setup/add-manage-audiences/audience-details.png){zoomable="yes"}

#### 身份标识 {#identities}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_identities"
>title="身份标识"
>abstract="按匹配键划分的构成该受众的身份标识细分视图。"

**[!UICONTROL Identities]**&#x200B;部分指示受众中存在的身份数。 部分还包含按匹配键对身份进行的身份细分，以帮助您了解受众的组成。

![单个受众工作区的“身份”部分。](/help/assets/setup/add-manage-audiences/audience-details-identities.png){zoomable="yes"}

将鼠标悬停在匹配键划分的各个部分上将会提供有关键的准确身份计数。

![显示具有匹配键的划分的个人受众工作区的“身份”部分。](/help/assets/setup/add-manage-audiences/audience-details-identities.png)

#### 类别 {#categories}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_categories"
>title="类别"
>abstract="标记您的受众，以便进行组织、筛选和检索。您可以使用多个类别标记受众，然后在产品的其他区域中使用这些类别标记筛选所需的受众。"

为便于受众的组织、筛选和检索，您可以标记受众。 您可以为具有多个类别的受众添加标签，然后在运行受众重叠报表时，使用这些类别标签在[发现](/help/guide/collaborate/discover.md)产品区域中过滤所需的受众。

要添加类别，请选择&#x200B;**[!UICONTROL 类别]**&#x200B;部分中的&#x200B;**[!UICONTROL 编辑]**&#x200B;选项。

![单个受众工作区的“类别”部分。](/help/assets/setup/add-manage-audiences/audience-details-categories.png){zoomable="yes"}

将显示&#x200B;**[!UICONTROL 类别]**&#x200B;对话框，允许您选择要添加到受众的类别。 要选择单个类别，请选中类别名称旁边的复选框。


#### 连接访问权限 {#connection-access}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_connection_access"
>title="连接访问权限"
>abstract="<p>受众可以分为三种类型：公共、私人和自定义。</p><p> 它们在与协作者合作的项目中是否可用取决于连接访问权限设置。</p>"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_access"
>title="了解更多信息"
>abstract=""

与协作者一起使用的项目中的受众可用性因连接访问设置而异。 在&#x200B;**[!UICONTROL 连接访问]**&#x200B;部分中，您可以选择受众是私有受众、公共受众还是仅适用于特定连接。 公共受众在连接中可用且可发现。

要更新受众的连接访问权限，请在&#x200B;**[!UICONTROL 连接访问]**&#x200B;部分中选择&#x200B;**[!UICONTROL 编辑]**&#x200B;选项。

![单个受众工作区的“连接访问”部分。](/help/assets/setup/add-manage-audiences/audience-details-connection-access.png){zoomable="yes"}

此时将显示&#x200B;**[!UICONTROL 连接访问]**&#x200B;对话框，其中包含三个可用的连接访问选项：

* **[!UICONTROL 专用受众]**。 这些受众&#x200B;*不*&#x200B;可用于重叠报表中或与任何协作者建立连接进行激活。 虽然受众不可供协作者查看或使用，但受众群体仍占&#x200B;**[!UICONTROL 比较受众部分]**&#x200B;中[所有受众](/help/guide/collaborate/discover.md#compare-audiences)视图的总群体的比例。 将设置更改为“公用”或“自定义”，以便将受众与协作者关联使用。
* **[!UICONTROL 公共受众]**。 这些受众可用于重叠报表中，并可用于与任何协作者建立连接以进行激活。
* **[!UICONTROL 自定义受众]**。 这些受众只能在重叠报表中使用，并且只能在指定的连接中进行激活。 虽然受众不可供协作者查看或使用，但受众群体仍占&#x200B;**[!UICONTROL 比较受众部分]**&#x200B;中[所有受众](/help/guide/collaborate/discover.md#compare-audiences)视图的总群体的比例。

选择所需的连接访问选项，然后选择&#x200B;**[!UICONTROL 保存]**&#x200B;以应用更改。

![显示具有可用选项的“连接访问”对话框。](/help/assets/setup/add-manage-audiences/audience-details-connection-access-dialog.png){zoomable="yes"}

>[!IMPORTANT]
>
>无论访问状态（公用、专用或自定义）如何，任何受众的群体都会为项目中&#x200B;**[!UICONTROL 比较受众]**&#x200B;分区的&#x200B;**[!UICONTROL 所有受众]**&#x200B;群体贡献内容。

与协作者一起使用的项目中的受众可用性因连接访问设置而异。

#### 元数据可见性 {#metadata-visibility}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_metadata_visibility"
>title="元数据可见性"
>abstract="<p>说明其他协作者在与您连接之前或在项目视图中可以看到哪些受众的元数据。</p> <p> **身份标识计数**&#x200B;决定了您的协作者在“发现”选项卡中查看重叠报告时是否可以看到您受众的身份标识计数。</p><p> **受众重叠率**&#x200B;决定了协作者是否能够看到他们的受众与您的受众之间的重叠百分比。</p><p> **[!UICONTROL 受众指数]**&#x200B;决定了协作者是否可以看到某个项目中的受众指数。您必须具有三个或更多活跃的受众，此功能才可用。</p> <br> 为了使元数据可见性设置生效，必须将受众设置为公开或自定义。"

>[!NOTE]
>
>如果您的协作者将所有受众都设置为私有，则项目的&#x200B;**[!UICONTROL 发现]**&#x200B;工作区中的&#x200B;**[!UICONTROL 相关受众]**&#x200B;部分将为空白。 有关详细信息，请阅读[发现](/help/guide/collaborate/discover.md#relevant-audiences)指南。

元数据可见性表示受众的元数据在其他协作者与您连接之前或在不同的项目视图中是否可见。 要更新受众的元数据可见性，请选择&#x200B;**[!UICONTROL 元数据可见性]**&#x200B;部分中的&#x200B;**[!UICONTROL 编辑]**&#x200B;选项。

![单个受众工作区的“元数据可见性”部分。](/help/assets/setup/add-manage-audiences/audience-details-metadata-visibility.png){zoomable="yes"}

将显示&#x200B;**[!UICONTROL 元数据可见性]**&#x200B;对话框，允许您配置受众的可见性设置。 您可以为每个受众配置两个元数据可见性设置：

**[!UICONTROL 显示身份计数]**：此设置控制当[在项目的“发现”选项卡](/help/guide/collaborate/discover.md#discover-overlaps)中查看重叠报告时，您的协作者是否可以查看受众的身份计数。

**[!UICONTROL 显示受众重叠%]**：此设置控制协作者是否能够在其受众和您的受众之间[发现重叠百分比](/help/guide/collaborate/discover.md#compare-audiences)。

**[!UICONTROL 受众索引]**：设置为true时，您的协作者可以查看项目中的[受众索引](/help/guide/collaborate/discover.md#audience-index-score)。 您必须具有三个或更多活跃的受众，此功能才可用。

>[!NOTE]
>
>要使元数据可见性设置生效，必须将受众设置为“公用”或“自定义”。

![显示具有可用选项的“元数据可见性”对话框。](/help/assets/setup/add-manage-audiences/audience-details-metadata-dialog.png){zoomable="yes"}

## 编辑多个受众 {#edit-audiences}

在受众仪表板中，您可以同时编辑多个受众。 要执行此操作，请选中要编辑的受众名称旁边的复选框。 选择受众后，您可以使用编辑菜单中提供的选项执行操作。

![选定了两个受众且编辑菜单突出显示的我的受众工作区。](/help/assets/setup/add-manage-audiences/audiences-bulk-edit.png)

### 批量编辑元数据可见性 {#bulk-edit-metadata-visibility}

在受众仪表板中选择受众后，从编辑菜单中选择&#x200B;**[!UICONTROL 编辑元数据可见性]**。

![突出显示了“编辑元数据可见性”选项的“我的受众”工作区。](/help/assets/setup/add-manage-audiences/audiences-bulk-edit-metadata.png)

此时将显示&#x200B;**[!UICONTROL 元数据可见性]**&#x200B;对话框，允许您配置所选受众的可见性设置。 默认情况下，不会选择任何选项。 选择要应用于所有选定受众的选项，然后选择&#x200B;**[!UICONTROL 保存]**。

![显示具有可用选项的“元数据可见性”对话框。](/help/assets/setup/add-manage-audiences/audience-details-metadata-dialog.png)

### 批量编辑连接访问权限 {#bulk-edit-connection-access}

在受众仪表板中选择受众后，从编辑菜单中选择&#x200B;**[!UICONTROL 编辑连接访问权限]**。

![突出显示具有“编辑连接”访问权限选项的“我的受众”工作区。](/help/assets/setup/add-manage-audiences/audiences-bulk-edit-connection-access.png)

将显示&#x200B;**[!UICONTROL 连接访问]**&#x200B;对话框，允许您为所选受众配置访问设置。 默认情况下，将选择&#x200B;**[!UICONTROL 专用受众]**&#x200B;选项。 选择要应用于所有选定受众的选项，然后选择&#x200B;**[!UICONTROL 保存]**。

![显示具有可用选项的“连接访问”对话框。](/help/assets/setup/add-manage-audiences/audience-details-connection-access-dialog.png)

### 批量编辑受众名称和描述 {#bulk-edit-audience-names-descriptions}

在受众仪表板中选择受众后，从编辑菜单中选择&#x200B;**[!UICONTROL 编辑名称和描述]**。

![突出显示了“编辑名称和描述”选项的“我的受众”工作区。](/help/assets/setup/add-manage-audiences/audiences-bulk-edit-name-description.png)

**[!UICONTROL 名称和描述]**&#x200B;对话框出现，允许您为每个选定的受众配置名称和描述。 默认情况下，将显示每个受众的当前名称和描述。 进行更改，然后选择&#x200B;**[!UICONTROL 保存]**。

![显示具有可用选项的“名称和描述”对话框。](/help/assets/setup/add-manage-audiences/audiences-bulk-edit-name-description-dialog.png)

### 批量编辑类别 {#bulk-edit-categories}

在受众仪表板中选择受众后，从编辑菜单中选择&#x200B;**[!UICONTROL 编辑类别]**。

![突出显示了“编辑类别”选项的“我的受众”工作区。](/help/assets/setup/add-manage-audiences/audiences-bulk-edit-categories.png)

将显示&#x200B;**[!UICONTROL 类别]**&#x200B;对话框，允许您为每个所选受众配置类别。 默认情况下，不会选择任何类别。 要选择类别，请先选择主类别，然后选择要包含的子类别。 进行更改，然后选择&#x200B;**[!UICONTROL 保存]**。

![显示具有可用选项的“类别”对话框。](/help/assets/setup/add-manage-audiences/audiences-bulk-edit-categories-dialog.png)

## 后续步骤

在获取受众源后，是时候发现与进行[连接](/help/guide/connect/establishing-connections.md)的协作者以协作项目了。
