---
audience: end-user
title: 配信ワークフローアクティビティの使用
description: 配信ワークフローアクティビティ（E メール、プッシュ、SMS）を追加する方法を説明します
badge: label="Alpha"
source-git-commit: d70c671e558613a27acc5252091e1e2836b675c7
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 12%

---


# メール、SMS、プッシュ {#channel}

Adobe Campaign Web を使用すると、E メール、SMS、プッシュチャネルをまたいでマーケティングキャンペーンを自動化および実行できます。 チャネルアクティビティをワークフローキャンバスに組み合わせて、顧客の行動とデータに基づいてアクションをトリガー化できるクロスチャネルワークフローを作成できます。

例えば、メール、SMS、プッシュなど、様々なチャネルをまたいだ一連のメッセージを含むようこそメールキャンペーンを作成できます。また、顧客が購入を完了した後にフォローアップ E メールを送信したり、SMS を使用してパーソナライズされた誕生日メッセージを顧客に送信したりできます。

チャネルアクティビティを使用すると、複数のタッチポイントをまたいで顧客を惹きつけ、コンバージョンを促進する、包括的でパーソナライズされたキャンペーンを作成できます。

次に、 **チャネル** ワークフロー内の「 」アクティビティ：

1. 必ず **オーディエンスの構築** アクティビティ。 オーディエンスは、配信のメインターゲットです。メッセージを受信した受信者。 キャンペーンワークフローのコンテキストでメッセージを送信する場合、メッセージオーディエンスは、チャネルアクティビティではなく、 **オーディエンスの構築** アクティビティ。 詳しくは、[この節](build-audience.md)を参照してください。

   ![](../../msg/assets/add-delivery-in-wf.png)

1. 配信アクティビティ（**[!UICONTROL メール]**、**[!UICONTROL SMS]**、**[!UICONTROL プッシュ通知（Android）]**&#x200B;または&#x200B;**[!UICONTROL プッシュ通知（iOS）]**）を選択します。

1. 配信を選択 **テンプレート**. テンプレートは、チャネルに固有の事前設定済みの配信設定です。 組み込みテンプレートは各チャネルで使用でき、デフォルトでは事前入力されます。 [詳細情報](../../msg/delivery-template.md)

   ![](../assets/delivery-activity-in-wf.png)


   左側のパネルのチャネルアクティビティ設定から別のテンプレートを選択できます。 以前に選択したオーディエンスがチャネルに対応していない場合は、テンプレートを選択できません。 これを解決するには、 **オーディエンスの構築** 「 」アクティビティを選択して、正しいターゲットマッピングを持つオーディエンスを選択します。 ターゲットマッピングの詳細については、 [Adobe Campaign v8 （コンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=ja){target="_blank"}.

1. クリック **配信を作成**. スタンドアロン配信の作成時と同様に、メッセージの設定とコンテンツを定義します。 また、コンテンツをスケジュールおよびシミュレートすることもできます。 [詳細情報](../../msg/gs-messages.md)

1. ワークフローに戻り、変更を保存します。

1. クリック **開始** をクリックして、ワークフローを起動します。

   デフォルトでは、ワークフローを開始すると、トリガーは直ちに送信されず、メッセージの準備ステージに移動します。

1. 配信アクティビティを開き、 **確認して送信** 」ボタンをクリックします。

1. 配信ダッシュボードで、 **送信**.

## 例

次に、セグメント化と 2 つの配信を含む、クロスチャネルワークフローの例を示します。 「 」ワークフローでは、パリに住み、コーヒーマシンに関心を持つすべての顧客をターゲットに設定します。 この母集団の中で、標準の顧客に E メールが送信され、VIPクライアントに SMS が送信されます。

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
