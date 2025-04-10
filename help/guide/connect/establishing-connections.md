---
title: 与广告商或发布商建立联系
description: 发现潜在的合作者后，了解如何建立联系并开始在项目上协作。
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

在协作的双方（最常见的是广告商和发布商）之间建立联系是实时 CDP 协作的先决条件，以便公司共同开展营销活动。 发布商和广告商都可以建立联系。 启动连接的一方之后将成为 *连接所有者*。

## 高级工作流程

概括地说，要在广告客户和发布商之间建立联系，工作流程如下所示：

1. 广告客户 [浏览发布商并发现](/help/guide/connect/discover-publishers.md) 他们想与之合作的发布商
2. 广告商发送连接邀请。
3. 发布者接受邀请。
4. 广告商发送连接设置，包括匹配密钥和其他设置。 这些连接设置表示协作的产品内条款。
5. 发布服务器接受连接设置。 如果需要，发布者可以拒绝初始连接设置并请求广告商提交修改后的连接设置。

![广告 — 发布者连接过程的高级关系图。](/help/assets/connect/establish-connection/advertiser-publisher-connection-process.png)

完成上述项目后，协作者可以继续[创建项目](/help/guide/collaborate/manage-projects.md#create-project)至[运行重叠报表](/help/guide/collaborate/discover.md)并启动广告营销活动。

>[!IMPORTANT]
>
>在建立两个协作者之间的连接后，便无法再修改连接设置。

## 发送邀请 {#send-invite}

若要设置连接，请在浏览发现发布者屏幕中的发布者清单时选择&#x200B;**[!UICONTROL 连接]**。

![连接选择器](/help/assets/connect/establish-connection/connect-selection.png)

此时，邀请已发出，您可以预览连接设置，但无法对其进行编辑。 您可以在“我的连接&#x200B;]**”选项卡中查看待处理的邀请**[!UICONTROL 。连接的状态为 **[!UICONTROL “已发送]**&#x200B;邀请”。

![发送给“我的连接”视图中显示的发布者的待处理邀请。](/help/assets/connect/establish-connection/pending-invite-sent.png)

协作者接受邀请后，即可配置连接设置并将它们发送给协作者进行审查和接受。

## 连接设置 {#connection-settings}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_usecases"
>title="用例"
>abstract="用例中预填充了所有选项。 您可以在提交连接设置之前编辑用例。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_matchkeys"
>title="匹配键"
>abstract="匹配键预填充了您在组织级别选择的键。 您可以关闭不想在此连接中使用的任何匹配键。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_creditsplit"
>title="积分拆分"
>abstract="本节确定谁为Real-Time CDP Collaboration中的相应活动付费。 目前，只能配置受众共享用例。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_creditsplit_audiencesharing"
>title="受众共享"
>abstract="Audience Sharing是指参与方请求由其协作合作伙伴激活其匹配的数据时采取的活动。"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_legalagreement"
>title="法律协议"
>abstract="验证双方之间是否存在数据共享协议。"

发送邀请后，您可以预览连接设置。 必须先接受邀请，然后才能完成连接设置。

![处于预览状态的连接设置视图。](/help/assets/connect/establish-connection/preview-connection-settings.png)

协作者接受连接后，您现在即可开始设置连接的连接设置。 连接设置定义了协作条款，如您将一起完成的使用案例、将在项目中使用的匹配键等等。

要设置连接设置并与协作者共享连接设置，请导航到&#x200B;**[!UICONTROL 我的连接]**。 对于状态为&#x200B;**[!UICONTROL 挂起]**&#x200B;的任何连接，您可以选择&#x200B;**[!UICONTROL 设置连接]**&#x200B;以配置连接设置。

![“我的连接”视图，其中突出显示了“挂起的连接”及其“设置连接”选项。](/help/assets/connect/establish-connection/pending-connection.png)

您可以编辑和定义以下字段：

![设置连接视图](/help/assets/connect/establish-connection/connection-view.png)

+++用例

用例已预先填充了所有可用的用例。 您可以通过选择&#x200B;**[!UICONTROL 编辑]**&#x200B;并切换任何您不想要的使用案例来选择您的连接将使用的使用案例。 选定的用例将影响您的项目中[可用的视图和选项](../collaborate/manage-projects.md#project-use-cases)。

![用例](/help/assets/connect/establish-connection/view-use-cases.png)

+++

+++匹配键

匹配密钥预填充了您[在组织级别](/help/guide/setup/onboard-organization.md#set-up-match-keys)选择的密钥。 您可以关闭任何不想在此连接中使用的匹配密钥，但无法添加任何在设置组织时未选择的匹配密钥。

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

做出选择后，选择“提交&#x200B;]**”**[!UICONTROL ，将建议的设置发送给协作者审阅。

如果您从协作者处收到建议的连接设置， **[!UICONTROL 则可以接受]** 或 **[!UICONTROL 拒绝]** 这些设置。 在接受连接设置之前，您需要确认并确认您与合作者之间已签订法律协议。 如果您拒绝连接设置，请在产品之外联系您的协作者，讨论他们应如何修改连接设置以便您接受。

## 删除连接 {#delete-connections}

您可以删除与协作者之间不希望继续使用的任何连接。 要删除现有连接，请执行以下操作：

1. 导航到“**[!UICONTROL 连接”>**[!UICONTROL “我的连接&#x200B;]**]**”。
2. 选择连接卡上的“查看连接&#x200B;]**”**[!UICONTROL &#x200B;以访问要删除的连接。
3. 选择删除图标 ![删除图标](/help/assets/common/delete.svg) 以显示删除连接确认对话框。
   ![突出显示的“删除连接”图标。](/help/assets/connect/establish-connection/delete-icon-highlighted.png)
4. 通过选择“删除&#x200B;]**”**[!UICONTROL 确认删除。
   ![用于确认删除连接的对话框。 ](/help/assets/connect/establish-connection/delete-connection-dialog.png)

>[!WARNING]
>
>删除连接后，您将不再与协作者建立连接，并且属于协作的所有现有项目都将被永久删除且无法恢复。

## 后续步骤

与协作者建立连接后，您和协作者现在可以[创建项目](/help/guide/collaborate/manage-projects.md#create-project)。
