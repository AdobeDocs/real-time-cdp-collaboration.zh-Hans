---
title: 与广告商或发布者联系
description: 发现潜在的协作者后，了解如何建立连接并开始协作项目。
audience: admin, publisher, advertiser
badgelimitedavailability: label="有限发布版" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 3fed93f7-1854-440c-802e-6b47e82918c9
source-git-commit: 81cedb2a06d930734b1f97304de82d450c06bf79
workflow-type: tm+mt
source-wordcount: '918'
ht-degree: 1%

---

# 与广告商或发布者联系

{{limited-availability-release-note}}

在Real-Time CDP Collaboration中，将合作的两方（最常见的是广告商和发布商）关联到一起开展营销活动的公司是先决条件。 发布者和广告商都可以建立连接。 之后，发起连接的各方将成为&#x200B;*连接所有者*。

## 高级工作流

从较高层面来看，为了建立广告商和发布商之间的连接，工作流程如下所示：

1. 广告商[浏览并发现要与之合作的发布者](/help/guide/connect/discover-publishers.md)
2. 广告商发送连接邀请。
3. 发布者接受邀请。
4. 广告商发送连接设置，包括匹配键和其他设置。 这些连接设置表示协作的产品内术语。
5. 发布者接受连接设置。 如果需要，发布者可以拒绝初始连接设置，并请求广告商提交修订后的连接设置。

![广告商 — 发布商连接过程的高级图表。](/help/assets/connect/establish-connection/advertiser-publisher-connection-process.png){zoomable="yes"}

完成上述项目后，协作者可以继续[创建项目](/help/guide/collaborate/manage-projects.md#create-project)至[运行重叠报表](/help/guide/collaborate/discover.md)并启动广告营销活动。

>[!IMPORTANT]
>
>在建立两个协作者之间的连接后，便无法再修改连接设置。

## 发送邀请 {#send-invite}

要设置连接，请在发现发布者屏幕中浏览发布者清单时选择&#x200B;**[!UICONTROL 连接]**。

![连接选择器](/help/assets/connect/establish-connection/connect-selection.png){zoomable="yes"}

此时，邀请已发出，您可以预览连接设置，但无法编辑它们。 您可以在&#x200B;**[!UICONTROL 我的连接]**&#x200B;选项卡中查看挂起的邀请。 连接的状态为&#x200B;**[!UICONTROL 发送邀请]**。

![发送给“我的连接”视图中显示的发布者的待处理邀请。](/help/assets/connect/establish-connection/pending-invite-sent.png){zoomable="yes"}

协作者接受邀请后，即可配置连接设置并将它们发送给协作者进行审查和接受。

## 连接设置 {#connection-settings}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_usecases"
>title="用例"
>abstract="用例已预先填充了所有选项。 您可以在提交连接设置之前编辑用例。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_matchkeys"
>title="匹配键"
>abstract="匹配键会预填充为您在组织级别选择的匹配键。 您可以关闭任何您不想在此连接中使用的匹配键。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_creditsplit"
>title="积分拆分"
>abstract="此部分确定谁将为Real-Time CDP Collaboration中的相应活动付费。 目前，只能配置受众共享用例。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_creditsplit_audiencesharing"
>title="受众共享"
>abstract="受众共享是参与方在请求其匹配的数据由其协作合作伙伴激活时所采取的活动。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_legalagreement"
>title="法律协议"
>abstract="验证双方之间是否存在数据共享协议。"

发送邀请后，您可以预览连接设置。 必须先接受邀请，然后才能完成连接设置。

![处于预览状态的连接设置视图。](/help/assets/connect/establish-connection/preview-connection-settings.png){zoomable="yes"}

协作者接受连接后，您现在即可开始设置连接的连接设置。 连接设置定义了协作条款，如您将一起完成的使用案例、将在项目中使用的匹配键等等。

若要设置连接设置并与协作者共享，请导航到&#x200B;**[!UICONTROL 我的连接]**。 对于状态为&#x200B;**[!UICONTROL 挂起]**&#x200B;的任何连接，可以选择&#x200B;**[!UICONTROL 设置连接]**&#x200B;来配置连接设置。

![已突出显示“我的连接”视图（包含挂起的连接）及其“设置连接”选项。](/help/assets/connect/establish-connection/pending-connection.png){zoomable="yes"}

您可以编辑和定义以下字段：

![设置连接视图](/help/assets/connect/establish-connection/connection-view.png){zoomable="yes"}

+++用例

用例已预先填充了所有可用的用例。 您可以通过选择&#x200B;**[!UICONTROL 编辑]**&#x200B;并切换任何您不想要的使用案例来选择您的连接将使用的使用案例。 选定的用例将影响您的项目中[可用的视图和选项](../collaborate/manage-projects.md#project-use-cases)。

![用例](/help/assets/connect/establish-connection/view-use-cases.png){zoomable="yes"}

+++

+++匹配键

匹配键已预填充为您[在组织级别](/help/guide/setup/onboard-organization.md#set-up-match-keys)选择的匹配键。 您可以关闭任何不希望在此连接中使用的匹配键，但无法添加在设置组织时未选择的任何匹配键。

![匹配键](/help/assets/connect/establish-connection/match-keys.png)

+++

+++信用拆分

使用信用分摊部分确定两个协作方中的哪个将覆盖活动的成本。

![信用拆分](/help/assets/connect/establish-connection/edit-billing-ownership.png)

+++

+++协议

在继续此连接之前，您必须确认双方之间存在数据共享协议。

![法律协议。](/help/assets/connect/establish-connection/legal-agreement.png)

+++

做出选择后，选择&#x200B;**[!UICONTROL 提交]**&#x200B;以将建议的设置发送给您的协作者进行审阅。

如果从协作者处收到建议的连接设置，您可以&#x200B;**[!UICONTROL 接受]**&#x200B;或&#x200B;**[!UICONTROL 拒绝]**&#x200B;这些设置。 在接受连接设置之前，您需要确认并确认您与协作者之间已签署法律协议。 如果您拒绝连接设置，请在产品之外联系您的协作者，讨论他们应如何修改连接设置以便您接受。

## 删除连接 {#delete-connections}

您可以删除与协作者之间不希望继续使用的任何连接。 要删除现有连接，请执行以下操作：

1. 导航到&#x200B;**[!UICONTROL 连接]** > **[!UICONTROL 我的连接]**。
2. 选择连接卡上的&#x200B;**[!UICONTROL 查看连接]**&#x200B;以访问要删除的连接。
3. 选择删除图标![删除图标](/help/assets/common/delete.svg)以打开删除连接确认对话框。
   ![删除连接图标突出显示。](/help/assets/connect/establish-connection/delete-icon-highlighted.png){zoomable="yes"}
4. 选择&#x200B;**[!UICONTROL 删除]**以确认删除。
   ![用于确认删除连接的对话框。](/help/assets/connect/establish-connection/delete-connection-dialog.png){zoomable="yes"}

>[!WARNING]
>
>删除连接后，您将不再与协作者连接，属于协作的所有现有项目都将永久删除并不可恢复。

## 后续步骤

与协作者建立连接后，您和协作者现在可以[创建项目](/help/guide/collaborate/manage-projects.md#create-project)。
