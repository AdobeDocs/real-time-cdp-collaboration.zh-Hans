---
title: 为受众源配置AWS权限
description: 了解如何配置AWS Identity and Access Management (IAM)权限，以授予Adobe对Real-Time CDP Collaboration中受众源的 [!DNL Amazon S3] 存储段的安全只读访问权限。
source-git-commit: 4f223890dabb4897c9e9264655ff9217e323dc91
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 0%

---

# 为受众源配置AWS权限

使用本指南配置AWS Identity and Access Management (IAM)策略和角色，这些策略和角色可授予Adobe对Amazon S3存储段的安全只读访问权限。 凭借此访问权限，Real-Time CDP Collaboration可从S3存储段获取受众。

## 先决条件 {#prerequisites}

在继续之前，请确认您满足以下要求并有权访问所需信息。

### 所需的AWS权限

要完成此设置，您的帐户必须具有AWS管理员访问权限。 管理员访问权限确保您可以创建和管理授权Adobe访问S3存储段所需的IAM策略和角色。 如果您没有管理员权限，请在继续操作之前联系AWS管理员。

### 所需信息

在执行以下步骤时，请注意以下信息。 这些详细信息在[[!DNL Amazon S3] 受众源UI指南](./configure-aws-s3-audience-sourcing.md)中使用。

* 存储受众文件的S3存储段名称。
* 受众文件所在的文件夹路径（前缀）。
* 新创建的IAM角色的Amazon资源名称(ARN)，例如： `arn:aws:s3:::my-company-data/audience-files/`

>[!TIP]
>
>Amazon资源名称(ARN)唯一标识AWS资源，如S3存储桶和IAM角色。 使用以下格式指定存储段和可选文件夹路径：
>
>```
>arn:aws:s3:::<bucket-name>/<optional-folder-path>
>```

## 创建IAM策略 {#create-policy}

要开始设置，请首先创建一个IAM策略，该策略将您的S3存储段授予&#x200B;**只读访问权限**。 此策略允许Adobe读取受众获取所需的文件，但不授予写入或删除权限。

打开[AWS管理控制台](https://aws.amazon.com/console/)，然后导航到&#x200B;**[!DNL IAM]** > **[!DNL Policies]** > **[!DNL Create policy]**。

在AWS创建策略工作区中，选择&#x200B;**JSON**&#x200B;选项卡并粘贴以下示例策略。

>[!NOTE]
>
>将`<Your AWS ARN for bucket folder path>`和`<Your AWS ARN for bucket>`替换为您的特定S3 ARN。 指定存储段文件夹路径时，在ARN末尾包含`/*`（例如，`arn:aws:s3:::my-company-data/audience-files/*`）。 这可确保Adobe有权访问指定文件夹路径中的所有文件和子文件夹。

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "Statement1",
      "Effect": "Allow",
      "Action": [
        "s3:GetObject",
        "s3:ListBucket",
        "s3:GetBucketLocation"
      ],
      "Resource": "<Your AWS ARN for bucket folder path>"
    },
    {
      "Sid": "Statement2",
      "Effect": "Allow",
      "Action": [
        "s3:ListBucket"
      ],
      "Resource": "<Your AWS ARN for bucket>"
    }
  ]
}
```

查看策略设置并选择&#x200B;**[!DNL Create policy]**。 记录策略名称以供在后续步骤中使用。

>[!TIP]
>
>要查找存储段名称和文件夹路径，请打开&#x200B;**Amazon S3管理控制台**。 在&#x200B;**存储桶**&#x200B;页面上，选择存储桶名称以将其打开。 **对象**&#x200B;视图列出了您的文件和文件夹，页面顶部的路径显示了您当前的文件夹路径。

## 创建IAM角色 {#create-role}

接下来，创建一个IAM角色，并将Real-Time CDP Collaboration AWS IAM角色设置为&#x200B;**受信任的实体**。 这使得Adobe的服务可以承担此角色，并安全地读取您的S3受众数据。

在Amazon S3管理控制台的&#x200B;**[!DNL IAM]**&#x200B;选项卡中，导航到&#x200B;**[!DNL Roles]** > **[!DNL Create role]**。

在[!DNL Step 1]工作流的[!DNL Create role]下，在&#x200B;**[!DNL Trusted entity type]**&#x200B;部分中选择&#x200B;**[!DNL Custom trust policy]**。 然后，在&#x200B;**[!DNL Custom trust policy]**&#x200B;编辑器中，粘贴以下示例并将`<Adobe IAM Role ARN>`替换为您所在地区的值。

* 适用于您所在地区的Adobe IAM角色ARN：

| 区域 | Adobe IAM角色ARN |
|---------|-------------------|
| 北美洲 | `arn:aws:iam::590183896800:role/rtcdp-collab-prod-va6-role` |
| 澳大利亚 | `arn:aws:iam::590183896800:role/rtcdp-collab-prod-aus3-role` |

信任策略示例：

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "Statement1",
      "Effect": "Allow",
      "Principal": {
        "AWS": "<Adobe IAM Role ARN>"
      },
      "Action": "sts:AssumeRole"
    }
  ]
}
```

查看策略并选择&#x200B;**下一步**&#x200B;以继续。

在[!DNL Step 2]工作流的&#x200B;**[!DNL Add permissions]** [!DNL Create role]部分中，搜索并附加您以前创建的[IAM策略](#create-policy)。 选择策略，然后选择&#x200B;**[!DNL Next]**&#x200B;以继续到[!DNL Step 3]。

在[!DNL Step 3] **[!DNL Name review, and create - Role details]**&#x200B;部分中，提供角色名称（例如，`s3-iam-role`）和可选描述。

此页显示受信任的实体策略、权限策略摘要以及您可能为内部组织和跟踪添加的任何标记。

最后，选择&#x200B;**创建角色**&#x200B;以确认设置。

>[!IMPORTANT]
>
>在创建角色后，必须记录Amazon资源名称(ARN)。 在&#x200B;**为受众源配置AWS S3**&#x200B;工作流的[对S3连接进行身份验证](./configure-aws-s3-audience-sourcing.md)步骤中，您需要提供IAM角色ARN。

## 后续步骤 {#next-steps}

此设置会授予Adobe对S3存储段的只读访问权限，并会与Adobe的IAM角色建立可信连接。

接下来，请继续[为受众源配置AWS S3](./configure-aws-s3-audience-sourcing.md)，以将您的S3存储段连接到Collaboration。

有关来源受众的详细信息，请参阅[Source和管理受众](./onboard-audiences.md)。
