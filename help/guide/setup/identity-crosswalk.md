---
title: 身份标识对照表
description: 全面了解Real-Time CDP Collaboration中的身份交叉通道，包括如何从不同来源引入身份交叉通道，以及如何管理身份交叉通道
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
hidefromtoc: true
hide: true
exl-id: a51f112d-3da7-4482-a24a-6d9f269d28d1
source-git-commit: 23dc33af83366806f7d99161b4b713a33daeec76
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 22%

---

# 身份标识对照表

{{limited-availability-release-note}}

全面了解Real-Time CDP Collaboration中的身份交叉通道，包括如何从不同来源引入身份交叉通道，以及如何管理身份交叉通道。

身份交叉通道有助于跨多个数据集和平台安全且符合隐私要求的客户身份关联。 通过使用哈希标识符，Real-Time CDP Collaboration可确保用户能够同步和协调身份，而无需公开个人身份信息(PII)。 这样可以统一了解客户，以便更好地协作和有针对性的营销工作。

<!--
In Real-Time CDP Collaboration, use identity crosswalks alongside your audiences by [TODO] insert material here. 
-->


第一步，必须将标识交叉通道导入Real-Time CDP Collaboration。 要将身份交叉通道导入Real-Time CDP Collaboration，请阅读以下部分：

>[!NOTE]
>
>在Real-Time CDP Collaboration的测试版中，您可以从Real-Time CDP中的数据集导入身份交叉通道。 后续版本中将提供其他选项。

## 将身份交叉通道导入Real-Time CDP Collaboration {#import-crosswalk}

导航到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 标识交叉通道]**&#x200B;选项卡，选择加号&#x200B;**+**&#x200B;符号，然后选择&#x200B;**[!UICONTROL 标识交叉通道]**

![如何进入屏幕添加身份交叉路线的录制](/help/assets/setup/identity-crosswalks/import-identity-crosswalk.gif)

### 选择对照表来源

选择要从中导入标识交叉路径的源。 在Real-Time CDP Collaboration的第一个版本中，Experience Platform是唯一受支持导入人行横幅的源。

>[!TIP]
>
>从Experience Platform导入的交叉表在Platform中称为&#x200B;*数据集*。

选择Experience Platform作为交叉路线的源后，选择要从中导入身份交叉路线的[Experience Platform沙盒](https://experienceleague.adobe.com/zh-hans/docs/experience-platform/sandbox/home)。

![有关如何选择交叉通路源的录制](/help/assets/setup/identity-crosswalks/select-crosswalk-source.gif)

### 选择对照表

选择Experience Platform作为交叉路线的来源后，

### 提供详细信息

为要导入到产品中的标识交叉通路提供名称和描述。

### 选择连接键 {#select-join-key}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_crosswalk_join_key"
>title="连接键"
>abstract="连接键是用于匹配和链接不同数据集之间的记录的唯一标识符。它确保来自各种来源的数据能够准确地与同一个人或实体相关联。所选交叉表中的任何列标题都可以作为连接键。"

连接键是用于匹配和链接不同数据集之间的记录的唯一标识符。它确保来自各种来源的数据能够准确地与同一个人或实体相关联。通过选择适当的连接键，您可以有效地合并和协调数据，从而提高营销策划的准确性和完整性。

所选交叉表中的任何列标题都可以作为连接键。

为交叉表选择所需的联接键并选择&#x200B;**[!UICONTROL 下一步]**&#x200B;以继续执行下一步。

### 审查

查看前面的屏幕中的任何选择。 对您的选择感到满意后，选择&#x200B;**[!UICONTROL 下一步]**&#x200B;以完成工作流。

## 后续步骤

了解如何将身份交叉路口导入Real-Time CDP后，您可以查看迄今为止添加到Real-Time CDP Collaboration的所有身份交叉路口。 现在，您还可以使用将受众导入Real-Time CDP Collaboration时导入的身份交叉表。
