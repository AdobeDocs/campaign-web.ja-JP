---
audience: end-user
title: ダイレクトメールチャネルのグローバルレポート
description: ダイレクトメールチャネルのグローバルレポートの詳細を説明します
badge: label="限定提供（LA）"
source-git-commit: a6d42e0abb64f87aecb2912cb469ba269aa02515
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 45%

---

# ダイレクトメールチャネルのグローバルレポート {#global-report-direct}

グローバルレポートでは、トラフィック指標とエンゲージメント指標の包括的な概要をチャネルレベルでユーザーに提供します。

次に移動： **[!UICONTROL レポート]** メニュー内 **[!UICONTROL レポート]** 」セクションに入力します。 レポートの日付、フォルダーまたはルールに応じて、データをフィルタリングできます。 [詳細情報](global-reports.md)

## 配信の概要 {#delivery-summary-direct}

### 配信の概要 {#delivery-overview-direct}

The **[!UICONTROL 配信の概要]** は、訪問者と各 E メール配信とのインタラクションに関する深いインサイトを提供する主要業績評価指標 (KPI) を示します。 指標の概要を以下に示します。

![](assets/global_report_email_delivery_overview.png){align="center"}

+++配信の概要指標について詳しく説明します。

* **[!UICONTROL 配信メッセージ数]**：配信の準備中に処理されたメッセージの合計数。

* **[!UICONTROL 配信済み数]**：送信されたメッセージの合計数に対して、正常に送信できたメッセージの数。

* **[!UICONTROL エラー数]**：配信と自動返信処理の間に、送信されたメッセージの合計数に関して累積したエラーの合計数。

* **[!UICONTROL 配信停止]**：購読解除をクリックした受信者の数。
+++

### 対象オーディエンス {#delivery-summary-direct-initial-target}

のテーブルとグラフ **[!UICONTROL ターゲットオーディエンス]** 以下に示す詳細な指標を使用して、受信者に関連するデータを紹介します。

![](assets/global_report_email_targeted_audience.png){align="center"}

+++ターゲットオーディエンス指標の詳細を説明します。

* **[!UICONTROL ターゲットオーディエンス]**：ターゲット受信者の合計数。

* **[!UICONTROL 配信メッセージ数]**：配信準備の後に配信されるメッセージの合計数。

* **[!UICONTROL 除外]**：ルール（アドレスが見つからない、強制隔離された、上など）を適用する際、分析中に無視されたアドブロックリストに加えるレスの合計数。

+++

### 配信統計 {#delivery-summary-direct-exec-stats}

The **[!UICONTROL 配信統計]** この表は、すべてのダイレクトメール配信の成功の分類と、以下に説明する詳細な指標を示しています。

![](assets/global_report_email_delivery_statistics.png){align="center"}

+++配信統計指標の詳細を説明します。

* **[!UICONTROL 配信メッセージ数]**：配信準備の後に配信されるメッセージの合計数。

* **[!UICONTROL 成功]**：配信されるメッセージ数に関して正常に処理されたメッセージ数。

* **[!UICONTROL エラー/バウンス]**：配信するメッセージ数に関して、配信と自動リバウンド処理の間に累積したエラーの合計数。

* **[!UICONTROL 新しい強制隔離]**：配信の失敗後（不明なユーザー、無効なドメイン）に、配信されるメッセージ数に関して強制隔離されたアドレスの合計数。

+++

### 除外の理由 {#causes-exclusion}

![](assets/global_report_email_exclusions.png){align="center"}

除外のグラフと表に、ターゲットプロファイルから除外されたユーザープロファイルがメッセージを受信できなかった理由を示します。

## 配信スループット {#delivery-throughput}

このレポートは、指定した期間内の配信スループットに関する包括的な詳細を提供します。 メッセージ配信の速度の測定に使用される主な指標は、1 時間あたりに送信されたメッセージの数です。

## 配信不能件数 {#non-deliverables-direct}

### タイプ別のエラー分類 {#delivery-summary-direct-breakdown-per-type}

The **[!UICONTROL タイプごとのエラーの分類]** 表とグラフに、様々なドメインで発生する可能性のあるエラーに関するデータと、以下に示す具体的な指標を示します。

このレポートに表示されるエラーにより、強制隔離プロセスが実行されることになります。強制隔離の管理について詳しくは、[Campaign v8（クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html?lang=ja){target="_blank"}を参照してください。

+++タイプ指標ごとのエラーの分類の詳細を説明します。

* **[!UICONTROL 不明なユーザー]**：アドレスが無効であることを示すエラータイプで、配信中に生成される。

* **[!UICONTROL 無効なドメイン]**：アドレスが正しくないか存在しないことを示すエラータイプで、配信の送信中に生成される。

* **[!UICONTROL メールボックス容量超過]**：受信者の受信ボックスにあるメッセージの数が多すぎることを示すエラータイプで、5 回の配信の試行後に生成される。

* **[!UICONTROL 無効なアカウント]**：アドレスが存在しないことを示すエラータイプ。配信の送信中に生成される。

* **[!UICONTROL 拒否]**：アドレスが IAP（インターネットアクセスプロバイダー）によって却下される場合に生成されるエラータイプ。例えば、セキュリティルールのアプリケーション（スパム対策ソフトウェア）によって却下された場合に生成される。

* **[!UICONTROL 未到達]**：SMTP リレーでのインシデント、ドメインへの一時的な未到達など、メッセージ配分文字列で発生するエラータイプ。

* **[!UICONTROL 未接続]**：受信者の携帯電話の電源が入っていない、または送信時にネットワーク接続が切断されていることを示すエラータイプ。

+++

### ドメイン別のエラー分類 {#delivery-summary-email-breakdown-per-domain}

The **[!UICONTROL ドメインごとのエラーの分類]** 表およびグラフでは、各ドメイン内の潜在的なエラーに関連するデータを確認できます。 指標は、上記の&#x200B;**[!UICONTROL タイプ別のエラー分類]**&#x200B;テーブルとグラフと共通です。

