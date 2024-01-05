---
audience: end-user
title: プッシュチャネルのグローバルレポート
description: プッシュチャネルのグローバルレポートについて
badge: label="限定提供（LA）"
source-git-commit: ac9a7918045e7ff02ef27c348b28a6ce09802caf
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 44%

---

# プッシュチャネルのグローバルレポート {#campaign-reports-push}

グローバルレポートでは、トラフィック指標とエンゲージメント指標の包括的な概要をチャネルレベルでユーザーに提供します。

次に移動： **[!UICONTROL レポート]** メニュー内 **[!UICONTROL レポート]** 」セクションに入力します。 レポートの日付、フォルダーまたはルールに応じて、データをフィルタリングできます。 [詳細情報](global-reports.md)

## 配信の概要 {#delivery-summary-push}

### 配信の概要 {#delivery-overview-push}

The **[!UICONTROL 配信の概要]** レポートは、プッシュ通知配信ごとに訪問者がどのように関与しているかに関する詳細な情報を提供する主要業績評価指標 (KPI) を提供します。 指標については、以下で詳しく説明します。

![](assets/global_report_push_delivery_overview.png)

+++配信の概要指標について詳しく説明します。

* **[!UICONTROL 配信メッセージ数]**：配信の準備中に処理されたメッセージの合計数。

* **[!UICONTROL 配信済み数]**：送信されたメッセージの合計数に対して、正常に送信できたメッセージの数。

* **[!UICONTROL 合計クリック数]**：配信で少なくとも 1 回クリックしたユニーク受信者の合計数。

* **[!UICONTROL エラー数]**：配信と自動返信処理の間に、送信されたメッセージの合計数に関して累積したエラーの合計数。

+++

### 対象オーディエンス {#delivery-summary-push-initial-target}

The **[!UICONTROL ターゲットオーディエンス]** 送信されたプッシュ通知配信ごとに、受信者に関する表とグラフに関する提示データを示します。 指標については、以下で詳しく説明します。

![](assets/global_report_push_targeted_audience.png)

+++ターゲットオーディエンス指標の詳細を説明します。

* **[!UICONTROL ターゲットオーディエンス]**：ターゲット受信者の合計数。

* **[!UICONTROL 配信メッセージ数]**：配信準備の後に配信されるメッセージの合計数。

* **[!UICONTROL 除外]**：ルール（アドレスが見つからない、強制隔離された、上など）を適用する際、分析中に無視されたアドブロックリストに加えるレスの合計数。

+++

### 配信統計 {#delivery-summary-push-exec-stats}

The **[!UICONTROL 配信統計]** 表には、各プッシュ通知配信の成功の詳細が示されます。 指標については、以下で詳しく説明します。

![](assets/global_report_push_delivery_statistics.png)

+++配信統計指標の詳細を説明します。

* **[!UICONTROL 合計メッセージ数]**：配信の準備後に配信されるメッセージの合計数。

* **[!UICONTROL 成功]**：配信されるメッセージ数に関して正常に処理されたメッセージ数。

* **[!UICONTROL エラー/バウンス]**：配信するメッセージ数に関して、配信と自動リバウンド処理の間に累積したエラーの合計数。

* **[!UICONTROL 新しい強制隔離]**：配信の失敗（無効な登録、メッセージ却下、ペイロードエラーなど）の後で強制隔離されたアドレスの合計数（割合は、配信されるメッセージの数に対する比率です）。

  プッシュ通知のエラータイプについては、[Adobe Campaign v8 （クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=ja#push-error-types){target="_blank"}を参照してください。

+++

### 除外の理由 {#causes-exclusion}

The **[!UICONTROL 除外の理由]** グラフおよびテーブルには、ターゲットプロファイルから除外されたユーザープロファイルがメッセージを受信できなかった理由が表示されます。

プッシュ通知のエラータイプについては、[Adobe Campaign v8 （クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=ja#push-error-types){target="_blank"}を参照してください。

## 配信スループット {#delivery-throughput-sms}

![](assets/global_report_push_delivery_throughput.png)

このレポートは、指定した期間内の配信スループットに関する包括的な詳細を提供します。

