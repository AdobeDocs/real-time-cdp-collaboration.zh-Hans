---
title: 发现重叠并比较受众
description: 发现与协作者受众之间的重叠。 了解如何发现可在营销活动中使用的最佳受众。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/cn/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 38c42ad3-9d01-4d09-b80e-37fb51cbf42b
source-git-commit: 76ad3357aa4cd02dbc0616e5d8bd03b03683b7fd
workflow-type: tm+mt
source-wordcount: '2068'
ht-degree: 12%

---

# 发现重叠并比较受众

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>**[!UICONTROL 发现]**&#x200B;工作区仅在连接过程&#x200B;**中启用了**&#x200B;受众发现[用例时才可用。 ](../connect/establishing-connections.md#connection-settings)有关用例的更多信息，请参阅[管理项目](./manage-projects.md#project-use-cases)指南。

在[创建项目](/help/guide/collaborate/manage-projects.md)之后，您可以将受众与协作者进行比较。 这有助于您识别营销活动的相关受众，并决定要将哪些受众发送给协作者进行激活。

>[!IMPORTANT]
>
>任何[数据草图](/help/guide/glossary.md#sketches)未更新或未刷新将在7天后删除。 发生这种情况时，此页面上各种重叠报表中显示的数字将变为零，并且受众共享将对这些过期的受众不可用。 数据草图将自动刷新具有[活动刷新计划](/help/guide/setup/onboard-audiences.md#schedule)的受众。

在连接过程[中设置](/help/guide/connect/establishing-connections.md#connection-settings)用于发现和比较受众的匹配键。 匹配键用于计算受众之间的重叠，可以开关该键。 要编辑匹配键，请选择&#x200B;**[!UICONTROL 编辑匹配键]**&#x200B;选项。

![显示受众分析的“发现”选项卡工作区。](/help/assets/collaborate/discover/discover-overview.png)

**[!UICONTROL 编辑匹配键]**&#x200B;对话框打开，您可以在其中关闭不想使用的匹配键。 选择&#x200B;**[!UICONTROL 保存]**&#x200B;以保存更改。

![发现工作区中的“编辑匹配键”对话框。](/help/assets/collaborate/discover/edit-match-keys.png)

## 先决条件 {#prerequisites}

若要开始使用项目中的&#x200B;**[!UICONTROL 发现]**&#x200B;选项卡，您应具有：

* [将受众源](/help/guide/setup/onboard-audiences.md)放入您的帐户
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
>abstract="根据您与协作者为该项目商定的匹配键，显示所选受众中的唯一 ID 数量。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_collaborator_identity_count"
>title="协作者身份标识计数"
>abstract="根据您与协作者为该项目商定的匹配键，显示协作者受众中的唯一 ID 数量。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlapping_identities_count"
>title="重叠的身份标识计数"
>abstract="根据您与协作者为该项目商定的匹配键，显示在您和协作者的受众中均存在的唯一 ID 数量。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlapping_identities_percentage"
>title="重叠的身份标识百分比"
>abstract="您与协作者所选受众之间的身份标识重合比例（以百分比表示）。"

使用比较受众部分可获取有关您的受众与协作者受众之间重叠的丰富信息。 要更改受众选择，请使用&#x200B;**[!UICONTROL 比较受众]**&#x200B;部分顶部的下拉选择器。 您可以选择一个或多个受众，以及协作者的一个或多个受众进行相互比较。

![在“比较受众”部分突出显示具有受众选择器的发现工作区。](/help/assets/collaborate/discover/compare-audiences-selector.png)

在比较受众部分中，您可以看到以下量度，这些量度基于您和您的协作者为项目商定的匹配键：

| 量度 | 描述 |
|---------|----------|
| **[!UICONTROL 身份计数]**（您的） | 选定受众中的唯一ID数量。 |
| **[!UICONTROL 身份计数]** （您的协作者） | 协作者受众中的唯一ID数量。 |
| **[!UICONTROL 身份重叠]** | 您的和协作者受众中同时存在的唯一ID数量。 |
| **[!UICONTROL 重叠%]** | 您和您的协作者所选受众之间重叠的轮廓百分比。 |
| **[!UICONTROL 受众索引]** | 一个分数，根据基础受众计数和重叠情况指示一个受众与另一个受众之间的关联程度。 要了解有关分数含义的更多信息，请阅读[受众索引分数](#audience-index-score)部分。 与协作者的基线（所有受众）进行比较时，无法使用受众索引分数。 |
| **[!UICONTROL 按匹配键划分身份]** | 根据每个协作者选择的受众，对项目中选定的每个匹配键的标识进行细分。 |

{style="table-layout:auto"}

>[!NOTE]
>
>重叠百分比数字和受众索引得分可能并非始终适用于所有受众。 重叠百分比和受众索引得分的可见性取决于您的协作者在[元数据可见性部分](/help/guide/setup/onboard-audiences.md#metadata-visibility)中为受众选择的设置。

如果协作者未启用受众索引或重叠百分比，则受众将没有任何可用的比较数据。

## 相关受众 {#relevant-audiences}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_relevant_audiences"
>title="相关受众"
>abstract="根据重叠百分比，这些受众可能非常适合您的营销活动。<br><br><b>身份标识计数</b>是协作者的受众规模。<br><br> <b>重叠的身份标识</b>表示推荐受众与您的所有受众之间的重叠。<br><br><b>重叠率</b>是指重叠的身份标识数量除以您的<i>所有</i>受众的规模。"

**[!UICONTROL 发现]**&#x200B;选项卡中的&#x200B;**[!UICONTROL 相关受众]**&#x200B;部分根据协作者受众与所有受众之间的重叠百分比，提供了前五个受众的策划列表。 此功能可帮助您快速识别重叠程度最高的受众，使您能够更有效地定位营销活动。 使用部分右上角的页面选择器，在相关受众之间切换。

![突出显示具有相关受众部分的发现工作区。](/help/assets/collaborate/discover/relevant-audiences.png)

>[!NOTE]
>
>协作者受众的可见性取决于协作者在[连接访问部分](/help/guide/setup/onboard-audiences.md#connection-access)和[元数据可见性部分](/help/guide/setup/onboard-audiences.md#metadata-visibility)中为受众选择的设置。 如果您的协作者已将所有受众设置为专用，则此部分不会显示任何受众。

**[!UICONTROL 相关受众]**&#x200B;部分显示每个推荐受众的以下信息：

| 量度 | 描述 |
|---------|----------|
| **[!UICONTROL 身份计数]** | 受众中唯一ID的数量。 |
| **[!UICONTROL 身份重叠]** | 推荐的受众与您的所有受众之间重叠的唯一ID数量。 |
| **[!UICONTROL 重叠%]** | 推荐受众和您的所有受众之间重叠身份的百分比。 |
| **[!UICONTROL 受众索引]** | 一个分数，根据基础受众计数和重叠情况指示一个受众与另一个受众之间的关联程度。 要了解有关分数含义的更多信息，请阅读[受众索引分数](#audience-index-score)部分。 |
| **[!UICONTROL 受众类别]** | 您的协作者分配给受众的类别。 |
| **[!UICONTROL 匹配键]** | 您的协作者为受众选择的匹配键。 |

{style="table-layout:auto"}

如果您为任何协作者受众启用了受众索引得分，则相关受众将基于受众索引得分，并且所有未启用受众索引的受众都不会包含在内。 基于受众索引分数的相关受众将进行排序，以便首先显示最高索引分数。 如果没有为协作者任何受众启用受众索引，则相关受众将基于重叠百分比。

## 发现重叠 {#discover-overlaps}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_overlaps_collaborator_audiences"
>title="发现与个体受众的重叠"
>abstract="深入了解您与协作者受众之间的重合情况。"

发现重叠，深入了解受众与协作者受众的对比情况。 默认情况下，此部分会将您的所有受众与协作者各自的受众进行比较。 使用部分底部的分页控件在可用受众中导航。

![突出显示具有发现重叠部分的发现工作区。](/help/assets/collaborate/discover/discover-overlaps.png)

>[!NOTE]
>
>协作者受众的可见性取决于协作者在[连接访问部分](/help/guide/setup/onboard-audiences.md#connection-access)和[元数据可见性部分](/help/guide/setup/onboard-audiences.md#metadata-visibility)中为受众选择的设置。 如果您的协作者已将所有受众设置为专用，则此部分不会显示任何受众。

如果您的协作者未启用受众索引或重叠百分比，则不会显示受众。

要更改受众选择，请选择&#x200B;**[!UICONTROL 更改受众]**。

![突出显示了“发现工作区”中的“更改受众”选项。](/help/assets/collaborate/discover/change-audience.png)

将打开&#x200B;**[!UICONTROL 更改受众]**&#x200B;对话框，您可以在其中选择要与协作者受众进行比较的特定受众。 选择所需的受众，或清除选择以选择所有受众，然后选择&#x200B;**[!UICONTROL 保存]**。

![发现工作区中的“更改受众”对话框。](/help/assets/collaborate/discover/change-audience-selection.png)

选择所需的受众后，**[!UICONTROL 发现重叠]**&#x200B;部分会显示每个受众的以下信息：

| 量度 | 描述 |
|---------|----------|
| **[!UICONTROL 身份计数]** | 受众中唯一ID的数量。 |
| **[!UICONTROL 身份重叠]** | 推荐的受众与您的所有受众之间重叠的唯一ID数量。 |
| **[!UICONTROL 重叠%]** | 推荐受众和您的所有受众之间重叠身份的百分比。 |
| **[!UICONTROL 受众索引]** | 一个分数，根据基础受众计数和重叠情况指示一个受众与另一个受众之间的关联程度。 要了解有关分数含义的更多信息，请阅读[受众索引分数](#audience-index-score)部分。 |
| **[!UICONTROL 受众类别]** | 您的协作者分配给受众的类别。 |
| **[!UICONTROL 匹配键]** | 您的协作者为受众选择的匹配键。 |

{style="table-layout:auto"}

## 受众索引得分 {#audience-index-score}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_discover_audience_index_score"
>title="受众索引得分"
>abstract="受众索引得分是一个细微的指标，可根据基础受众计数和重叠情况显示一个受众与另一个受众之间的关联程度。 原始索引得分被转换为相关性区段，该相关性区段对受众索引得分从非常低到非常高进行分类。 这使您能够快速评估受众与协作者的受众之间的关系强度。"

受众索引得分是一个细微的指标，可根据基础受众计数和重叠情况显示一个受众与另一个受众之间的关联程度。 这有助于使受众见解符合情境，并确定潜在受众和营销活动定位的潜在受众。

使用以下公式计算索引得分：

![计算索引分数的公式。](/help/assets/collaborate/discover/index-score-formula.png)

想象一下，一家汽车生产商想与一家大型电视发行商就一款新款SUV展开广告攻势。 这家汽车制造商掌握了目前拥有相似车型的客户数据，希望利用这些数据找到更多潜在客户，将他们转化为客户。 这家汽车生产商从CTV发布商的受众中寻找与目前SUV拥有者密切相符的受众。

![汽车广告商与CTV发布者受众。](/help/assets/collaborate/discover/audience-index-score-example.png)

将计算索引得分，并可用于确定促销活动是否可能成功：

| CTV发布者受众 | 公式 | 索引得分(i) | 解释 |
|------------------------|-------------|----------------|----------------|
| 基线（所有受众） | (（1.3米/1.3米）/（50米/50米）) * 100 | 100 | 这是与协作者的其他受众进行比较的基准。 |
| 狂欢的观察者 | (（50万/ 130万）/（20米/ 50米）) * 100 | 96 | 通过定位此受众，您获得SUV拥有者的可能性比基线低4%。 |
| 喜剧爱好者 | (（20万/ 130万） / （6万/ 50万）) * 100 | 128 | 通过定位此受众，您获得SUV所有者的可能性比基线高出28%。 |
| 男性25-34岁 | (（70万/ 130万）/（12万/ 50万）) * 100 | 224 | 通过定位此受众，您获得SUV所有者的可能性比基线高出124%。 |
| 技术爱好者 | (（50万/ 130万） / （8米/ 50米）) * 100 | 240 | 通过定位此受众，您获得SUV所有者的可能性比基线高出140%。 |

为了更好地了解索引分数如何影响您的营销活动，将与分数一起提供相关性范围。

### 相关性区段 {#audience-index-relevance-bands}

为了能够轻松地对不同受众和营销活动进行比较，Collaboration将索引分数转换为相关性范围（从很低到很高）。 这使您能够快速评估受众与协作者的受众之间的关系强度。

| 索引得分(i) | 相关性范围 | 描述 |
|---------|----------|-----------|
| i &lt; 60 | 非常低 | 与您的受众相比，重叠在目标受众中较少发生，这表明关系非常薄弱。 使用此受众的客户访问其目标受众的可能性要低得多。 |
| 60 &lt; i &lt; 80 | 低 | 与您的受众相比，重叠在目标受众中不太普遍，这表明关系薄弱。 使用此受众的客户访问其目标受众的可能性较小。 |
| 80 &lt; i &lt; 120 | 媒介 | 重叠在目标受众中和在您的受众中一样普遍，这显示了典型的关系。 使用此受众的客户平均可能会访问其目标受众。 |
| 120 &lt; i &lt; 140 | 高 | 与您的受众相比，重叠现象在目标受众中更为普遍，表现出很强的关系。 使用此受众的客户更有可能接触到其目标受众。 |
| i > 140 | 非常高 | 与您的受众相比，重叠在目标受众中更为普遍，这反映了非常牢固的关系。 使用此受众的客户更有可能接触到其目标受众。 |

在发现重叠部分中，受众索引得分将与得分一起显示相关性范围。 得分将进行颜色编码以指示相关带，使得很容易一眼就识别关系的强度。 极低相关带和低相关带以橙色显示，中相关带以黑色显示，高相关带和极高相关带以绿色显示。

## 后续步骤

浏览并发现所需的受众后，是时候[激活](/help/guide/collaborate/activate.md)应在营销活动中使用的受众了。
