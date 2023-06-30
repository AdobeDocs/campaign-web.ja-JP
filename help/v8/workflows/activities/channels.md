---
audience: end-user
title: 配信ワークフローアクティビティの使用
description: 配信ワークフローアクティビティ（メール、プッシュ、SMS）を追加する方法を学ぶ
badge: label="Alpha"
source-git-commit: d70c671e558613a27acc5252091e1e2836b675c7
workflow-type: ht
source-wordcount: '425'
ht-degree: 100%

---


# メール、SMS、プッシュ {#channel}

Adobe Campaign web を使用すると、メール、SMS、プッシュチャネルをまたいでマーケティングキャンペーンを自動化および実行できます。チャネルアクティビティをワークフローキャンバスに組み合わせて、顧客の行動とデータに基づいてアクションをトリガーできるクロスチャネルワークフローを作成できます。

例えば、メール、SMS、プッシュなど、様々なチャネルをまたいだ一連のメッセージを含むようこそメールキャンペーンを作成できます。また、顧客が購入を完了した後や、SMS を使用してパーソナライズされた誕生日メッセージを顧客に送信した後に、フォローアップメールを送信することもできます。

チャネルアクティビティを使用すると、複数のタッチポイントで顧客を引きつけてコンバージョンを促進する、包括的でパーソナライズされたキャンペーンを作成できます。

**チャネル**&#x200B;アクティビティをワークフローに追加する手順を次に示します。

1. **オーディエンスを作成**&#x200B;アクティビティを追加します。オーディエンスは配信のメインターゲットであり、メッセージを受信する受信者となります。キャンペーンワークフローのコンテキストでメッセージを送信する場合、メッセージオーディエンスはチャネルアクティビティではなく、**オーディエンスを作成**&#x200B;アクティビティで定義されます。詳しくは、[この節](build-audience.md)を参照してください。

   ![](../../msg/assets/add-delivery-in-wf.png)

1. 配信アクティビティ（**[!UICONTROL メール]**、**[!UICONTROL SMS]**、**[!UICONTROL プッシュ通知（Android）]**&#x200B;または&#x200B;**[!UICONTROL プッシュ通知（iOS）]**）を選択します。

1. 配信&#x200B;**テンプレート**&#x200B;を選択します。テンプレートは、チャネルに固有の事前設定済みの配信設定です。組み込みテンプレートは各チャネルで使用でき、デフォルトでは事前入力されます。[詳細情報](../../msg/delivery-template.md)

   ![](../assets/delivery-activity-in-wf.png)


   チャネルアクティビティ設定の左側のパネルから別のテンプレートを選択できます。以前に選択したオーディエンスがチャネルに対応していない場合は、テンプレートを選択できません。これを解決するには、**オーディエンスを作成**&#x200B;アクティビティを更新して、ターゲットマッピングが正しいオーディエンスを選択します。ターゲットマッピングについて詳しくは、[Adobe Campaign v8（コンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=ja){target="_blank"}を参照してください。

1. 「**配信を作成**」をクリックします。スタンドアロン配信の作成時と同様に、メッセージの設定とコンテンツを定義します。また、コンテンツをスケジュールおよびシミュレートすることもできます。[詳細情報](../../msg/gs-messages.md)

1. ワークフローに戻り、変更を保存します。

1. 「**開始**」をクリックして、ワークフローを開始します。

   デフォルトでは、ワークフローを開始すると、メッセージはすぐに送信されずに、メッセージの準備ステージに移動します。

1. 配信アクティビティを開き、「**確認して送信**」ボタンから送信を確定します。

1. 配信ダッシュボードで、「**送信**」をクリックします。

## 例

セグメント化と 2 つの配信を含むクロスチャネルワークフローの例を次に示します。 ワークフローでは、パリに在住し、コーヒーマシンに興味があるすべての顧客をターゲットにします。この母集団の中で、通常の顧客にはメールが送信され、VIP クライアントには SMS が送信されます。

![](../assets/workflow-channel-example.png)
<!--
description, which use case you can perform (common other activities that you can link before of after the activity)

how to add and configure the activity

example of a configured activity within a workflow
The Email delivery activity allows you to configure the sending an email in a workflow. 

-->



<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.
Email recipients are defined upstream of the activity in the same workflow, via an Audience targeting activity.

-->


<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->
