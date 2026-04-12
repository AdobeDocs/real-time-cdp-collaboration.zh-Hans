---
title: 衡量绩效
description: 衡量不同渠道中的促销活动效果。 了解如何使用和解读各种报表。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: c92b263e-1f96-49f1-841a-ef2e97a4cb9a
source-git-commit: e06ee94afdd1edbf86430cbe348dc448419b8f4e
workflow-type: tm+mt
source-wordcount: '2612'
ht-degree: 5%

---

# 衡量绩效

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>只有在连接过程[&#128279;](../connect/establishing-connections.md#connection-settings)期间启用了的&#x200B;**测量**&#x200B;用例时，**[!UICONTROL 测量]**&#x200B;工作区才可用。 有关用例的更多信息，请参阅[管理项目](./manage-projects.md#project-use-cases)指南。

了解Adobe Real-Time CDP Collaboration中的可用报表，并了解如何衡量和分析营销活动在各种渠道中的表现。

## 先决条件 {#prerequisites}

在Collaboration中访问测量报表之前，您必须：

* [Connect](/help/guide/connect/establishing-connections.md)与启用了&#x200B;**Measurement**&#x200B;用例的协作者
* 与您的协作者协作处理至少一个项目。 了解如何[创建项目](/help/guide/collaborate/manage-projects.md#create-project)。
* 运行您的营销活动，并确保为营销活动[&#128279;](../collaborate/manage-projects.md#manage-campaign-id)提供了营销活动ID：
   * 如果您是发布者，请输入链接到广告商促销活动的Campaign ID。
   * 如果您是广告商，请要求您的协作者（发布者）提供营销活动ID。 在度量值工作区[&#128279;](#create-measurement-report)中生成报告时需要此项。
* 如果要[创建归因报表](#create-attribution-report)，请[将测量数据](/help/guide/setup/onboard-measurement-data.md)上传到Collaboration。

## 查看报告 {#view-reports}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_measurement_create_report_campaignID"
>title="营销活动 ID"
>abstract="用于在用户界面中添加相关说明的信息占位符，以便解释“营销活动 ID”的含义。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_measurement_create_report"
>title="营销活动 ID"
>abstract="用于在用户界面中添加相关说明的信息占位符，以便解释“营销活动 ID”的含义。"

要查看测量选项卡中可用的报表，请执行以下操作：

1. 导航到&#x200B;**[!UICONTROL 协作]** > **[!UICONTROL 我的项目]**。
2. 对于所需的项目，请选择&#x200B;**[!UICONTROL 查看]**。
3. 在项目中，选择&#x200B;**[!UICONTROL 度量]**&#x200B;选项卡。

选择&#x200B;**[!UICONTROL 查看完整报告]**&#x200B;以访问各种可用报告，详见下文。

![如何进入项目中的测量选项卡。](/help/assets/collaborate/measure/measurement.gif)

### 摘要视图

测量选项卡中的页面顶部视图会显示一个营销活动摘要，其中包含一些可供您引用的高级数字：

**[!UICONTROL 展示次数]**：创意内容显示的总次数。
**[!UICONTROL 唯一范围]**：查看过该创意的个人身份的数量。
**[!UICONTROL 总平均频率]**：展示次数除以达到的唯一身份数。 此图显示了每个身份展示创意内容的频率。

![营销活动摘要视图](/help/assets/collaborate/measure/campaign-summary.png)

### 随时间变化的量度 {#metrics-over-time}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_measure_metricsovertime"
>title="随时间变化的量度"
>abstract="使用“随时间变化的量度”视图，了解在营销活动期间为您的创意显示的总展示次数。 您最多可以选择两个维度在报告中显示。"

使用“随时间变化的量度”视图，了解在营销活动期间为您的创意显示的总展示次数。 请注意，您最多可以选择两个量度以在报表中显示和分析。

![时间视图中的量度。](/help/assets/collaborate/measure/metrics-over-time.png)

### 频率分布 {#frequency-distribution}

使用频率分布视图可了解向每个独特用户显示的展示次数划分情况。 此视图可帮助您在将来的营销活动中决定要从哪一点开始禁止受众。 例如，您可能希望禁止已查看过三次创意内容的用户档案。

![频率分布视图。](/help/assets/collaborate/measure/frequency-distribution.gif)

### 按维度划分的量度 {#metric-by-dimension}

在投放位置媒体的上下文中分析不同的量度，如展示次数、可视展示次数、唯一范围、成本等。 分析哪些媒体（例如移动流媒体、CTV编程媒体或其他）为您的活动带来最佳结果。

![按维度列出的量度。](/help/assets/collaborate/measure/metric-by-dimension.png)

### 累计触达率曲线 {#cumulative-reach-curve}

随着营销活动的进展和展示次数的增加，请了解您能够联系到的用户数量是否也有所增加。 营销活动中的常见模式是，在达到某个时间点后，达到一个平台期，在此期间将创意内容反复显示给同一人。 此视图可帮助您调整未来营销活动的长度，具体取决于不再联系新用户的时刻。

![累积到达曲线。](/help/assets/collaborate/measure/cumulative-reach-curve.png)

### 按放置环境划分的展示次数 {#impressions-by-placement}

了解哪种媒介有助于提升您的创意印象。 这可以帮助您确定在将来的营销活动中要将广告支出投向何处。

![展示次数（按投放位置）。](/help/assets/collaborate/measure/impressions-by-placement.png)

### 累计转化次数 {#cumulative-conversions}

此视图以表格格式提供您选择测量的转化事件的详细细目。 该表包括：

* **转化事件**：您正在跟踪的每个转化事件的名称。
* **转化计数**：每个事件发生的转化总数。
* **预计收入**：归因于每个转化事件的预计值。

请查看此表以评估促销活动在推动所需操作方面的有效性。

![累计转化次数。](/help/assets/collaborate/measure/cumulative-conversions.png)

### 每日转化次数 {#conversions-by-day}

此图表按天划分您在创建归因报表时设置的每个事件的转化。 使用此视图可揭示每日模式，识别转化活动高或低的时段，并比较不同转化事件在营销活动时间轴中的执行情况。

![按天列出的转化。](/help/assets/collaborate/measure/conversions-by-day.gif)

## 创建测量报告 {#create-measurement-report}

在Collaboration中，您可以创建两种主要类型的测量报表：

* **促销活动摘要**：提供高级别的量度，例如范围、展示次数、平均频度和按渠道的投放次数，从而快速了解整体促销活动效果。
* **归因**：衡量营销活动风险如何推动转化或购买等下游操作，从而帮助您了解营销活动有效性。

您可以自行运行促销活动摘要报表，而归因报表要求同时选择这两种报表类型。

### 创建营销活动摘要报告 {#create-campaign-summary-report}

发布者和广告商都可以生成&#x200B;**促销活动摘要**&#x200B;报告以评估促销活动效果。 使用这些报告深入了解关键量度，如[范围](#cumulative-reach-curve)、[频率](#frequency-distribution)和[展示次数](#impressions-by-placement)，并了解您的营销活动的交付方式及其整体影响。

要生成&#x200B;**促销活动摘要**&#x200B;报告，请从&#x200B;**[!UICONTROL Collaborator]**&#x200B;工作区导航到项目工作区。 从&#x200B;**[!UICONTROL 度量]**&#x200B;选项卡中，选择添加图标（![添加图标。](/help/assets/icons/plus.png)） 然后选择&#x200B;**[!UICONTROL 度量]**。

如果这是您的第一个报告，您还可以选择&#x200B;**[!UICONTROL 运行报告]**&#x200B;选项。

![突出显示“运行报告”选项和“度量”选项的“度量”选项卡。](/help/assets/collaborate/measure/run-measure-report.png)

此时将显示&#x200B;**[!UICONTROL 创建测量报告]**&#x200B;屏幕，其中包含在&#x200B;**[!UICONTROL 帐单详细信息]**、**[!UICONTROL 促销活动详细信息]**&#x200B;和&#x200B;**[!UICONTROL 报告详细信息]**&#x200B;部分下分组的信息和输入字段。

#### 计费详细信息 {#billing-details}

本节介绍如何在生成测量报表时使用积分。 在[连接设置](../connect/establishing-connections.md#credit-split)期间已建立信用责任。 在运行任何报表之前，请确保与协作者一起查看并确认信用拆分设置和报表角色。

#### 营销活动详细信息 {#campaign-details}

在&#x200B;**[!UICONTROL 促销活动详细信息]**&#x200B;部分中，选择要与报表关联的相应&#x200B;**广告商ID**。 在[连接设置](../connect/establishing-connections.md#advertiser-names)期间添加了这些广告商名称或ID。 如果只配置了一个名称，则默认显示该名称。 如果未设置名称，则&#x200B;**[!UICONTROL 广告商ID （名称）]**&#x200B;字段将被禁用并预填充广告商帐户名称。

![显示“广告商ID （名称）”选项的“创建测量报告”屏幕已禁用。](/help/assets/collaborate/measure/advertiser-id.png)

然后，从&#x200B;**[!UICONTROL 促销活动ID]**&#x200B;下拉菜单中选择所需的促销活动。 此菜单列出了发布者为您的项目输入的所有营销活动ID。 如果所需的营销活动不可用，请在生成报告之前[将其添加到UI](./manage-projects.md#manage-campaign-id)中。

![创建测量报告屏幕显示“促销活动ID”下拉菜单已展开。](/help/assets/collaborate/measure/campaign-id.png)

接下来，指定您希望报告涵盖的时段。 选择&#x200B;**[!UICONTROL 报告日期范围]**，然后使用该日历选择开始日期和结束日期。

![显示报告日期范围日历的“创建测量报告”屏幕。](/help/assets/collaborate/measure/report-date-range.png)

#### 报告详细信息 {#report-details}

**报告运行日期**

在&#x200B;**[!UICONTROL 报告详细信息]**&#x200B;部分，选择报告运行的日期。 选择&#x200B;**[!UICONTROL 报告运行日期]**&#x200B;并从日历中选择首选日期。

* 如果您选择今天的日期或过去的日期，则会立即运行&#x200B;**促销活动摘要**&#x200B;报告。
* 如果您选择未来的日期，则计划在该日期运行&#x200B;**促销活动摘要**&#x200B;报告。

![创建测量报告屏幕显示报告运行日期日历。](/help/assets/collaborate/measure/report-run-date.png)

**报告类型**

* 如果您是广告商，则可以从可用选项中选择&#x200B;**[!UICONTROL 促销活动摘要]**&#x200B;报告类型。 只有广告商可以生成归因报表。
* 如果您是发布者，**[!UICONTROL 营销活动摘要]**&#x200B;报告类型为预选类型，无法更改。 目前，发布者无法运行归因报表。

![创建测量报告屏幕将“营销活动”摘要选项显示为预选且不可更改的报告类型。](/help/assets/collaborate/measure/cs-report-type.png)

最后，查看您的设置并选择&#x200B;**[!UICONTROL 创建]**。 如果运行日期为当天或更早，或者为选定的将来日期，则会立即生成促销活动摘要报表。 您可以在计划报表运行日期之前对其进行编辑。 有关分步说明，请参阅[编辑测量报告]一节。

一旦可用，您就可以随时在项目工作区的&#x200B;**[!UICONTROL 度量]**&#x200B;选项卡中查看报告。

![创建测量报告屏幕显示的信息和突出显示的创建选项。](/help/assets/collaborate/measure/cs-review.png)

### 创建归因报表 {#create-attribution-report}

作为广告商，您可以生成&#x200B;**归因**&#x200B;报告，以评估您的营销活动曝光次数对注册或购买等关键结果的贡献情况。 使用这些报表可了解用户与促销活动的交互情况、确定哪些接触点产生的影响最大，并告知更有效的营销策略。

>[!IMPORTANT]
>
> 在生成归因报表之前，您必须[将测量数据](../setup/onboard-measurement-data.md#add-measurement-data)源到Collaboration中。
>![具有测量数据要求和禁用的Measure选项的Measure选项卡。](/help/assets/collaborate/measure/require-measurement-data.png)

要生成&#x200B;**归因**&#x200B;报告，请从&#x200B;**[!UICONTROL Collaborator]**&#x200B;工作区导航到项目工作区。 从&#x200B;**[!UICONTROL 度量]**&#x200B;选项卡中，选择添加图标（![添加图标。](/help/assets/icons/plus.png)） 然后选择&#x200B;**[!UICONTROL 度量]**。

如果这是您的第一个报告，您还可以选择&#x200B;**[!UICONTROL 运行报告]**&#x200B;选项。

![突出显示“运行报告”选项和“度量”选项的“度量”选项卡。](/help/assets/collaborate/measure/run-measure-report-attribution.png)

此时将显示&#x200B;**[!UICONTROL 创建测量报告]**&#x200B;屏幕，其中包含在&#x200B;**[!UICONTROL 帐单详细信息]**、**[!UICONTROL 促销活动详细信息]**&#x200B;和&#x200B;**[!UICONTROL 报告详细信息]**&#x200B;部分下分组的信息和输入字段。

请阅读并按照[创建营销活动摘要报告](#create-campaign-summary-report)部分中的步骤来配置以下设置：

* [帐单详细信息](#billing-details)
* [营销活动详细信息](#campaign-details)

#### 归因报表的报表详细信息 {#report-details-attribution}

**报告运行日期**

>[!IMPORTANT]
>
> 对于归因报表，报表运行日期必须是将来的日期，并且必须在报表日期范围的结束日期加上定义的回溯时段的完整持续时间后至少一天发生。
> **报告运行日期≥报告结束日期+回顾时间范围+ 1**
> 
> 例如，如果您的报表日期范围在6月15日结束并且回溯时段为14天，则报表运行日期为6月30日或更高版本。

在&#x200B;**[!UICONTROL 报告详细信息]**&#x200B;部分，选择报告运行的日期。 选择&#x200B;**[!UICONTROL 报告运行日期]**&#x200B;并从日历中选择首选日期。

**报告类型**

作为广告商，除了&#x200B;**[!UICONTROL 促销活动摘要]**&#x200B;之外，您还可以选择&#x200B;**[!UICONTROL 归因]**&#x200B;作为报表类型。 当您选择归因报表时，您的结果既包括标准的促销活动摘要量度，又包括详细的归因分析，从而全面了解促销活动效果。

![创建测量报告屏幕突出显示所选的Campaign摘要和归因报告类型。](/help/assets/collaborate/measure/attribution-report-type.png)

选择&#x200B;**[!UICONTROL 归因]**&#x200B;作为报表类型时，将显示&#x200B;**[!UICONTROL 归因]**&#x200B;配置部分，其中包含其他必需的设置：

* **以天为单位的回看窗口期**：定义报表在每次转化前考虑促销活动展示的间隔时间。 只有此期间的展示才有资格获得归因点数。
* **转换事件**：指定要测量的转换操作，例如购买或注册。 当您[将测量数据](../setup/onboard-measurement-data.md#add-conversion-event)源到Collaboration中时，必须提前设置这些事件。

首先，输入&#x200B;**[!UICONTROL 以天]**&#x200B;为单位的回溯时段值，或使用增量/减量选项对其进行调整。

![创建测量报告屏幕突出显示以天为单位的回看窗口值。](/help/assets/collaborate/measure/lookback-window-in-days.png)

接下来，从可用列表中选择最多&#x200B;**3**&#x200B;个转化事件。 有关特定事件的详细信息，请选择&#x200B;**[!UICONTROL i]**&#x200B;图标以查看其详细信息。

![创建测量报告屏幕突出显示所选转化事件和购买事件的信息。](/help/assets/collaborate/measure/attribution-conversion-events.png)

最后，查看您的设置并选择&#x200B;**[!UICONTROL 创建]**&#x200B;以计划报告。 您的归因报告将在指定的运行日期生成。 您可以在计划报表运行日期之前对其进行编辑。 有关分步说明，请参阅[编辑测量报告]一节。

一旦可用，您就可以随时在项目工作区的&#x200B;**[!UICONTROL 度量]**&#x200B;选项卡中查看报告。

![创建测量报告屏幕显示的信息和突出显示的创建选项。](/help/assets/collaborate/measure/attribution-review.png)

## 编辑测量报告 {#edit-measurement-report}

>[!IMPORTANT]
>
>仅当计划在将来运行测量报表时，才能编辑测量报表的设置。 对于已执行的报表，无法更改设置。

更新测量报表设置，以确保报表在特定时间段内提供对营销活动的正确分析，并在所需的日期运行。

要开始，请导航到要更新的测量报告的工作区。 选择删除图标旁边的编辑图标（![编辑图标](/help/assets/icons/edit.png)）。

![突出显示“编辑”图标的测量报告工作区。](/help/assets/collaborate/measure/edit-report.png)

>[!TIP]
>
>在&#x200B;**[!UICONTROL 度量]**&#x200B;选项卡中，导航到要编辑的报告部分。 选择&#x200B;**[!UICONTROL 查看完整报告]**&#x200B;旁边的编辑图标（![编辑图标](/help/assets/icons/edit.png)）以更新其设置。
>![“度量”选项卡突出显示报表节中的“编辑”图标。](/help/assets/collaborate/measure/measure-tab-edit-report.png)

此时将显示&#x200B;**[!UICONTROL 编辑测量报告]**&#x200B;对话框，其中包含报告当前设置，具体包含以下部分：

* [**计费详细信息**](#billing-details)：在运行测量报告时显示积分信息。 无需配置。
* [**促销活动详细信息**](#campaign-details)：显示广告商、促销活动ID、报告时段和用户友好报表名称的设置。
* [**报告详细信息**](#report-details)：显示特定于归因报告的报告类型、报告运行日期和配置选项的设置。

![“编辑测量报告”对话框显示“计费详细信息”、“促销活动详细信息”和“报告详细信息”部分下的当前设置。](/help/assets/collaborate/measure/edit-measurement-report-dialog.png)

### 编辑营销活动详细信息 {#edit-campaign-details}

在&#x200B;**[!UICONTROL 编辑度量报告]**&#x200B;对话框中，使用&#x200B;**[!UICONTROL 广告商ID （名称）]**&#x200B;和&#x200B;**[!UICONTROL 促销活动ID]**&#x200B;下拉菜单编辑报告的广告商和促销活动ID。

![突出显示Campaign ID下拉菜单的“编辑测量报告”对话框打开。](/help/assets/collaborate/measure/edit-campaign-id.png)

接下来，选择&#x200B;**[!UICONTROL 报告日期范围]**&#x200B;并使用日历更改报告的开始和结束日期。

![突出显示报告日期范围日历的“编辑测量报告”对话框打开。](/help/assets/collaborate/measure/edit-report-date-range.png)

输入更新的友好报表名称以捕获您最近的更改。 这有助于您识别并在将来查找此报告。

![突出显示更新的友好报告名称的“编辑测量报告”对话框。](/help/assets/collaborate/measure/edit-friendly-report-name.png)

### 编辑报告详细信息 {#edit-report-details}

要计划其他日期的报告，请导航到&#x200B;**[!UICONTROL 报告详细信息]**&#x200B;部分。 选择当前运行日期选项，然后使用日历选择首选日期。

![突出显示报告运行日期日历的“编辑测量报告”对话框。](/help/assets/collaborate/measure/edit-report-run-date.png)

作为广告商，除了&#x200B;**[!UICONTROL 促销活动摘要]**&#x200B;之外，您还可以选择或删除&#x200B;**[!UICONTROL 归因]**&#x200B;报表类型。 如果选择&#x200B;**[!UICONTROL 归因]**，则您的归因报表将包括标准“促销活动摘要”量度和深入的归因分析。 有关&#x200B;**促销活动摘要**&#x200B;和&#x200B;**归因**&#x200B;报告类型的详细信息，请参阅[创建测量报告](#create-measurement-report)部分。

>[!IMPORTANT]
>
>如果您是&#x200B;**发布者**，则默认报表类型为&#x200B;**[!UICONTROL 营销活动摘要]**，此时无法更改。

* 如果选择&#x200B;**[!UICONTROL 归因]**&#x200B;作为报表类型，则必须在&#x200B;**[!UICONTROL 归因]**&#x200B;部分中填写必填字段。 有关设置说明，请参阅[归因报告详细信息](#report-details-attribution)部分。
* 如果您之前在创建报告时配置了归因设置，则可以选择编辑回顾时间范围（以天为单位测量）并选择要报告的转化事件。

要更新&#x200B;**[!UICONTROL 以天]**&#x200B;为单位的回溯时段，请输入一个数值，或使用增量/减量选项对其进行调整。 接下来，选择要报告的转化事件。 您可以从可用列表中选择最多&#x200B;**3**&#x200B;次转化。

![突出显示已更新的转化事件的“编辑测量报告”对话框。](/help/assets/collaborate/measure/edit-conversion-events.png)

完成后，查看更新并选择&#x200B;**[!UICONTROL 编辑]**&#x200B;以应用更改。

![突出显示了“编辑”选项的“编辑测量报告”对话框。](/help/assets/collaborate/measure/edit-report-confirm.png)

确认对话框用于确认您的报告已成功保存。

## 删除测量报表 {#delete-measurement-report}

删除Collaboration中的测量报表会将其从系统中永久删除。 无法撤消此操作。 为此，请在&#x200B;**[!UICONTROL 度量]**&#x200B;选项卡中选择要删除的报告。

在测量报表工作区中，选择删除图标（![删除图标](/help/assets/common/delete.svg)）。

![突出显示“删除”图标的测量报告工作区。](/help/assets/collaborate/measure/delete-report.png)

出现&#x200B;**[!UICONTROL 删除报告]**&#x200B;对话框，提示您确认删除。 选择&#x200B;**[!UICONTROL 删除]**。

![突出显示带有“删除”选项的“删除报告”对话框。](/help/assets/collaborate/measure/delete-report-confirm.png)

确认对话框用于确认报告已成功删除。
