---
title: Amazon Marketing Cloud
description: 了解如何在Real-Time CDP Collaboration中与Amazon Marketing Cloud协作。
audience: publisher, advertiser
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/cn/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 1a1b8fec-384b-465f-832d-0772c518fdf1
TQID: https://experienceleague.adobe.com/jNTQWEaUuuvgqKboJWsUH4XoKStP49nB0GLUSze0eXw
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
feature_v2:
  - id: ba929a52-9339-4154-9487-317dc875a3c7
topic_v2:
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: b29c92fa411198ec4e9a0a493c91ee302a327697
workflow-type: tm+mt
source-wordcount: 699
ht-degree: 11%

---

# Amazon Marketing Cloud

{{limited-availability-release-note}}

与[!DNL Amazon Marketing Cloud] ([!DNL AMC])建立连接后，广告商可以[创建项目](../manage-projects.md#create-project)以与[!DNL AMC]协作。 [!DNL AMC]项目支持两种用例：使用&#x200B;**[!UICONTROL 发现]**&#x200B;分区的&#x200B;**受众发现**&#x200B;和使用&#x200B;**[!UICONTROL 度量]**&#x200B;选项卡的&#x200B;**度量**。

## 发现 {#discover}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_compare_audiences"
>title="比较受众"
>abstract="将您的受众与通过 Amazon Ads 触达的所有消费者进行比较。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_relevant_audiences"
>title="相关受众"
>abstract="在仅考虑 DSP 展示的情况下，与您的受众重叠度最高的 Amazon 定向区段（这些区段仅可在 DSP 中进行定向）。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_resolved_ids"
>title="已解析的 ID"
>abstract="Amazon通过身份解析能够使用受众数据解析的ID数量。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_overlapping_ad_exposed_ids"
>title="重叠的广告展示 ID"
>abstract="这表示已上传受众中也通过Amazon Ads向广告公开的“已解决ID”的数量。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_overlap_percentage"
>title="重叠 %"
>abstract="通过Amazon Ads向广告公开的“已解决ID”比例。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_amazon_breakdown"
>title="按 Amazon 广告产品细分"
>abstract="Amazon Ads赞助产品和/或Amazon Ads DSP达到的“重叠广告显示ID”的细分。"

在&#x200B;**[!UICONTROL 发现]**&#x200B;部分中，您可以将AMC受众与通过Amazon广告访问的所有消费者进行比较。 您还可以查看受众与重叠程度最高的区段的Amazon定位，其中仅考虑DSP展示次数（这些区段只能在DSP中定位）。

>[!IMPORTANT]
>
>受众数据通过上传到您[!DNL Amazon Ads]帐户的受众进行处理。 要了解如何使用Experience Platform的目标功能将受众发送到您的[!DNL Amazon Ads]帐户，请阅读[Amazon Ads连接](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/destinations/catalog/advertising/amazon-ads)指南。

![使用Amazon Marketing Cloud的项目中的“发现”部分。](/help/assets/collaborate/advertising-platforms/amc-discover.png){zoomable="yes"}

### 比较受众 {#compare-audiences}

**[!UICONTROL 比较受众]**&#x200B;部分提供了有关您的[!DNL AMC]受众如何与Amazon广告所触及的消费者重叠的分析。 在&#x200B;**[!UICONTROL 比较受众]**&#x200B;部分中，可以查看以下量度：

| 量度 | 描述 |
|--------------------------------|---------------------------------------------------------------------------------------------------|
| [!UICONTROL 已解析的ID] | 使用您的受众数据能够解析的ID数量[!DNL Amazon's Identity Resolution]。 |
| [!UICONTROL 重叠的广告公开ID] | 已上传受众中也通过[!DNL Amazon Ads]向广告公开的[!UICONTROL 已解决ID]的数量。 |
| [!UICONTROL 重叠%] | 已通过[!DNL Amazon Ads]向广告公开的[!UICONTROL 已解析ID]的比例。 |
| [!UICONTROL 按Amazon广告产品细分] | [!UICONTROL 赞助的产品]和/或[!UICONTROL DSP]所达到的[!UICONTROL 重叠的广告公开ID]的划分。 每个ID均以广告公开ID总数的单个百分比表示。 由于ID同时属于[!UICONTROL 赞助的产品]和[!UICONTROL DSP]，因此百分比总和不能为100%。 |


### 相关受众 {#relevant-audiences}

**[!UICONTROL 相关受众]**&#x200B;部分提供了有关您的受众与重叠程度最高的区段或受众的[!DNL Amazon]的分析，其中仅考虑了DSP展示次数（这些区段只能在DSP中定位）。 您可以在所有相关受众之间切换，并在每个部分中，查看以下量度：

| 量度 | 描述 |
|--------------------------------|---------------------------------------------------------------------------------------------------|
| [!UICONTROL 已解析的ID] | 使用您的受众数据能够解析的ID数量[!DNL Amazon's Identity Resolution]。 |
| [!UICONTROL 重叠的广告公开ID] | 这表示已上传受众中也已通过[!DNL Amazon Ads]向广告公开的[!UICONTROL 已解析ID]的数量。 这仅考虑DSP展示次数。 |
| [!UICONTROL 重叠%] | 已通过[!DNL Amazon Ads]向广告公开的[!UICONTROL 已解析ID]的比例。 |
| [!UICONTROL 类别] | 受众所属的类别。 一个受众可以属于多个类别。 |

### 发现与[!DNL Amazon Marketing Cloud]的重叠 {#discover-overlaps}

**[!UICONTROL 发现与Amazon Marketing Cloud的重叠]**&#x200B;部分提供了有关您的受众如何与[!DNL Amazon]定位区段或受众重叠的分析。 您可以查看以下量度：

| 量度 | 描述 |
|--------------------------------|---------------------------------------------------------------------------------------------------|
| [!UICONTROL 已解析的ID] | 使用您的受众数据能够解析的ID数量[!DNL Amazon's Identity Resolution]。 |
| [!UICONTROL 重叠的广告公开ID] | 这表示已上传受众中也已通过[!DNL Amazon Ads]向广告公开的[!UICONTROL 已解析ID]的数量。 这仅考虑DSP展示次数。 |
| [!UICONTROL 重叠%] | 已通过[!DNL Amazon Ads]向广告公开的[!UICONTROL 已解析ID]的比例。 |

## 测量 {#measure}

当[!DNL AMC]实例包含营销活动ID时，**[!UICONTROL 度量]**&#x200B;选项卡可用。 创建项目时，Real-Time CDP Collaboration会对[!DNL AMC]数据运行后台查询以填充[!UICONTROL 发现]部分以及用于配置测量报告的营销活动和转化事件列表。

有关创建和解释[!DNL AMC]测量报告的分步说明，请阅读[创建AMC测量报告](./amc-measure.md)指南。
