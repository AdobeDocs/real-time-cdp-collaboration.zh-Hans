---
title: 受众概述
description: 了解Real-Time CDP Collaboration中的受众，包括这些受众的来源。
audience: admin, publisher
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
product_v2:
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
topic_v2:
  - id: b5520579-b31f-4df7-9281-f0d9f91e2edc
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: f7cd44177d60bfd3d3db384f7b1a250ace4c3633
workflow-type: tm+mt
source-wordcount: 707
ht-degree: 5%

---


# 受众概述

{{limited-availability-release-note}}

在Adobe Real-Time CDP Collaboration中，受众是您带入Collaboration的用户组或客户组。 在采购后，您可以使用受众来发现与协作者之间的重叠、激活受众以及衡量促销活动效果。 您可以根据受众数据的存放位置，从各种源类型获取受众，包括Adobe Experience Platform、云存储和共享系统以及文件上传工作流。

## 您可以对受众执行的操作 {#audiences-in-collaboration}

将受众来源引入Collaboration后，即可在支持的协作工作流中使用。

使用Collaboration中的受众可以：

* 比较您的受众与协作者受众
* 识别重叠和机会
* 激活受众
* 衡量结果和营销活动效果
* 管理受众可见性和相关设置

## 受众如何适应Collaboration {#conceptual-diagram}

>[!NOTE]
>
> 下图从较高层面说明了来源受众如何适应Collaboration并在项目中的使用情况。

```text
Source → Data connection → Audience → Project
                                         │
                          ┌──────────────┼──────────────┐
                          ▼              ▼              ▼
                      Discover       Activate       Measure
                                         │
                                         ▼
                                    Destination
```

## 核心概念 {#core-concepts}

以下概念描述了受众来源和协作工作流中涉及的关键对象。

**Source**\
受众数据的来源系统或位置，如Adobe Experience Platform、云存储位置或文件上传。

**数据连接**\
Collaboration用于从源访问受众数据的已配置连接。 数据连接包括特定于源的配置详细信息，如身份验证、字段映射和调度。

**受众**\
一组源自Collaboration并可用于项目中的用户或客户。

**Connection**\
您的组织与另一个组织之间的协作关系。

**项目**\
协作者可在其中将受众一起用于支持的用例（如发现、激活和测量）的工作区。

**目标**\
发送激活受众的外部平台或系统。

**匹配键**
Collaboration用于跨数据集和协作者匹配记录的标识符。 匹配键支持受众重叠、激活和测量等工作流程。

## 受众生命周期 {#audience-lifecycle}

在Collaboration中，您通过数据连接来获取受众，在&#x200B;**[!UICONTROL 设置]**&#x200B;中管理这些受众，并在项目中使用受支持的用例。

1. **Source受众**：通过数据连接将受众数据引入Collaboration。
2. **管理受众**：查看和管理受众详细信息、可见性和相关设置。
3. **在项目中使用受众**：在项目中将源受众用于支持的用例，包括&#x200B;**Discover**、**Activate**&#x200B;和&#x200B;**Measure**。

并非每个受众都用于每个用例。 例如，可以在不激活的情况下为进行&#x200B;**发现**&#x200B;而提供和使用受众，或者可以在不发送到目标的情况下在&#x200B;**度量**&#x200B;工作流中使用受众。

有关获取和管理受众的详细信息，请参阅[Source和管理受众](./onboard-audiences.md)。 有关管理数据连接的信息，请参阅[管理数据连接](./manage-data-connection.md)。

## 受众来源 {#supported-sources}

Collaboration支持多种受众源类型。 您选择的源将决定设置流程、先决条件、身份验证要求、数据格式、字段映射、刷新行为以及将受众引入Collaboration的可用配置选项。

* Adobe Experience Platform
* 云存储，包括Amazon S3、Google Cloud Storage和Azure存储
* 数据共享服务，包括Snowflake和Databricks Delta Share
* Adobe Audience Manager
* CSV文件上传

有关支持的源和特定于源的设置步骤的列表，请参阅[源概述](./source-overview.md#available-sources)。

## 受众由哪些部分组成 {#match-keys}

RTCDP Collaboration中的受众由匹配键组成。 根据您的帐户配置，支持的匹配密钥可以包括&#x200B;**人员ID**、**设备ID**&#x200B;和&#x200B;**合作伙伴ID**。 匹配键支持诸如&#x200B;**受众重叠**、**激活**&#x200B;和&#x200B;**测量**&#x200B;的工作流。

若要了解详细信息，请参阅[设置匹配键](../setup/onboard-account.md#set-up-match-keys)和[管理数据连接](../setup/manage-data-connection.md#match-keys)

## 在项目中使用受众 {#audiences-in-projects}

项目提供了与其他组织协作的上下文。 在项目中，您可以将受众用于支持的协作用例：

* **发现**：比较受众并查看重叠见解。 查看[发现受众重叠](../collaborate/discover.md)。
* **激活**：激活选定受众以供营销活动使用。 激活是从项目工作区中的[!UICONTROL 激活]选项卡启动的，并将受众发送到连接的配置目标。 请参阅[激活受众](../collaborate/activate.md)。
* **度量**：查看与项目关联的活动投放和转化报告。 查看[度量绩效](../collaborate/measure.md)。

有关创建和管理项目的详细信息，请参阅[创建和管理项目](../collaborate/manage-projects.md)。 有关配置目标的信息，请参阅[目标概述](../destinations/overview.md)。

## 后续步骤 {#next-steps}

* [查看可用的受众源](./source-overview.md)
* [Source和管理受众](./onboard-audiences.md)
* [创建和管理项目](../collaborate/manage-projects.md)
* [发现受众重叠](../collaborate/discover.md)
* [激活受众](../collaborate/activate.md)
* [衡量绩效](../collaborate/measure.md)
* [目标概述](../destinations/overview.md)
