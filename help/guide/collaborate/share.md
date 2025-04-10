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

要开始共享受众，请导航到项目工作区中的&#x200B;**[!UICONTROL 共享]**&#x200B;选项卡。 只有&#x200B;**广告商组织**&#x200B;可以共享营销活动的受众。 在此选项卡中，您可以查看和管理共享的受众群体。

**选择加号 （+）** 或 共享&#x200B;**[!UICONTROL 受众]** 选项（如果以前没有共享受众），开始受众共享流程。

![没有共享受众的默认视图。](/help/assets/collaborate/share/share-new-audiences.png)

此时会显示一个新面板，您可以在其中选择要与协作者共享的受众。

![共享新的受众工作流。](/help/assets/collaborate/share/share-audiences-workflow.png)

### 选择要共享的受众

在分享对象选择窗口中，您可以通过在搜索栏中输入分享对象名称来搜索要分享的特定分享对象。 选择浏览 **[!UICONTROL 受众]** ，然后使用可用的排序选项查找所需的确切受众。

![在选定访问群体的情况下浏览访问群体视图。](/help/assets/collaborate/share/browse-audiences-view.png)

### 修改匹配键并设置定位选项

选择要共享的所需受众后，您现在可以为共享活动选择其他配置选项。

![编辑匹配键并锁定或抑制突出显示的选择器](/help/assets/collaborate/share/match-keys-and-targeting.png)

选择&#x200B;**[!UICONTROL 编辑匹配键]**&#x200B;以指示应该为受众中的身份使用的匹配键。 这些选项继承自最初设置协作者之间连接时选择的设置。 如果当时选择的匹配键不适用于此特定营销活动，则可以将其删除，但此时无法添加新的匹配键。

![编辑匹配键。](/help/assets/collaborate/share/update-match-keys.png)

对于每个受众群体，选择您希望在广告系列中定位还是禁止显示该受众群体的成员。 被禁止显示的个人资料显然不会属于发布商激活的受众群体。

### 设置受众刷新频率和间隔

最后，设置受众刷新的所需频率和日期范围。 当前支持的受众刷新模式为&#x200B;**[!UICONTROL 一次]**&#x200B;和&#x200B;**[!UICONTROL 每日]**。

选择&#x200B;**[!UICONTROL 一次]**&#x200B;时，在整个营销活动期间不会刷新受众成员资格。 选择&#x200B;**[!UICONTROL 每日]**&#x200B;时，在营销活动期间，受众成员资格每天刷新一次。

![频率选项突出显示。](/help/assets/collaborate/share/audience-refresh-frequency.png)

如果对您的选择满意，请选择&#x200B;**[!UICONTROL 共享]**&#x200B;以完成工作流。

>[!SUCCESS]
>
>您现在可以在 **[!UICONTROL “共享]** ”选项卡中看到新的受众群体共享活动。 如果需要，您可以返回并编辑所做的任何选择。

## 查看当前共享的受众群体

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
| **[!UICONTROL 身份计数]** | 根据最新的身份计数评估，指示与此受众关联的所有身份中的配置文件数量。 这些数字每 24 小时刷新一次。 |
| **[!UICONTROL 身份重叠]** | 指示此受众成员之间的重叠身份数以及协作者库存中的配置文件总人口。 |
| **[!UICONTROL 匹配键划分]** | 显示受众中使用的每个标识的标识计数。 例如，总身份数为50万的用户可能包括40万用户中断了经过哈希处理的电子邮件身份的连接，以及10万用户中断了移动ID身份的连接。 请注意，在此处描述的示例中，受众中可能有同一用户使用其电子邮件和移动ID身份两次。 |
| **[!UICONTROL 目标]** | **[!UICONTROL “抑制]** ”或 **[!UICONTROL “目标]**”。 指示是应定位受众成员还是应将其从营销活动中排除。 |

该页面还提供了暂停分享和编辑受众&#x200B;]**群体的控件**[!UICONTROL 。****

## 编辑受众 {#edit-audiences}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_share_edit_audiences_usecases"
>title="定位或禁止显示用例"
>abstract="<p>如果希望受众中的用户档案在营销活动中显示广告，请选择&#x200B;**Target**。</p> <p>如果要将受众中的用户档案从营销活动消息中排除，请选择&#x200B;**禁止**。</p>"

选择 编辑访问群体&#x200B;]**以**[!UICONTROL &#x200B;更改在访问群体共享模块中共享的访问群体，以及更改与共享访问群体的方式相关的多个配置。

![编辑受众模式视图](/help/assets/collaborate/share/edit-audiences-modal.png)

<!--

Search for audiences that you want to add to the sharing module. 

For each audience, you can select whether you'd like to target or suppress those profiles in campaigns. 

To remove an audience from the sharing module, select the trash can icon [TODO: add spectrum icon and folder].

Select how often you would like the audience membership to be refreshed and the date range within which you want the membership of the audience to be refreshed. 

TODO: are there any limitations for frequency in the M1 release?

-->

## 后续步骤

发布商收到共享受众后，他们现在 [将在数字广告活动中激活](/help/guide/collaborate/activate.md) 它们。
