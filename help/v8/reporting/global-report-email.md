---
audience: end-user
title: E メールチャネルのグローバルレポート
description: E メールチャネルのグローバルレポートの詳細を説明します
badge: label="限定提供（LA）"
source-git-commit: c5b4e1d44977b43324e85a7b5e173ef3154a620d
workflow-type: tm+mt
source-wordcount: '1594'
ht-degree: 52%

---

# E メールチャネルのグローバルレポート {#global-report-direct}

グローバルレポートでは、トラフィック指標とエンゲージメント指標の包括的な概要をチャネルレベルでユーザーに提供します。

次に移動： **[!UICONTROL レポート]** メニュー内 **[!UICONTROL レポート]** 」セクションに入力します。 レポートの日付、フォルダーまたはルールに応じて、データをフィルタリングできます。 [詳細情報](global-reports.md)

## 配信の概要 {#delivery-summary-email}

### 配信の概要 {#delivery-overview-email}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_deliveries_overview_email"
>title="配信の概要"
>abstract="The **配信の概要** オーディエンスと送信する E メール配信およびキャンペーンとの関わり方に関する深いインサイトを提供する主要業績評価指標 (KPI) を表示します。"

The **[!UICONTROL 配信の概要]** は、訪問者と各 E メール配信とのインタラクションに関する深いインサイトを提供する主要業績評価指標 (KPI) を示します。 指標の概要を以下に示します。

![](assets/global_report_email_delivery_overview.png){align="center"}

+++配信の概要指標について詳しく説明します。

* **[!UICONTROL 配信メッセージ数]**：配信の準備中に処理されたメッセージの合計数。

* **[!UICONTROL 配信済み数]**：送信されたメッセージの合計数に対して、正常に送信できたメッセージの数。

* **[!UICONTROL 合計開封数]**：メッセージを 1 回以上開封したターゲット受信者の合計数。

* **[!UICONTROL 合計クリック数]**：配信で少なくとも 1 回クリックした受信者の合計数。

* **[!UICONTROL バウンスとエラー]**：送信されたメッセージの合計数に関する、配信および自動返信処理の間に累積したエラーの合計。

* **[!UICONTROL 配信停止]**：購読解除をクリックした受信者の数。
+++

### 対象オーディエンス {#delivery-summary-email-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_target_audience_email"
>title="初期ターゲットオーディエンス統計"
>abstract="The **ターゲットオーディエンス** 表とグラフに、受信者のエンゲージメントに関するインサイトを示し、キャンペーンと配信の有効性を評価するのに役立ちます。"

のテーブルとグラフ **[!UICONTROL ターゲットオーディエンス]** 以下に示す詳細な指標を使用して、受信者に関連するデータを紹介します。

![](assets/global_report_email_targeted_audience.png){align="center"}

+++ターゲットオーディエンス指標の詳細を説明します。

* **[!UICONTROL ターゲットオーディエンス]**：ターゲット受信者の合計数。

* **[!UICONTROL 配信メッセージ数]**：配信準備の後に配信されるメッセージの合計数。

* **[!UICONTROL 除外]**：ルール（アドレスが見つからない、強制隔離された、上など）を適用する際、分析中に無視されたアドブロックリストに加えるレスの合計数。

+++

### 配信統計 {#delivery-summary-email-delivery-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_email_delivery_stats"
>title="配信統計"
>abstract="The **配信統計** グラフおよびテーブルでは、配信の成功、エラー、新しい強制隔離など、主要指標の概要を説明し、配信パフォーマンスを評価するための簡潔な概要を提供します。"

The **[!UICONTROL 配信統計]** この表は、各 E メール配信の成功の分類と、以下に示す詳細な指標を示しています。

![](assets/global_report_email_delivery_statistics.png){align="center"}

+++配信統計指標の詳細を説明します。

* **[!UICONTROL 配信メッセージ数]**：配信準備の後に配信されるメッセージの合計数。

* **[!UICONTROL 成功]**：配信されるメッセージ数に関して正常に処理されたメッセージ数。

* **[!UICONTROL エラー/バウンス]**：配信するメッセージ数に関して、配信と自動リバウンド処理の間に累積したエラーの合計数。

* **[!UICONTROL 新しい強制隔離]**：配信の失敗後（不明なユーザー、無効なドメイン）に、配信されるメッセージ数に関して強制隔離されたアドレスの合計数。

+++

### 除外の理由 {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_exclusion_email"
>title="除外の理由"
>abstract="The **除外の理由** グラフと表に、配信の準備中にメッセージが却下される具体的な理由を示し、ルール別の詳細な分類を示します。"

![](assets/global_report_email_exclusions.png){align="center"}

除外のグラフと表に、ターゲットプロファイルから除外されたユーザープロファイルがメッセージを受信できなかった理由を示します。

メールのエラータイプは、[Adobe Campaign v8 （クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=ja#email-error-types){target="_blank"}に記載されています。

## 配信スループット {#delivery-throughput}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_email"
>title="配信スループット"
>abstract="この **配信スループット** 配信スループットに関する包括的なインサイトを提供し、指定した期間内の成功率とエラー率を強調します。"

![](assets/global_report_email_delivery_throughput.png){align="center"}

配信スループットレポートは、配信プロセスの効率性に関する詳細なインサイトを提供し、指定期間内の成功率とエラー率の詳細な概要を示します。

+++配信スループット指標の詳細を説明します。

* **[!UICONTROL 成功]**：配信されるメッセージ数に関して正常に処理されたメッセージ数。

* **[!UICONTROL エラー]**：配信と自動リバウンド処理の間に、配信されるメッセージ数に関して累積したエラーの合計数。

+++

## 配信不能件数 {#non-deliverables-email}

### タイプ別のエラー分類 {#delivery-summary-email-breakdown-per-type}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_error_type_email"
>title="タイプ別のエラー分類"
>abstract="の詳細を示すテーブルとグラフ **タイプごとのエラーの分類** プロセス中に発生した様々なエラータイプ（不明なユーザー、メールボックス容量超過、無効なドメインなど）に関する情報を含みます。"

![](assets/global_report_email_breakdown_type.png){align="center"}

The **[!UICONTROL タイプごとのエラーの分類]** 表とグラフに、様々なドメインで発生する可能性のあるエラーに関するデータと、以下に示す具体的な指標を示します。

このレポートに表示されるエラーにより、強制隔離プロセスが実行されることになります。強制隔離の管理について詳しくは、[Campaign v8（クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html?lang=ja){target="_blank"}を参照してください。

+++タイプ指標ごとのエラーの分類の詳細を説明します。

* **[!UICONTROL 不明なユーザー]**：メールアドレスが無効であることを示すエラータイプで、配信中に生成される。

* **[!UICONTROL 無効なドメイン]**：メールアドレスが正しくないか存在しないことを示すエラータイプ。配信の送信中に生成される。

* **[!UICONTROL メールボックス容量超過]**：受信者の受信ボックスにあるメッセージの数が多すぎることを示すエラータイプで、5 回の配信の試行後に生成される。

* **[!UICONTROL 無効なアカウント]**：アドレスが存在しないことを示すエラータイプ。配信の送信中に生成される。

* **[!UICONTROL 拒否]**：アドレスが IAP（インターネットアクセスプロバイダー）によって却下される場合に生成されるエラータイプ。例えば、セキュリティルールのアプリケーション（スパム対策ソフトウェア）によって却下された場合に生成される。

* **[!UICONTROL 未到達]**：SMTP リレーでのインシデント、ドメインへの一時的な未到達など、メッセージ配分文字列で発生するエラータイプ。

* **[!UICONTROL 未接続]**：受信者の携帯電話の電源が入っていない、または送信時にネットワーク接続が切断されていることを示すエラータイプ。

+++

### ドメイン別のエラー分類 {#delivery-summary-email-breakdown-per-domain}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_error_domain_email"
>title="ドメイン別のエラー分類"
>abstract="の表とグラフ **ドメインごとのエラーの分類** は、発生した各エラータイプに対応するデータを、特定のドメイン別に分類して表示します。"

![](assets/global_report_email_breakdown_domain.png){align="center"}

The **[!UICONTROL ドメインごとのエラーの分類]** 表およびグラフでは、各ドメイン内の潜在的なエラーに関連するデータを確認できます。 指標は、上記の&#x200B;**[!UICONTROL タイプ別のエラー分類]**&#x200B;テーブルとグラフと共通です。

## トラッキング指標 {#tracking-indicators-email}

### 配信統計 {#delivery-summary-email-statistics}

>[!CONTEXTUALHELP]
>id="acw_global_delivery_statistics_summary_email"
>title="配信統計"
>abstract="The **配信統計** 主要業績評価指標 (KPI) は、配信とキャンペーンのパフォーマンスの包括的な概要を提供し、配信の成功、発生したエラー、ユーザーエンゲージメントの両方に関するインサイトを提供します。"

The **[!UICONTROL 配信統計]** 指標には、各 E メール配信に関連付けられたデータに関する詳細情報を提供する主要業績評価指標 (KPI) が含まれます。 これらの指標の詳細については、以下で説明します。

![](assets/global_report_email_delivery_statistics_tracking.png){align="center"}

+++配信統計指標の詳細を説明します。

* **[!UICONTROL 配信メッセージ数]**：配信の準備中に処理されたメッセージの合計数。

* **[!UICONTROL 成功]**：配信されるメッセージ数に関して正常に処理されたメッセージ数。

* **[!UICONTROL ユニーク開封数]**：メッセージを 1 回以上開封したターゲット受信者の合計数。

* **[!UICONTROL 合計開封数]**：メッセージを 1 回以上開封した、このドメインのユニークターゲット受信者の数。

* **[!UICONTROL オプトアウトリンクのクリック数]**：購読解除リンクのクリック数。

* **[!UICONTROL ミラーリンクのクリック数]**：ミラーページへのリンクのクリック数。

* **[!UICONTROL 推定転送数]**：ターゲット受信者によって転送されるメール数の推定値。
+++

### 開封率およびクリックスルー率 {#delivery-summary-open-rate}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_open_clickthrough_email"
>title="開封率とクリックスルー率"
>abstract="のテーブル **開封率およびクリックスルー率** 受信者との配信のエンゲージメントを示し、開封率とクリックスルー率に関するデータを表示して、すばやく洞察に富んだ概要を示します。"

**[!UICONTROL 開封率およびクリックスルー率]**&#x200B;テーブルには、受信者に関連するデータが表示されます。指標については、以下で詳しく説明します。

![](assets/global_report_email_opens.png){align="center"}

+++開封率およびクリックスルー率指標の詳細をご覧ください。

* **[!UICONTROL 送信済み]**：送信されたメッセージの合計数。

* **[!UICONTROL 苦情件数]**：このドメインのメッセージのうち、受信者によって望ましくないとレポートされたメッセージ数と割合。

* **[!UICONTROL ユニーク開封数]**：メッセージを 1 回以上開封した、このドメインのユニークターゲット受信者の数と割合。

* **[!UICONTROL ユニーククリック数]**：同じ配信で 1 回以上クリックしたユニークターゲット受信者の数と割合。

* **[!UICONTROL 反応率（生データ）]**：配信を少なくとも 1 回開封した受信者数に対する、配信で少なくとも 1 回クリックした受信者数の割合。
+++

## URL とクリックストリーム {#url-email}

### URL とクリックストリームの KPI {#url-email-kpis}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_urls_clickstreams_email"
>title="URL とクリックストリーム"
>abstract="The **URL とクリックストリーム** レポートは、配信中に最もクリックされた URL に関する詳細なインサイトを提供する、重要な主要業績評価指標 (KPI) を提供します。"

The **[!UICONTROL URL とクリックストリーム]** レポートは、配信中に最も高いクリック数を獲得した URL に関する詳細なインサイトを提供する主要業績評価指標 (KPI) を提供します。 指標については、以下で詳しく説明します。

![](assets/campaign_report_email_9.png){align="center"}

+++ URL とクリックストリーム指標の詳細を説明します。

* **[!UICONTROL 反応度]**：配信を開封した推定ターゲット受信者数に対する、配信でクリックしたターゲット受信者数の割合。

* **[!UICONTROL ユニーククリック数]**：配信で 1 回以上クリックしたユニーク受信者の合計数。

* **[!UICONTROL 合計クリック数]**：配信におけるリンクの合計クリック数。

* **[!UICONTROL プラットフォームの平均]**：この平均率は、それぞれの率（反応度、ユニーククリック数および累積クリック数）の下に表示され、過去 6 ヶ月間に送信された配信に対して計算されます。同じタイポロジを持つ、同じチャネルでの配信のみが考慮されます。配達確認は除外されます。
+++

### 最も訪問されたリンク上位 10 件 {#top10-global-report-email}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_top10_email"
>title="最も訪問されたリンク上位 10 件"
>abstract="The **最も多く訪問された上位 10 件のリンク**  グラフとテーブルは、各リンクを使用した受信者のインタラクションに関する包括的なデータを示します。"

**[!UICONTROL 最も訪問されたリンク上位 10 件]**&#x200B;グラフおよびテーブルには、リンクごとの受信者の行動に関する入手可能なデータが表示されます。指標については、以下で詳しく説明します。

![](assets/global_report_email_top10.png){align="center"}

+++最も多く訪問されたリンク指標の上位 10 位の詳細を説明します。

* **[!UICONTROL 合計クリック数]**：配信におけるリンクの合計クリック数。

* **[!UICONTROL 割合]**：配信で操作したユーザーの割合。

+++

### 時間の経過に伴うクリック数の分類 {#global-report-email-breakdown-clicks}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_urls_click_breakdown_email"
>title="時間の経過に伴うクリック数の分類"
>abstract="The **時間の経過に伴うクリック数の分類** グラフでは、指定した期間内に受信者がリンクとどのように関わっているかを包括的に確認できます。"

**[!UICONTROL 時間の経過に伴うクリック数の分類]**&#x200B;グラフには、リンクごとの受信者の行動に関する入手可能なデータが表示されます。

![](assets/global_report_email_breakdown_clicks.png){align="center"}

## ユーザーアクティビティ {#user-activities-email}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_user_activities_email"
>title="ユーザーアクティビティ"
>abstract="のグラフィック表現 **ユーザーアクティビティ** は、有益なグラフ形式での開封数とクリック数を示した、受信者のインタラクションの詳細な分類を提供します。"

**[!UICONTROL ユーザーアクティビティ]**&#x200B;レポートには、開封数とクリック数の分類がチャート形式で表示されます。このレポートの指標については、以下で詳しく説明します。

![](assets/global_report_email_user.png){align="center"}

+++ユーザーアクティビティ指標の詳細を説明します。

* **[!UICONTROL 合計クリック数]**：配信におけるリンクの合計クリック数。

* **[!UICONTROL 合計開封数]**：メッセージを少なくとも 1 回開封した、このドメインのユニークターゲット受信者の合計数。

+++
