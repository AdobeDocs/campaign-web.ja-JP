---
audience: end-user
title: プッシュ配信レポート
description: プッシュ配信レポートへのアクセス方法と使用方法を学ぶ
exl-id: 4187b553-8de7-40f4-8f30-f62e43323862
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 73%

---

# プッシュ配信レポート {#push-report}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_sending_push"
>title="送信のレポート"
>abstract="レポート内の「**送信**」タブでは、訪問者の配信とのやり取りや、訪問者が遭遇した可能性のある潜在的なエラーに関する詳細なインサイトを提供します。"

**プッシュ配信レポート**&#x200B;は、プッシュチャネルの完全な概要を提供し、広範なインサイトと特定のデータを提供します。各配信のパフォーマンス、有効性、結果に関する包括的な情報を提供します。

## プッシュの概要 {#push-summary}

### 配信の概要 {#push-delivery-overview}

>[!CONTEXTUALHELP]
>id="acw_push_report_overview"
>title="プッシュ配信の概要"
>abstract="**プッシュ配信の概要**&#x200B;は、広範なインサイトと特定のデータを提供する、プッシュ配信の包括的な概要を示します。配信のパフォーマンス、効果、結果に関する包括的な情報を確認できます。"

**[!UICONTROL 配信の概要]**&#x200B;レポートは、プッシュメッセージに対する訪問者のエンゲージメントの詳細を示す主要業績評価指標（KPI）を提供します。

![ このスクリーンショットは、プッシュメッセージに対する訪問者のエンゲージメントに関する KPI を提供する、配信の概要レポートを示します。](assets/reporting_push_3.png){zoomable="yes"}

+++プッシュ配信レポート指標の詳細情報。

* **[!UICONTROL 合計送信数]**：配信の準備中に処理されたメッセージの合計数。
* **[!UICONTROL 配信済み数]**：送信されたメッセージの合計数に対して、正常に送信できたメッセージの数。
* **[!UICONTROL クリック数]**：プッシュメッセージの操作を行った受信者の合計数。
* **[!UICONTROL エラー]**：配信中に発生し、プロファイルに送信できなかったエラーの合計数。

+++

### ターゲット母集団 {#push-delivery-targeted-population}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_push_targeted_population"
>title="プッシュのターゲット母集団"
>abstract="**ターゲット母集団**&#x200B;グラフおよびテーブルには、プッシュメッセージングオーディエンスに関連するデータ（配信メッセージ数と除外件数）が表示されます。"

**ターゲット母集団**&#x200B;グラフおよびテーブルには、オーディエンスに関連するデータ（配信メッセージ数と除外件数）が表示されます。指標については、以下で詳しく説明します。

![ このスクリーンショットは、配信するメッセージと除外に関するデータを表示するターゲット母集団グラフとテーブルを示しています。](assets/reporting_push_4.png){zoomable="yes"}

+++プッシュ配信レポート指標の詳細情報。

* **[!UICONTROL 配信]**：配信の準備中に処理されたメッセージの合計数。
* **[!UICONTROL 除外]**：分析から除外されたプロファイルの数。

+++

### 全体的な統計 {#push-delivery-overall}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_push_overall_stats"
>title="プッシュの全体的な統計"
>abstract="**全体的な統計**&#x200B;レポートには、送信されたプッシュ通知のデータ（成功、エラーおよび強制隔離）が表示されます。"

**全般的な統計** レポートには、送信されたプッシュ通知に関するデータ（成功、エラー、強制隔離）が表示されます。 指標については、以下で詳しく説明します。

![ このスクリーンショットは、全体的な統計レポートを示しています。ここには、送信されたプッシュ通知の成功、エラーおよび強制隔離に関するデータが表示されます。](assets/reporting_push_5.png){zoomable="yes"}

+++プッシュ配信レポート指標の詳細情報。

* **[!UICONTROL 成功]**：正常に処理されたメッセージ数。
* **[!UICONTROL エラー]**：配信中に発生し、特定のプロファイルにメッセージを送信できなかったエラーの合計数。
* **[!UICONTROL 新しい強制隔離]**：除外され、強制隔離に追加されたプロファイルの数。

+++

### 除外 {#push-delivery-exclusions}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_push_exclusions"
>title="プッシュの除外"
>abstract="**除外**&#x200B;グラフおよびテーブルには、ターゲットプロファイルから除外されたユーザープロファイルがメッセージを受信できなかった様々な理由が表示されます。"

**[!UICONTROL 除外]**&#x200B;グラフおよびテーブルには、ターゲットプロファイルから除外されたユーザープロファイルがメッセージを受信できなかった様々な理由が表示されます。除外ルールについて詳しくは、[Campaign v8（コンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=ja#push-error-types){_blank}を参照してください。

![ このスクリーンショットは、除外されたユーザープロファイルがメッセージを受信できない理由を示す、除外のグラフとテーブルを示しています。](assets/reporting_push_6.png){zoomable="yes"}

## 配信スループット {#delivery-throughput}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_throughput_push"
>title="配信スループットレポート"
>abstract="配信スループットレポートには、指定した期間内のプラットフォーム全体の配信スループットに関する詳細情報が表示されます。"

**配信スループット**&#x200B;レポートには、指定された期間内のプラットフォーム全体の配信スループットに関する詳細情報が表示されます。メッセージ配信速度の測定に使用される主な指標は、1 時間あたりに送信されるメッセージの数です。

![ このスクリーンショットは、配信スループットレポートを表示します。このレポートには、指定した期間内のプラットフォームのメッセージ配信速度に関する詳細が示されます。](assets/reporting_push_2.png){zoomable="yes"}