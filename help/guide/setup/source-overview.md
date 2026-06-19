---
title: 源概述
description: 了解Adobe Real-Time CDP Collaboration中的源连接器
audience: admin, publisher, advertiser
source-git-commit: b30d1b01e929e586404faac34650c7fd479d071b
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 10%

---

# 源概述

在Adobe Real-Time CDP Collaboration中，源（或数据连接）是受众数据的来源。 您可以从本地系统连接到各种源类型，如Adobe应用程序、基于云的存储或文件，以便[为Collaboration项目提供和管理受众](./onboard-audiences.md)。 在受众源工作流程中，您可以根据组织的需求选择和设置首选来源。

## 连接源 {#connect-a-source}

要连接来源，您需要输入来源补充工作流。 首先，导航到&#x200B;**[!UICONTROL 设置]**&#x200B;工作区中的&#x200B;**[!UICONTROL 我的受众]**&#x200B;选项卡。

选择添加图标（![添加图标。](/help/assets/icons/plus.png)） 然后选择&#x200B;**[!UICONTROL 受众]**&#x200B;以启动源工作流。

![突出显示了“添加”选项和“受众”选项的“我的受众”工作区。](/help/assets/setup/add-manage-audiences/add-audiences.png)

在工作流程期间，系统将提示您通过选择源来添加新数据连接。 您选择的源将决定如何将受众数据引入Collaboration。 有关所有受支持源的列表，请参阅[可用源](#available-sources)表。

![突出显示了“添加新数据连接”选项的“添加受众”工作区。](/help/assets/setup/add-manage-audiences/add-data-connection.png)

选择源后，工作流将指导您完成特定于连接的设置步骤，包括身份验证、字段映射、计划和受众选择。

### 可用源 {#available-sources}

Collaboration中有以下源。 要查看该来源的分步采购指南，请选择下表中的来源名称。 如果您对某个当前不可用的源感兴趣，请联系您的Adobe代表。

| 来源 | 描述 | 可用性 |
| --- | --- | --- |
| [Adobe Experience Platform](./onboard-audiences.md) | 从连接的Experience Platform实例引入受众并重用现有的客户区段。 | 可用 |
| [Amazon S3](./configure-aws-s3-audience-sourcing.md) | 连接您的S3存储桶以从云基础架构中获取大型第一方数据集。 | 可用 |
| [[!DNL Snowflake]](./configure-snowflake-audience-sourcing.md) | 连接您的[!DNL Snowflake Secure Data Share]以引入大规模受众数据集。 | 可用 |
| [[!DNL Google Cloud Storage]](./configure-gcs-audience-sourcing.md) | 连接您的GCS存储桶以引入存储在您的[!DNL Google Cloud]环境中的受众数据。 | 可用 |
| [CSV文件上传](./upload-csv-audience-sourcing.md) | 直接从本地系统上传格式化的CSV文件。 | 可用 |
| Adobe Audience Manager | 将现有Audience Manager区段引入您的Collaboration项目。 | *即将推出* |
| [[!DNL Azure Blob Storage]](./configure-azure-storage-audience-sourcing.md) | 将您的[!DNL Azure Blob Storage]容器连接到[!DNL Microsoft Azure]环境中的源第一方数据集。 | 可用 |
| [[!DNL Azure Data Lake Storage]](./configure-azure-storage-audience-sourcing.md) | 连接您的[!DNL Azure Data Lake Storage Gen 2]帐户以引入存储在[!DNL Azure]数据湖中的受众数据。 | 可用 |

{style="table-layout:auto"}

## 后续步骤

连接源并引入受众后，您可以查看详细信息、更新配置或删除现有源。 有关详细信息，请参阅[管理数据连接](./manage-data-connection.md)指南。
