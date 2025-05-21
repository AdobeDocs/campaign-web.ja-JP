---
audience: end-user
title: Adobe Campaign Web でのキャンペーンの作成
description: Adobe Campaign Web を使用してクロスチャネルキャンペーンを作成する方法を学ぶ
exl-id: a6e01470-73e5-4973-aa6a-9836a6ee1cd2
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 最初のキャンペーンを作成 {#create-first-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_properties"
>title="キャンペーン作成プロパティ"
>abstract="この画面では、キャンペーン設定を定義します。テンプレートを選択し、キャンペーンのラベルを入力します。追加の設定を参照して、デフォルトの内部名とフォルダーの変更、説明の追加、担当者の選択を行います。"

>[!CONTEXTUALHELP]
>id="acw_campaign_properties"
>title="キャンペーンプロパティ"
>abstract="この画面では、ラベル、内部名、フォルダー、説明などのキャンペーン設定を確認および更新できます。また、割り当て先のユーザーを表示することもできます。"

新しいキャンペーンを作成するには、その設定を定義し、ワークフローと配信をスケジュールして含めます。

## キャンペーンの作成 {#campaign-create}

新しいキャンペーンを作成するには、次の手順に従います。

1. **[!UICONTROL キャンペーン]**&#x200B;メニューをクリックし、「**[!UICONTROL キャンペーンを作成]**」ボタンをクリックします。

   ![キャンペーンメニューの「キャンペーンを作成」ボタンを示すスクリーンショット](assets/create-campaign-button.png)

1. 使用する&#x200B;**テンプレート**&#x200B;を選択し、キャンペーンのラベルを入力します。[詳細情報](manage-campaigns.md#manage-campaign-templates)。
1. 必要に応じて、内部名、フォルダー、担当者、説明、特性などの&#x200B;**追加オプション**&#x200B;を変更します。
1. キャンペーンの&#x200B;**スケジュール**&#x200B;を定義します。キャンペーンスケジュールを設定する方法について詳しくは、[この節](#campaign-schedule)を参照してください。
1. 「**作成**」をクリックします。

   ![内部名、フォルダー、担当者、説明、特性のフィールドを含む、キャンペーンプロパティ画面を示すスクリーンショット。](assets/create-a-campaign-properties.png)

1. キャンペーンにワークフローと配信を追加します。

   * 「**ワークフロー**」タブで、「**ワークフローを作成**」をクリックします。キャンペーンの作成時に、デフォルトのワークフローが自動的に追加されます。詳しくは、[ワークフローの作成](../workflows/create-workflow.md)方法を参照してください。

   * 「**配信**」タブで、「**配信を作成**」をクリックします。[詳細情報](../msg/gs-messages.md)

## キャンペーンの監視とトラック {#campaign-monitoring}

キャンペーンの監視は、キャンペーンの有効性を分析するための重要な手順です。キャンペーンを開き、「**ログ**」ボタンをクリックします。

また、専用のレポートを表示するには、「**レポート**」ボタンをクリックします。 [こちら](../reporting/campaign-reports.md)を参照してください。

## キャンペーンスケジュールの定義 {#campaign-schedule}

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_schedule"
>title="キャンペーンスケジュール"
>abstract="キャンペーンスケジュールを選択します。キャンペーンを作成して、開始日になるとキャンペーンが開始されます。デフォルトでは、キャンペーンの開始日は作成日であり、期間は 5 日間です。開始日と終了日は、キャンペーンリストに表示され、フィルターとして使用できます。"

キャンペーンは、開始日になると開始します。開始日にならない限り、キャンペーンは&#x200B;**[!UICONTROL ドラフト]**&#x200B;ステータスになります。開始日になると、**[!UICONTROL 処理中]**&#x200B;に変わります。終了日になると、キャンペーンは&#x200B;**[!UICONTROL 完了]**&#x200B;に設定されます。

開始日と終了日は、キャンペーンリストに表示され、フィルターとして使用できます。[こちら](manage-campaigns.md#access-campaigns)を参照してください。

>[!NOTE]
>
>これらのプロパティは、キャンペーンラベルの横にある「**キャンペーン設定を指定**」アイコンから後で変更できます。この[節](gs-campaigns.md#campaign-dashboard)を参照してください。

日付に達すると、ワークフローのコンテキストでは、そのキャンペーンで作成され、送信準備が整った配信が実際に送信されます。このためには、ワークフローを開始しておく必要があります。

<!--
    +++WORKF
++screen
## Create a cross-channel campaign {#cross-channel-campaign}

In a cross-channel campaign, a single marketing communication uses different channels. Data is passed between the channels. The customer receives communication through multiple channels based on, for example, their interaction with the previous communication.
-->
<!--
existing campaign: settings button -> properties like when creation
schedule in header

About plans, programs and campaigns
Adobe Campaign allows you to plan marketing campaigns in which you can create and manage different types of activities: emails, SMS messages, push notifications, workflows, landing pages. These campaigns and their contents can be gathered into programs.

The programs and campaigns allow you to regroup and view the different marketing activities that are linked to them.

A program may contain other programs as well as campaigns, workflows, and landing pages. It appears in the timeline and helps you organize your marketing activities: you can separate them by country, by brand, by unit, and similar criteria.

A campaign enables you to gather all the marketing activities of your choice under a single entity. A campaign may contain emails, SMS, push notifications, direct mails, workflows, and landing pages.

To better organize your marketing plans, Adobe recommends the following hierarchy: Program > Sub-programs > Campaigns > Workflows > Deliveries.

Reports on programs and campaigns allow you to analyze their impact. For example, you can build reports at the campaign level to aggregate data on all deliveries contained in that campaign.

Related topics:

* Timeline
* About dynamic reports
* Creating a campaign

In programs and sub-programs, you can add campaigns. Campaigns can contain marketing activities such as emails, SMS, push notifications, workflows, and landing pages.

From the Adobe Campaign home page, select the Programs & Campaigns card, and access a program or sub-program.

Click on the Create button, and select Campaign.

In the Creation mode screen, select a campaign type.

The campaign types available are based on templates defined in Resources > Templates > Campaign templates. For more on this, refer to the Managing templates section.

In the Properties screen, enter the name and ID of the campaign.

Select a start and end date for your campaign. These dates only apply to the campaign itself.

Click on Create to confirm the creation of the campaign.

The campaign is created and displayed. Use the Create button to add marketing activities to your campaign.

>[!NOTE]
>
>Depending on your license agreement, you may access only some of these activities.

You can also create a campaign from the marketing activity list. You can choose to link the marketing activity to a parent program or sub-program via the properties window of the campaign.

Programs and campaigns icons and statuses:

Each program and each campaign in the list has a visual symbol and an icon whose color indicates the execution status. This status depends on the validity period of the program or the campaign.

* Gray: the program/campaign has not yet started - Editing status.
* Blue: the program/campaign is in progress - In progress status.
* Green: the program/campaign has finished - Finished status.

By default, the current date is automatically shown as the validity start date, and the end date is calculated according to the start date (D+186 days). You can change these dates in the program or campaign properties.

Business.Adobe.com resources
-->