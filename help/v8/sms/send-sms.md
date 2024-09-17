---
audience: end-user
title: SMS 配信の送信
description: Adobe Campaign Web で SMS を送信する方法を学ぶ
exl-id: 901faf3b-fcdd-4a4e-8de7-7d088686250f
source-git-commit: 81fa26e44739d70218b949712a41a3d520900fa0
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# SMS 配信のプレビューと送信 {#send-sms-delivery}

>[!CONTEXTUALHELP]
>id="acw_deliveries_metrics_newquarantines"
>title="新しい強制隔離指標"
>abstract="配信の失敗後（不明なユーザー、無効なドメイン）、配信されるメッセージ数に関して強制隔離されたアドレスの合計数。"

## SMS 配信のプレビュー{#preview-sms}

メッセージコンテンツを定義したら、テストプロファイルを使用してプレビューとテストを行うことができます。パーソナライズされたコンテンツを挿入してある場合は、そのコンテンツがメッセージにどのように表示されるかを、テストプロファイルデータを利用して確認できます。これにより、メッセージが意図したとおりに表示され、パーソナライズされた情報が正しく表示されるようになります。

SMS 配信をプレビューする主な手順は次のとおりです。配信のプレビュー方法の詳細については、[この節](../preview-test/preview-content.md)を参照してください。

1. 配信コンテンツページから、「**[!UICONTROL コンテンツをシミュレート]**」を使用して、パーソナライズされたコンテンツをプレビューします。

   ![](assets/sms_send_1.png){zoomable="yes"}

1. 「**[!UICONTROL テストプロファイルを追加]**」をクリックして、1 つ以上のテストプロファイルを選択します。

   <!--
    Once your test profiles are selected, click **[!UICONTROL Select]**.
    ![](assets/sms_send_2.png){zoomable="yes"}
    -->

1. 右側のパネルには SMS 配信のプレビューが表示され、パーソナライズされた要素が選択したプロファイルのデータに動的に置き換えられます。

   ![](assets/sms_send_3.png){zoomable="yes"}

これで、SMS メッセージを確認してオーディエンスに送信できるようになりました。

## SMS 配信のテスト {#test-sms}

**Adobe Campaign** を使用すると、メインオーディエンスに送信する前にメッセージをテストできます。これは、メールキャンペーンを検証し、潜在的な問題を特定する際に重要な手順です。

本配信前確認の送信は、配信の品質と有効性を保証するための重要な手順です。本配信前確認の受信者は、リンク、オプトアウトリンク、画像などの様々な要素を確認し、レンダリング、コンテンツ、パーソナライゼーション設定、SMS 設定のエラーを特定できます。このプロセスは、メインオーディエンスに到達する前に SMS を徹底的に評価して最適化するのに役立ちます。

![](../assets/do-not-localize/book.png)本配信前確認の送信方法については、[この節](../preview-test/test-deliveries.md)を参照してください。

![](assets/sms_send_6.png){zoomable="yes"}

## SMS 配信の送信 {#send-sms}

1. SMS コンテンツをパーソナライズした後、**[!UICONTROL 配信]**&#x200B;ページで「**[!UICONTROL 確認して送信]**」をクリックします。

   ![](assets/sms_send_4.png){zoomable="yes"}

1. 「**[!UICONTROL 準備]**」をクリックし、表示される進行状況と統計を監視します。

   エラーが発生した場合は、ログメニューでエラーに関する詳細情報を参照してください。

1. 「**[!UICONTROL 送信]**」をクリックしてメッセージを送信し、最終的な送信プロセスに進みます。

   ![](assets/sms_send_5.png){zoomable="yes"}

   SMS 配信がスケジュールされている場合は、「**[!UICONTROL スケジュールどおりに送信]**」ボタンをクリックします。配信スケジュールについて詳しくは、[この節](../msg/gs-messages.md#schedule-the-delivery-sending)を参照してください。


1. 「**[!UICONTROL 送信]**」ボタンをクリックして、送信アクションを確定します。

配信が送信されると、配信ページから KPI（主要業績評価指標）データをトラックし、**[!UICONTROL ログ]**&#x200B;メニューからデータをトラックできます。

これで、組み込みレポートを使用して、メッセージの影響の測定を開始できます。[詳細情報](../reporting/sms-report.md)
