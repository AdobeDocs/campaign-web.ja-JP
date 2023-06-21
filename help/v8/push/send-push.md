---
audience: end-user
title: プッシュ通知配信を送信
description: Adobe Campaign Web でプッシュ通知配信を送信する方法を学ぶ
badge: label="Alpha"
source-git-commit: 4a439abca9c7b1f2cc5d82214efb0aae033a996c
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 57%

---

# プッシュ通知配信のプレビューと送信 {#send-push-delivery}

## プッシュ通知配信をプレビュー {#preview-push}

メッセージのコンテンツを定義したら、テスト購読者を利用して、メッセージをプレビューおよびテストできます。 パーソナライズされたコンテンツが含まれている場合は、テストプロファイルデータを使用して、このコンテンツがメッセージにどのように表示されるかを調べることができます。 ここで、メッセージが正しくレンダリングされ、パーソナライズされた要素が適切に組み込まれていることを確認できます。

SMS 配信をプレビューする主な手順は次のとおりです。 配信のプレビュー方法の詳細については、 [この節](../preview-test/preview-content.md).

1. 配信コンテンツページから、 **[!UICONTROL コンテンツをシミュレート]** パーソナライズされたコンテンツをプレビューする

   ![](assets/push_send_1.png)

1. クリック **[!UICONTROL 購読者を追加]** :1 つまたは複数のプロファイルを選択し、プッシュ通知コンテンツ内のデータをプレビューします。


   <!--Once your test subscribers are selected, click **[!UICONTROL Select]**.
    ![](assets/push_send_5.png)-->

1. 右側のウィンドウには、プッシュ通知のプレビューが表示されます。パーソナライズされた要素は、選択したプロファイルのデータで動的に置き換えられます。

   ![](assets/push_send_7.png)

これで、プッシュ通知を確認してオーディエンスに送信できるようになりました。

## プッシュ通知配信をテスト {#test-push}

**Adobe Campaign** を使用すると、プッシュ通知をメインオーディエンスに送信する前にテストできます。この手順は、配信を検証し、問題を特定する上で重要です。
テスト受信者は、リンク、画像、パーソナライゼーション設定などの要素を確認し、最適なパフォーマンスの確保やエラー検出を行うことができます。このプロセスは、メインオーディエンスに届ける前にプッシュ通知を調整し、最適化するのに役立ちます。

![](../assets/do-not-localize/book.png) でテストプッシュ通知を送信する方法を説明します。 [この節](../preview-test/test-deliveries.md#subscribers).

![](assets/push_send_6.png)

## プッシュ通知配信を送信 {#send-push}

1. プッシュ通知コンテンツをパーソナライズした後、**[!UICONTROL 配信]**&#x200B;ページから「**[!UICONTROL 確認して送信]**」をクリックします。

   ![](assets/push_send_2.png)

1. 「**[!UICONTROL 準備]**」をクリックし、表示される進行状況と統計を監視します。

   エラーが発生した場合は、ログメニューでエラーに関する詳細情報を参照してください。

   ![](assets/push_send_3.png)

1. 「**[!UICONTROL 送信]**」をクリックしてメッセージを送信し、最終的な送信プロセスに進みます。

1. 「**[!UICONTROL 送信]**」または「**[!UICONTROL スケジュールどおりに送信]**」ボタンをクリックして、送信アクションを確認します。

   ![](assets/push_send_4.png)

配信が送信されると、配信ページの KPI（主要業績評価指標）データと、 **[!UICONTROL ログ]** メニュー

これで、組み込みレポートを使用して、メッセージの影響の測定を開始できます。[詳細情報](../reporting/push-report.md)
