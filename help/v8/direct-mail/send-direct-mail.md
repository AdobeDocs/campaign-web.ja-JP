---
audience: end-user
title: ダイレクトメール配信のプレビューと送信
description: Adobe Campaign Web を使用したダイレクトメール配信のプレビューと送信の方法について説明します
source-git-commit: 717f6f2fb5e07213fb6a16f7ed701f450d1e257e
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 18%

---


# ダイレクトメール配信のプレビューと送信 {#send-direct-mail}

ダイレクトメール配信用に抽出ファイルを設定したら、テストプロファイルを利用してプレビューできます。 パーソナライズされたコンテンツが含まれている場合は、テストプロファイルデータを使用して、このコンテンツが列にどのように表示されるかを調べることができます。 これにより、ファイルコンテンツが正しくレンダリングされ、パーソナライズされた要素が適切に組み込まれていることを確認できます。

抽出ファイルの準備が整ったら、ダイレクトメール配信を送信して、ファイルを生成し、ダイレクトメールプロバイダーと共有できます。 [ダイレクトメール配信の送信方法を説明します](#dm-send)

## 抽出ファイルのプレビュー {#preview-dm}

抽出ファイルをプレビューする主な手順は次のとおりです。 配信のプレビュー方法の詳細については、[この節](../preview-test/preview-content.md)を参照してください。

1. 配信コンテンツページから、「**[!UICONTROL コンテンツをシミュレート]**」を使用して、パーソナライズされたコンテンツをプレビューします。

   ![](assets/dm-simulate.png){zoomable=&quot;yes&quot;}

1. クリック **[!UICONTROL テストプロファイルを追加]** :1 つまたは複数のプロファイルを選択し、抽出ファイルコンテンツ内のデータをプレビューします。

1. 右側のウィンドウには抽出ファイルのプレビューが表示され、パーソナライズされた要素が、選択したプロファイルのデータで動的に置き換えられます。

   ![](assets/dm-preview-right.png){zoomable=&quot;yes&quot;}

## 本配信前確認の送信 {#test-dm}

**Adobe Campaign** を使用すると、メインオーディエンスに送信する前に本配信前確認を送信できます。この手順は、配信を検証し、問題を特定する際に重要です。 テスト受信者は、パーソナライゼーション設定などの要素を確認し、最適なパフォーマンスを確保し、エラーを検出できます。 このプロセスにより、メインオーディエンスに到達する前に抽出ファイルを調整し、最適化することができます。

ダイレクトメール配信の場合、配達確認の送信により、選択したテストプロファイルのデータを使用して、抽出ファイルのサンプルが生成されます。 アクセスするには、次の手順に従います。

1. コンテンツをシミュレート画面で、 **[!UICONTROL 配達確認を送信]** ボタンをクリックし、任意のタイプの配信と同じ手順で配達確認を送信します。 [本配信前確認の送信方法を学ぶ](../preview-test/test-deliveries.md)

1. 配達確認が送信されたら、次の場所からアクセスできます： **[!UICONTROL 配達確認を表示]** 」ボタンをクリックするか、配信リストから選択します。 [送信済みの配達確認にアクセスする方法を説明します](../preview-test/test-deliveries.md#access-test-deliveries)

1. 配達確認配信ダッシュボードで、 **[!UICONTROL ファイルをプレビュー]** ボタンをクリックして、抽出ファイルのプレビューにアクセスします。

   ![](assets/dm-proof.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >プレビューファイルには、最初の 100 行のみが表示されます。

## ダイレクトメール配信を送信 {#send-dm}

ダイレクトメールを顧客に送信する準備が整ったら、配信を送信して、指定した抽出ファイルでのデータ抽出を開始できます。 これを行うには、次の手順に従います。

1. 抽出ファイルのコンテンツをデザインしたら、「 **[!UICONTROL レビューと送信]** から **[!UICONTROL 配信]** ページに貼り付けます。

   ![](assets/dm-review-send.png){zoomable=&quot;yes&quot;}

1. 「**[!UICONTROL 準備]**」をクリックし、表示される進行状況と統計を監視します。

   エラーが発生した場合は、 **[!UICONTROL ログ]** メニューを参照してください。

   ![](assets/dm-prepare.png){zoomable=&quot;yes&quot;}

1. 「**[!UICONTROL 送信]**」をクリックしてメッセージを送信し、最終的な送信プロセスに進みます。

1. 「**[!UICONTROL 送信]**」ボタンをクリックして、送信アクションを確定します。

   ダイレクトメール配信がスケジュールされている場合は、 **[!UICONTROL 予定どおりに送信]** 」ボタンをクリックします。 配信スケジュールについて詳しくは、[この節](../msg/gs-messages.md#schedule-the-delivery-sending)を参照してください。

配信が送信されると、抽出ファイルが自動的に生成され、 **[!UICONTROL Routing]** 配信テンプレートの [詳細設定](../advanced-settings/delivery-settings.md).

KPI（主要業績評価指標）データを配信ページから、また **[!UICONTROL ログ]** メニュー。

また、組み込みレポートを使用して、メッセージの影響の測定を開始できます。 [詳細情報](../reporting/direct-mail.md)