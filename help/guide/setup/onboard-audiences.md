---
title: 导入和管理受众
description: 了解如何在Adobe Real-Time CDP Collaboration中导入和管理受众
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/cn/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 0a5158fa-73d3-4406-af20-2b6c7be9934e
source-git-commit: fda414120decc0c76712616ff85b83febede53e9
workflow-type: tm+mt
source-wordcount: '2961'
ht-degree: 20%

---

# 导入和管理受众

{{limited-availability-release-note}}

受众是根据各种属性划分的特定用户或客户组。 这些功能使广告商和发布商能够协作进行有针对性的营销和个性化体验，从而更有效地进行广告宣传。

使用此页面作为您的登录信息，了解您可以查看的所有与受众相关的量度，以及将受众导入Adobe Real-Time CDP Collaboration的工作流步骤。

>[!TIP]
>
>使用此屏幕中的信息可获取有关受众所需的所有信息，并且[发现并重叠屏幕](/help/guide/collaborate/discover.md)可深入了解哪些受众最适合不同的营销活动类型（与发布者库存相比）。

>[!BEGINSHADEBOX]

您可以在此文档页面上找到以下内容：

* [将受众导入Real-Time CDP Collaboration](#import-audiences)
* [查看受众仪表板](#view-audiences-dashboard)
* [查看单个受众](#view-individual-audiences)

>[!ENDSHADEBOX]

## 将受众导入Real-Time CDP Collaboration {#import-audiences}

>[!IMPORTANT]
>
>要导入受众，需要将您的用户分配到包含两个配置文件管理权限的角色 — 查看配置文件和查看区段。 有关分配必要权限的信息，请参阅[受众导入](../permissions/overview.md#audience-importation)指南。

需要先将受众导入到Real-Time CDP Collaboration中，然后才能通过协作者激活受众并运行重叠计算。 要导入受众，请按照以下部分中的工作流步骤操作。

从&#x200B;**[!UICONTROL 步骤]**&#x200B;工作区的&#x200B;**[!UICONTROL 我的受众]**&#x200B;选项卡中选择添加图标（![添加图标）。](/help/assets/icons/plus.png))或&#x200B;**[!UICONTROL 添加]选项**，然后选择&#x200B;**受众**。

![突出显示了“添加”选项和“受众”选项的“我的受众”工作区。](/help/assets/setup/add-manage-audiences/add-audiences.png)

### 选择数据连接 {#select-data-connection}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_marketing_actions"
>title="营销操作"
>abstract="<p>使用营销操作来控制从 Experience Platform 向 Real-Time CDP Collaboration 导入哪些受众数据。<strong>数据协作</strong>营销操作支持 C4、C5 和 C9 数据使用标签。<strong>数据科学</strong>营销操作支持 C9 数据使用标签。</p> <p> <ul><li> <em>启用</em>该复选框后，Experience Platform 中标有上述标签的任何数据都会被排除，并且<strong>不</strong>被纳入 Real-Time CDP Collaboration。</li><li> <em>禁用</em>该复选框后，从 Experience Platform 导入 Real-Time CDP Collaboration 的数据不受限制。</li></ul></p>"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/data-governance/labels/overview.html?lang=zh-Hans" text="数据使用标签概述"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/data-governance/labels/reference.html?lang=zh-Hans" text="数据使用标签词汇表"

>[!IMPORTANT]
>
>在建立到您的第一个数据连接并导入第一个受众后，您可以从现有数据连接导入多个受众。 添加其他受众时，您将从[选择受众](#select-audience)步骤开始，因为其他步骤中的所有先决条件信息都将从现有连接导入。

数据连接是从中将受众导入Real-Time CDP Collaboration的数据源。 目前，唯一支持的数据连接是Adobe Experience Platform。

您为数据连接配置的任何设置（例如计划）都会应用于从此数据连接导入的所有受众。

>[!TIP]
>
>您可以在一个单独的工作流中查看和编辑数据连接。 有关详细信息，请遵循[管理数据连接](/help/guide/setup/manage-data-connection.md)指南。

若要开始添加数据连接，请选择&#x200B;**[!UICONTROL 添加新数据连接]**，然后选择&#x200B;**[!UICONTROL 下一步]**。

![突出显示了“添加新数据连接”选项的“添加受众”工作区。](/help/assets/setup/add-manage-audiences/add-data-connection.png)

#### 选择数据源

接下来，您将选择数据连接的源。 可用的源包括：

* **Adobe Experience Platform**：选择此选项可从Adobe Experience Platform Real-Time CDP引入受众。
* **CSV文件**（未来版本）：上载包含受众数据的CSV文件以快速而直接地摄取数据。
* **Amazon Web Services**（未来版本）：连接到您的Amazon S3存储，以直接从S3存储桶导入受众数据。
* **Snowflake**（未来版本）：使用Snowflake数据仓库无缝提取受众数据。

选择您的数据源，然后选择&#x200B;**[!UICONTROL 下一步]**。

![突出显示了Adobe Experience Platform选项的“添加受众”工作区。](/help/assets/setup/add-manage-audiences/select-data-connection-source.png)

#### 选择沙盒

选择数据源后，必须选择包含将要导入的受众的沙盒。 从可用沙盒列表中选择沙盒，然后选择&#x200B;**[!UICONTROL 下一步]**

![已选中沙盒的“添加受众”工作区。](/help/assets/setup/add-manage-audiences/select-sandbox.png)

#### 治理策略和实施行动 {#governance-policy-and-enforcement-actions}

接下来，必须确保对导入的数据设置正确的营销操作。 您还需要同意从Real-Time CDP导入用于数据协作的数据。

使用营销操作来控制从 Experience Platform 向 Real-Time CDP Collaboration 导入哪些受众数据。**数据协作**&#x200B;营销操作支持 C4、C5 和 C9 数据使用标签。**数据科学**&#x200B;营销操作支持 C9 数据使用标签。

详细了解[C4、C5和C9数据使用标签](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/data-governance/labels/reference#contract){target="_blank"}。

* *启用*&#x200B;该复选框后，Experience Platform 中标有上述标签的任何数据都会被排除，并且&#x200B;*不*&#x200B;被纳入 Real-Time CDP Collaboration。
* *禁用*&#x200B;该复选框后，从 Experience Platform 导入 Real-Time CDP Collaboration 的数据不受限制。

有关数据使用标签的更多信息，请参阅Experience Platform文档：

* [数据使用标签概述](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/data-governance/labels/overview){target="_blank"}
* [数据使用标签术语表](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/data-governance/labels/reference){target="_blank"}

此外，您还需要选择conset规则以应用于要导入Real-Time CDP Collaboration的数据。

![位于治理策略和执行操作部分的“添加受众”工作区。](/help/assets/setup/add-manage-audiences/data-collaboration-consent.png)

选择营销操作和同意规则后，选择&#x200B;**[!UICONTROL 下一步]**&#x200B;以继续执行下一步。 将出现一个确认对话框，要求您接受条款。 选中该复选框，然后选择&#x200B;**[!UICONTROL 确定]**&#x200B;进行确认。

![选中了复选框和“确定”选项的“治理策略和执行操作”对话框。](/help/assets/setup/add-manage-audiences/data-collaboration-consent-confirmation.png)

### 提供详细信息

接下来，提供数据连接的名称和描述。 此信息将帮助您以后识别数据连接。

![添加受众工作区，可选择提供名称和描述。](/help/assets/setup/add-manage-audiences/data-connection-details.png)

### 映射字段 {#map-fields}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_source_fields"
>title="源字段"
>abstract="源字段是来自您现有的 Real-Time CDP 实施的身份标识命名空间和属性。您可以将它们映射到 Real-Time CDP Collaboration 中定义的目标字段。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_target_fields"
>title="目标字段"
>abstract="目前，经过哈希处理的电子邮件是唯一受支持的匹配键。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_apply_transformation"
>title="应用转换"
>abstract="从来源导入&#x200B;*非哈希*&#x200B;字段时，使用此选项可让 Real-Time CDP Collaboration 应用哈希算法，将纯文本字段转换为哈希字段。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_identity_namespaces"
>title="身份标识命名空间"
>abstract="从 Experience Platform 组织中可用的标准的及自定义的身份标识命名空间中选择一个身份标识命名空间。"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/identity/features/namespaces.html?lang=zh-Hans#standard" text="Experience Platform 中的标准和身份标识命名空间"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_profile_attributes"
>title="轮廓属性"
>abstract="从 Experience Platform 中的轮廓类的联合架构中选择属性。此视图显示联合架构中存在的且属于 XDM 个人轮廓类的属性。"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/profile/union-schemas/union-schema.html?lang=zh-Hans" text="Experience Platform 中的联合架构"

接下来，您将选择要映射到Real-Time CDP Collaboration中目标字段的源字段。

![添加受众工作区，可选择将源字段映射到目标字段。](/help/assets/setup/add-manage-audiences/add-map-fields.png)

>[!TIP]
>
>您可以将多个源字段映射到同一个目标字段。 例如，如果在Experience Platform中的两个单独字段中都有电子邮件地址，则可以将这两个地址映射到&#x200B;**[!UICONTROL 哈希电子邮件]**&#x200B;目标字段作为两个单独的行。

>[!BEGINSHADEBOX]

**[!UICONTROL Source字段]**&#x200B;是来自您现有Real-Time CDP实施的身份命名空间和属性。 这些是标识在从中导入数据的源中的存在方式。 Source字段会被映射到Real-Time CDP Collaboration中定义的目标字段。

**[!UICONTROL 目标字段]**&#x200B;指示标识在Real-Time CDP Collaboration中的引用方式。 目前，经过哈希处理的电子邮件是唯一受支持的匹配键。

当您从源导入&#x200B;*非散列*&#x200B;字段时，请使用&#x200B;**[!UICONTROL 应用转换]**&#x200B;选项。 在这种情况下，Real-Time CDP Collaboration将应用哈希并转换字段。 Adobe使用的哈希算法是SHA256。

>[!ENDSHADEBOX]

选择目标字段旁边的空源字段。 将显示&#x200B;**[!UICONTROL 选择源字段]**&#x200B;对话框。 在&#x200B;**[!UICONTROL 身份命名空间]**&#x200B;和&#x200B;**[!UICONTROL 配置文件属性]**&#x200B;选项之间选择以查找所需的源字段，然后从列表中选择源字段，并使用搜索选项查找所需的字段。

![显示电子邮件选项的“选择源字段”对话框。](/help/assets/setup/add-manage-audiences/select-source-field.png)

若要处理多个电子邮件字段，请使用&#x200B;**[!UICONTROL 应用转换]**&#x200B;映射非散列电子邮件源字段。

![将电子邮件源字段映射到目标字段的“添加受众”工作区中的“应用”转换打开。](/help/assets/setup/add-manage-audiences/apply-transformation.png)

根据需要继续添加映射对，然后选择&#x200B;**[!UICONTROL 下一步]**。

### 计划 {#schedule}

接下来，安排何时开始和结束填充受众。 受众将按照此计划进行刷新。

![显示计划选项的“添加受众”工作区。](/help/assets/setup/add-manage-audiences/audience-scheduling.png)

>[!IMPORTANT]
>
>调整受众更新的频率将有助于管理[受众管理信用活动](/help/guide/setup/my-activity.md#types-of-activities)，该活动是按受众刷新计算的。 选择更高的频率可能会影响可用于受众发现报告和受众激活的数据的刷新率。

从&#x200B;**[!UICONTROL 频率]**&#x200B;下拉列表中选择受众刷新频率。

![打开“频率”下拉菜单的“添加受众计划”工作区。](/help/assets/setup/add-manage-audiences/audience-scheduling-frequency.png)

接下来，选择&#x200B;**[!UICONTROL 日期范围]**。 开始日期是受众开始填充用户档案的日期，结束日期是受众停止刷新时的日期。

![显示了“添加受众计划工作区”中的“日期范围”选项。](/help/assets/setup/add-manage-audiences/audience-scheduling-date-range.png)

>[!IMPORTANT]
>
>在日期范围内的结束日期之后，从此数据连接导入的所有受众将停止刷新。 若要续订连接，请转到[管理数据连接](/help/guide/setup/manage-data-connection.md)，并设置新的结束日期。

### 选择受众 {#select-audience}

选择受众源后，您将选择要包含的特定受众。 使用搜索和筛选选项从数据源查找相关受众。 选择所需的受众，然后选择&#x200B;**[!UICONTROL 下一步]**。

![包含可用受众列表的添加受众工作区。](/help/assets/setup/add-manage-audiences/select-audience.png)

### 审查

在最终确定受众添加之前，请查看所有配置和设置。 确保所有详细信息正确，然后选择&#x200B;**[!UICONTROL 完成]**&#x200B;以完成创建数据连接。

![显示所有选定配置的“添加受众”工作区。](/help/assets/setup/add-manage-audiences/review-connection.png)

## 查看受众仪表板 {#view-audiences-dashboard}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_missing_identities"
>title="缺少身份标识"
>abstract="按照配置的计划，身份标识计数将在下一次数据连接刷新后可用。初始刷新通常发生在数据连接建立后的 24 小时内。正在进行的刷新将遵循配置的计划。 "

将受众导入Real-Time CDP Collaboration后，**[!UICONTROL 我的受众]**&#x200B;工作区会显示您的组织当前导入到Real-Time CDP Collaboration中的所有受众。


每个受众都包含以下信息的概述：

| 项目 | 描述 |
|----------|---------|
| **[!UICONTROL 标识]** | 指示此受众中存在的身份数。 请注意，如果同一配置文件具有两个或更多身份，并且这些身份在项目中被用作匹配键，则该配置文件将在计数中显示两次。 |
| **[!UICONTROL 状态]** | 指示受众是否处于活动状态以及是否可以在项目中使用。 **[!UICONTROL 待处理]**&#x200B;状态表示受众最近刚刚导入，且受众成员尚未填充。 导入的受众将在初始刷新后填充用户档案，初始刷新通常发生在设置数据连接后的24小时内。 |
| **[!UICONTROL Source]** | 指示从中导入受众的源。 在Real-Time CDP Collaboration的当前版本中，Adobe Experience Platform是唯一受支持的源。 |
| **[!UICONTROL 数据连接]** | 受众来源的数据连接。 您可以选择名称以查看数据连接。 |
| **[!UICONTROL 连接访问]** | 定义受众是私有还是公共。 公共受众可在重叠报表中找到，并可在项目中激活。 |
| **[!UICONTROL 已创建]** | 指示将受众导入到Real-Time CDP Collaboration中的时间。 |
| **[!UICONTROL 上次更新时间]** | 指示上次更新受众任何方面的日期和时间。 |

![我的受众工作区显示所有已导入的受众。](/help/assets/setup/add-manage-audiences/audiences-workspace.png)

要对受众执行快速操作，请选择受众名称旁边的省略号&#x200B;**...**。 可以使用以下选项：

* **[!UICONTROL 编辑类别]**&#x200B;允许您向受众添加不同的类别标记。 有关详细信息，请参阅下面的[类别](#categories)部分。
* **[!UICONTROL 删除]**&#x200B;将从数据连接中删除受众。

![我的受众工作区中打开了省略号菜单，并突出显示了“编辑类别”和“删除”选项。](/help/assets/setup/add-manage-audiences/audiences-ellipsis-menu.png)

## 查看单个受众 {#view-individual-audiences}

要查看单个受众的更多信息并编辑其配置，请从&#x200B;**[!UICONTROL 我的受众]**&#x200B;工作区中选择该受众。 受众工作区显示有关所选受众的详细信息，包括其详细信息、标识、类别、连接访问和元数据可视化设置。

### 受众详情

将显示每个受众的以下信息：

| 项目 | 描述 |
|----------|---------|
| **[!UICONTROL 状态]** | 指示受众是否处于活动状态以及是否可以在项目中使用。 |
| **[!UICONTROL Source]** | 指示从中导入受众的源。 在Real-Time CDP Collaboration的当前版本中，Adobe Experience Platform是唯一受支持的源。 |
| **[!UICONTROL 数据连接]** | 受众来源的数据连接。 |
| **[!UICONTROL 上次更新时间]** | 指示上次更新受众的日期和时间。 |
| **[!UICONTROL 上次更新者]** | 指示上次更新受众的用户。 |
| **[!UICONTROL 已创建]** | 指示将受众导入到Real-Time CDP Collaboration中的时间。 |
| **[!UICONTROL 创建者]** | 指示将受众导入Real-Time CDP Collaboration的用户。 |

![单个受众的工作区。](/help/assets/setup/add-manage-audiences/audience-details.png)

此外，受众工作区中还提供以下控件：

* **[!UICONTROL 删除]**：从数据连接中删除受众。
* **[!UICONTROL 编辑]**：编辑受众的名称或描述。

![突出显示了“编辑并删除”选项的单个受众的工作区。](/help/assets/setup/add-manage-audiences/audience-details-edit-delete.png)

接下来，您可以在受众的工作区中更新以下部分：

* [身份标识](#identities)
* [类别](#categories)
* [连接访问权限](#connection-access)
* [元数据可见性](#metadata-visibility)

### 身份标识 {#identities}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_identities"
>title="身份标识"
>abstract="展示构成该受众的身份标识明细视图，并显示每类身份标识所对应的轮廓总数。"

**[!UICONTROL 标识]**&#x200B;部分指示在导入受众时选定任何标识的受众中存在的配置文件数。 部分还包含身份细分，以便您分辨哪些身份构成了最多的受众群体。

![单个受众工作区的“身份”部分。](/help/assets/setup/add-manage-audiences/audience-details-identities.png)

### 类别 {#categories}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_categories"
>title="类别"
>abstract="标记您的受众，以便进行组织、筛选和检索。您可以使用多个类别标记受众，然后在产品的其他区域中使用这些类别标记筛选所需的受众。"

为便于受众的组织、筛选和检索，您可以标记受众。 您可以为具有多个类别的受众添加标签，然后在运行受众重叠报表时，使用这些类别标签在[发现](/help/guide/collaborate/discover.md)产品区域中过滤所需的受众。

要添加类别，请选择&#x200B;**[!UICONTROL 类别]**&#x200B;部分中的&#x200B;**[!UICONTROL 编辑]**&#x200B;选项。

![单个受众工作区的“类别”部分。](/help/assets/setup/add-manage-audiences/audience-details-categories.png)

将显示&#x200B;**[!UICONTROL 类别]**&#x200B;对话框，允许您选择要添加到受众的类别。 要选择单个类别，请选中类别名称旁边的复选框。

![显示具有可用类别的“类别”对话框。](/help/assets/setup/add-manage-audiences/audience-details-categories-select.png)

### 连接访问权限 {#connection-access}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_connection_access"
>title="连接访问权限"
>abstract="<p>受众可以分为三种类型：公共、私人和自定义。</p><p> 它们在与协作者合作的项目中是否可用取决于连接访问权限设置。您始终可以将连接访问权限从私有更改为公开，但一旦与协作者共同激活了某个受众，该设置将无法恢复为私有。</p>"

与协作者一起使用的项目中的受众可用性因连接访问设置而异。 在&#x200B;**[!UICONTROL 连接访问]**&#x200B;部分中，您可以选择受众是私有受众，还是可用且可在连接中发现。

要更新受众的连接访问权限，请在&#x200B;**[!UICONTROL 连接访问]**&#x200B;部分中选择&#x200B;**[!UICONTROL 编辑]**&#x200B;选项。

![单个受众工作区的“连接访问”部分。](/help/assets/setup/add-manage-audiences/audience-details-connection-access.png)

此时将显示&#x200B;**[!UICONTROL 连接访问]**&#x200B;对话框，其中包含三个可用的连接访问选项：

* **[!UICONTROL 专用受众]**。 这些受众&#x200B;*不*&#x200B;可用于重叠报表中或与任何协作者建立连接进行激活。 虽然受众不可供协作者查看或使用，但受众群体仍占[比较受众部分](/help/guide/collaborate/discover.md#compare-audiences)中&#x200B;**[!UICONTROL 所有受众]**&#x200B;视图的总群体的比例。 将设置更改为“公用”或“自定义”，以便将受众与协作者关联使用。
* **[!UICONTROL 公共受众]**。 这些受众可用于重叠报表中，并可用于与任何协作者建立连接以进行激活。
* **[!UICONTROL 自定义受众]**。 这些受众只能在重叠报表中使用，并且只能在指定的连接中进行激活。 虽然受众不可供协作者查看或使用，但受众群体仍占[比较受众部分](/help/guide/collaborate/discover.md#compare-audiences)中&#x200B;**[!UICONTROL 所有受众]**&#x200B;视图的总群体的比例。

选择所需的连接访问选项，然后选择&#x200B;**[!UICONTROL 保存]**&#x200B;以应用更改。

![显示具有可用选项的“连接访问”对话框。](/help/assets/setup/add-manage-audiences/audience-details-connection-access-dialog.png)

>[!IMPORTANT]
>
>无论访问状态（公用、专用或自定义）如何，任何受众的群体都会为项目内&#x200B;**[!UICONTROL 比较受众]**&#x200B;分区中的&#x200B;**[!UICONTROL 所有受众]**&#x200B;群体贡献内容。<br>

与协作者一起使用的项目中的受众可用性因连接访问设置而异。 您始终可以将连接访问权限从专用更改为公用，但一旦激活受众，您就无法再更改此设置。

### 元数据可见性 {#metadata-visibility}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_metadata_visibility"
>title="元数据可见性"
>abstract="<p>指示在其他组织与您的组织建立连接之前，哪些受众元数据对其可见。 </p> <p> **身份标识计数**&#x200B;控制了您的合作伙伴在“发现”选项卡中查看重叠报告时是否可以查看您受众的身份标识计数。**受众重叠率**&#x200B;控制了协作者是否能够发现他们的受众与您的受众之间的重叠百分比。"

>[!NOTE]
>
>如果您的协作者将所有受众都设置为私有，则项目的&#x200B;**[!UICONTROL 发现]**&#x200B;工作区中的&#x200B;**[!UICONTROL 相关受众]**&#x200B;部分将为空白。 有关详细信息，请阅读[发现](/help/guide/collaborate/discover.md#relevant-audiences)。 指南。

元数据可见性表示受众的元数据在连接到您的组织之前在其他组织中或在不同的项目视图中可见。 要更新受众的元数据可见性，请选择&#x200B;**[!UICONTROL 元数据可见性]**&#x200B;部分中的&#x200B;**[!UICONTROL 编辑]**&#x200B;选项。

![单个受众工作区的“元数据可见性”部分。](/help/assets/setup/add-manage-audiences/audience-details-metadata.png)

将显示&#x200B;**[!UICONTROL 元数据可见性]**&#x200B;对话框，允许您配置受众的可见性设置。 您可以为每个受众配置两个元数据可见性设置：

**[!UICONTROL 显示身份计数]**：此设置控制当[在项目的“发现”选项卡](/help/guide/collaborate/discover.md#discover-overlaps)中查看重叠报告时，您的协作者是否可以查看受众的身份计数。

**[!UICONTROL 显示受众重叠%]**：如果设置为true，协作者将能够在其受众和您的受众之间[发现重叠百分比](/help/guide/collaborate/discover.md#compare-audiences)。

![显示具有可用选项的“元数据可见性”对话框。](/help/assets/setup/add-manage-audiences/audience-details-metadata-dialog.png)

## 后续步骤

导入受众后，是时候发现[连接](/help/guide/connect/establishing-connections.md)的发布者并开始协作项目了。
