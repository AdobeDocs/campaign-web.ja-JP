---
audience: end-user
title: プッシュ通知ワークフローアクティビティを使用
description: プッシュ通知ワークフローアクティビティの使用方法を学ぶ
badge: label="アルファ版"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 100%

---


# プッシュ通知 {#push-activity}

**プッシュ通知**&#x200B;配信アクティビティでは、ワークフローでプッシュ通知の送信を設定できます。

>[!BEGINTABS]

>[!TAB プッシュ通知（Android）]

1. 新しいワークフローを作成して設定した後、オーディエンスを作成アクティビティを追加して既存のオーディエンスを選択するか、ルールビルダーを使用して独自のクエリを定義します。

1. プッシュ通知（Android）チャネルアクティビティをワークフローに追加します。

<!--
1. Select the Type of delivery:

    * Single delivery: Choose this option if you want the push notification to be sent only once. You have the flexibility to choose whether or not to include an outbound transition from this activity.

    * Recurring delivery: Choose this option if you want the push notification to be sent multiple times based on a defined frequency. The frequency can be configured using a Scheduler activity, allowing you to schedule the push notification to be sent at regular intervals.
-->

1. アクティビティを選択します。 配信メニューから、この配信に使用するテンプレートを選択します。テンプレートの詳細情報

1. 「配信を作成」をクリックして、プッシュ通知配信を設定します。プッシュ通知（Android）配信について詳しくは、このページを参照してください。

1. 配信の送信準備が整ったら、ワークフローに戻り、「開始」をクリックしてワークフローを起動します。

1. デフォルトでは、配信ワークフローを開始すると、メッセージはすぐに送信されずに、メッセージの準備ステージに移動します。

   プッシュ通知（Android）チャネルアクティビティの詳細設定メニューで「確認して送信」をクリックし、送信を確定します。

1. プッシュ通知配信ダッシュボードで、「送信」をクリックします。

>[!TAB プッシュ通知 (iOS)]

1. 新しいワークフローを作成して設定した後、オーディエンスを作成アクティビティを追加して既存のオーディエンスを選択するか、ルールビルダーを使用して独自のクエリを定義します。

1. プッシュ通知（iOS）チャネルアクティビティをワークフローに追加します。

<!--
1. Select the Type of delivery:

    * Single delivery: Choose this option if you want the push notification to be sent only once. You have the flexibility to choose whether or not to include an outbound transition from this activity.

    * Recurring delivery: Choose this option if you want the push notification to be sent multiple times based on a defined frequency. The frequency can be configured using a Scheduler activity, allowing you to schedule the push notification to be sent at regular intervals.
-->

1. アクティビティを選択します。 配信メニューから、この配信に使用するテンプレートを選択します。テンプレートの詳細情報

1. 「配信を作成」をクリックして、プッシュ通知配信を設定します。プッシュ通知（iOS）配信について詳しくは、このページを参照してください。

1. 配信の送信準備が整ったら、ワークフローに戻り、「開始」をクリックしてワークフローを起動します。

1. デフォルトでは、配信ワークフローを開始すると、メッセージはすぐに送信されずに、メッセージの準備ステージに移動します。

   プッシュ通知（iOS）チャネルアクティビティの詳細設定メニューで「確認して送信」をクリックし、送信を確定します。

1. プッシュ通知配信ダッシュボードで、「送信」をクリックします。

>[!ENDTABS]