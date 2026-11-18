---
audience: end-user
title: グローバルレポートの基本を学ぶ
description: グローバルレポートについて
exl-id: e64d9765-f602-4fee-9923-a3665130c63a
TQID: 'https://experienceleague.adobe.com/UG5Dn-gdKdU1PfOUmCtoVzAjuYRG4pUPwGggZq2diiQ'
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: 62a8e2ac2a726b568e3c25b4e435d4de2f305b5f
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 62%
---
# グローバルレポートの基本を学ぶ {#global-report-gs}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_global_report"
>title="グローバルレポート"
>abstract="グローバルレポートは、キャンペーンのパフォーマンスを分析する強力で効率的な方法を提供します。 これらのレポートは、キャンペーン内の各チャネルの主なトラフィックとエンゲージメント指標の統合ビューを提供します。"

「**グローバルレポート**」は効果的なツールとして機能し、Campaign インスタンス内の各チャネルのトラフィックとエンゲージメント指標の統合された全体的な概要を提供します。 これらのレポートは様々なウィジェットで構成され、それぞれがキャンペーンや配信パフォーマンスに関する明確な観点を提供します。

主要業績評価指標（KPI）は、最新のインサイトが得られるよう、1 時間ごとに更新されます。 デフォルトでは、過去 30 日間を対象にデータがフィルタリングされ、キャンペーンと配信パフォーマンスに関する最新かつ関連性の高い観点を提供します。

各チャネルのレポートと関連指標の完全なリストについては、下記のページを参照してください。

* [メールグローバルレポート](global-report-email.md)
* [SMS グローバルレポート](global-report-sms.md)
* [プッシュグローバルレポート](global-report-push.md)
* [ダイレクトメールグローバルレポート](global-report-direct.md)

## レポートダッシュボードの管理 {#manage-reports}

グローバルレポートにアクセスして管理するには、次の手順に従います。

1. 「**[!UICONTROL レポート]**」セクション内の&#x200B;**[!UICONTROL レポート]**&#x200B;メニューに移動します。

1. 左側のメニューで、リストからレポートを選択し、タブ間を移動して各チャネルからのデータを表示します。

   ![各チャネルからデータを移動するための左側のメニューとタブを示すスクリーンショット](assets/global_report_manage_3.png){zoomable="yes"}

1. ダッシュボードから、**開始時間**&#x200B;と&#x200B;**[!UICONTROL 終了時間]**&#x200B;を選択して、特定のデータをターゲットにします。

   ![データターゲティングの開始時刻と終了時刻を選択するオプションを含むダッシュボードを示すスクリーンショット](assets/global_report_manage_1.png){zoomable="yes"}

1. 「**[!UICONTROL フォルダーを選択]**」フィールドで、特定のフォルダーから配信またはキャンペーンをターゲットにするかどうかを選択します。

   ![ 配信またはキャンペーンを選択するための「フォルダーを選択」フィールドを示すスクリーンショット](assets/global_report_manage_2.png){zoomable="yes"}

1. 「**[!UICONTROL ルールを追加]**」をクリックしてクエリの作成を開始し、レポートデータをより適切にフィルタリングします。 [詳しくは、クエリモデラーの使用方法を参照してください](../query/query-modeler-overview.md)。

1. **[!UICONTROL URL とクリックストリーム]**&#x200B;から、**[!UICONTROL 上位訪問リンク]**&#x200B;または&#x200B;**[!UICONTROL 期間]**&#x200B;を選択します。

   「**[!UICONTROL 表示条件]**」オプションを使用すると、URL、ラベルまたはカテゴリでフィルタリングできます。

## LINE チャネルのレポート {#line-reports}

LINE チャネルで使用可能なレポートは以下のとおりです。

### 配信の概要 {#line-delivery-overview}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_line_deliveries_overview"
>title="LINE配信の概要"
>abstract="LINEの配信メッセージ、配信メッセージ、配信エラーを表示します。"

**[!UICONTROL 配信の概要]** レポートには、配信するメッセージ、配信されたメッセージ、およびLINEの配信エラーが表示されます。

### ターゲットオーディエンス {#line-targeted-audience}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_line_targeted_audience"
>title="LINE ターゲットオーディエンス"
>abstract="LINE配信がターゲットとするオーディエンスと、その配信結果を表示します。"

**[!UICONTROL ターゲットオーディエンス]**&#x200B;のグラフとテーブルには、LINE配信によってターゲティングされたオーディエンスと、その結果の配信結果が表示されます。

### 配信統計 {#line-delivery-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_line_delivery_stats"
>title="LINE配信の統計"
>abstract="配信メッセージ、配信メッセージ、配信エラーなど、LINE メッセージの主要な配信結果を表示します。"

**[!UICONTROL 配信統計]**&#x200B;のグラフとテーブルには、配信メッセージ、配信メッセージ、配信エラーなど、LINE メッセージの主要な配信結果が表示されます。

### 除外の理由 {#line-exclusions}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_line_exclusions"
>title="LINEの除外の原因"
>abstract="対象プロファイルがLINE配信から除外された理由（適格性、検証、設定ルールなど）を表示します。"

除外の原因&#x200B;**[!UICONTROL グラフとテーブルには、ターゲットプロファイルがLINE配信から除外された理由（適格性、検証、設定ルールなど）が表示されます。]**

### 配信スループット {#line-delivery-throughput}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_line"
>title="LINE配信スループット"
>abstract="LINE メッセージの送信率を経時的に表示します。"

**[!UICONTROL 配信スループット]** レポートには、LINE メッセージの送信率が時間の経過とともに表示されます。
