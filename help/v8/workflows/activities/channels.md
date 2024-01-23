---
audience: end-user
title: 配信ワークフローアクティビティの使用
description: 配信ワークフローアクティビティ（メール、プッシュ、SMS）を追加する方法を学ぶ
badge: label="限定提供（LA）"
exl-id: 155b40e2-1aa2-4251-bbaa-7e16e36f649e
source-git-commit: 74102899efa10e37705cbd3c7c6796eb6ac0b18e
workflow-type: tm+mt
source-wordcount: '900'
ht-degree: 70%

---

# メール, SMS, プッシュアクティビティ {#channel}

Adobe Campaign web を使用すると、メール、SMS、プッシュチャネルをまたいでマーケティングキャンペーンを自動化および実行できます。チャネルアクティビティをワークフローキャンバスに組み合わせて、顧客の行動とデータに基づいてアクションをトリガーできるクロスチャネルワークフローを作成できます。

例えば、メール、SMS、プッシュなど、様々なチャネルをまたいだ一連のメッセージを含むウェルカムメールキャンペーンを作成できます。また、顧客が購入を完了した後や、SMS を使用してパーソナライズされた誕生日メッセージを顧客に送信した後に、フォローアップメールを送信することもできます。

チャネルアクティビティを使用すると、複数のタッチポイントで顧客を引きつけてコンバージョンを促進する、包括的でパーソナライズされたキャンペーンを作成できます。

>[!NOTE]
>
>キャンペーンワークフローのコンテキスト外で、1 回限りの配信を作成することもできます。詳しくは、以下の節を参照してください。
>* [スタンドアロンメール配信を作成](../../email/create-email.md)
>* [スタンドアロン SMS 配信を作成](../../sms/create-sms.md)
>* [スタンドアロンプッシュ配信を作成](../../push/create-push.md)

## ワークフローを作成 {#build-your-workflow}

次の関連するアクティビティを使用して、ワークフローの作成を開始します。

* チャネルアクティビティを挿入する前に、オーディエンスを定義する必要があります。 オーディエンスは、配信の主なターゲットである、メッセージを受信するプロファイルです。 キャンペーンワークフローのコンテキストでメッセージを送信する場合、メッセージオーディエンスは、チャネルアクティビティでは定義されず、次のような専用のアクティビティ内で定義されます。

   * A **オーディエンスの構築** アクティビティ。 [詳細情報](build-audience.md)。

     ![](../../msg/assets/add-delivery-in-wf.png)

   * A **ファイルを読み込み** アクティビティの後に **紐づけ** アクティビティ。 [詳細情報](load-file.md)。

     ![](../assets/workflow-reconciliation-criteria.png)



* 繰り返し配信を送信するには、 **スケジューラ** アクティビティ。 また、 **スケジューラ** 「ワンショット単一配信のアクティビティ」：その配信のコンタクト日を設定します。 このコンタクト日は、配信設定でも設定できます。 詳しくは、[この節](scheduler.md)を参照してください。


## チャネルアクティビティを設定 {#create-a-delivery-in-a-workflow}

>[!CONTEXTUALHELP]
>id="acw_orchestration_email"
>title="メールアクティビティ"
>abstract="「メール」アクティビティでは、ワークフロー内でのメール送信を促進し、1 回限りのメッセージと繰り返しメッセージの両方を送信できます。これは、同じワークフロー内で計算されたターゲットにメールを送信するプロセスを自動化する役割を果たします。チャネルアクティビティをワークフローキャンバスに組み合わせて、顧客の行動とデータに基づいてアクションをトリガーできるクロスチャネルワークフローを作成できます。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_sms"
>title="SMS アクティビティ"
>abstract="「SMS」アクティビティでは、ワークフロー内で SMS 送信を促進し、1 回限りのメッセージと繰り返しメッセージの両方を送信できます。これは、同じワークフロー内で計算されたターゲットに SMS を送信するプロセスを自動化する役割を果たします。チャネルアクティビティをワークフローキャンバスに組み合わせて、顧客の行動とデータに基づいてアクションをトリガーできるクロスチャネルワークフローを作成できます。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_push_ios"
>title="iOS アクティビティをプッシュ"
>abstract="「iOS をプッシュ」アクティビティでは、ワークフローの一部として iOS プッシュ通知を送信するプロセスを効率化します。これにより、1 回限りのメッセージと繰り返しメッセージの両方の配信が可能になり、同じワークフロー内の定義済みターゲットへの iOS プッシュ通知の送信が自動化されます。チャネルアクティビティをワークフローキャンバスに組み合わせて、顧客の行動とデータに基づいてアクションをトリガーできるクロスチャネルワークフローを作成できます。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_push_android"
>title="Android アクティビティをプッシュ"
>abstract="「Android をプッシュ」アクティビティでは、ワークフローの一部として Android プッシュ通知を送信するプロセスを効率化します。これにより、1 回限りのメッセージと繰り返しメッセージの両方の配信が可能になり、同じワークフロー内の定義済みターゲットへの Android プッシュ通知の送信が自動化されます。チャネルアクティビティをワークフローキャンバスに組み合わせて、顧客の行動とデータに基づいてアクションをトリガーできるクロスチャネルワークフローを作成できます。"

ワークフローのコンテキストで配信を設定するには、次の手順に従います。

1. チャネルアクティビティ（**[!UICONTROL メール]**、**[!UICONTROL SMS]**、**[!UICONTROL プッシュ通知（Android）]**&#x200B;または&#x200B;**[!UICONTROL プッシュ通知（iOS）]**）を追加します。

1. 「**配信のタイプ**」（単一または繰り返し）を選択します。

   * A **単一の配信** はワンショット配信で、例えばブラックフライデーの E メールなど 1 回だけ送信されます。
   * A **繰り返し配信** は、 [スケジューラーアクティビティ](scheduler.md). ワークフローが実行されるたびに、オーディエンスが再計算され、更新されたオーディエンスに配信が送信され、コンテンツも更新されます。 例えば、毎週のニュースレターや、誕生日の E メールなどを送信できます。

1. 配信&#x200B;**テンプレート**&#x200B;を選択します。テンプレートは、チャネルに固有の事前設定済みの配信設定です。ビルトインテンプレートは各チャネルで使用でき、デフォルトでは事前入力されます。[詳細情報](../../msg/delivery-template.md)

   ![](../assets/delivery-activity-in-wf.png)

   左側のパネルでチャネルアクティビティの設定からテンプレートを選択できます。 以前に選択したオーディエンスがチャネルに対応していない場合は、テンプレートを選択できません。これを解決するには、**オーディエンスを作成**&#x200B;アクティビティを更新して、ターゲットマッピングが正しいオーディエンスを選択します。ターゲットマッピングの詳細については、 [この節](../../audience/targeting-dimensions.md)

1. 「**配信を作成**」をクリックします。その後、スタンドアロン配信を作成する場合と同じ方法で、メッセージの設定とコンテンツを定義できます。 また、コンテンツをテストしてシミュレートすることもできます。 [詳細情報](../../msg/gs-messages.md)

1. ワークフローに戻ります。ワークフローを続行する場合は、 **アウトバウンドトランジションを生成** オプションを使用して、チャネルアクティビティの後にトランジションを追加できます。

1. 「**開始**」をクリックして、ワークフローを開始します。

   デフォルトでは、ワークフローを開始すると、メッセージはすぐに送信されずに、メッセージの準備ステージに移動します。

1. チャネルアクティビティを開き、 **レビューと送信** 」ボタンをクリックします。

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

また、繰り返しワークフローを作成して、毎月初日の午後 8 時にパーソナライズされた SMS をパリ在住のすべてのお客様に送信することもできます。

![](../assets/workflow-channel-example2.png)

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.
Email recipients are defined upstream of the activity in the same workflow, via an Audience targeting activity.

-->


<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->
