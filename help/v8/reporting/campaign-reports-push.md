---
audience: end-user
title: プッシュチャネルのキャンペーンレポート
description: プッシュチャネルのキャンペーンレポートについて
exl-id: 5e7ac2b8-b543-427b-846c-7c0b489cc21c
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: ht
source-wordcount: '533'
ht-degree: 100%

---

# プッシュチャネルのキャンペーンレポート {#campaign-reports-push-channel}

各キャンペーンレポートは、キャンペーンの成功とエラーの詳細を表示する様々なウィジェットに分かれています。プッシュチャネルのレポートと指標について、以下で詳しく説明します。キャンペーンレポートにアクセスする方法について詳しくは、[このページ](campaign-reports.md)を参照してください。

## 配信の概要 {#delivery-summary-push}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_deliveries_overview"
>title="配信の概要"
>abstract="**配信の概要**&#x200B;レポートは、プッシュ通知配信に対する訪問者のエンゲージメントの詳細を示す主要業績評価指標（KPI）を提供します。"

**[!UICONTROL 配信の概要]**&#x200B;レポートは、プッシュ通知配信に対する訪問者のエンゲージメントの詳細を示す主要業績評価指標（KPI）を提供します。指標について詳しくは、以下で説明します。

![配信の概要レポートに表示される配信の概要指標](assets/campaign-reporting-push-summary.png){zoomable="yes"}

+++プッシュキャンペーンレポート指標の詳細情報

* **[!UICONTROL 配信メッセージ数]**：配信の準備中に処理されたメッセージの合計数。

* **[!UICONTROL 配信済み数]**：送信されたメッセージの合計数に対する、正常に送信されたメッセージの数。

* **[!UICONTROL エラー数]**：配信および自動返信処理中に送信されたメッセージの合計数に対する累積したエラーの合計数。

* **[!UICONTROL 合計クリック数]**：配信で少なくとも 1 回クリックしたユニーク受信者の合計数。

+++

### 初期ターゲットオーディエンス統計 {#delivery-summary-push-initial-target}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_target"
>title="初期ターゲットオーディエンス統計"
>abstract="**初期ターゲットオーディエンス統計**&#x200B;テーブルには、受信者に関連するデータが表示されます。"

**[!UICONTROL 初期ターゲットオーディエンス統計]**&#x200B;テーブルには、受信者に関連するデータが表示されます。指標について詳しくは、以下で説明します。

![レポートに表示される初期ターゲットオーディエンス統計](assets/campaign-reporting-push-target.png){zoomable="yes"}

+++プッシュキャンペーンレポート指標の詳細情報

* **[!UICONTROL 初期オーディエンス]**：ターゲット受信者の合計数。

* **[!UICONTROL 配信メッセージ数]**：配信準備の後に配信されるメッセージの合計数。

* **[!UICONTROL ルールにより却下]**：アドレスが不明、強制隔離された、ブロックリストに登録されているなど、ルールを適用する際や分析中に無視されたアドレスの合計数。

+++

### 実行統計 {#delivery-summary-push-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_exec_stats"
>title="実行統計"
>abstract="**実行統計**&#x200B;テーブルには、配信するメッセージ、成功、エラーおよび新しい強制隔離など、配信の成功の詳細が表示されます。"

**[!UICONTROL 実行統計]**&#x200B;テーブルには、配信の成功の詳細が表示されます。指標について詳しくは、以下で説明します。

![レポートに表示される実行統計](assets/campaign-reporting-push-exec.png){zoomable="yes"}

+++プッシュキャンペーンレポート指標の詳細情報

* **[!UICONTROL 配信メッセージ数]**：配信準備の後に配信されるメッセージの合計数。

* **[!UICONTROL 成功数]**：配信されるメッセージ数に対する、正常に処理されたメッセージ数。

* **[!UICONTROL エラー数]**：配信と自動リバウンド処理中に配信されたメッセージの数に対する累積したエラーの合計数。

* **[!UICONTROL 新しい強制隔離数]**：配信の失敗後（無効な登録、メッセージ却下、ペイロードエラーなど）、配信されるメッセージ数に関して強制隔離されたアドレスの合計数。

  プッシュ通知のエラータイプについて詳しくは、[Adobe Campaign v8 （クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=ja#push-error-types){target="_blank"}を参照してください。

+++

### クリックストリーム {#delivery-summary-push-click-streams}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_click_streams"
>title="クリックストリーム"
>abstract="**クリックストリーム**&#x200B;テーブルには、受信者による配信の操作に関する入手可能なデータが表示されます。"

**[!UICONTROL クリックストリーム]**&#x200B;テーブルには、受信者による配信の操作に関するデータが表示されます。指標について詳しくは、以下で説明します。

![レポートに表示された生成クリックストリーム](assets/campaign-reporting-push-clicks.png){zoomable="yes"}

+++プッシュキャンペーンレポート指標の詳細情報

* **[!UICONTROL ユニーククリック数]**：配信で少なくとも 1 回クリックしたユニーク受信者の合計数。

* **[!UICONTROL 合計クリック数]**：配信におけるリンクの合計クリック数。

* **[!UICONTROL 反応度]**：配信を開封したと推定されるターゲット受信者数に対する、配信をクリックしたターゲット受信者数の割合。

+++