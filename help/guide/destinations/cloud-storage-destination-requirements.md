---
title: 目标连接要求
description: 查看在Real-Time CDP Collaboration中配置受支持的目标所需的连接信息。
audience: admin, publisher
source-git-commit: c84582bb81289ce761c664af7db177535ff00a00
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 1%

---

# 目标连接要求

在Real-Time CDP Collaboration中配置目标之前，请获取目标提供商所需的凭据和连接信息。

此页总结了Collaboration中可用的身份验证方法。 有关创建凭据、分配权限、配置网络访问或准备目标系统的说明，请参阅链接的Adobe Experience Platform目标文档。

>[!NOTE]
>
>链接的Adobe Experience Platform文档描述了标准目标工作流。 在Real-Time CDP Collaboration中配置目标时，某些步骤、字段或选项可能不适用。

## 需求概览 {#requirements-at-a-glance}

| 目标 | 身份验证或连接方法 | 开始前准备 | 详细要求 |
|---|---|---|---|
| [!DNL Amazon S3] | 访问密钥和密钥，或承担的角色 | AWS访问密钥对或IAM角色ARN；存储段和文件夹信息 | [[!DNL Amazon S3] 目标文档](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/destinations/catalog/cloud-storage/amazon-s3) |
| SFTP | 密码或SSH密钥 | 服务器域、端口、用户名、身份验证凭据和文件夹路径 | [SFTP目标文档](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/destinations/catalog/cloud-storage/sftp) |
| [!DNL Azure Blob Storage] | 连接字符串 | Azure存储连接字符串、容器和文件夹信息 | [[!DNL Azure Blob Storage] 目标文档](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/destinations/catalog/cloud-storage/azure-blob) |
| [!DNL Google Cloud Storage] | 访问密钥ID和访问密钥 | [!DNL Google Cloud Storage]互操作性凭据、存储段和文件夹信息 | [[!DNL Google Cloud Storage] 目标文档](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/destinations/catalog/cloud-storage/google-cloud-storage) |
| [!DNL Snowflake Batch] | [!DNL Snowflake]数据共享 | [!DNL Snowflake]帐户ID、地区、专用链接状态以及对专用列表的访问权限 | [[!DNL Snowflake Batch] 目标文档](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/destinations/catalog/warehouse/snowflake-batch) |
| [!DNL Data Landing Zone] | 无需单独的身份验证 | 目标文件夹路径和文件输出首选项 | [[!DNL Data Landing Zone] 目标文档](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/destinations/catalog/cloud-storage/data-landing-zone) |

## 连接器说明 {#connector-notes}

在配置目标之前，请查看以下特定于连接器的身份验证方法和工作流差异。

### [!DNL Amazon S3] {#amazon-s3}

Collaboration支持&#x200B;**[!UICONTROL 访问密钥]**&#x200B;和&#x200B;**[!UICONTROL 假定角色]**&#x200B;身份验证。 访问密钥身份验证需要访问密钥和访问密钥。 承担角色身份验证需要Adobe可以承担的AWS IAM角色的ARN。

有关凭据、角色和权限设置，请参阅[对 [!DNL Amazon S3] 目标进行身份验证](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/destinations/catalog/cloud-storage/amazon-s3#authenticate)。

### SFTP {#sftp}

Collaboration支持使用密码&#x200B;**的**&#x200B;[!UICONTROL &#x200B; SFTP和使用SSH密钥&#x200B;]&#x200B;**身份验证的** SFTP。 这两种方法都需要服务器域、端口和用户名。 端口默认为`22`。

有关SSH密钥格式、服务器、网络和的要求，请参阅[SFTP身份验证信息](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/destinations/catalog/cloud-storage/sftp#authentication-information)。

### [!DNL Azure Blob Storage] {#azure-blob-storage}

Collaboration使用storage-account连接字符串向[!DNL Azure Blob Storage]进行身份验证。

有关获取连接字符串和分配存储权限的说明，请参阅[向 [!DNL Azure Blob Storage] 目标](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/destinations/catalog/cloud-storage/azure-blob#authenticate)进行身份验证。

### [!DNL Google Cloud Storage] {#google-cloud-storage}

Collaboration需要通过[!DNL Google Cloud Storage]互操作性设置生成的[!DNL Google Cloud Storage]访问密钥ID和访问密钥。

有关凭据生成和分段权限要求，请参阅[向 [!DNL Google Cloud Storage] 目标](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/destinations/catalog/cloud-storage/google-cloud-storage#authenticate)进行身份验证。

### [!DNL Snowflake Batch] {#snowflake-batch}

[!DNL Snowflake Batch]使用[!DNL Snowflake]数据共享，而不是将文件导出到客户管理的存储。 在Collaboration中，没有单独的身份验证步骤。 在目标创建期间输入Snowflake帐户ID、区域、专用链接状态和帐户所有权确认。

有关帐户准备和私有列表的要求，请参阅[[!DNL Snowflake Batch] 目标文档](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/destinations/catalog/warehouse/snowflake-batch)。

### [!DNL Data Landing Zone] {#data-landing-zone}

[!DNL Data Landing Zone]由Adobe配置，不需要在Collaboration中执行单独的身份验证步骤。 在目标创建过程中，指定目标文件夹路径和文件输出设置。

有关访问AWS设置的[!DNL Data Landing Zone]的信息，请参阅[对AWS设置的数据登录区进行身份验证](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/destinations/catalog/cloud-storage/data-landing-zone#authenticate-dlz-aws)。

## 后续步骤 {#next-steps}

获取所需的连接信息后，[配置和管理目标](./manage-destinations.md)。
