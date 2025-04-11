---
audience: end-user
title: 配信ワークフローアクティビティの使用
description: 配信ワークフローアクティビティ（メール、プッシュ、SMS、ダイレクトメール）を追加する方法を説明します。
exl-id: 155b40e2-1aa2-4251-bbaa-7e16e36f649e
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '966'
ht-degree: 38%

---

# メール, SMS, プッシュ, ダイレクトメールアクティビティ {#channel}

Adobe Campaign web を使用すると、メール、SMS、ダイレクトメール、プッシュチャネルをまたいでマーケティングキャンペーンを自動化および実行できます。 チャネルアクティビティをワークフローキャンバスに組み合わせて、顧客の行動とデータに基づいてアクションをトリガーにするクロスチャネルワークフローを作成できます。

例えば、メール、SMS、プッシュ、ダイレクトメールなど、様々なチャネルをまたいだ一連のメッセージを含むようこそメールキャンペーンを作成します。 また、顧客が購入を完了した後や、SMS を使用してパーソナライズされた誕生日メッセージを顧客に送信した後に、フォローアップメールを送信することもできます。

チャネルアクティビティを使用することで、複数のタッチポイントで顧客を引きつけてコンバージョンを促進する、包括的でパーソナライズされたキャンペーンを作成します。

>[!NOTE]
>
>キャンペーンワークフローのコンテキスト外で、1 回限りの配信を作成することもできます。 詳しくは、以下の節を参照してください。
>* [スタンドアロンメール配信を作成](../../email/create-email.md)
>* [スタンドアロン SMS 配信を作成](../../sms/create-sms.md)
>* [スタンドアロンプッシュ配信を作成](../../push/create-push.md)
>* [スタンドアロンダイレクトメール配信を作成](../../direct-mail/create-direct-mail.md)

## 前提条件 {#channel-activity-prereq}

関連するアクティビティを使用してワークフローの作成を開始します。

* チャネルアクティビティを挿入する前に、オーディエンスを定義します。 オーディエンスは配信のメインターゲット、つまりメッセージを受信するプロファイルです。キャンペーンワークフローのコンテキストでメッセージを送信する場合、メッセージオーディエンスはチャネルアクティビティではなく、次のような専用アクティビティ内で定義されます。

   * 「**オーディエンスを作成**」アクティビティ。[詳細情報](build-audience.md)。

     ![ ワークフローへの配信の追加を示すスクリーンショット ](../../msg/assets/add-delivery-in-wf.png)

   * 「**ファイルを読み込み**」アクティビティと、これに続く「**紐付け**」アクティビティ。[詳細情報](load-file.md)。

     ![ ワークフローの紐付け条件を示すスクリーンショット ](../assets/workflow-reconciliation-criteria.png)

* 繰り返し配信を送信するには、「**スケジューラー**」アクティビティでワークフローを開始します。1 回限りの単一配信に **スケジューラー** アクティビティを使用して、その配信のコンタクト日を設定します。 この連絡日は、配信設定でも設定できます。詳しくは、[このセクション](scheduler.md)を参照してください。

## チャネルアクティビティを設定 {#create-a-delivery-in-a-workflow}

>[!CONTEXTUALHELP]
>id="acw_orchestration_email"
>title="メールアクティビティ"
>abstract="「メール」アクティビティでは、ワークフロー内でのメール送信を促進し、1 回限りのメッセージと繰り返しメッセージの両方を送信できます。同じワークフロー内で計算されたターゲットにメールを送信するプロセスを自動化します。 チャネルアクティビティをワークフローキャンバスに組み合わせて、顧客の行動とデータに基づいてアクションをトリガーにするクロスチャネルワークフローを作成できます。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_sms"
>title="SMS アクティビティ"
>abstract="「SMS」アクティビティでは、ワークフロー内で SMS 送信を促進し、1 回限りのメッセージと繰り返しメッセージの両方を送信できます。同じワークフロー内で計算されたターゲットに SMS を送信するプロセスを自動化します。 チャネルアクティビティをワークフローキャンバスに組み合わせて、顧客の行動とデータに基づいてアクションをトリガーにするクロスチャネルワークフローを作成できます。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_push_ios"
>title="iOS アクティビティをプッシュ"
>abstract="「iOS をプッシュ」アクティビティでは、ワークフローの一部として iOS プッシュ通知を送信するプロセスを効率化します。1 回限りのメッセージと繰り返しメッセージの両方を配信でき、同じワークフロー内の定義済みターゲットにiOSのプッシュ通知を自動的に送信できます。 チャネルアクティビティをワークフローキャンバスに組み合わせて、顧客の行動とデータに基づいてアクションをトリガーにするクロスチャネルワークフローを作成できます。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_push_android"
>title="Android アクティビティをプッシュ"
>abstract="「Android をプッシュ」アクティビティでは、ワークフローの一部として Android プッシュ通知を送信するプロセスを効率化します。1 回限りのメッセージと繰り返しメッセージの両方を配信でき、同じワークフロー内の定義済みターゲットにAndroidのプッシュ通知を自動的に送信できます。 チャネルアクティビティをワークフローキャンバスに組み合わせて、顧客の行動とデータに基づいてアクションをトリガーにするクロスチャネルワークフローを作成できます。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_directmail"
>title="ダイレクトメールアクティビティ"
>abstract="ダイレクトメールアクティビティでは、ワークフロー内でダイレクトメール送信を促進し、1 回限りのメッセージと繰り返しメッセージの両方を送信できます。ダイレクトメールプロバイダーに必要な抽出ファイルの生成プロセスを自動化します。 チャネルアクティビティをワークフローキャンバスに組み合わせて、顧客の行動とデータに基づいてアクションをトリガーにするクロスチャネルワークフローを作成できます。"

ワークフローのコンテキストで配信を設定するには、次の手順に従います。

1. チャネルアクティビティ（**[!UICONTROL メール]**、**[!UICONTROL SMS]**、**[!UICONTROL プッシュ通知（Android）]**、**[!UICONTROL プッシュ通知（iOS）]** または **[!UICONTROL ダイレクトメール]** を追加します。

1. 「**配信のタイプ**」（単一または繰り返し）を選択します。

   * **単一配信** は、ブラックフライデーのメールなど、1 回だけ送信されるワンショット配信です。
   * **繰り返し配信**&#x200B;は、「[スケジューラーアクティビティ](scheduler.md)」で定義した実行頻度に基づいて複数回送信されます。ワークフローが実行されるたびに、オーディエンスが再計算され、更新されたコンテンツを含む配信が更新されたオーディエンスに送信されます。 週刊ニュースレターや誕生日の定期的な誕生日メールなどがあります。

1. 配信&#x200B;**テンプレート**&#x200B;を選択します。テンプレートは、チャネルに固有の事前設定済み配信設定です。 組み込みテンプレートはチャネルごとに使用でき、デフォルトでは事前入力されます。 [詳細情報](../../msg/delivery-template.md)

   ![ ワークフロー内の配信アクティビティを示すスクリーンショット ](../assets/delivery-activity-in-wf.png)

   チャネルアクティビティ設定の左側のペインからテンプレートを選択します。 以前に選択したオーディエンスがチャネルに対応していない場合は、テンプレートを選択できません。 これを解決するには、**オーディエンスを作成**&#x200B;アクティビティを更新して、ターゲットマッピングが正しいオーディエンスを選択します。ターゲットマッピングについて詳しくは、[この節](../../audience/targeting-dimensions.md)を参照してください。

1. 「**配信を作成**」をクリックします。スタンドアロン配信の作成時と同様に、メッセージの設定とコンテンツを定義します。コンテンツをテストしシミュレートします。 [詳細情報](../../msg/gs-messages.md)

1. ワークフローに戻ります。ワークフローを続行するには、「**アウトバウンドトランジションを生成**」オプションを切り替えて、チャネルアクティビティの後にトランジションを追加します。

1. 「**開始**」をクリックして、ワークフローを開始します。

   デフォルトでは、ワークフローを開始すると、メッセージはすぐに送信されずに、メッセージの準備ステージにトリガーが送られます。

1. チャネルアクティビティを開き、「**確認して送信**」ボタンから送信を確定します。

1. 配信ダッシュボードで、「**送信**」をクリックします。

## 例 {#cross-channel-workflow-sample}

セグメント化と 2 つの配信を含むクロスチャネルワークフローの例を次に示します。 このワークフローは、パリに在住し、コーヒーマシンに興味があるすべての顧客をターゲットにします。 この母集団の中で、通常の顧客にはメールが送信され、VIP クライアントには SMS が送信されます。

![ クロスチャネルワークフローの例を示すスクリーンショット ](../assets/workflow-channel-example.png)

また、繰り返しワークフローを作成して、毎月初日の午後 8 時にパーソナライズされた SMS をパリ在住のすべてのお客様に送信することもできます。

![ 繰り返しワークフローの例を示すスクリーンショット ](../assets/workflow-channel-example2.png)

<!--
description, which use case you can perform (common other activities that you can link before or after the activity)

how to add and configure the activity

example of a configured activity within a workflow
The Email delivery activity allows you to configure the sending of an email in a workflow. 
-->

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.
Email recipients are defined upstream of the activity in the same workflow, via an Audience targeting activity.

-->

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->