---
title: 共享受众
description: 了解如何与您的协作者共享受众以用于广告营销活动。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 0fdf0598-89c9-452d-a2e3-ce868df0b9d2
source-git-commit: acaaaa1e1fab981d874210639c16e76e48fc3394
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 1%

---

# 共享受众

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>**[!UICONTROL 共享]**&#x200B;工作区仅在连接过程](../connect/establishing-connections.md#connection-settings)中启用了[的&#x200B;**受众共享和激活**&#x200B;用例时才可用。 有关用例的更多信息，请参阅[管理项目](./manage-projects.md#project-use-cases)指南。

作为广告商，了解如何与您的出版商共享受众，以便他们能够开展营销活动。 如果您的协作已启用&#x200B;**发现受众**&#x200B;用例，请首先在[发现选项卡](/help/guide/collaborate/discover.md)中运行重叠报表，以确定要共享的最佳受众。

## 共享新受众

要开始共享受众，请导航到项目工作区中的&#x200B;**[!UICONTROL 共享]**&#x200B;选项卡。 只有&#x200B;**广告商组织**&#x200B;可以共享营销活动的受众。 在此选项卡中，您可以查看和管理共享受众。

选择&#x200B;**加号(+)**&#x200B;或&#x200B;**[!UICONTROL 共享受众]**&#x200B;选项（如果未共享任何以前的受众）以开始受众共享流程。

![默认视图，没有共享的受众。](/help/assets/collaborate/share/share-new-audiences.png)

此时将显示一个新面板，您可以在其中选择要与协作者共享的受众。

![共享新的受众工作流。](/help/assets/collaborate/share/share-audiences-workflow.png)

### 选择要共享的受众

在受众选择窗口中，通过在搜索栏中输入受众名称来搜索要共享的特定受众。 选择&#x200B;**[!UICONTROL 浏览受众]**&#x200B;并使用可用的排序选项查找所需的确切受众。

![浏览选定受众的受众视图。](/help/assets/collaborate/share/browse-audiences-view.png)

### 编辑匹配键并设置定位选项

选择要共享的所需受众后，您现在可以为共享活动选择其他配置选项。

![编辑匹配键并突出显示目标或禁止选择器](/help/assets/collaborate/share/match-keys-and-targeting.png)

选择&#x200B;**[!UICONTROL 编辑匹配键]**&#x200B;以指示应该为受众中的身份使用的匹配键。 这些选项继承自最初设置协作者之间连接时选择的设置。 如果当时选择的匹配键不适用于此特定营销活动，则可以将其删除，但此时无法添加新的匹配键。

![编辑匹配键。](/help/assets/collaborate/share/update-match-keys.png)

对于每个受众，选择要在营销活动中定位还是禁止显示该受众的成员。 禁止显示的配置文件将不会明确属于发布者激活的受众。

### 设置受众刷新频率和间隔

最后，设置受众刷新的所需频率和日期范围。 当前支持的受众刷新模式为&#x200B;**[!UICONTROL 一次]**&#x200B;和&#x200B;**[!UICONTROL 每日]**。

选择&#x200B;**[!UICONTROL 一次]**&#x200B;时，在整个营销活动期间不会刷新受众成员资格。 选择&#x200B;**[!UICONTROL 每日]**&#x200B;时，在营销活动期间，受众成员资格每天刷新一次。

![频率选项突出显示。](/help/assets/collaborate/share/audience-refresh-frequency.png)

如果对您的选择满意，请选择&#x200B;**[!UICONTROL 共享]**&#x200B;以完成工作流。

>[!SUCCESS]
>
>您现在可以在&#x200B;**[!UICONTROL 共享]**&#x200B;选项卡中看到新的受众共享活动。 如果需要，您可以返回并编辑您所做的任何选择。

## 查看当前共享的受众

在&#x200B;**[!UICONTROL 共享]**&#x200B;选项卡中，可以查看协作者之间当前共享的受众（在受众共享活动中分组）。

![共享选项卡概述。](/help/assets/collaborate/share/share-tab-overview.png)

<!--

The banner at the top of the page shows figures across all audience sharing activities. 

![The hero banner in the sharing tab.](/help/assets/collaborate/share/share-hero-banner.png)


|Metric | Description |
|---------|----------|
| **[!UICONTROL Shared audiences]** | Indicates the number of audiences shared between collaborators in this project, across all audience sharing modules. |
| **[!UICONTROL Estimated addressable reach]** | Indicates the approximate number of profiles that you can reach across all the audiences that are currently shared in the project. [TODO: ADD INFORMATION ABOUT HOW THIS IS CALCULATED] |
| **[!UICONTROL Target identities]** | The number of identities across all audiences shared in this project for which you selected to target the profiles. |
| **[!UICONTROL Suppress identities]** | The number of identities across all audiences shared in this project for which you selected to suppress the profiles and thereby not target them in campaigns. |

-->

在每个受众共享活动中，您可以获取有关每个共享受众的信息。

| 量度 | 描述 |
|---------|----------|
| **[!UICONTROL 身份计数]** | 指示根据最新的身份计数评估，与此受众关联的所有身份中的配置文件数。 这些数字每24小时刷新一次。 |
| **[!UICONTROL 身份重叠]** | 指示此受众成员之间的重叠身份数以及协作者库存中的配置文件总人口。 |
| **[!UICONTROL 匹配键划分]** | 显示受众中使用的每个标识的标识计数。 例如，总身份数为50万的用户可能包括40万用户中断了经过哈希处理的电子邮件身份的连接，以及10万用户中断了移动ID身份的连接。 请注意，在此处描述的示例中，受众中可能有同一用户使用其电子邮件和移动ID身份两次。 |
| **[!UICONTROL 目标]** | **[!UICONTROL 禁止]**&#x200B;或&#x200B;**[!UICONTROL 目标]**。 指示是应定位受众成员还是应将其从营销活动中排除。 |

该页面还提供了用于&#x200B;**[!UICONTROL 暂停共享]**&#x200B;和&#x200B;**[!UICONTROL 编辑受众]**&#x200B;的控件。

## 编辑受众 {#edit-audiences}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_share_edit_audiences_usecases"
>title="定位或禁止显示用例"
>abstract="<p>如果希望受众中的用户档案在营销活动中显示广告，请选择&#x200B;**Target**。</p> <p>如果要将受众中的用户档案从营销活动消息中排除，请选择&#x200B;**禁止**。</p>"

选择&#x200B;**[!UICONTROL 编辑受众]**&#x200B;以更改在受众共享模块中共享的受众，以及更改与受众共享方式相关的多个配置。

![编辑受众模式视图](/help/assets/collaborate/share/edit-audiences-modal.png)

<!--

Search for audiences that you want to add to the sharing module. 

For each audience, you can select whether you'd like to target or suppress those profiles in campaigns. 

To remove an audience from the sharing module, select the trash can icon [TODO: add spectrum icon and folder].

Select how often you would like the audience membership to be refreshed and the date range within which you want the membership of the audience to be refreshed. 

TODO: are there any limitations for frequency in the M1 release?

-->

## 后续步骤

在发布者收到共享受众后，他们现在将在数字广告营销活动中[激活](/help/guide/collaborate/activate.md)这些受众。
