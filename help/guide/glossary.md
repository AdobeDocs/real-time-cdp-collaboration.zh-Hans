---
title: 术语表
description: 了解Real-Time CDP Collaboration的关键术语
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 870c45d0-df68-487f-bbe2-d9862a8ea62e
source-git-commit: b929cf9d75b4fc844ba03799f07a5e372b8f9052
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 2%

---

# 术语表

{{limited-availability-release-note}}

此术语表提供在Adobe Real-Time CDP Collaboration产品和文档中识别的关键术语的定义。 了解这些术语将有助于您更好地利用产品及其功能。

## A

### 广告商

任何将花费营销预算来覆盖出版商或其他品牌合作伙伴的受众以实现品牌意识、潜在客户、重新接触和转化目标的实体。

## C

### 云存储

云存储是一种云计算解决方案，可通过云计算提供商在互联网上存储数据和文件，并且几乎总是组织数据栈栈的一部分。 示例包括Amazon Web Services (AWS)、Microsoft Azure和Google Cloud Platform (GCP)。

### 连接请求

连接请求是从一个组织发送到另一个组织以建立数据共享连接的正式请求。 一旦被接受，它允许双方安全地协作和共享受众数据。

### 连接设置

接受连接请求后，该请求的发起方将连接设置发送给协作者进行审批。 这些连接设置控制协作者协同处理项目的方式，并包括使用的匹配密钥、账单所有权等。

<!--

### Crosswalk

An identity crosswalk is a tool used to connect different identifiers across datasets to enrich your audience data with additional attributes or dimensions. It creates a bridge between different data points, allowing for a more comprehensive and cohesive view of the data.

-->

## D

### 数据清理室

一个安全的协作环境，允许两个或更多参与者利用数据资产进行特定的、相互同意的用途，同时保证严格的数据访问限制的实施。 此基础架构层通常由云存储提供商和/或数据仓库(如Snowflake和数据库)提供，最适合技术用户（如数据工程师和精通SQL等技能的数据科学家）。

### 数据协作

数据协作涉及出于各种目的（如受众定位、测量和见解）组合和分析公司内或合作伙伴的数据。 数据协作平台提供了安全的环境，可在满足隐私和安全问题的同时安全地共享数据。

### 数据连接

数据连接是将数据导入Real-Time CDP Collaboration的来源。 目前，Experience Platform是唯一可用的数据连接。 阅读有关[管理数据连接](/help/guide/setup/manage-data-connection.md)的更多信息。

### 数据共享协议

数据共享协议是两个或更多方之间的正式合同，概述了共享数据的条款和条件。 它确保各方遵守法律和隐私要求，并制定了数据使用和保护准则。

### 设备标识符

设备标识符是与设备（如智能手机或平板电脑）相关联的唯一编号。 它用于在各种平台和服务中跟踪和识别设备，从而实现个性化用户体验和定向广告。

## I

### 邀请

Adobe Real-Time CDP Collaboration中的邀请是指发送给其他用户或组织以加入项目或数据协作工作的请求。 邀请有助于促进对共享数据和资源的安全且受控的访问。

<!--

## J

### Join key

In the context of identity crosswalks, a join key is a unique identifier used to match and link different identifiers across datasets, enabling the integration and unification of audience data from various sources. For example, a hashed email (HEM) can be a join key.

-->

## M

### 匹配键

匹配键是用于链接不同数据集上的记录的唯一标识符。 它们有助于确保来自不同来源的数据能够准确匹配和集成，从而促进更好的数据分析和受众分段。

## O

### 重叠

重叠（或受众重叠）是指存在于不同数据集之间的公共受众片段。 了解受众重叠有助于发现潜在的协作机会，并允许通过利用共享受众数据开展更具针对性的营销工作。

## P

### 项目

Adobe Real-Time CDP Collaboration中的项目是一个工作区，用户可以在该工作区中协作完成特定数据集成和受众分段任务。 项目有助于组织和管理数据共享工作，使协作更加高效和简化。

### 公共受众

在项目上下文中，这是可由您的协作者发现的受众。 受众可以是私有、自定义或公共受众。 任何其他协作者均无法发现私人受众。 自定义受众只能由某些协作者发现，而公共受众则可由所有协作者发现。

### 发布者

出版商是在线内容或服务的拥有者或运营者，在同意情况下收集个人数据，并可由其他实体用于数字广告和受众测量。

## S

### 草图 {#sketches}

草图（或数据草图）是Real-Time CDP Collaboration中使用的受众数据的简化摘要。 它们允许品牌和出版商分析受众重叠和见解，而无需共享实际客户数据。 把它们想象成匿名员工人数，而不是详细的客户资料。
在Adobe Real-Time CDP Collaboration中，数据草图：

* 帮助确定两个受众的相似程度
* 在启用协作时维护隐私
* 需要至少每7天更新一次才能保持有效

如果草图未定期刷新，则观众重叠报告将显示零值，并且观众共享可能暂时不可用。 每当Real-Time CDP Collaboration中的受众成员资格更新时，数据草图都会自动刷新。

## U

### 用例

用例定义了可以使用Adobe Real-Time CDP Collaboration解决的特定业务场景或问题。 在Real-Time CDP Collaboration中，受众发现或营销活动测量等示例用例可用于帮助实现特定目标。
