---
title: Real-Time CDP Collaboration入门快速入门
description: 了解如何在Real-Time CDP Collaboration中载入您的组织，包括设置角色和组织、受众配置、激活和测量。 本指南可帮助广告商和出版商配置协作设置并开始安全高效地使用共享受众。
audience: admin, publisher, advertiser
source-git-commit: 4435788917dd82cb127525e054f7f09803e1dcdf
workflow-type: tm+mt
source-wordcount: '1595'
ht-degree: 0%

---

# Real-Time CDP Collaboration入门快速入门

通过配置您的组织、配置受众并启用以隐私为中心的激活和测量，开始使用Real-Time Customer Data Platform (CDP) Collaboration。

## 先决条件

在开始之前，请确保您具备以下条件：

- 有效的Real-Time CDP Collaboration许可证。
- [系统或产品管理员访问Adobe Experience Platform](./permissions/overview.md#use-cases)。
- [已为最终用户设置访问权限](./permissions/manage-user-access.md)。
- 为您的组织创建并分配给用户的[角色](./permissions/manage-roles.md)。
- 访问品牌推广资产，如贵组织的名称、徽标和横幅。
- [定义的匹配键策略](./setup/onboard-organization.md#set-up-match-keys) （当前哈希电子邮件是唯一受支持的匹配键）。
- （可选）如果您未使用Experience Platform作为目标，请访问支持的云源(Amazon S3或Snowflake)。

## 步骤1：完成基于角色的设置 {#complete-role-based-setup}

>[!NOTE]
>
>此步骤适用于广告商和发布商。

贵组织的访问角色决定了用户可以在Real-Time CDP Collaboration中查看和执行的操作。 在继续操作之前，请确保已正确设置基于角色的权限，以确保在平台中具有适当的访问权和可见性。

**资源：**

- [用户访问文档](./permissions/manage-user-access.md)
- [角色设置文档](./permissions/manage-roles.md)


观看本视频，了解如何使用Admin Console和Experience Platform UI为Collaboration分配产品访问权限。

>[!VIDEO](https://video.tv.adobe.com/v/3452240/?learn=on&enablevpops&captions=chi_hans)

## 第2步：设置您的Real-Time CDP Collaboration组织 {#set-up-your-organization}

>[!NOTE]
>
>此步骤适用于广告商和发布商。

在添加受众之前，必须在Collaboration中配置您的组织。 它可控制贵组织在界面中的显示方式和行为。

如果您没有Experience Platform的管理员访问权限，请联系贵组织的管理员，以获取完成此设置的帮助。

定义贵组织在Collaboration中的角色，提供品牌策略资产，并配置匹配键以跨连接对齐受众。 然后，完成以下步骤以完成设置，并准备您的组织来参与连接。

>[!NOTE]
>
>在设置过程中，您可以创建一个或多个协作者（例如广告商或出版商配置文件）。 某些字段，如品牌推广资源和联系电子邮件，稍后可在&#x200B;**[!UICONTROL 设置]**&#x200B;工作区中更新。 匹配键可以在项目级别删除，但不能添加，因此请仔细计划。

- **分配角色** — 确定您的组织是充当广告商、发布者还是两者。 您的角色定义您具有的协作功能，例如启动受众共享（广告商）或使受众可用（发布者）。 要了解有关角色如何影响协作工作流的详细信息，请参阅[端到端工作流指南](./end-to-end-workflow.md)。
- **品牌推广资产** — 将以下内容添加到您的帐户：
   - 品牌名称（最多100个字符）
   - 品牌描述（最多1,000个字符）
   - Brand徽标(SVG &lt;20 KB，最好为正方形)
   - 品牌横幅(JPG 2688x1536或更高版本)
- **联系电子邮件** — 提供协作者在建立连接后使用的业务电子邮件。

  >[!NOTE]
  >
  >如果您正在创建发布者帐户，并希望在Collaboration的连接目录中公开显示，请联系您的Adobe客户代表。 发布者帐户需要自定义品牌横幅(JPG 2688x1536)；此文件可以直接与您的代表共享。

- **配置匹配键** — 选择用于受众匹配的标识符（当前，散列电子邮件是唯一受支持的匹配键）。

创建组织并配置品牌和匹配键后，您的组织即可开始配置受众和激活数据。

要了解有关初始组织设置的更多信息，包括如何定义角色、上传品牌推广资产和配置匹配密钥，请参阅[初始组织设置文档](./setup/onboard-organization.md#initial-organization-setup){target="_blank"}。

观看广告商设置的分步说明，包括帐户创建、品牌推广和关键配置的匹配。

>[!VIDEO](https://video.tv.adobe.com/v/3452264/?learn=on&enablevpops)

## 步骤3：Source受众(来自Experience Platform或云源) {#source-audiences}

选择以下一个或两个数据存储作为源受众。 使用Collaboration UI或与Adobe协调，以保留隐私的格式配置受众。

### 选项A：Experience Platform中的Source

[使用Collaboration目标UI链接包含受众的沙盒](./setup/onboard-audiences.md)。 使用此自助方法从Experience Platform实例中引用现有受众区段。

### 选项B：来自Snowflake或Amazon S3的Source

要配置云源（例如，[!DNL AWS S3]或[!DNL Snowflake]），请使用以下[受众规范PDF](../assets/quick-start/RTCDP_Collaboration_Audience_Onboarding_Spec_v1.0.pdf)准备受众数据。 完成后，或者如果您有任何疑问，请联系您的Adobe客户代表以完成设置。 此方法不是自助方法，需要Adobe帮助。

>[!IMPORTANT]
>
>基于云的受众文件必须遵循受众规范PDF中列出的所需架构。 文件必须包含哈希标识符（小写SHA256）、必需的元数据字段（如`segment_name`和`activation_id`），并使用支持的格式，如CSV或Parquet。 Adobe在激活之前不会标准化数据。 根据受众的生命周期强制执行TTL。
>
>在此阶段，上传文件中的所有受众都将完全获得来源。 对特定合作伙伴组织的访问权限是通过Collaboration UI单独设置的。

### 配置受众

配置如何准备、匹配和管理受众以用于连接。

- **选择受众** *(仅限Experience Platform)* — 选择具有支持标识符的受众区段。
- **映射匹配键** — 将受众字段与配置的匹配键对齐。
- **根据需要应用转换** — 哈希纯文本值（例如，电子邮件）。
- **计划刷新** — 定义更新频率（例如，每天）。
- **配置同意设置** — 通过选择同意模式：“选择启用”、“选择禁用”或“无”，确定哪些配置文件有资格包含在连接中。

>[!NOTE]
>
>您可以直接在Collaboration UI中添加或删除受众以及更新刷新计划。 要更改其他设置（如匹配键或同意模式），您必须删除并重新创建数据连接。

>[!IMPORTANT]
>
>**每个协作者角色的最大受众数：**
>
>- **广告商**&#x200B;最多可以配置25个受众。
>- **发布者**&#x200B;最多可以设置250个受众（每个受众具有至少5,000个ID）。

>[!IMPORTANT]
>
>**匹配关键要求：**
>
>所有匹配键必须是&#x200B;**修剪**、**小写**&#x200B;和&#x200B;**SHA256-hashed**。\
>如果您提供的哈希值使用大写字符，Collaboration会自动将其转换为小写。\
>如果您的源包含&#x200B;**纯文本标识符**，请使用UI中的&#x200B;**[!UICONTROL 应用转换]**&#x200B;选项来应用散列。 仅当从Experience Platform获取受众时，此选项才可用，而基于云的源不支持此选项。
>
>有关详细信息，请参阅导入和管理受众指南的[映射字段](./setup/onboard-audiences.md#map-fields)部分。

要观看如何使用Collaboration UI引用受众的完整演练，请观看下面的Collaboration受众引用演示视频。

>[!VIDEO](https://video.tv.adobe.com/v/3452217/?learn=on&enablevpops)

或者，查看有关[使受众在Real-Time CDP Collaboration](https://experienceleague.adobe.com/zh-hans/docs/real-time-cdp-collaboration/using/setup/onboard-audiences#import-audiences)中可用的文档。

## 步骤4：激活受众(到Experience Platform或云目标) {#activate-audiences}

>[!NOTE]
>
>此步骤适用于广告商和发布商。

使用Collaboration UI将受众激活到Experience Platform实例或云目标。

### 选项A：激活到Experience Platform

完成[将Adobe Experience Platform配置为目标](https://experienceleague.adobe.com/zh-hans/docs/real-time-cdp-collaboration/using/destinations/experience-platform)指南中概述的以下步骤。

- **创建目标** — 使用UI设置Experience Platform目标（沙盒级别）。
- **映射匹配键** — 选择标识符（例如，`hashedEmail`）。
- **定义TTL** — 设置过期时间（1-30天）。
- **在受众门户中验证** — 协作者向您发送受众后，请验证该受众是否显示在受众门户中的来源“[!UICONTROL Real-Time CDP Collaboration]”下。

### 选项B：激活到云

要将受众激活到云目标（如[!DNL AWS S3]或[!DNL Snowflake]），请联系您的Adobe客户代表以启动设置过程。 您需要提供目标详细信息，例如文件路径、凭据和预期的文件格式。 在设置过程中，还必须指定匹配键（例如，`hashedEmail`），并定义所需的TTL和刷新节奏。 配置完成后，Adobe将配置目标并确保正确传输数据。

发送到云目标的受众数据遵循预定义架构。 有关必填字段和格式的详细说明，请下载[Collaboration Audience Activation指南](../assets/quick-start/RTCDP_Collaboration_Audience_Activation_Spec_v1.0.pdf)。

### 主要差异

下表重点列出了Experience Platform和Cloud激活选项之间的差异：

- Experience Platform的激活是完全自助式的，并且可在Audience Portal中看到。
- 云目标需要Adobe协调，并且在用户界面中不可见。

## 步骤5：设置测量（可选） {#set-up-measurement}

>[!AVAILABILITY]
>
>此功能处于&#x200B;**测试版**&#x200B;中，仅供有限可用性计划中的客户使用。 请联系您的Adobe代表以请求获取访问权限。

>[!IMPORTANT]
>
>只有在连接进程[&#128279;](./connect/establishing-connections.md#connection-settings)期间启用了的&#x200B;**[!UICONTROL 测量]**&#x200B;用例时，**[!UICONTROL 测量]**&#x200B;工作区才可用。 有关用例的更多信息，请参阅[管理项目](./collaborate/manage-projects.md#project-use-cases)指南。

Collaboration提供了多种报告来分析促销活动的范围、频率和有效性。 虽然&#x200B;**[!UICONTROL Measure]**&#x200B;工作区在UI中可用，但完整的报表功能可能需要后端启用。

要了解如何查看和解读测量报告，请参阅[测量指南](./collaborate/measure.md)。 它涵盖归因、营销活动摘要量度和仪表板，如范围曲线和频率分布。

<!-- Commenting out the below information as this workflow is not yet in Beta but will be imminently. A guided measurement configuration workflow will be available in a future release."
### Configure measurement workflow

Collaboration supports two measurement workflows:

- **Attribution using Adobe Experience Platform datasets**
- **Campaign summary using only partner-provided data**

Choose the appropriate workflow below based on your campaign measurement goals.

#### Option A: Attribution using Experience Platform datasets

Use this workflow to measure conversion activity using datasets stored in Experience Platform.

1. **Create a measurement data connection**
   - Select the dataset that contains your conversion events.
   - Map identity fields from your dataset to the match keys used in Collaboration.
   - Manage consent and governance settings.
   - Define one or more conversion events to measure.
   - Review and confirm your setup.

2. **Run a measurement report**
   - Go to the **[!UICONTROL Measure]** workspace within the associated project.
   - Input the report name, date range, and report run date.
   - Select **[!UICONTROL Attribution]** as the report type.
   - Select the defined conversion event(s).
   - Submit the report. It will run on the specified date and populate within 24 hours.

#### Option B: Campaign summary using partner-provided data

Use this workflow to generate campaign summary insights based on advertiser-supplied identifiers (for example, campaign ID).

1. **Set up the connection**
   - In the connection settings, ensure **[!UICONTROL Measurement]** is selected as a use case.
   - Create a project under the connection with **[!UICONTROL Measurement]** as an activity.

2. **Provide campaign context**
   - Input required campaign identifiers (for example, **Campaign ID**) for the partner to reference.
   - Align with your partner on campaign scope and reporting timeline.

3. **Run a measurement report**
   - Navigate to the **[!UICONTROL Measure]** workspace within the project.
   - Input the report name, date range, and report run date.
   - Select **[!UICONTROL Campaign summary]** as the report type.
   - Submit the report. It will run on the selected date and populate within 24 hours. -->

## 验证

激活后，请验证受众是否已成功交付或在相应的目标中可用。

- 验证受众是否显示在Audience Portal中(用于Experience Platform激活)。
- 通过外部目标日志或确认，确认云投放成功。

## 步骤6：与协作者联系 {#connect-with-collaborators}

设置和数据配置完成后，您的组织现在可以通过发送或接受邀请并提交项目设置以供审批来与协作者联系。 此连接过程包括发送或接收邀请、审核和提交连接设置（如用例和信用消耗）以及确认关系。

使用Collaboration UI左侧导航菜单中的&#x200B;**[!UICONTROL Connect]**&#x200B;工作区来浏览可用的发布者（当前无法浏览广告商）。 有关此流程的概述，请参阅[与广告商或发布者联系指南](./connect/establishing-connections.md){target="_blank"}。 有关连接过程的可视化演练，包括浏览协作者和管理连接设置，请观看[广告商帐户设置视频](https://experienceleague.adobe.com/zh-hans/docs/platform-learn/tutorials/collaboration/connect-with-publishers){target="_blank"}。

## 后续步骤

您现在已完成入门培训并配置您的组织以进行安全协作。 接下来，探索以下资源，以加深您对激活、测量和数据治理的了解：

- [受众激活工作流文档](./collaborate/activate.md)
- [测量用例](./collaborate/measure.md)
- [Collaboration治理最佳实践](./setup/onboard-audiences.md#governance-policy-and-enforcement-actions)
