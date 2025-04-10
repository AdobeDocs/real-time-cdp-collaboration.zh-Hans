---
title: 导入和管理受众
description: 了解如何在Adobe Real-Time CDP Collaboration中导入和管理受众
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 0a5158fa-73d3-4406-af20-2b6c7be9934e
source-git-commit: ff22dde9730fab89481338753b1dc4a0adf1d57e
workflow-type: tm+mt
source-wordcount: '2642'
ht-degree: 2%

---

# 导入和管理访问群体

{{limited-availability-release-note}}

受众是根据各种属性细分的特定用户或客户组。 这些使得广告商和出版商能够合作进行有针对性的营销和个性化体验，以开展更有效的广告活动。

使用此页面作为切入点，了解可以查看的所有与受众相关的指标，以及将受众导入Adobe Real-Time CDP Collaboration的工作流程步骤。

>[!TIP]
>
>使用此屏幕中的信息获取关于受众的所有信息，并且[发现与重叠屏幕](/help/guide/collaborate/discover.md)可了解与发行商库存相比，哪些受众最适合不同的营销活动类型。

>[!BEGINSHADEBOX]

您可以在此文档页面上找到以下内容：

* [将受众导入Real-Time CDP Collaboration](#import-audiences)
* [查看受众信息板](#view-audiences-dashboard)
* [查看单个受众](#view-individual-audiences)

>[!ENDSHADEBOX]

## 将受众导入Real-Time CDP Collaboration {#import-audiences}

>[!IMPORTANT]
>
>要导入访问群体，需要为您的用户分配一个角色，该角色包含两个配置文件管理权限 — “查看配置文件”和“查看段”。 有关分配必要权限的信息，请参阅[受众导入](../permissions/overview.md#audience-importation)指南。

在与协作者共享受众以及运行重叠计算之前，需要将受众导入Real-Time CDP Collaboration。 要导入受众，请按照下面部分中的工作流程步骤进行操作。

![在将任何受众添加到组织之前，会先显示“我的受众”屏幕。](/help/assets/setup/add-manage-audiences/org-without-audiences-added.png)

从&#x200B;**[!UICONTROL 我的观众]**&#x200B;选项卡中，选择加号&#x200B;**+**&#x200B;符号，然后选择&#x200B;**观众**。

### 选择数据连接 {#select-data-connection}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_marketing_actions"
>title="营销操作"
>abstract="<p>使用营销操作可控制要将哪些受众数据从Experience Platform导入Real-Time CDP Collaboration。 <strong>数据Collaboration</strong>营销操作支持C4、C5和C9数据使用标签。 <strong>数据科学</strong>营销操作支持C9数据使用标签。</p> <p> <ul><li> 如果选中<em>启用</em>复选框，则会排除在Experience Platform中使用上述标签标记的任何数据，并且<strong>不会</strong>将这些数据带入Real-Time CDP Collaboration。</li><li> 如果选中复选框<em>已禁用</em>，则对可从Experience Platform导入到Real-Time CDP Collaboration的数据不做任何限制。</li></ul></p>"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/data-governance/labels/overview.html?lang=zh-Hans" text="数据使用标签概述"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/data-governance/labels/reference.html" text="数据使用标签词汇表"

>[!IMPORTANT]
>
>连接到第一个数据连接并导入第一个受众后，您可以选择从此现有数据连接导入多个受众。 在这种情况下，工作流将直接带您进入[选择受众](#select-audience)步骤，因为其他步骤中的所有先决条件信息将从现有连接导入。

数据连接是您从中将受众导入Real-Time CDP Collaboration的数据源。 在第一个版本的Real-Time CDP Collaboration中，唯一支持的数据连接是Adobe Experience Platform。

您为数据连接配置的任何设置（如身份映射或计划）都将应用于从此数据连接导入的所有访问群体。

>[!TIP]
>
>有一个单独的工作流程，您始终可以在其中查看和编辑在此步骤中添加的所有数据连接。 阅读有关[管理数据连接](/help/guide/setup/manage-data-connection.md)的更多信息。

![选择受众源屏幕，其中显示AEP RTCDP、CSV文件、Amazon S3和Snowflake的选项。](/help/assets/setup/add-manage-audiences/Step-Select-Audience-Source.png)

#### 选择数据源

在此步骤中，您将选择受众数据的源。 可用源包括：

* **Adobe Experience Platform**：选择此选项可从Adobe Experience Platform Real-Time CDP引入受众。
* **CSV文件**（未来版本）：上传包含您的受众数据的CSV文件，以便快速而直接地获取数据。
* **Amazon Web Services**（未来版本）：连接到您的Amazon S3存储以直接从S3存储桶导入受众数据。
* **Snowflake**（未来版本）：使用Snowflake数据仓库可无缝地引入受众数据。

#### 选择沙盒

选择&#x200B;**Adobe Experience Platform**&#x200B;作为数据源后，必须选择沙盒，其中包含将要导入的受众。

![选择沙盒以导入受众](/help/assets/setup/add-manage-audiences/import-audiences-select-sandbox.png)

选择所需的沙盒后，选择&#x200B;**[!UICONTROL 下一步]**。

#### 治理策略和实施行动 {#governance-policy-and-enforcement-actions}

接下来，您必须确保对导入的数据设置了正确的市场营销操作。 对于从Real-Time CDP导入的数据，您还需要同意才能将其用于数据协作。

使用营销操作控制要将哪些受众数据从Experience Platform导入Real-Time CDP Collaboration。 **数据协作**&#x200B;营销操作支持C4、C5和C9数据使用标签。 **数据科学**&#x200B;营销操作支持C9数据使用标签。

阅读有关[C4、C5和C9数据使用标签](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/labels/reference#contract){target="_blank"}的更多信息。

* 如果选中&#x200B;*启用*&#x200B;复选框，则会排除在Experience Platform中使用上述标签标记的任何数据，并且&#x200B;*不会*&#x200B;将这些数据带入Real-Time CDP Collaboration。
* 如果选中复选框&#x200B;*已禁用*，则对可从Experience Platform导入到Real-Time CDP Collaboration的数据不做任何限制。

阅读有关Experience Platform文档中数据使用标签的更多信息：

* [数据使用标签概述](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/labels/overview){target="_blank"}
* [数据使用标签术语表](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/labels/reference){target="_blank"}

![数据协作所需的营销操作。](/help/assets/setup/add-manage-audiences/data-collaboration-consent.png)

### 提供详细信息

接下来，提供一个名称和说明，以便将来识别此数据连接。

<!--

>[!IMPORTANT]
>
>Note a difference in terminology where the sandbox selected from Real-Time CDP is considered a dataset in the UI in Real-Time CDP Collaboration.

-->

### 映射字段 {#map-fields}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_source_fields"
>title="源字段"
>abstract="Source字段是指您现有Real-Time CDP实施中的身份命名空间和属性。 您可以将这些字段映射到Real-Time CDP Collaboration中定义的目标字段。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_target_fields"
>title="目标字段"
>abstract="目标字段与您登录公司时选择的匹配密钥相对应。 目前，仅支持散列电子邮件匹配键。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_apply_transformation"
>title="应用转换"
>abstract="从源导入&#x200B;*非散列*&#x200B;字段时，使用此选项可让Real-Time CDP Collaboration应用散列并将纯字段转换为散列字段。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_identity_namespaces"
>title="身份标识命名空间"
>abstract="从Experience Platform组织中可用的标准和自定义标识命名空间中选择标识命名空间。"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/identity/features/namespaces.html#standard" text="Experience Platform中的标准和标识命名空间"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_profile_attributes"
>title="轮廓属性"
>abstract="从Union Schema中为Experience Platform中的Profile类选择属性。 此视图显示联合架构中存在的属于XDM Individual Profile类的属性。"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/profile/union-schemas/union-schema.html" text="Experience Platform中的合并架构"

![映射字段屏幕，显示映射到目标字段的源字段。](/help/assets/setup/add-manage-audiences/Step-Map-Fields.png)

在映射字段步骤中，您可以选择从数据连接导入的配置文件的任何标识字段如何映射到您在组织中选择的匹配项。

>[!TIP]
>
>您可以将多个源字段映射到同一目标字段。 例如，如果电子邮件地址位于Experience Platform的两个单独字段中，则可以将这两个地址分别映射到&#x200B;**[!UICONTROL 哈希电子邮件]**&#x200B;目标字段，形成两个单独的行。

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

-->

### 计划 {#schedule}

安排何时开始和结束填充和刷新受众。 受众会员资格将按照此计划进行刷新。

![显示填充受众的开始和结束日期的计划屏幕。](/help/assets/setup/add-manage-audiences/Step-Schedule.png)

选择受众的刷新率。 可用选项为1天到6天的刷新率。

>[!IMPORTANT]
>
>调整受众更新的频率将有助于管理[Audience Management积分活动](/help/guide/setup/my-activity.md#types-of-activities)，这是根据受众成员资格刷新计算的。 其影响可能在于提供给受众发现报告以及受众共享和激活的新鲜数据减少。

![计划屏幕显示更新受众成员资格的不同频率间隔。](/help/assets/setup/add-manage-audiences/Step-Schedule-Set-Frequency.png)

>[!IMPORTANT]
>
>在日期范围内的结束日期之后，从此数据连接导入的所有访问群体都将停止刷新。 要续订连接，请转到[管理数据连接](/help/guide/setup/manage-data-connection.md)，然后设置新的结束日期。

### 选择受众 {#select-audience}

选择受众源后，您将选择要包含的特定受众。 使用页面上的搜索和筛选选项从所选数据源查找相关受众。

![选择受众屏幕，其中显示了一个包含复选框以选择受众的可用受众列表。](/help/assets/setup/add-manage-audiences/Step-Select-Audience.png)

### 审查

在最终确定受众添加之前，请查看所有配置和设置。 确保所有详细信息正确无误，并选择&#x200B;**[!UICONTROL 完成]**&#x200B;以完成该流程。

## 查看受众仪表板 {#view-audiences-dashboard}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_missing_identities"
>title="缺少身份"
>abstract="将受众导入Real-Time CDP Collaboration后大约24小时内，身份计数会显示`-`。 在此时间范围之后，身份计数将随受众中存在的用户档案数更新。"

将受众导入Real-Time CDP Collaboration后，您可以在功能板视图中获取有关这些受众的信息。 **[!UICONTROL 我的受众]**&#x200B;页面中的默认视图显示贵组织当前导入到Real-Time CDP Collaboration中的所有受众。

![显示广告商导入的所有受众的“受众概述”页面](/help/assets/setup/add-manage-audiences/audiences-overview.png)

您可以查看有关每个受众的以下相关信息：

| 项目 | 描述 |
|----------|---------|
| **[!UICONTROL 标识]** | 指示此受众中存在的标识数。 请注意，如果同一配置文件具有两个或更多标识，并且这些标识用作项目中的匹配键，则配置文件将在计数中显示两次。 |
| **[!UICONTROL 状态]** | 指示受众是否处于活动状态以及是否可以在项目中使用。 待定状态表示受众最近刚刚导入，且受众成员尚未填充。 导入的受众通常会在24小时内填充用户档案。 |
| **[!UICONTROL 源]** | 指示从中导入此受众的源。 在当前版本的Real-Time CDP Collaboration中，Adobe Experience Platform是唯一受支持的源。 |
| **[!UICONTROL 数据连接]** | 有关此访问群体从何处导入的详细信息。 例如，从Experience Platform源导入受众时，贵组织有权访问的各个沙盒被视为数据连接。 |
| **[!UICONTROL 连接访问]** | 定义此受众是私人还是公共受众。 公共受众可在重叠报表中发现，并可与协作者共享。 |
| **[!UICONTROL 已创建]** | 指示何时将此受众导入到Real-Time CDP Collaboration。 |
| **[!UICONTROL 上次更新时间]** | 指示上次更新此受众的任何方面的日期和时间。 |

选择&#x200B;**[!UICONTROL 管理数据连接]**以查看和编辑已设置的所有数据连接。
选择省略号并**[!UICONTROL 删除]**以移除受众。
选择省略号和**[!UICONTROL 编辑类别]**&#x200B;以向受众添加不同的类别标签。 在下面的[类别](/#categories)部分中获取更多信息。
选择受众名称以检查或编辑单个受众。

## 查看单个受众 {#view-individual-audiences}

受众视图可显示有关您的受众的更多信息。

![查看和检查单个受众。](/help/assets/setup/add-manage-audiences/view-inspect-audience.png)

您可以在此屏幕中查看的度量如下所述：

| 项目 | 描述 |
|----------|---------|
| **[!UICONTROL 状态]** | 指示受众是否处于活动状态以及是否可以在项目中使用。 |
| **[!UICONTROL 源]** | 指示从中导入此受众的源。 在当前版本的Real-Time CDP Collaboration中，Adobe Experience Platform是唯一受支持的源。 |
| **[!UICONTROL 数据连接]** | 有关从何处导入此受众的更多深入信息。 例如，从Experience Platform源导入受众时，贵组织有权访问的各个沙盒被视为数据连接。 |
| **[!UICONTROL 上次更新时间]** | 指示上次更新此受众任何方面的日期和时间。 |
| **[!UICONTROL 上次更新者]** | 指示上次更新此受众的用户。 |
| **[!UICONTROL 已创建]** | 指示何时将此受众导入到Real-Time CDP Collaboration。 |
| **[!UICONTROL 创建者]** | 指示将受众导入到Real-Time CDP Collaboration中的用户。 |


您可以在页面上使用另外两个控件来编辑或移除访问群体：

* **[!UICONTROL 删除]**：从清单中删除受众
* **[!UICONTROL 编辑]**：编辑受众元数据，如其名称或描述。

![查看和检查单个受众。](/help/assets/setup/add-manage-audiences/audiences-edit-delete-controls.png)

有关受众的更多信息，请参阅以下部分可编辑的构件：

![查看和检查单个受众。](/help/assets/setup/add-manage-audiences/audiences-further-info-boxes.png)

* [身份标识](#identities)
* [类别](#categories)
* [连接访问](#connection-access)
* [元数据可见性](#metadata-visibility)

### 身份标识 {#identities}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_identities"
>title="身份标识"
>abstract="获取构成此受众的身份的划分视图，以及具有相应身份的配置文件总数。"

此部分指示受众中存在的具有您在导入受众时指定的任何身份的用户档案数。 部分还包含身份细分，以便您分辨哪些身份构成了最多的受众群体。

### 类别 {#categories}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_categories"
>title="类别"
>abstract="标记受众以方便组织、筛选和检索。 您可以为受众添加多个类别的标签，然后使用这些类别标签筛选产品其他领域中所需的受众。"

为了便于受众的组织、筛选和检索，您可以标记受众。 您可以使用多个类别为受众添加标签，然后在运行受众重叠报告时，使用这些类别标签在[发现](/help/guide/collaborate/discover.md)产品区域中筛选所需的受众。

### 连接访问 {#connection-access}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_connection_access"
>title="连接访问"
>abstract="<p>受众可以分为三种类型：公共、专用和自定义。</p><p> 根据连接访问设置，它们在与协作者一起使用的项目中的可用性有所不同。 您始终可以将连接访问权限从专用更改为公用，但是一旦与协作者共享受众，就不能更改此设置。</p>"

选择受众是您私有，还是可以在连接中使用和可搜索的。 三个可用选项为：

* **[!UICONTROL 公共受众]**。 这些受众可用于重叠报告，并与任何协作者共享和激活。
* **[!UICONTROL 私人受众]**。 这些受众&#x200B;*不*&#x200B;可用于重叠报告以及与任何协作者共享和激活连接。 尽管协作者无法查看或使用，但此受众的填充仍会构成[发现和重叠部分](/help/guide/collaborate/discover.md#compare-audiences)中&#x200B;**[!UICONTROL 所有受众]**&#x200B;视图的总填充量。 将设置更改为“公共”或“自定义”以使用与协作者关联的受众。
* **[!UICONTROL 自定义受众]**。 这些受众只能在重叠报表中使用，并且只能在指定的连接中进行共享和激活。 虽然该受众的群体并不可供所有协作者查看或使用，但该受众的群体仍在[发现和重叠部分](/help/guide/collaborate/discover.md)的&#x200B;**[!UICONTROL 所有受众]**&#x200B;视图中占总体人口。

>[!IMPORTANT]
>
>无论访问状态（公用、专用或自定义）如何，任何受众的群体都会向受众发现重叠分析视图中的&#x200B;**[!UICONTROL 所有受众]**&#x200B;群体贡献内容。<br> ![受众发现重叠分析中系统生成的&#x200B;**所有受众**&#x200B;受众包含具有所有连接访问状态（公共、私有、自定义）的受众。](/help/assets/setup/add-manage-audiences/all-audiences-view.png "在**受众发现**重叠分析中，系统生成的**所有受众**受众包含具有所有连接访问状态（公共、私有、自定义）的受众。"){width="100" zoomable="yes"}

在包含协作者的项目中使用的受众可用性因连接访问设置而异。 您始终可以将连接访问权限从“专用”更改为“公用”，但在与协作者共享受众后，不能更改此设置。

### 元数据可见性 {#metadata-visibility}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_metadata_visibility"
>title="元数据可见性"
>abstract="<p>指示其他组织在与您的组织连接之前可以查看哪些受众元数据信息。 </p> <p> **身份计数**&#x200B;控制当您的合作伙伴在发现选项卡中查看重叠报告时是否可以查看受众的身份计数。 **受众重叠%**&#x200B;控制协作者能否发现其受众与您的受众之间的重叠百分比。"

>[!NOTE]
>
>如果协作者将所有受众都设置为“私密”，则audience insights中的&#x200B;**[!UICONTROL 相关受众]**&#x200B;视图将为空白。 [了解更多信息](/help/guide/collaborate/discover.md#relevant-audiences)。

指示其他组织在与您的组织连接之前或在不同的项目视图中可以看到哪些受众元数据信息。

**[!UICONTROL 显示身份计数]**：此设置控制当[在发现选项卡](/help/guide/collaborate/discover.md#discover-overlaps)中查看重叠报告时，您的合作伙伴是否可以查看受众的身份计数。

![取消选择并选择了“显示身份计数”选项的并排图像。](/help/assets/setup/add-manage-audiences/show-identity-count.png)

**[!UICONTROL 显示受众重叠%]**：设置为true时，协作者将能够在其受众和属于您的受众之间[发现重叠百分比](/help/guide/collaborate/discover.md#compare-audiences)。 例如，在下面的录制中，受众`agora-advertiser-aud3`将此配置设置为true，协作者可以查看与该受众的重叠百分比。 受众`agora-advertiser-aud1`将此设置设为false，因此协作者无法查看重叠百分比。

![两个不同受众的受众重叠百分比。](/help/assets/setup/add-manage-audiences/audience-overlap-percentage.gif)

## 后续步骤

导入受众后，使用[连接](/help/guide/connect/establishing-connections.md)部分发现要连接的发布者并开始协作项目。
