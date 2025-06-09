---
title: 发现重叠并比较受众
description: 发现与协作者受众之间的重叠。 了解如何发现可在营销活动中使用的最佳受众。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 38c42ad3-9d01-4d09-b80e-37fb51cbf42b
source-git-commit: f19aff1b7d10a446dd209721e7a6fdf537c9d63e
workflow-type: tm+mt
source-wordcount: '1206'
ht-degree: 11%

---

# 发现重叠并比较受众

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>**[!UICONTROL 发现]**&#x200B;工作区仅在连接过程[&#128279;](../connect/establishing-connections.md#connection-settings)中启用了受众发现&#x200B;**用例时才可用。**&#x200B;有关用例的更多信息，请参阅[管理项目](./manage-projects.md#project-use-cases)指南。

在[创建项目](/help/guide/collaborate/manage-projects.md)之后，您可以将受众与协作者进行比较。 这有助于您识别营销活动的相关受众，并决定要将哪些受众发送给发布者进行激活。

>[!IMPORTANT]
>
>任何[数据草图](/help/guide/glossary.md#sketches)未更新或未刷新将在7天后删除。 发生这种情况时，此页面上各种重叠报表中显示的数字将变为零，并且受众共享将对这些过期的受众不可用。 数据草图将自动刷新具有[活动刷新计划](/help/guide/setup/onboard-audiences.md#schedule)的受众。

在连接过程[&#128279;](/help/guide/connect/establishing-connections.md#connection-settings)中设置用于发现和比较受众的匹配键。 匹配键用于计算受众之间的重叠，可以切换开关。 要编辑匹配键，请选择&#x200B;**[!UICONTROL 编辑匹配键]**&#x200B;选项。 此

![显示受众分析的“发现”选项卡工作区。](/help/assets/collaborate/discover/discover-overview.png)

**[!UICONTROL 编辑匹配键]**&#x200B;对话框打开，您可以在其中关闭不想使用的匹配键。 选择&#x200B;**[!UICONTROL 保存]**&#x200B;以保存更改。

![发现工作区中的“编辑匹配键”对话框。](/help/assets/collaborate/discover/edit-match-keys.png)

## 先决条件 {#prerequisites}

若要开始使用项目中的&#x200B;**[!UICONTROL 发现]**&#x200B;选项卡，您应具有：

* [已将受众](/help/guide/setup/onboard-audiences.md)导入您的组织
* [已连接](/help/guide/connect/establishing-connections.md)，协作者启用了&#x200B;**受众发现**&#x200B;用例
* [已创建您与协作者之间的项目](/help/guide/collaborate/manage-projects.md)

在满足这些先决条件后，您可以开始探索和比较您与协作者受众之间的重叠。

## 比较受众 {#compare-audiences}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_compare_audiences"
>title="比较受众"
>abstract="发现您和您的协作者的受众群体之间的重叠部分。您可以调整下拉选择器中的设置，发现您的一个或多个受众与您协作者的一个或多个受众之间的重叠部分。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_your_identity_count"
>title="您的身份标识计数"
>abstract="所选受众中的唯一ID数量，基于您和协作者为项目商定的匹配键。"
>
>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_collaborator_identity_count"
>title="协作者身份标识计数"
>abstract="协作者的受众中的唯一ID数量，基于您和协作者为项目商定的匹配键。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlapping_identities_count"
>title="重叠的身份标识计数"
>abstract="根据您和协作者为项目商定的匹配键，您和协作者的受众中同时存在的唯一ID数量。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlapping_identities_percentage"
>title="重叠的身份标识百分比"
>abstract="您与协作者所选受众之间重叠身份的百分比。"

使用比较受众部分可获取有关您的受众与协作者受众之间重叠的丰富信息。 要更改受众选择，请使用&#x200B;**[!UICONTROL 比较受众]**&#x200B;部分顶部的下拉选择器。 您可以选择一个或多个受众，以及协作者的一个或多个受众进行相互比较。

![在“比较受众”部分突出显示具有受众选择器的发现工作区。](/help/assets/collaborate/discover/compare-audiences-selector.png)

在比较受众部分中，您可以看到以下量度，这些量度基于您和您的协作者为项目商定的匹配键：

| 量度 | 描述 |
|---------|----------|
| **[!UICONTROL 身份计数]**（您的） | 选定受众中的唯一ID数量。 |
| **[!UICONTROL 身份计数]** （您的协作者） | 协作者受众中的唯一ID数量。 |
| **[!UICONTROL 身份重叠]** | 您的和协作者受众中同时存在的唯一ID数量。 |
| **[!UICONTROL 重叠%]** | 您和您的协作者所选受众之间重叠的轮廓百分比。 |
| **[!UICONTROL 按匹配键划分身份]** | 根据每个协作者选择的受众，对项目中选定的每个匹配键的标识进行细分。 |

{style="table-layout:auto"}

>[!TIP]
>
>并非所有受众都始终可以使用重叠百分比数字。 重叠百分比指示器的可见性取决于您的协作者在[元数据可见性部分](/help/guide/setup/onboard-audiences.md#metadata-visibility)中为受众选择的设置。

## 相关受众 {#relevant-audiences}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_relevant_audiences"
>title="相关受众"
>abstract="根据重叠百分比，这些发布者受众可能非常适合您的营销活动。<br><br><b>身份标识计数</b>是发布者的受众规模。<br><br> <b>重叠的身份标识</b>表示推荐发布者受众与所有广告商受众之间的重叠。<br><br><b>重叠率</b>是指重叠的身份标识数量除以<i>所有</i>广告商受众的规模。"

**[!UICONTROL 发现]**&#x200B;选项卡中的&#x200B;**[!UICONTROL 相关受众]**&#x200B;部分根据协作者受众与所有受众之间的重叠百分比，提供了前五个受众的策划列表。 此功能可帮助您快速识别重叠程度最高的受众，使您能够更有效地定位营销活动。 使用部分右上角的页面选择器，在相关受众之间切换。

![突出显示具有相关受众部分的发现工作区。](/help/assets/collaborate/discover/relevant-audiences.png)

>[!NOTE]
>
>协作者受众的可见性取决于协作者在[元数据可见性部分](/help/guide/setup/onboard-audiences.md#metadata-visibility)中为受众选择的设置。 如果您的协作者已将所有受众设置为专用，则此部分不会显示任何受众。

**[!UICONTROL 相关受众]**&#x200B;部分显示每个推荐受众的以下信息：

| 量度 | 描述 |
|---------|----------|
| **[!UICONTROL 身份计数]** | 受众中的唯一ID名称。 |
| **[!UICONTROL 身份重叠]** | 推荐的受众与您的所有受众之间重叠的唯一ID数量。 |
| **[!UICONTROL 重叠%]** | 推荐受众和您的所有受众之间重叠身份的百分比。 |
| **[!UICONTROL 受众类别]** | 您的协作者分配给受众的类别。 |
| **[!UICONTROL 匹配键]** | 您的协作者为受众选择的匹配键。 |

{style="table-layout:auto"}

>[!NOTE]
>
>协作者受众的可见性取决于协作者在[元数据可见性部分](/help/guide/setup/onboard-audiences.md#metadata-visibility)中为受众选择的设置。 如果您的协作者已将所有受众设置为专用，则此部分不会显示任何受众。

## 发现重叠 {#discover-overlaps}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlaps_collaborator_audiences"
>title="发现与个体受众的重叠"
>abstract="深入了解受众和协作者受众之间的重叠。"

发现重叠，深入了解受众与协作者受众的对比情况。 默认情况下，此部分会将您的所有受众与协作者各自的受众进行比较。 使用部分底部的分页控件在可用受众中导航。

![突出显示具有发现重叠部分的发现工作区。](/help/assets/collaborate/discover/discover-overlaps.png)

>[!NOTE]
>
>协作者受众的可见性取决于协作者在[元数据可见性部分](/help/guide/setup/onboard-audiences.md#metadata-visibility)中为受众选择的设置。 如果您的协作者已将所有受众设置为专用，则此部分不会显示任何受众。

要更改受众选择，请选择&#x200B;**[!UICONTROL 更改受众]**。

![突出显示了“发现工作区”中的“更改受众”选项。](/help/assets/collaborate/discover/change-audience.png)

将打开&#x200B;**[!UICONTROL 更改受众]**&#x200B;对话框，您可以在其中将特定受众与协作者受众进行比较。 选择所需的受众，或清除选择以选择所有受众，然后选择&#x200B;**[!UICONTROL 保存]**。

![发现工作区中的“更改受众”对话框。](/help/assets/collaborate/discover/change-audience-selection.png)

选择所需的受众后，**[!UICONTROL 发现重叠]**&#x200B;部分会显示每个受众的以下信息：

| 量度 | 描述 |
|---------|----------|
| **[!UICONTROL 身份计数]** | 受众中的唯一ID名称。 |
| **[!UICONTROL 身份重叠]** | 推荐的受众与您的所有受众之间重叠的唯一ID数量。 |
| **[!UICONTROL 重叠%]** | 推荐受众和您的所有受众之间重叠身份的百分比。 |
| **[!UICONTROL 受众类别]** | 您的协作者分配给受众的类别。 |
| **[!UICONTROL 匹配键]** | 您的协作者为受众选择的匹配键。 |

{style="table-layout:auto"}

## 后续步骤

浏览并发现所需的受众后，是时候[激活](/help/guide/collaborate/activate.md)应在营销活动中使用的受众了。
