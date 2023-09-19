---
audience: end-user
title: 配信ワークフローアクティビティの使用
description: 配信ワークフローアクティビティ（メール、プッシュ、SMS）を追加する方法を学ぶ
badge: label="Beta"
source-git-commit: f5d2cb68b3df42105da9d6b346e6e9c57e14723a
workflow-type: tm+mt
source-wordcount: '781'
ht-degree: 59%

---


# E メール、SMS、プッシュアクティビティ {#channel}

Adobe Campaign web を使用すると、メール、SMS、プッシュチャネルをまたいでマーケティングキャンペーンを自動化および実行できます。チャネルアクティビティをワークフローキャンバスに組み合わせて、顧客の行動とデータに基づいてアクションをトリガーできるクロスチャネルワークフローを作成できます。

例えば、メール、SMS、プッシュなど、様々なチャネルをまたいだ一連のメッセージを含むウェルカムメールキャンペーンを作成できます。また、顧客が購入を完了した後や、SMS を使用してパーソナライズされた誕生日メッセージを顧客に送信した後に、フォローアップメールを送信することもできます。

チャネルアクティビティを使用すると、複数のタッチポイントで顧客を引きつけてコンバージョンを促進する、包括的でパーソナライズされたキャンペーンを作成できます。

>[!NOTE]
>
>また、キャンペーンワークフローのコンテキスト外で、ワンショット配信を作成することもできます。 詳しくは、次の節を参照してください。
>* [スタンドアロンの E メール配信を作成](../../email/create-email.md)
>* [スタンドアロンの SMS 配信を作成する](../../sms/create-sms.md)
>* [スタンドアロンのプッシュ配信を作成](../../push/create-push.md)

## ワークフローの作成{#build-your-workflow}

配信を配置する前に、関連するアクティビティを使用してワークフローの作成を開始します。

* 修復配信を送信する場合は、 **スケジューラ** アクティビティ。 ワンショット配信を送信する場合は、 **スケジューラ** アクティビティを作成するか、配信設定でスケジュールを定義します。 詳しくは、[この節](scheduler.md)を参照してください。

* **オーディエンスを作成**&#x200B;アクティビティを追加します。オーディエンスは配信のメインターゲットであり、メッセージを受信する受信者となります。キャンペーンワークフローのコンテキストでメッセージを送信する場合、メッセージオーディエンスはチャネルアクティビティではなく、**オーディエンスを作成**&#x200B;アクティビティで定義されます。詳しくは、[この節](build-audience.md)を参照してください。

  ![](../../msg/assets/add-delivery-in-wf.png)

## チャネルアクティビティの設定 {#create-a-delivery-in-a-workflow}


>[!CONTEXTUALHELP]
>id="acw_orchestration_email"
>title="E メールアクティビティ"
>abstract="E メール、SMS、プッシュチャネルをまたいでマーケティングキャンペーンを自動化および実行します。 チャネルアクティビティをワークフローキャンバスに組み合わせて、顧客の行動とデータに基づいてアクションをトリガーできるクロスチャネルワークフローを作成できます。"


>[!CONTEXTUALHELP]
>id="acw_orchestration_sms"
>title="SMS アクティビティ"
>abstract="E メール、SMS、プッシュチャネルをまたいでマーケティングキャンペーンを自動化および実行します。 チャネルアクティビティをワークフローキャンバスに組み合わせて、顧客の行動とデータに基づいてアクションをトリガーできるクロスチャネルワークフローを作成できます。"


>[!CONTEXTUALHELP]
>id="acw_orchestration_push_ios"
>title="iOSアクティビティをプッシュ"
>abstract="E メール、SMS、プッシュチャネルをまたいでマーケティングキャンペーンを自動化および実行します。 チャネルアクティビティをワークフローキャンバスに組み合わせて、顧客の行動とデータに基づいてアクションをトリガーできるクロスチャネルワークフローを作成できます。"


>[!CONTEXTUALHELP]
>id="acw_orchestration_push_android"
>title="Android アクティビティをプッシュ"
>abstract="E メール、SMS、プッシュチャネルをまたいでマーケティングキャンペーンを自動化および実行します。 チャネルアクティビティをワークフローキャンバスに組み合わせて、顧客の行動とデータに基づいてアクションをトリガーできるクロスチャネルワークフローを作成できます。"

ワークフローのコンテキストで配信を設定するには、次の手順に従います。

1. チャネルアクティビティを追加します。 **[!UICONTROL 電子メール]**, **[!UICONTROL SMS]**, **[!UICONTROL プッシュ通知 (Android)]** または **[!UICONTROL プッシュ通知 (iOS)]**.

1. を選択します。 **配信のタイプ**：単一または繰り返し。

   * **単一の配信**：これは 1 回限りのワンショット配信で、例えば、ブラックフライデーの E メールなど 1 回だけ送信されます。
   * **繰り返し配信**：このタイプの配信の場合は、 [スケジューラーアクティビティ](scheduler.md). ワークフローが実行されるたびに、オーディエンスが再計算され、更新されたコンテンツと共に配信が送信されます。 これは、週刊ニュースレターでも、誕生日の定期 E メールでもかまいません。

1. 配信&#x200B;**テンプレート**&#x200B;を選択します。テンプレートは、チャネルに固有の事前設定済みの配信設定です。ビルトインテンプレートは各チャネルで使用でき、デフォルトでは事前入力されます。[詳細情報](../../msg/delivery-template.md)

   ![](../assets/delivery-activity-in-wf.png)

   チャネルアクティビティ設定の左側のパネルから別のテンプレートを選択できます。以前に選択したオーディエンスがチャネルに対応していない場合は、テンプレートを選択できません。これを解決するには、**オーディエンスを作成**&#x200B;アクティビティを更新して、ターゲットマッピングが正しいオーディエンスを選択します。ターゲットマッピングの詳細については、 [Adobe Campaign v8 （クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=ja){target="_blank"}.

1. 「**配信を作成**」をクリックします。スタンドアロン配信の作成時と同様に、メッセージの設定とコンテンツを定義します。また、コンテンツをスケジュールおよびシミュレートすることもできます。[詳細情報](../../msg/gs-messages.md)

1. ワークフローに戻ります。 ワークフローを続行する場合に選択します **アウトバウンドトランジションを生成** チャネルアクティビティの後にトランジションを追加する場合。

1. 「**開始**」をクリックして、ワークフローを開始します。

   デフォルトでは、ワークフローを開始すると、メッセージはすぐに送信されずに、メッセージの準備ステージに移動します。

1. 配信アクティビティを開き、「**確認して送信**」ボタンから送信を確定します。

1. 配信ダッシュボードで、「**送信**」をクリックします。

## 例 {#cross-channel-workflow-sample}

セグメント化と 2 つの配信を含むクロスチャネルワークフローの例を次に示します。ワークフローでは、パリに在住し、コーヒーマシンに興味があるすべての顧客をターゲットにします。この母集団の中で、通常の顧客にはメールが送信され、VIP クライアントには SMS が送信されます。

![](../assets/workflow-channel-example.png)

<!--
description, which use case you can perform (common other activities that you can link before of after the activity)

how to add and configure the activity

example of a configured activity within a workflow
The Email delivery activity allows you to configure the sending an email in a workflow. 

-->

また、パリに住むすべてのお客様に、毎月初日の午後 8 時にパーソナライズされた SMS を送信する繰り返しワークフローを作成することもできます。

![](../assets/workflow-channel-example2.png)

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.
Email recipients are defined upstream of the activity in the same workflow, via an Audience targeting activity.

-->


<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->
