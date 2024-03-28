---
audience: end-user
title: ダイレクトメールレポート
description: ダイレクトメールレポートにアクセスして使用する方法を説明します
exl-id: 268fe1e3-bd5c-40f1-8973-7671cd8c9960
source-git-commit: 5cedffdc504ef82cbd3a262beb80d3c55f2831ab
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 51%

---

# ダイレクトメール配信レポート {#direct-mail-report}

The **ダイレクトメール配信レポート** は、ダイレクトメール配信に固有の包括的なインサイトとデータを提供します。 個々の配信のパフォーマンス、有効性、結果に関する詳細情報が提供され、包括的な概要が得られます。

## 配信の概要 {#delivery-summary-direct-mail}

### 配信の概要 {#delivery-overview-direct-mail}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_overview_direct_mail"
>title="配信の概要"
>abstract="**配信の概要**&#x200B;には、各ダイレクトメール配信と訪問者のインタラクションに関する詳細なインサイトを提供する主要業績評価指標（KPI）が表示されます。指標の概要を以下に示します。"

The **[!UICONTROL 配信の概要]** では、訪問者が各ダイレクトメール配信とどのようにやり取りするかに関する詳細なインサイトを提供し、重要な主要業績評価指標 (KPI) を示します。  指標の概要を以下に示します。

![](assets/direct-overview.png){zoomable=&quot;yes&quot;}{align="center"}

+++配信の概要指標の詳細情報

* **[!UICONTROL 配信メッセージ数]**：配信の準備中に処理されたメッセージの合計数。

* **[!UICONTROL ターゲット]**：ダイレクトメールメッセージのターゲットプロファイルとして認定されるユーザープロファイルの数。

* **[!UICONTROL 除外する]**：ターゲットプロファイルから除外され、ダイレクトメールメッセージを受信しないユーザープロファイルの数。
+++

### 初期ターゲット母集団 {#direct-mail-delivery-targeted-population}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_initial_target_direct_mail"
>title="初期ターゲット母集団"
>abstract="**初期ターゲット母集団**&#x200B;グラフには、配信準備の結果に基づいて、受信者とメッセージに関するデータが表示されます。"

**[!UICONTROL 初期ターゲット母集団]**&#x200B;グラフには、受信者に関するデータが表示されます。指標は配信の準備中に計算され、初期オーディエンス、送信するメッセージの数、除外された受信者の数を示します。

![](assets/direct-mail-delivery-targeted-population.png){zoomable=&quot;yes&quot;}

グラフの一部にマウスを合わせると、正確な数が表示されます。

![](assets/direct-mail-delivery-targeted-population_2.png){zoomable=&quot;yes&quot;}

+++ダイレクトメール配信レポート指標の詳細を説明します。

* **[!UICONTROL 初期オーディエンス]**：ターゲット受信者の合計数。

* **[!UICONTROL 配信]**：配信準備の後に配信されるメッセージの合計数。

* **[!UICONTROL 除外]**：ターゲット母集団から除外された受信者の合計数。
+++

### 配信統計 {#direct-mail-delivery-stats}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_summary_direct_mail"
>title="配信統計"
>abstract="**配信統計**&#x200B;グラフには、ダイレクトメール配信の成功と発生したエラーの詳細が表示されます。"

The **[!UICONTROL 配信統計]** グラフは、配信パフォーマンスの包括的な概要と、成功度と効果度を測定するための詳細な指標を提供します。

![](assets/direct-mail-delivery-stats.png){zoomable=&quot;yes&quot;}

+++ダイレクトメールキャンペーンレポート指標の詳細を説明します。

* **[!UICONTROL 送信済みメッセージ]**：配信準備の後に配信されるメッセージの合計数。

* **[!UICONTROL 成功]**：配信されるメッセージ数に関して正常に処理されたメッセージ数。

* **[!UICONTROL エラー]**：配信と自動リバウンド処理の間に、配信されるメッセージ数に関して累積したエラーの合計数。

* **[!UICONTROL 新しい強制隔離]**：配信されるメッセージ数に関して、配信の失敗後（不明なユーザー、無効なドメイン）に強制隔離されたアドレスの合計数。

+++

### 除外の理由 {#direct-mail-delivery-exclusions}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_causes_exclusion_direct_mail"
>title="配信の除外の理由"
>abstract="**除外の理由**&#x200B;グラフには、配信の準備中に却下されたメッセージの配分がルールごとに分類されて表示されます。"

The **[!UICONTROL 除外の理由]** グラフでは、配信の準備中に却下されたメッセージの理由の詳細な分類が表示されます。 この分類は、様々なルールに従って整理され、メッセージの除外に貢献する要因を包括的に把握できます。 除外ルールについて詳しくは、 [Campaign v8（コンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=ja#email-error-types){_blank}を参照してください。

![](assets/direct-mail-delivery-exclusions.png){zoomable=&quot;yes&quot;}{align="center" zoomable="yes"}

+++除外指標の原因について詳しく説明します。

* **[!UICONTROL 強制隔離中のアドレス]**：アドレスが強制隔離に置かれたときに生成されるエラータイプ。

* **[!UICONTROL アドレスが指定されていません]**：アドレスが存在しないことを示すエラータイプで、配信の送信中に生成される。

* **[!UICONTROL 低品質のアドレス]**：郵送先住所の品質評価が低すぎる場合に生成されるエラータイプ。

* **[!UICONTROL ブロックリストに加える住所]**：配信の実行時に受信者が送信されブロックリストに加えるた際に生成されるエラータイプ。

* **[!UICONTROL ダブル]**：受信者のキー値が一意でなかったので、受信者を除外した際に生成されたエラータイプ。

* **[!UICONTROL コントロール母集団]**：受信者のアドレスはコントロール母集団に含まれています。

* **[!UICONTROL サイズが制限されたターゲット]**：受信者に対する最大配信サイズに達しました。

+++

### 除外 {#direct-mail-exclusions}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_exclusions_direct_mail"
>title="除外"
>abstract="**[!UICONTROL 除外]**&#x200B;テーブルには、配信準備プロセス中に却下されたメッセージの詳細な分類がルールごとに表示されます。"

The **[!UICONTROL 除外]** この表は、配信の準備段階で拒否されたメッセージの詳細な分類を特定のルール別に分類したものです。 この包括的な分類により、配信プロセスからこれらのメッセージが除外される理由を明確に把握できます。

![](assets/direct-mail-exclusions.png){zoomable=&quot;yes&quot;}{align="center" zoomable="yes"}

使用可能な指標は、 [除外の理由](#direct-mail-delivery-exclusions) 上記の説明。
