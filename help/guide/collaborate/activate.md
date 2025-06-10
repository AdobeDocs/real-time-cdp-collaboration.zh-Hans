---
title: 激活受众
description: 了解如何在Adobe Real-Time CDP Collaboration中激活受众。
audience: admin, publisher
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: fd82fcbf-ab39-48e0-9438-0a9046693431
source-git-commit: 691161cdc1f9338a470373988fbc0dee9a5be6db
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 1%

---

# 激活受众

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>**[!UICONTROL 激活]**&#x200B;工作区仅在连接进程[&#128279;](../connect/establishing-connections.md#connection-settings)期间启用&#x200B;**受众激活**&#x200B;用例时才可用。 有关用例的更多信息，请参阅[管理项目](./manage-projects.md#project-use-cases)指南。

Audience Activation允许您在营销活动中激活受众。 活动流程是广告商和发布商之间的协作。 在[发现营销活动的最佳受众](./discover.md)之后，受众可以激活目标受众。 激活的受众会发送到发布者预配置的目标，例如Adobe Experience Platform，以用于营销活动。 有关设置目标的详细信息，请参阅[目标概述](../destinations/overview.md)指南。

>[!IMPORTANT]
>
>目前，当广告商激活受众时，他们随后会自动激活到发布者为其组织配置的目标。 发布者&#x200B;**必须**&#x200B;在&#x200B;*之前配置目标*&#x200B;广告商激活受众。 如果未配置目标，则会将受众发送到发布者，但无法在任何营销活动中激活受众。

## 激活新受众

要开始激活受众，请导航到项目工作区中的&#x200B;**[!UICONTROL 激活]**&#x200B;选项卡。

选择添加图标（![添加图标）。](/help/assets/icons/plus.png))或&#x200B;**[!UICONTROL 激活受众]**&#x200B;选项（如果未发送以前的受众进行激活）。

![未添加受众的项目中的激活工作区。](/help/assets/collaborate/activate/activate-new-audiences.png)

激活受众工作流将打开，您可以在其中选择要发送给协作者受众。 使用下拉菜单选择受众，或搜索特定受众。 要在进行选择之前查看有关受众的详细信息，请选择&#x200B;**[!UICONTROL 浏览受众]**

![突出显示了下拉列表和浏览受众选项的Audience激活工作流。](/help/assets/collaborate/activate/audience-activation.png)

在&#x200B;**[!UICONTROL 浏览受众]**&#x200B;中，您可以看到每个受众的&#x200B;**[!UICONTROL 身份计数]**、**[!UICONTROL 重叠身份]**&#x200B;和&#x200B;**[!UICONTROL 重叠%]**。

![显示可用受众的“浏览受众”对话框。](/help/assets/collaborate/activate/browse-audiences.png)

选择要在营销活动中激活的受众，然后选择&#x200B;**[!UICONTROL 保存]**。 该受众现在显示出来，您可以看到所选受众的&#x200B;**[!UICONTROL 身份计数]**、**[!UICONTROL 重叠身份]**&#x200B;和&#x200B;**[!UICONTROL 重叠%]**。

![显示具有选定受众的受众激活工作流。](/help/assets/collaborate/activate/audience-selected.png)

### 编辑匹配键

接下来，您可以通过选择受众中的&#x200B;**[!UICONTROL 编辑匹配键]**&#x200B;来编辑受众的匹配键。 最初设置协作者之间的连接时，这些选项继承自匹配的键选择。 如果所选匹配键不适用于特定营销活动，则可以将其删除，但无法添加新的匹配键。

![突出显示了“编辑匹配键”选项的Audience激活工作流。](/help/assets/collaborate/activate/edit-match-keys.png)

**[!UICONTROL 编辑匹配键]**&#x200B;对话框打开，您可以在其中关闭不想使用的匹配键。 选择&#x200B;**[!UICONTROL 保存]**&#x200B;以保存更改。

>[!NOTE]
>
>必须至少选择一个匹配键。 在当前版本中，唯一可用的匹配密钥是&#x200B;**[!UICONTROL 哈希电子邮件]**，因此您不能删除此匹配密钥。

![受众激活工作流中的“编辑匹配密钥”对话框。](/help/assets/collaborate/activate/edit-match-keys-selection.png)

### 设置受众刷新频率和间隔

最后，设置受众刷新的所需频率和日期范围。 在当前版本中，唯一支持的频率选项是&#x200B;**[!UICONTROL 一次]**。 **[!UICONTROL 一次]**&#x200B;频率表示只激活一次受众，不刷新受众。 **[!UICONTROL Date]**&#x200B;选项自动填充了当前日期。

![已突出显示“频率”部分的Audience激活工作流。](/help/assets/collaborate/activate/audience-frequency.png)

如果对您的选择满意，请选择&#x200B;**[!UICONTROL 激活]**&#x200B;以完成工作流。 该受众现已激活，您可以在&#x200B;**[!UICONTROL 激活]**&#x200B;选项卡中查看它。 协作者还可以在&#x200B;**[!UICONTROL 激活]**&#x200B;选项卡中使用该功能，他们可以在营销活动中使用它。

您可以编辑受众的名称编辑图标（![铅笔图标）。](/help/assets/icons/edit.png))，或通过选择&#x200B;**[!UICONTROL 停用]**&#x200B;来停用受众。

![显示激活受众并突出显示“编辑”和“停用”选项的“激活”选项卡。](/help/assets/collaborate/activate/edit-activate-audience.png)

## 查看激活的受众

在&#x200B;**[!UICONTROL 激活]**&#x200B;选项卡中，发布者和广告商都可以查看当前激活的受众。 目前，受众会在广告商激活后自动发送到发布者配置的目标。

![“激活”选项卡概述，展示激活的受众。](/help/assets/collaborate/activate/activate-overview.png)

在每个激活的受众中，您可以看到以下量度：

| 量度 | 描述 |
|---------|----------|
| **[!UICONTROL 已激活的身份]** | 指示受众中激活的标识数。 |
| **[!UICONTROL 身份重叠]** | 指示此受众之间的重叠身份数以及协作者库存中的配置文件总人口。 |
| **[!UICONTROL 匹配键划分]** | 显示受众中使用的每个标识的标识计数。 例如，总身份数为50万的用户可能包括40万用户中断了经过哈希处理的电子邮件身份的连接，以及10万用户中断了移动ID身份的连接。 请注意，在此处描述的示例中，受众中可能有同一用户使用其电子邮件和移动ID身份两次。 |

## 后续步骤 {#next-steps}

在激活数据和运行营销活动后，与Adobe启用和工程团队合作，上传测量数据并查看相应的[测量报告](/help/guide/collaborate/measure.md)。
