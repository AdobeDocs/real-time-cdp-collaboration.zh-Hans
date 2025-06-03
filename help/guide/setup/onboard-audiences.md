---
title: 导入和管理受众
description: 了解如何在Adobe Real-Time CDP Collaboration中导入和管理受众
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 0a5158fa-73d3-4406-af20-2b6c7be9934e
source-git-commit: dd1386f9371cb40285315d11e07b139d3115e147
workflow-type: tm+mt
source-wordcount: '2685'
ht-degree: 24%

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

在与协作者共享受众并运行重叠计算之前，需要将受众导入Real-Time CDP Collaboration。 要导入受众，请按照以下部分中的工作流步骤操作。

![将任何受众添加到组织之前，我的受众屏幕。](/help/assets/setup/add-manage-audiences/org-without-audiences-added.png)

从&#x200B;**[!UICONTROL 我的受众]**&#x200B;选项卡中，选择加号&#x200B;**+**&#x200B;符号，然后选择&#x200B;**受众**。

### 选择数据连接 {#select-data-connection}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_marketing_actions"
>title="营销操作"
>abstract="<p>使用营销操作来控制从 Experience Platform 向 Real-Time CDP Collaboration 导入哪些受众数据。<strong>数据协作</strong>营销操作支持 C4、C5 和 C9 数据使用标签。<strong>数据科学</strong>营销操作支持 C9 数据使用标签。</p> <p> <ul><li> <em>启用</em>该复选框后，Experience Platform 中标有上述标签的任何数据都会被排除，并且<strong>不</strong>被纳入 Real-Time CDP Collaboration。</li><li> <em>禁用</em>该复选框后，从 Experience Platform 导入 Real-Time CDP Collaboration 的数据不受限制。</li></ul></p>"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/data-governance/labels/overview.html?lang=zh-Hans" text="数据使用标签概述"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/data-governance/labels/reference.html" text="数据使用标签词汇表"

>[!IMPORTANT]
>
>连接到第一个数据连接并导入第一个受众后，您可以选择从此现有数据连接导入多个受众。 在这种情况下，工作流会将您直接转到[选择受众](#select-audience)步骤，因为其他步骤中的所有先决条件信息都将从现有连接导入。

数据连接是从中将受众导入Real-Time CDP Collaboration的数据源。 对于Real-Time CDP Collaboration的第一个版本，唯一支持的数据连接是Adobe Experience Platform。

您为数据连接配置的任何设置（如身份映射或计划）均应用于从此数据连接导入的所有受众。

>[!TIP]
>
>有一个单独的工作流，您始终可以查看和编辑在此步骤中添加的所有数据连接。 阅读有关[管理数据连接](/help/guide/setup/manage-data-connection.md)的更多信息。

![选择受众源屏幕，其中显示AEP RTCDP、CSV文件、Amazon S3和Snowflake的选项。](/help/assets/setup/add-manage-audiences/Step-Select-Audience-Source.png)

#### 选择数据源

在此步骤中，您将选择受众数据的来源。 可用的源包括：

* **Adobe Experience Platform**：选择此选项可从Adobe Experience Platform Real-Time CDP引入受众。
* **CSV文件**（未来版本）：上载包含受众数据的CSV文件以快速而直接地摄取数据。
* **Amazon Web Services**（未来版本）：连接到您的Amazon S3存储，以直接从S3存储桶导入受众数据。
* **Snowflake**（未来版本）：使用Snowflake数据仓库无缝提取受众数据。

#### 选择沙盒

选择&#x200B;**Adobe Experience Platform**&#x200B;作为数据源后，必须选择沙盒，其中包含将要导入的受众。

![选择沙盒以导入受众](/help/assets/setup/add-manage-audiences/import-audiences-select-sandbox.png)

选择所需的沙盒后，选择&#x200B;**[!UICONTROL 下一步]**。

#### 治理策略和实施行动 {#governance-policy-and-enforcement-actions}

接下来，必须确保对导入的数据设置正确的营销操作。 您还需要同意从Real-Time CDP导入用于数据协作的数据。

使用营销操作来控制从 Experience Platform 向 Real-Time CDP Collaboration 导入哪些受众数据。**数据协作**&#x200B;营销操作支持 C4、C5 和 C9 数据使用标签。**数据科学**&#x200B;营销操作支持 C9 数据使用标签。

详细了解[C4、C5和C9数据使用标签](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/labels/reference#contract){target="_blank"}。

* *启用*&#x200B;该复选框后，Experience Platform 中标有上述标签的任何数据都会被排除，并且&#x200B;*不*&#x200B;被纳入 Real-Time CDP Collaboration。
* *禁用*&#x200B;该复选框后，从 Experience Platform 导入 Real-Time CDP Collaboration 的数据不受限制。

有关数据使用标签的更多信息，请参阅Experience Platform文档：

* [数据使用标签概述](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/labels/overview){target="_blank"}
* [数据使用标签术语表](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/labels/reference){target="_blank"}

![数据协作所需的营销操作。](/help/assets/setup/add-manage-audiences/data-collaboration-consent.png)

### 提供详细信息

接下来，为您提供名称和描述，以便将来识别此数据连接。

<!--

>[!IMPORTANT]
>
>Note a difference in terminology where the sandbox selected from Real-Time CDP is considered a dataset in the UI in Real-Time CDP Collaboration.

-->

### 映射字段 {#map-fields}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_source_fields"
>title="源字段"
>abstract="源字段是来自您现有的 Real-Time CDP 实施的身份标识命名空间和属性。您可以将它们映射到 Real-Time CDP Collaboration 中定义的目标字段。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_target_fields"
>title="目标字段"
>abstract="目标字段是您在加入公司时选择的匹配键。目前，经过哈希处理的电子邮件是唯一受支持的匹配键。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_apply_transformation"
>title="应用转换"
>abstract="从来源导入&#x200B;*非哈希*&#x200B;字段时，使用此选项可让 Real-Time CDP Collaboration 应用哈希算法，将纯文本字段转换为哈希字段。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_identity_namespaces"
>title="身份标识命名空间"
>abstract="从 Experience Platform 组织中可用的标准的及自定义的身份标识命名空间中选择一个身份标识命名空间。"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/identity/features/namespaces.html#standard" text="Experience Platform 中的标准和身份标识命名空间"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_profile_attributes"
>title="轮廓属性"
>abstract="从 Experience Platform 中的轮廓类的联合架构中选择属性。此视图显示联合架构中存在的且属于 XDM 个人轮廓类的属性。"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/profile/union-schemas/union-schema.html" text="Experience Platform 中的联合架构"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_target_namespaces"
>title="Target 命名空间"
>abstract="这里将填写适当的描述。"

![映射字段屏幕显示映射到目标字段的源字段。](/help/assets/setup/add-manage-audiences/Step-Map-Fields.png)

在映射字段步骤中，您可以选择从数据连接引入的用户档案的任意标识字段如何映射到您在组织中选择的匹配键。

>[!TIP]
>
>您可以将多个源字段映射到同一个目标字段。 例如，如果在Experience Platform中的两个单独字段中都有电子邮件地址，则可以将这两个地址映射到&#x200B;**[!UICONTROL 哈希电子邮件]**&#x200B;目标字段作为两个单独的行。

>[!BEGINSHADEBOX]

**[!UICONTROL Source字段]**&#x200B;指示在从中导入数据的源中如何引用标识。

**[!UICONTROL 目标字段]**&#x200B;指示标识在Real-Time CDP Collaboration中的引用方式。 您可以在此处选择的值对应于您在公司载入工作流中设置的匹配键。

当您从源导入&#x200B;*非散列*&#x200B;字段时，请使用&#x200B;**[!UICONTROL 应用转换]**&#x200B;选项。 在这种情况下，Real-Time CDP Collaboration将应用哈希并转换字段。 Adobe使用的哈希算法是SHA256。

>[!ENDSHADEBOX]

根据需要添加任意数量的映射对，然后选择&#x200B;**[!UICONTROL 下一步]**&#x200B;以继续执行下一步。

<!--

In this step, you can also add any identity crosswalks that you would like to use.

Identity crosswalks will be supported after the beta release.

#### Add identity crosswalk

Use identity crosswalks to connect different identifiers across datasets to enrich your audience data with additional attributes or dimensions. 

TODO add GIF Identity crosswalks screen showing a list of available identity crosswalks with details.

Select **[!UICONTROL Add identity crosswalk]** to see a screen where you can choose from various identity crosswalks that you have previously [imported into Real-Time CDP Collaboration](/help/guide/setup/identity-crosswalk.md#import-crosswalk). Each entry includes details such as the table name, type, description, and creation date.

After selecting the desired crosswalk, use a source field join key to map to the crosswalk table join key. 

>[!NOTE]
>
>After selecting an identity crosswalk, the **[!UICONTROL Add identity crosswalk]** control is greyed out. 

For further reading about identity crosswalks, refer to the [glossary](/help/guide/glossary.md).

-->


<!-- will uncomment this part when Manage use cases part becomes available

### Manage use cases {#manage-use-cases}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_usecases"
>title="Use cases for identities"
>abstract="This control is disabled in the initial release of Real-Time CDP Collaboration"

![Manage use cases screen.](/help/assets/setup/add-manage-audiences/Step-manage-use-cases.png)

For every identity selected in the mapping step, select the use cases that you can use the identity for. Available use cases are: 

* Discover
* Share
* Activate
* Measure

Note that this control is disabled in the initial release of Real-Time CDP Collaboration.

After selecting the desired use cases for each identity, proceed to the next step. 

-->›

### 计划 {#schedule}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_audience_expiration"
>title="受众过期"
>abstract="有关受众过期的详细信息即将公布。"

安排何时开始和结束填充和刷新受众。 受众会员资格将按照此计划进行刷新。

![显示填充受众的开始和结束日期的计划屏幕。](/help/assets/setup/add-manage-audiences/Step-Schedule.png)

选择受众的刷新率。 可用选项为1天到6天的刷新率。

>[!IMPORTANT]
>
>调整受众更新的频率将有助于管理[受众管理信用活动](/help/guide/setup/my-activity.md#types-of-activities)，该活动是按受众成员资格刷新计算的。 其影响可能包括提供给受众发现报表以及受众共享和激活的新增数据减少。

![计划屏幕，其中显示更新受众成员资格的不同频率间隔。](/help/assets/setup/add-manage-audiences/Step-Schedule-Set-Frequency.png)

>[!IMPORTANT]
>
>在日期范围内的结束日期之后，从此数据连接导入的所有受众将停止刷新。 若要续订连接，请转到[管理数据连接](/help/guide/setup/manage-data-connection.md)，并设置新的结束日期。

### 选择受众 {#select-audience}

选择受众源后，您将选择要包含的特定受众。 使用页面上的搜索和筛选选项从所选数据源查找相关受众。

![选择受众屏幕，其中显示了一个包含复选框以选择受众的可用受众列表。](/help/assets/setup/add-manage-audiences/Step-Select-Audience.png)

### 审查

在最终确定受众添加之前，请查看所有配置和设置。 确保所有详细信息正确无误，并选择&#x200B;**[!UICONTROL 完成]**&#x200B;以完成该流程。

## 查看受众仪表板 {#view-audiences-dashboard}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_missing_identities"
>title="缺少身份标识"
>abstract="按照配置的计划，身份标识计数将在下一次数据连接刷新后可用。初始刷新通常发生在数据连接建立后的 24 小时内。正在进行的刷新将遵循配置的计划。 "

将受众导入Real-Time CDP Collaboration后，您可以在功能板视图中获取有关这些受众的信息。 **[!UICONTROL 我的受众]**&#x200B;页面中的默认视图显示贵组织当前导入到Real-Time CDP Collaboration中的所有受众。

![显示广告商导入的所有受众的“受众概述”页面](/help/assets/setup/add-manage-audiences/audiences-overview.png)

您可以查看有关每个受众的以下相关信息：

| 项目 | 描述 |
|----------|---------|
| **[!UICONTROL 标识]** | 指示此受众中存在的身份数。 请注意，如果同一配置文件具有两个或更多身份，并且这些身份在项目中被用作匹配键，则该配置文件将在计数中显示两次。 |
| **[!UICONTROL 状态]** | 指示受众是否处于活动状态以及是否可以在项目中使用。 待定状态表示受众最近刚刚导入，且受众成员尚未填充。 导入的受众将在按照配置的时间表进行下一次数据连接刷新后填充用户档案。 初始刷新通常发生在数据连接设置后的24小时内                                         . |
| **[!UICONTROL Source]** | 指示从中导入此受众的来源。 在Real-Time CDP Collaboration的当前版本中，Adobe Experience Platform是唯一受支持的源。 |
| **[!UICONTROL 数据连接]** | 有关从何处导入此受众的更多深入信息。 例如，从Experience Platform源导入受众时，贵组织有权访问的各个沙盒被视为数据连接。 |
| **[!UICONTROL 连接访问]** | 定义此受众是私人还是公共受众。 公共受众可在重叠报表中发现，并可与协作者共享。 |
| **[!UICONTROL 已创建]** | 指示将此受众导入到Real-Time CDP Collaboration中的时间。 |
| **[!UICONTROL 上次更新时间]** | 指示上次更新此受众任何方面的日期和时间。 |

选择&#x200B;**[!UICONTROL 管理数据连接]**以查看和编辑已设置的所有数据连接。
选择省略号和**[!UICONTROL 删除]**以删除受众。
选择省略号和**[!UICONTROL 编辑类别]**&#x200B;以向受众添加不同的类别标记。 在下面的[类别](/#categories)部分中获取更多信息。
选择受众名称以检查或编辑单个受众。

## 查看单个受众 {#view-individual-audiences}

受众视图将显示有关受众的更多信息。

![查看和检查单个受众。](/help/assets/setup/add-manage-audiences/view-inspect-audience.png)

您可以在此屏幕中查看的量度描述如下：

| 项目 | 描述 |
|----------|---------|
| **[!UICONTROL 状态]** | 指示受众是否处于活动状态以及是否可以在项目中使用。 |
| **[!UICONTROL Source]** | 指示从中导入此受众的来源。 在Real-Time CDP Collaboration的当前版本中，Adobe Experience Platform是唯一受支持的源。 |
| **[!UICONTROL 数据连接]** | 有关从何处导入此受众的更多深入信息。 例如，从Experience Platform源导入受众时，贵组织有权访问的各个沙盒被视为数据连接。 |
| **[!UICONTROL 上次更新时间]** | 指示上次更新此受众任何方面的日期和时间。 |
| **[!UICONTROL 上次更新者]** | 指示上次更新此受众的用户。 |
| **[!UICONTROL 已创建]** | 指示将此受众导入到Real-Time CDP Collaboration中的时间。 |
| **[!UICONTROL 创建者]** | 指示将受众导入Real-Time CDP Collaboration的用户。 |


您可以在页面上使用另外两个控件来编辑或删除受众：

* **[!UICONTROL 删除]**：从库存中删除受众
* **[!UICONTROL 编辑]**：编辑受众元数据，如其名称或描述。

![查看和检查单个受众。](/help/assets/setup/add-manage-audiences/audiences-edit-delete-controls.png)

有关受众的更多信息，可在以下小组件中查看或部分编辑：

![查看和检查单个受众。](/help/assets/setup/add-manage-audiences/audiences-further-info-boxes.png)

* [身份标识](#identities)
* [类别](#categories)
* [连接访问权限](#connection-access)
* [元数据可见性](#metadata-visibility)

### 身份标识 {#identities}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_identities"
>title="身份标识"
>abstract="获取构成该受众的身份标识的细分视图，以及具有相应身份标识的轮廓总数。"

此部分指示受众中存在的具有您在导入受众时指定的任何身份的用户档案数。 部分还包含身份细分，以便您分辨哪些身份构成了最多的受众群体。

### 类别 {#categories}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_categories"
>title="类别"
>abstract="标记您的受众，以便进行组织、筛选和检索。您可以使用多个类别标记受众，然后在产品的其他区域中使用这些类别标记筛选所需的受众。"

为便于受众的组织、筛选和检索，您可以标记受众。 您可以为具有多个类别的受众添加标签，然后在运行受众重叠报表时，使用这些类别标签在[发现](/help/guide/collaborate/discover.md)产品区域中过滤所需的受众。

### 连接访问权限 {#connection-access}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_connection_access"
>title="连接访问权限"
>abstract="<p>受众可以分为三种类型：公共、私人和自定义。</p><p> 它们在与协作者合作的项目中是否可用取决于连接访问权限设置。您可以随时将连接访问权限从私人更改为公开，但一旦与合作者共享了受众，就无法再更改该设置。</p>"

选择受众是您私有，还是可以在连接中使用和可搜索的。 三个可用选项包括：

* **[!UICONTROL 公共受众]**。 这些受众可用于重叠报表，并可用于与任何协作者共享和激活连接。
* **[!UICONTROL 专用受众]**。 这些受众&#x200B;*不*&#x200B;可用于重叠报表，也可用于与任何协作者共享和激活连接。 尽管无法供协作者查看或使用，但此受众的群体仍在[发现和重叠部分](/help/guide/collaborate/discover.md#compare-audiences)的&#x200B;**[!UICONTROL 所有受众]**&#x200B;视图中占总体人口。 将设置更改为“公用”或“自定义”，以便将受众与协作者关联使用。
* **[!UICONTROL 自定义受众]**。 这些受众只能在重叠报表中使用，并且只能在指定的连接中进行共享和激活。 虽然该受众的群体并不可供所有协作者查看或使用，但该受众的群体仍在[发现和重叠部分](/help/guide/collaborate/discover.md)的&#x200B;**[!UICONTROL 所有受众]**&#x200B;视图中占总体人口。

>[!IMPORTANT]
>
>无论访问状态（公用、专用或自定义）如何，任何受众的群体都会向受众发现重叠分析视图中的&#x200B;**[!UICONTROL 所有受众]**&#x200B;群体贡献内容。<br> ![受众发现重叠分析中系统生成的&#x200B;**所有受众**&#x200B;受众包含具有所有连接访问状态（公共、私有、自定义）的受众。](/help/assets/setup/add-manage-audiences/all-audiences-view.png "在**受众发现**重叠分析中，系统生成的**所有受众**受众包含具有所有连接访问状态（公共、私有、自定义）的受众。"){width="100" zoomable="yes"}

与协作者一起使用的项目中的受众可用性因连接访问设置而异。 您可以随时将连接访问权限从私人更改为公开，但一旦与合作者共享了受众，就无法再更改该设置。

### 元数据可见性 {#metadata-visibility}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_metadata_visibility"
>title="元数据可见性"
>abstract="<p>表示其他组织在与您的组织建立联系之前可以看到哪些受众元数据信息。 </p> <p> **身份标识计数**&#x200B;控制了您的合作伙伴在“发现”选项卡中查看重叠报告时是否可以查看您受众的身份标识计数。**受众重叠率**&#x200B;控制了协作者是否能够发现他们的受众与您的受众之间的重叠百分比。"

>[!NOTE]
>
>如果协作者将所有受众都设置为私人，则受众分析中的&#x200B;**[!UICONTROL 相关受众]**&#x200B;视图将为空白。 [了解详情](/help/guide/collaborate/discover.md#relevant-audiences)。

指示其他组织在连接到您的组织或在不同的项目视图内之前对其可见的受众元数据信息中的哪些。

**[!UICONTROL 显示身份计数]**：此设置控制当[在发现选项卡](/help/guide/collaborate/discover.md#discover-overlaps)中查看重叠报告时，您的合作伙伴是否可以查看受众的身份计数。

![取消选择并选择了“显示身份计数”选项的并排图像。](/help/assets/setup/add-manage-audiences/show-identity-count.png)

**[!UICONTROL 显示受众重叠%]**：设置为true时，协作者将能够在其受众和属于您的受众之间[发现重叠百分比](/help/guide/collaborate/discover.md#compare-audiences)。 例如，在下面的录制中，受众`agora-advertiser-aud3`将此配置设置为true，协作者可以查看与该受众的重叠百分比。 受众`agora-advertiser-aud1`的此设置已设置为false，因此协作者无法查看重叠百分比。

![两个不同受众的受众重叠百分比。](/help/assets/setup/add-manage-audiences/audience-overlap-percentage.gif)

## 后续步骤

导入受众后，使用[连接](/help/guide/connect/establishing-connections.md)部分发现要连接的发布者并开始协作项目。
