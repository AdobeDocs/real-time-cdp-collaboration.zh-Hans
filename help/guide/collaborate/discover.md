---
title: 发现重叠并比较受众
description: 发现与协作者受众之间的重叠。 了解如何发现可在营销活动中使用的最佳受众。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 38c42ad3-9d01-4d09-b80e-37fb51cbf42b
source-git-commit: acaaaa1e1fab981d874210639c16e76e48fc3394
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 24%

---

# 发现重叠并比较受众

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>**[!UICONTROL 发现]**&#x200B;工作区仅在连接过程](../connect/establishing-connections.md#connection-settings)中启用了[受众发现&#x200B;**用例时才可用。**&#x200B;有关用例的更多信息，请参阅[管理项目](./manage-projects.md#project-use-cases)指南。

在广告商和发布商之间的协作空间中[创建项目](/help/guide/collaborate/manage-projects.md)后，您现在可以将受众与协作者受众进行比较。 通过这种方法，您可以发现受众之间的重叠，并获得按匹配键或身份划分的见解。 这有助于广告商决定与发布者共享哪些受众以进行激活。

>[!IMPORTANT]
>
>任何[数据草图](/help/guide/glossary.md#sketches)未更新或未刷新将在7天后删除。 发生这种情况时，此页面上各种重叠报表中显示的数字将变为零，并且受众共享将对这些过期的受众不可用。 数据草图将自动刷新具有[活动刷新计划](/help/guide/setup/onboard-audiences.md#schedule)的受众。

![发现重叠](/help/assets/collaborate/discover-overlaps/discover-overlaps.png)

当您[与发布者](/help/guide/connect/establishing-connections.md#connection-settings)连接时，将设置用于发现和比较受众的匹配键。 要更改为运行营销活动做准备时指示的重叠百分比，您可以删除匹配键，但此时无法添加新的匹配键。 为此，请转到协作者之间的[连接设置](/help/guide/connect/establishing-connections.md#connection-settings)。

![编辑匹配键屏幕](/help/assets/collaborate/discover-overlaps/edit-match-keys.png)

## 先决条件 {#prerequisites}

要充分利用&#x200B;**[!UICONTROL 协作]**&#x200B;工作流的&#x200B;**[!UICONTROL 发现]**&#x200B;选项卡中的功能，您已：

* [导入的受众](/help/guide/setup/onboard-audiences.md)
* [已连接](/help/guide/connect/establishing-connections.md)，其中所需的广告商或发布商启用了&#x200B;**受众发现**&#x200B;用例
* [已创建您与协作者之间的项目](/help/guide/collaborate/manage-projects.md)

满足上述先决条件后，您就可以开始探索和比较与协作者的受众之间的重叠。

## 比较受众 {#compare-audiences}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_compare_audiences"
>title="比较受众"
>abstract="发现您和您的协作者的受众群体之间的重叠部分。您可以调整下拉选择器中的设置，发现您的一个或多个受众与您协作者的一个或多个受众之间的重叠部分。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_your_identity_count"
>title="您的身份标识计数"
>abstract="属于您所选受众的、具有选定身份标识的轮廓数量"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_collaborator_identity_count"
>title="协作者身份标识计数"
>abstract="属于您协作者所选受众的、具有选定身份标识的轮廓数量"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlapping_identities_count"
>title="重叠的身份标识计数"
>abstract="您和您的协作者的受众中同时存在的具有选定身份标识的轮廓数量"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlapping_identities_percentage"
>title="重叠的身份标识百分比"
>abstract="您和您的协作者所选受众之间重叠的轮廓百分比。"

使用比较受众卡可获取有关您的受众与协作者受众之间重叠的丰富信息。 您可以选择比较以下任何受众组合：

* 您的其中一个受众与您的协作者的其中一个受众
* 您的其中一个受众与您的协作者所在的所有受众对决
* 针对某个协作者受众的所有受众
* 针对协作者所有受众的所有受众

所显示的信息与：

| 量度 | 描述 |
|---------|----------|
| **[!UICONTROL 身份计数]**（您的） | 所选受众中具有选定标识的配置文件数。 |
| **[!UICONTROL 身份计数]** （您的协作者） | 具有选定身份且属于协作者选定受众的配置文件数。 |
| **[!UICONTROL 身份重叠]** | 您的和协作者受众中同时存在的具有选定标识的配置文件数。 |
| **[!UICONTROL 重叠百分比]** | 您和您的协作者所选受众之间重叠的轮廓百分比。 |
| **[!UICONTROL 按匹配键划分身份]** | 根据您和您的协作者为项目商定的匹配键，按各个匹配键查看重叠计算中的身份组成。 |

{style="table-layout:auto"}

>[!TIP]
>
>并非所有受众都始终可以使用重叠百分比数字。 重叠百分比指示器的可见性取决于您的协作者在[元数据可见性部分](/help/guide/setup/onboard-audiences.md#metadata-visibility)中为受众选择的设置。

## 相关受众 {#relevant-audiences}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_relevant_audiences"
>title="相关受众"
>abstract="根据重叠百分比，这些发布者受众可能非常适合您的营销活动。<br><br><b>身份标识计数</b>是发布者的受众规模。<br><br> <b>重叠的身份标识</b>表示推荐发布者受众与所有广告商受众之间的重叠。<br><br><b>重叠率</b>是指重叠的身份标识数量除以<i>所有</i>广告商受众的规模。"

**[!UICONTROL 发现]**&#x200B;模块中的&#x200B;**[!UICONTROL 相关受众]**&#x200B;视图根据重叠百分比提供了前五个受众的精选列表。 此功能可帮助您快速识别与当前数据重叠程度最高的受众，使您能够更有效地定位营销活动。

* **[!UICONTROL 标识计数]**&#x200B;是发布者的受众大小。
* **[!UICONTROL 标识重叠]**&#x200B;表示推荐的发布者受众与所有广告商受众之间的重叠。
* **[!UICONTROL 重叠%]**&#x200B;表示重叠身份数除以&#x200B;*所有*&#x200B;广告商受众的大小。

![相关受众视图](/help/assets/collaborate/discover-overlaps/relevant-audiences-highlighted.png)

## 发现重叠 {#discover-overlaps}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlaps_collaborator_audiences"
>title="发现与个体受众的重叠"
>abstract="了解该受众群体及其与协作者身份标识范围的重叠情况。"

![发现与不同受众视图的重叠](/help/assets/collaborate/discover-overlaps/discover-overlaps-cards-view.png)

获取有关您的协作者受众的广泛信息，并查看重叠信息，将这些受众与您的所有受众中的全部群体计数或您的特定受众进行比较。

>[!TIP]
>
>屏幕快照中指示的某些数字可能并非始终适用于所有受众。 其可见性取决于您的协作者在[元数据可见性部分](/help/guide/setup/onboard-audiences.md#metadata-visibility)中为受众选择的设置。

## 后续步骤

在浏览并发现所需的受众后，是时候[与发布者](/help/guide/collaborate/share.md)共享应在营销活动中使用的受众了。
