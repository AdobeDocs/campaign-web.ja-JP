---
audience: end-user
title: ダイレクトメールレポート
description: ダイレクトメールレポートへのアクセス方法と使用方法について説明します。
exl-id: 268fe1e3-bd5c-40f1-8973-7671cd8c9960
source-git-commit: 1a2ab055822bea4cd55230fb63b59234aa114ff7
workflow-type: tm+mt
source-wordcount: '696'
ht-degree: 94%

---

# 外部配信レポート {#direct-mail-report}

**外部配信レポート** では、外部配信に固有の包括的なインサイトとデータが提供されます。 個々の配信のパフォーマンス、有効性、結果に関する詳細情報が含まれ、完全な概要が得られます。

ダイレクトメールのコンテキストでは、次のレポートについて説明します。 また、コールセンターやカスタム外部チャネルでも使用できます。

## 配信の概要 {#delivery-summary-direct-mail}

### 配信の概要 {#delivery-overview-direct-mail}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_overview_direct_mail"
>title="配信の概要"
>abstract="**配信の概要**&#x200B;には、各ダイレクトメール配信における訪問者のインタラクションに関する詳細なインサイトを提供する主要業績評価指標（KPI）が表示されます。指標の概要を以下に示します。"

**[!UICONTROL 配信の概要]**&#x200B;では、各ダイレクトメール配信での訪問者のインタラクションに関する詳細なインサイトが提供され、重要な主要業績評価指標（KPI）が表示されます。指標の概要を以下に示します。

![ダイレクトメール配信の主要業績評価指標を示す配信の概要指標グラフ。](assets/direct-overview.png){zoomable="yes"}{align="center"}

+++配信の概要指標の詳細情報

* **[!UICONTROL 配信メッセージ数]**：配信の準備中に処理されたメッセージの合計数。
* **[!UICONTROL ターゲット]**：ダイレクトメールメッセージのターゲットプロファイルとして選定されるユーザープロファイルの数。
* **[!UICONTROL 除外]**：ターゲットプロファイルから除外され、ダイレクトメールメッセージを受信しないユーザープロファイルの数。
+++

### 初期ターゲット母集団 {#direct-mail-delivery-targeted-population}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_initial_target_direct_mail"
>title="初期ターゲット母集団"
>abstract="**初期ターゲット母集団**&#x200B;グラフには、配信準備の結果に基づいて、受信者とメッセージに関するデータが表示されます。"

**[!UICONTROL 初期ターゲット母集団]**&#x200B;グラフには、受信者に関するデータが表示されます。指標は配信の準備中に計算され、初期オーディエンス、送信メッセージ数、除外された受信者の数が含まれます。

![オーディエンスサイズ、送信メッセージ数および除外数を示す初期ターゲット母集団グラフ。](assets/direct-mail-delivery-targeted-population.png){zoomable="yes"}

グラフの一部にマウスを合わせると、正確な数が表示されます。

![マウス機能を使用した初期ターゲット母集団グラフの詳細ビュー。](assets/direct-mail-delivery-targeted-population_2.png){zoomable="yes"}

+++ダイレクトメール配信レポート指標の詳細情報

* **[!UICONTROL 初期オーディエンス数]**：ターゲット受信者の合計数。
* **[!UICONTROL 配信]**：配信準備の後に配信されるメッセージの合計数。
* **[!UICONTROL 除外]**：ターゲット母集団から除外された受信者の合計数。
+++

### 配信統計 {#direct-mail-delivery-stats}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_summary_direct_mail"
>title="配信統計"
>abstract="**配信統計**&#x200B;グラフには、ダイレクトメール配信の成功と発生したエラーの詳細が表示されます。"

**[!UICONTROL 配信統計]**&#x200B;グラフは、配信パフォーマンスの概要と、成功度と有効性を測定するための詳細な指標を提供します。

![成功率、エラー、強制隔離を示す配信統計グラフ](assets/direct-mail-delivery-stats.png){zoomable="yes"}

+++ダイレクトメールキャンペーンレポート指標の詳細情報

* **[!UICONTROL 送信済みメッセージ]**：配信準備完了後に配信されるメッセージの合計数。
* **[!UICONTROL 成功数]**：配信するメッセージ数と比較した、正常に処理されたメッセージ数。
* **[!UICONTROL エラー数]**：配信と自動リバウンド処理の間に、配信されるメッセージ数と比較した、累積したエラーの合計数。
* **[!UICONTROL 新しい強制隔離数]**：配信の失敗後（例：不明なユーザー、無効なドメイン）、配信されるメッセージ数と比較した、強制隔離されたアドレスの合計数。
+++

### 除外の理由 {#direct-mail-delivery-exclusions}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_causes_exclusion_direct_mail"
>title="配信の除外の理由"
>abstract="**除外の理由**&#x200B;グラフには、配信の準備中に却下されたメッセージの配分がルールごとに分類されて表示されます。"

**[!UICONTROL 除外の理由]**&#x200B;グラフには、配信準備中にメッセージが却下された理由の分類が表示されます。この分類は、様々なルールにもとづいて整理されており、メッセージの除外要因を詳細に把握できます。除外ルールについて詳しくは、[Campaign v8（コンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=ja#email-error-types){_blank}を参照してください。

![却下されたメッセージのルール別の割合を示す除外の理由グラフ](assets/direct-mail-delivery-exclusions.png){zoomable="yes"}{align="center" zoomable="yes"}

+++除外の理由指標の詳細情報

* **[!UICONTROL 強制隔離中のアドレス]**：アドレスが強制隔離された場合に生成されるエラータイプ。
* **[!UICONTROL アドレスが未指定]**：アドレスが存在しない場合に生成されるエラータイプ。
* **[!UICONTROL 低品質のアドレス]**：郵送先住所の品質評価が低すぎる場合に生成されるエラータイプ。
* **[!UICONTROL ブロックリスト登録済みアドレス]**：配信中に受信者がブロックリストに登録されていた場合に生成されるエラータイプ。
* **[!UICONTROL 重複]**：キー値が一意でないことにより、受信者が除外された場合に生成されるエラータイプ。
* **[!UICONTROL コントロール母集団]**：受信者のアドレスはコントロール母集団に含まれています。
* **[!UICONTROL サイズが制限されたターゲット]**：受信者に対する最大配信サイズに達しました。
+++

### 除外 {#direct-mail-exclusions}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_exclusions_direct_mail"
>title="除外"
>abstract="**[!UICONTROL 除外]**&#x200B;テーブルには、配信準備プロセス中に却下されたメッセージの詳細な分類がルール別に表示されます。"

**[!UICONTROL 除外]**&#x200B;テーブルには、配信の準備中に却下されたメッセージを特定のルールで分類した詳細を提供します。この分類により、メッセージ除外の背後にある理由を明確に理解できます。

![却下されたメッセージの詳細な分類をルール別に示す除外テーブル。](assets/direct-mail-exclusions.png){zoomable="yes"}{align="center" zoomable="yes"}

使用可能な指標は、上記の[除外の理由](#direct-mail-delivery-exclusions)の指標と同じです。