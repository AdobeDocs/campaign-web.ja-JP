---
audience: end-user
title: プッシュ通知配信を送信
description: Adobe Campaign Web でプッシュ通知配信を送信する方法を学ぶ
exl-id: 16b3b33b-36db-4635-8e44-707694b859db
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 82%

---

# プッシュ配信のプレビューと送信 {#send-push-delivery}

## プッシュ通知配信をプレビュー {#preview-push}

メッセージのコンテンツを定義したら、テストサブスクライバーを利用して、メッセージをプレビューしテストできます。パーソナライズされたコンテンツを挿入してある場合は、そのコンテンツがメッセージにどのように表示されるかを、テストプロファイルデータを利用して確認できます。ここで、メッセージが正しくレンダリングされ、パーソナライズされた要素が適切に組み込まれていることを確認できます。

プッシュ通知をプレビューする主な手順は次のとおりです。配信のプレビュー方法の詳細については、[この節](../preview-test/preview-content.md)を参照してください。

1. 配信コンテンツページから、「**[!UICONTROL コンテンツをシミュレート]**」を使用して、パーソナライズされたコンテンツをプレビューします。

   ![](assets/push_send_1.png){zoomable=&quot;yes&quot;}

1. 「**[!UICONTROL サブスクライバーを追加]**」をクリックし、1 つまたは複数のプロファイルを選択して、プッシュ通知コンテンツ内のデータをプレビューします。


   <!--Once your test subscribers are selected, click **[!UICONTROL Select]**.
    ![](assets/push_send_5.png){zoomable="yes"}-->

1. 右側のパネルにはプッシュ通知のプレビューが表示され、パーソナライズされた要素が選択したプロファイルのデータに動的に置き換えられます。

   ![](assets/push_send_7.png){zoomable=&quot;yes&quot;}

これで、プッシュ通知を確認してオーディエンスに送信できるようになりました。

## プッシュ通知配信をテスト {#test-push}

使用 **Adobe Campaign**&#x200B;に値を入力すると、配達確認を送信してからメインオーディエンスに送信することができます。 この手順は、配信を検証し、問題を特定する際に重要です。

テストプロファイルは、配達確認の受信者です。 リンク、画像、パーソナライゼーションなどのコンポーネントや設定を確認および検証でき、最適なパフォーマンスを確保し、エラーを検出できます。 このプロセスは、メインオーディエンスにリーチする前にプッシュ通知を調整し、最適化するのに役立ちます。 [配達確認の送信方法を学ぶ](../preview-test/test-deliveries.md#subscribers)

![](assets/push_send_6.png){zoomable=&quot;yes&quot;}

## プッシュ通知配信を送信 {#send-push}

1. プッシュ通知コンテンツをパーソナライズした後、**[!UICONTROL 配信]**&#x200B;ページから「**[!UICONTROL 確認して送信]**」をクリックします。

   ![](assets/push_send_2.png){zoomable=&quot;yes&quot;}

1. 「**[!UICONTROL 準備]**」をクリックし、表示される進行状況と統計を監視します。

   エラーが発生した場合は、ログメニューでエラーに関する詳細情報を参照してください。

   ![](assets/push_send_3.png){zoomable=&quot;yes&quot;}

1. 「**[!UICONTROL 送信]**」をクリックしてメッセージを送信し、最終的な送信プロセスに進みます。

1. 「**[!UICONTROL 送信]**」ボタンをクリックして、送信アクションを確定します。

   プッシュ配信がスケジュールされている場合は、「**[!UICONTROL スケジュールどおりに送信]**」ボタンをクリックします。配信について詳しくは、[この節](../msg/gs-messages.md#schedule-the-delivery-sending)を参照してください。

   ![](assets/push_send_4.png){zoomable=&quot;yes&quot;}

配信が送信されると、配信ページから KPI（主要業績評価指標）データをトラックし、**[!UICONTROL ログ]**&#x200B;メニューからデータをトラックできます。

これで、組み込みレポートを使用して、メッセージの影響の測定を開始できます。[詳細情報](../reporting/push-report.md)
