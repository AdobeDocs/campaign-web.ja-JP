---
audience: end-user
title: ダイレクトメールチャネルのグローバルレポート
description: ダイレクトメールチャネルのグローバルレポートについての詳細情報
exl-id: a42536fe-375b-4169-8775-d47ed26692f8
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 59%

---

# ダイレクトメールチャネルのグローバルレポート {#global-report-direct}

ダイレクトメールのグローバルレポートでは、トラフィックおよびエンゲージメント指標の包括的な概要をチャネルレベルでユーザーに提供します。

**[!UICONTROL レポート]**&#x200B;セクション内の「**[!UICONTROL レポート]**」メニューに移動します。レポートの日付、フォルダー、ルールに応じて、データをフィルタリングできます。 [詳細情報](global-reports.md)

## 配信の概要 {#delivery-summary-direct}

### 配信の概要 {#delivery-overview-direct}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_delivery_overview_direct_mail"
>title="配信の概要"
>abstract="**配信の概要**&#x200B;には、各ダイレクトメール配信における訪問者のインタラクションに関する詳細なインサイトを提供する主要業績評価指標（KPI）が表示されます。指標の概要を以下に示します。"

**[!UICONTROL 配信の概要]** では、主要業績評価指標（KPI）を紹介し、各ダイレクトメール配信での訪問者のインタラクションに関する詳細なインサイトを提供します。 指標の概要を以下に示します。

![ この画像は、ダイレクトメール配信の配信の概要指標を示しています。](assets/global_report_direct_mail_delivery_overview.png){zoomable="yes"}{align="center"}

+++配信の概要指標の詳細を説明します。

* **[!UICONTROL 配信メッセージ数]**：配信の準備中に処理されたメッセージの合計数。

* **[!UICONTROL 配信済み数]**：送信されたメッセージの合計数に対して、正常に送信できたメッセージの数。

* **[!UICONTROL エラー]**：配信と自動返信処理の間に、送信されたメッセージの合計数に関して蓄積されたエラーの合計数。

* **[!UICONTROL 購読解除]**：購読解除リンクをクリックした受信者の数。

+++

### 対象オーディエンス {#delivery-summary-direct-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_target_audience_direct_mail_graph"
>title="対象オーディエンス"
>abstract="受信者のデータとメッセージ情報は、配信準備の分析を反映して、**対象オーディエンス**&#x200B;グラフに表示されます。"

>[!CONTEXTUALHELP]
>id="acw_global_reporting_target_audience_direct_mail_table"
>title="対象オーディエンス"
>abstract="**対象オーディエンス**&#x200B;テーブルには、配信準備プロセスの結果に基づいて、受信者と対応するメッセージの詳細な分類が表示されます。"

**[!UICONTROL ターゲットオーディエンス]**&#x200B;のテーブルおよびグラフには、受信者に関連するデータが表示され、下に詳細な指標が示されます。

![ この画像は、ダイレクトメール配信のターゲットオーディエンス指標を示しています。](assets/global_report_direct_mail_targeted_audience.png){zoomable="yes"}{align="center"}

+++ターゲットオーディエンス指標の詳細情報。

* **[!UICONTROL ターゲットオーディエンス]**：ターゲット受信者の合計数。

* **[!UICONTROL 配信メッセージ数]**：配信準備の後に配信されるメッセージの合計数。

* **[!UICONTROL 除外]**：アドレスが不明、強制隔離された、ブロックリスト上にあるなどのルールを適用する際、分析中に無視されたアドレスの合計数。

+++

### 配信統計 {#delivery-summary-direct-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_delivery_statistics_summary_direct_mail_graph"
>title="配信統計"
>abstract="**配信統計**&#x200B;グラフには、成功した配信や発生したエラーなど、ダイレクトメール配信の有効性に関するインサイトが表示されます。"

>[!CONTEXTUALHELP]
>id="acw_global_reporting_delivery_statistics_summary_direct_mail_table"
>title="配信統計"
>abstract="**配信統計**&#x200B;テーブルには、ダイレクトメール配信の成功と発生したエラーの詳細が表示されます。"

**[!UICONTROL 配信統計]**&#x200B;グラフおよびテーブルには、すべてのダイレクトメール配信の成功の分類と、以下に概要を示す詳細な指標が表示されます。

+++配信統計指標の詳細を説明します。

* **[!UICONTROL 配信メッセージ数]**：配信準備の後に配信されるメッセージの合計数。

* **[!UICONTROL 成功]**：配信されるメッセージ数に関して、正常に処理されたメッセージ数。

* **[!UICONTROL エラー/バウンス]**：配信と自動リバウンド処理の間に、配信されるメッセージ数に関して蓄積されたエラーの合計数。

* **[!UICONTROL 新しい強制隔離]**：配信の失敗後（不明なユーザー、無効なドメインなど）、配信されるメッセージ数に関して強制隔離されたアドレスの合計数。

+++

### 除外の理由 {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_exclusions_direct_mail_table"
>title="除外"
>abstract="**除外の理由**&#x200B;テーブルには、配信準備プロセス中に却下されたメッセージの詳細な分類がルールごとに表示されます。"

>[!CONTEXTUALHELP]
>id="acw_global_reporting_causes_exclusion_direct_mail_graph"
>title="除外の理由"
>abstract="**除外の理由**&#x200B;グラフには、配信の準備中に却下されたメッセージの配分がルールごとに分類されて表示されます。"

![ この画像は、ダイレクトメール配信の除外指標の原因を示しています。](assets/global_report_direct_mail_exclusions.png){zoomable="yes"}{align="center"}

除外グラフおよびテーブルには、ターゲットプロファイルから除外されたユーザープロファイルがメッセージを受信できなかった理由が表示されます。

+++除外指標の原因の詳細はこちら。

* **[!UICONTROL 強制隔離中のアドレス]**：アドレスが強制隔離される際に生成されるエラータイプ。

* **[!UICONTROL アドレスが未指定]**：配信の送信時に生成され、アドレスが存在しないことを示すエラータイプ。

* **[!UICONTROL 品質の悪い住所]**：郵送先住所の品質評価が低すぎる場合に生成されるエラータイプ。

* **[!UICONTROL ブロックリスト登録済みアドレス]**：配信実行時に受信者がブロックリストに登録されていた場合に生成されるエラータイプ。

* **[!UICONTROL Double]**：キー値が一意でなかったので受信者が除外された場合に生成されるエラータイプ。

* **[!UICONTROL コントロール母集団]**：受信者のアドレスはコントロール母集団に含まれています。

* **[!UICONTROL サイズが制限されたターゲット]**：受信者に対する最大配信サイズに達しました。

+++