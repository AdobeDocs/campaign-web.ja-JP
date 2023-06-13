---
audience: end-user
title: Adobe Campaign Web でのキャンペーンの作成
description: Adobe Campaign Web を使用してクロスチャネルキャンペーンを作成する方法を学ぶ
badge: label="Alpha" type="Positive"
exl-id: a6e01470-73e5-4973-aa6a-9836a6ee1cd2
source-git-commit: 7daead11e097f6179c99adb0e9496dec567cb29a
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 17%

---


# クロスチャネルキャンペーンの作成 {#create-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_properties"
>title="キャンペーン作成プロパティ"
>abstract="キャンペーンのプロパティとメタデータを定義します。"

>[!CONTEXTUALHELP]
>id="acw_campaign_properties"
>title="キャンペーンプロパティ"
>abstract="キャンペーンの設定とメタデータを定義します。"

キャンペーンには、ワークフローとスタンドアロン配信を含めることができます。

新しいキャンペーンを作成するには、次の手順に従います。

1. 次をクリック： **[!UICONTROL キャンペーン]** メニューで、 **[!UICONTROL キャンペーンを作成]** 」ボタンをクリックします。
1. を選択します。 **テンプレート** を使用して、キャンペーンのラベルを指定します。 キャンペーンテンプレートは、新しいキャンペーンの作成に再利用できるように事前設定されています。 クライアントコンソールから作成されます。
   [詳細情報](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-templates.html?lang=ja)。
1. 必要に応じて、次の項目を変更できます **その他のオプション**:内部名、フォルダー、担当者、説明および特性
1. 次を定義： **スケジュール** キャンペーンの キャンペーンは、開始日になると開始されます。 開始日と終了日はキャンペーンリストに表示され、フィルターとして使用できます。 [こちら](gs-campaigns.md#access-campaigns)を参照してください。

   ![キャンペーンプロパティの定義](assets/campaign-properties.png)

   >[!NOTE]
   >
   >これらのプロパティは、後で **キャンペーンの設定** アイコン（キャンペーンラベルの横）をクリックします。 参照 [セクション](gs-campaigns.md#campaign-dashboard)

1. 「**作成**」をクリックします。
1. キャンペーンにワークフローと配信を追加します。

   * 次の **ワークフロー** タブ、クリック **ワークフローを作成**. キャンペーンの作成時に、デフォルトのワークフローが自動的に追加されます。 詳しくは、 [ワークフローの作成](../workflows/create-workflow.md)
   * 次の **配信** タブ、クリック **配信を作成**. [詳細情報](../msg/gs-messages.md)
1. 以下を使用： **ログ** および **レポート** ボタンを使用してキャンペーンを分析します。

## ログの監視とトラッキング{#campaign-monitoring}

キャンペーンの監視は、キャンペーンを分析するための重要な手順です。 キャンペーンを開き、 **ログ** 」ボタンをクリックします。

また、 **レポート** 」ボタンをクリックします。 [こちら](../reporting/campaign-reports.md)を参照してください。

## キャンペーンの複製と削除

キャンペーンの複製や削除は、次の場合におこなえます。

* キャンペーンのリストで、省略記号ボタンをクリックし、「 **複製** または **削除**.
* キャンペーン自体から、 **詳細** ボタンをクリックし、 **複製** または **削除**.

>[!NOTE]
>
>この **配信** 「 」タブには、キャンペーンにリンクされているすべての配信が表示されますが、ワークフローで作成された配信はこのタブからは削除できません。 ワークフローのコンテキストで作成された配信を削除するには、ワークフローから配信アクティビティを削除する必要があります。


<!--
## Create a cross-channel campaign {#cross-channel-campaign}


>[!CONTEXTUALHELP]
>id="acw_campaign_creation_workflow"
>title="Workflow list"
>abstract="List of workflows available for your campaign. Use the 'Create workflow' button to add a workflow in your campaign."

In a cross-channel campaign, a single marketing communication uses different channels. Data is passed between the channels. The customer receives communication through multiple channels based on, for example, their interaction with the previous communication.

-->
<!--
existing campaign: settings button -> properties like when creation
schedule in header


About plans, programs and campaigns
Adobe Campaign allows you to plan marketing campaigns in which you can create and manage different types of activities: emails, SMS messages, push notifications, workflows, landing pages. These campaigns and their contents can be gathered into programs.

The programs and campaigns allow you to regroup and view the different marketing activities that are linked to them.

A program may contain other programs as well as campaigns, workflows, and landing pages. It appears in the timeline and help you organize your marketing activities: you can separate them by country, by brand, by unit, etc.
A campaign enables you to gather all the marketing activities of your choice under a single entity. A campaign may contain emails, SMS, push notifications, direct mails, workflows, and landing pages.
To better organize your marketing plans, Adobe recommends the following hierarchy: Program > Sub-programs > Campaigns > Workflows > Deliveries.

Reports on programs and campaigns allow you to analyze their impact. For example, you can build reports at the campaign level to aggregate data on all deliveries contained in that campaign.

Related topics:

Timeline
About dynamic reports
Creating a campaign
In programs and sub-programs, you can add campaigns. Campaigns can contain marketing activities such as emails, SMS, push notifications, workflows, and landing pages.

From the Adobe Campaign home page, select the Programs & Campaigns card and access a program or sub-program.

Click on the Create button and select Campaign.

In the Creation mode screen, select a campaign type.



The campaign types available are based on templates defined in Resources > Templates > Campaign templates. For more on this, refer to the Managing templates section.

In the Properties screen, enter the name and ID of the campaign.

Select a start and end date to your campaign. These dates only apply to the campaign itself.



Click on Create to confirm the creation of the campaign.

The campaign is created and displayed. Use the Create button to add marketing activities to your campaign.

NOTE
Depending on your license agreement, you may access only some of these activities.

You can also create a campaign from the marketing activity list. You can choose to link the marketing activity to a parent program or sub-program via the properties window of the campaign.


Programs and campaigns icons and statuses
Each program and each campaign in the list has a visual symbol and an icon whose color indicates the execution status. This status depends on the validity period of the program or the campaign.

Gray: the program/campaign has not yet started - Editing status.
Blue: the program/campaign is in progress - In progress status.
Green: the program/campaign has finished - Finished status. By default, the current date is automatically shown as the validity start date and the end date is calculated according to the start date (D+186 days). You can change these dates in the program or campaign properties.


Business.Adobe.com resources
-->
