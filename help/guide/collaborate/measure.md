---
title: 衡量绩效
description: 衡量不同渠道中的促销活动效果。 了解如何使用和解读各种报表。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/cn/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: c92b263e-1f96-49f1-841a-ef2e97a4cb9a
source-git-commit: b52fd181d80d5a70331571f7a4cbe3e5a7ec1d7c
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 18%

---

# 衡量绩效

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>只有在连接过程[&#128279;](../connect/establishing-connections.md#connection-settings)期间启用了的&#x200B;**测量**&#x200B;用例时，**[!UICONTROL 测量]**&#x200B;工作区才可用。 有关用例的更多信息，请参阅[管理项目](./manage-projects.md#project-use-cases)指南。

了解Real-Time CDP Collaboration中的可用报表，并了解如何衡量和分析营销活动在各种渠道中的表现。

## 先决条件

在访问Real-Time CDP Collaboration中的测量报表之前，您已：

* [已连接](/help/guide/connect/establishing-connections.md)，其所需的广告商或发布者启用了&#x200B;**Measurement**&#x200B;用例，并开始在[项目](/help/guide/collaborate/manage-projects.md)上进行协作
* 运行活动并[将测量数据](/help/guide/setup/onboard-measurement-data.md)上传到Real-Time CDP Collaboration。

<!--

## Create a report {#create-report}

Hidden until functionality is live. At that point, move the contextualhelp from below into this section. 

The syntax rtcdp_collaboration_measurement_create_report is currently implemented in the UI. However, a preference would be to imlement the other contextualhelp ID from below instead, since that explicitly includes campaignID in the syntax. Need to sync up with UI team. More details in CORE-116991.

-->

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
>abstract="使用“随时间变化的量度”视图，了解在营销活动期间为您的创意显示的总展示次数。您最多可以选择两个维度在报告中显示。"

使用“随时间变化的量度”视图，了解在营销活动期间为您的创意显示的总展示次数。请注意，您最多可以选择两个量度以在报表中显示和分析。

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

## 后续步骤

![发现、激活、测量广告商。](/help/assets/end-to-end-workflow/discover-activate-measure.png)

秉承上图中循环播放的精神，利用您在规划下一场营销活动时从查看报告获得的洞察力。 作为广告商，如有必要，请返回以发现不同的发布者，然后运行重叠来发现您的后续促销活动的不同受众。
