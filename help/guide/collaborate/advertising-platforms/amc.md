---
title: Amazon Marketing Cloud
description: 了解如何在Real-Time CDP Collaboration中与Amazon Marketing Cloud协作。
audience: publisher, advertiser
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/cn/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
source-git-commit: 57b847c25edbf88f4708bda74be41fe6141472a7
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 4%

---

# Amazon Marketing Cloud

{{limited-availability-release-note}}

与[!DNL Amazon Marketing Cloud] ([!DNL AMC])建立连接后，广告商可以[创建项目](../manage-projects.md#create-project)以与[!DNL AMC]协作，从而利用其高级分析功能。 创建项目后，您可以使用&#x200B;**[!UICONTROL 发现]**&#x200B;部分来比较受众分析并发现营销活动的相关受众。

>[!IMPORTANT]
>
>[!DNL AMC]唯一支持的用例是&#x200B;**受众发现**&#x200B;和&#x200B;**测量**。 当前，在具有&#x200B;**[!UICONTROL 的项目中，只有]**&#x200B;发现[!DNL AMC]部分可用。

## 发现 {#discover}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_compare_audiences"
>title="比较受众"
>abstract="将您的受众与通过Amazon广告触及的所有消费者进行比较。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_relevant_audiences"
>title="相关受众"
>abstract="Amazon仅考虑DSP展示次数，以定位受众重叠程度最高的区段(这些区段只能在DSP中定位)。"

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

在&#x200B;**[!UICONTROL 发现]**&#x200B;部分中，您可以将AMC受众与通过Amazon广告访问的所有消费者进行比较。 您还可以查看受众与重叠程度最高的区段的Amazon定位，其中仅考虑DSP展示次数(这些区段只能在DSP中定位)。

>[!IMPORTANT]
>
>受众数据通过上传到您[!DNL Amazon Ads]帐户的受众进行处理。 要了解如何使用Experience Platform的目标功能将受众发送到您的[!DNL Amazon Ads]帐户，请阅读[Amazon Ads连接](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/destinations/catalog/advertising/amazon-ads)指南。

![使用Amazon Marketing Cloud的项目中的“发现”部分。](/help/assets/collaborate/advertising-platforms/amc-discover.png){zoomable="yes"}

### 比较受众 {#compare-audiences}

**[!UICONTROL 比较受众]**&#x200B;部分提供了有关您的[!DNL AMC]受众如何与Amazon广告所触及的消费者重叠的分析。 在&#x200B;**[!UICONTROL 比较受众]**&#x200B;部分中，可以查看以下量度：

| 量度 | 描述 |
|--------------------------------|---------------------------------------------------------------------------------------------------|
| [!UICONTROL 已解析的ID] | 使用您的受众数据能够解析的ID数量[!DNL Amazon’s Identity Resolution]。 |
| [!UICONTROL 重叠的广告公开ID] | 已上传受众中也通过[!UICONTROL 向广告公开的]已解决ID[!DNL Amazon Ads]的数量。 |
| [!UICONTROL 重叠%] | 已通过[!UICONTROL 向广告公开的]已解析ID[!DNL Amazon Ads]的比例。 |
| [!UICONTROL 按Amazon广告产品细分] | [!UICONTROL 赞助的产品]和/或[!UICONTROL DSP]所达到的[!UICONTROL 重叠的广告公开ID]的划分。 每个ID均以广告公开ID总数的单个百分比表示。 由于ID同时属于[!UICONTROL 赞助的产品]和[!UICONTROL DSP]，因此百分比总和不能为100%。 |


### 相关受众 {#relevant-audiences}

**[!UICONTROL 相关受众]**&#x200B;部分提供了有关您的受众与重叠程度最高的区段或受众的[!DNL Amazon]的分析，其中仅考虑了DSP展示次数(这些区段只能在DSP中定位)。 您可以在所有相关受众之间切换，并在每个部分中，查看以下量度：

| 量度 | 描述 |
|--------------------------------|---------------------------------------------------------------------------------------------------|
| [!UICONTROL 已解析的ID] | 使用您的受众数据能够解析的ID数量[!DNL Amazon’s Identity Resolution]。 |
| [!UICONTROL 重叠的广告公开ID] | 这表示已上传受众中也已通过[!UICONTROL 向广告公开的]已解析ID[!DNL Amazon Ads]的数量。 这仅考虑DSP展示次数。 |
| [!UICONTROL 重叠%] | 已通过[!UICONTROL 向广告公开的]已解析ID[!DNL Amazon Ads]的比例。 |
| [!UICONTROL 类别] | 受众所属的类别。 一个受众可以属于多个类别。 |

### 发现与[!DNL Amazon Marketing Cloud]的重叠 {#discover-overlaps}

**[!UICONTROL 发现与Amazon Marketing Cloud的重叠]**&#x200B;部分提供了有关您的受众如何与[!DNL Amazon]定位区段或受众重叠的分析。 您可以查看以下量度：

| 量度 | 描述 |
|--------------------------------|---------------------------------------------------------------------------------------------------|
| [!UICONTROL 已解析的ID] | 使用您的受众数据能够解析的ID数量[!DNL Amazon’s Identity Resolution]。 |
| [!UICONTROL 重叠的广告公开ID] | 这表示已上传受众中也已通过[!UICONTROL 向广告公开的]已解析ID[!DNL Amazon Ads]的数量。 这仅考虑DSP展示次数。 |
| [!UICONTROL 重叠%] | 已通过[!UICONTROL 向广告公开的]已解析ID[!DNL Amazon Ads]的比例。 |