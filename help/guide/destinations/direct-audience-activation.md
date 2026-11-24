---
title: 直接激活受众(1P Audience Activation) - Beta
description: 了解如何在没有项目的情况下激活您自己的或共享的第一方受众、选择目标、查看字段映射并设置激活计划。
badgeBeta: label="Beta" type="Informative"
source-git-commit: 5f823194a18468b9205f64853551719ae8a3752f
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 1%
---

# 直接激活受众(1P Audience Activation) {#activate-audiences-directly}

在[!DNL Adobe Real-Time CDP Collaboration]中使用直接第一方(1P)受众激活将受众发送到目标而不创建项目。 激活您拥有的受众或与您共享的受众以供第一方使用。

从配置的目标或&#x200B;**[!UICONTROL 激活的受众]**&#x200B;开始，然后选择受众并设置激活计划。

若要通过协作项目发送和激活受众，请参阅[发送和激活项目中的受众](/help/guide/collaborate/activate.md)。

## 受众访问权限以进行激活 {#audience-access-for-activation}

检查受众源，确定激活之前是否需要授权。

| 受众来源 | 访问要求 |
| --- | --- |
| 您自己的受众 | 您拥有受众。 |
| 与您共享的受众 | 您需要具有直接激活权限的活动授权。 提供商保留所有权。 |

{style="table-layout:auto"}

通过虚拟受众授权，无需移动共享受众的数据即可引用该受众。 然后，您可以激活受众以将其数据发送到您选择的目标。

有关授权和提供程序控制的详细信息，请参阅[虚拟受众访问（受众授权）](/help/guide/setup/virtual-audience-access.md)。

## 先决条件 {#prerequisites}

在开始之前，请确认您拥有：

* 您拥有的受众或通过合格的第一方(1P)授权共享的受众。
* 由您控制并支持直接激活的配置目标。
* 目标至少有一个匹配键字段映射。

要激活共享受众，请确认其活动的连接范围授予符合[资格条件](#check-shared-audience-access)。 使用&#x200B;**[!UICONTROL 激活]**&#x200B;工作区。 您不需要项目。

### 共享受众资格 {#check-shared-audience-access}

授权必须符合每个条件才能支持直接激活。

| 要求 | 条件 |
| --- | --- |
| 受众权限 | 该授权包括直接激活权限。 |
| 访问持续时间 | 该授权可无限期或于指定日期范围内有效。 |

{style="table-layout:auto"}

单独的&#x200B;**[!UICONTROL 构建新受众]**&#x200B;权限允许您使用共享受众来创建同类群组受众。 您不需要此权限即可直接激活。

### 目标字段映射 {#review-destination-field-mappings}

直接激活使用为您的目标配置的匹配键映射。 激活期间不选择匹配的密钥。

要配置目标，请参阅[目标概述](../destinations/overview.md)。

## 开始直接激活 {#start-direct-activation}

从配置的目标或激活的受众列表开始。 Adobe Experience Platform目标不支持第一方激活。

### 从目标开始 {#start-from-a-destination}

要打开具有选定目标的工作流，请从配置的目标开始。 首先，打开&#x200B;**[!UICONTROL 激活]**&#x200B;工作区，然后选择&#x200B;**[!UICONTROL 目标]**。

接下来，从要使用的目标的操作中选择&#x200B;**[!UICONTROL 激活受众]**。

此时将打开工作流，并选中目标。 然后，继续[配置激活](#configure-the-activation)。

### 从激活的受众开始 {#start-from-activated-audiences}

要在工作流中选择目标，请从激活的受众列表开始。 首先，打开&#x200B;**[!UICONTROL 激活]**&#x200B;工作区，然后选择&#x200B;**[!UICONTROL 激活的受众]**。

接下来，通过选择页面上的&#x200B;**[!UICONTROL 激活受众]**&#x200B;或选择“添加”图标（![添加受众激活。](/help/assets/icons/plus.png)）来启动工作流 然后&#x200B;**[!UICONTROL 激活受众]**。

此时会打开工作流，但不会选择目标。 然后，继续[配置激活](#configure-the-activation)。

## 配置激活 {#configure-the-activation}

来自您自己的受众或与您共享的受众的Select每个激活对应一个受众。 使用预选的目标，或者如果未选择任何目标，则选择已配置的目标。 工作流应用为该目标配置的[现有映射](#review-destination-field-mappings)。

选择运行激活的时间，然后在提交之前查看选定的受众、目标和计划。

## 访问更改和计划的运行 {#access-changes-and-scheduled-runs}

仅在提供商授予访问权限时激活共享受众。

| 访问更改 | 效果 |
| --- | --- |
| 授予过期 | 系统每小时处理过期时间。 收件人在处理过期后会失去虚拟受众访问权限。 |
| 提供程序撤销授权 | 收件人会立即失去虚拟受众访问权限。 |
| 计划的激活运行 | 系统会检查授权。 授权已撤销或已过期的受众不符合激活条件。 |

{style="table-layout:auto"}

过期或吊销不会删除已交付到目标的受众数据。

## 后续步骤 {#next-steps}

激活受众后，请使用这些指南管理目标或协作者连接。

* [配置和管理目标](/help/guide/destinations/manage-destinations.md)
* [管理协作者连接](/help/guide/connect/manage-connections.md)
