---
audience: end-user
title: インターフェイスを確認
description: Campaign v8 Web ユーザーインターフェイス
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
badge: label="ベータ版"
source-git-commit: 523a43bef4f179740a96039ac2fc5f4f858aa1dc
workflow-type: tm+mt
source-wordcount: '1430'
ht-degree: 100%

---

# インターフェイスを確認 {#user-interface}

新しい Campaign v8 web インターフェイスは、マーケティングキャンペーンのデザインと配信を簡素化する、最新の直感的なユーザーエクスペリエンスを提供します。この新しいインターフェイスは、Adobe Experience Cloud のアプリおよびソリューションと統合されています。


>[!NOTE]
>
>このドキュメントは、製品のユーザーインターフェイスに対する最新の変更を反映するために頻繁に更新されています。ただし、一部のスクリーンショットは、お使いのユーザーインターフェイスと多少異なる場合があります。


## 左側のナビゲーションメニュー {#user-interface-left-nav}

左側のリンクを参照すると、Campaign v8 web 機能にアクセスできます。いくつかのリンクを選択すると、並べ替えやフィルタリングが可能なオブジェクトのリストが表示されます。また、必要なすべての情報を表示するように列を設定することもできます。[こちら](#list-screens)を参照してください。一部のリスト画面は読み取り専用です。左側のナビゲーションメニューとリストに表示される項目は、ユーザーの権限によって異なります。権限について詳しくは、[この節](permissions.md)を参照してください。

![](assets/home.png)

### ホーム {#user-interface-home}

この画面には、主な Campaign v8 web 機能にすばやくアクセスするための主要なリンクやリソースが含まれています。

>[!CONTEXTUALHELP]
>id="acw_homepage_recent"
>title="最近使用したもの"
>abstract="**最近使用したもの**&#x200B;リストには、最近作成および変更した配信へのショートカットが一覧表示されます。このリストには、チャネル、ステータス、所有者、作成日、変更日が表示されます。"

**最近使用したもの**&#x200B;リストには、最近作成および変更した配信へのショートカットが一覧表示されます。このリストには、チャネル、ステータス、所有者、作成日、変更日が表示されます。さらに配信を読み込むには、**詳細を表示**&#x200B;リンクをクリックします。

**主要業績評価指標**&#x200B;では、一般的な KPI を通じてプラットフォームの有効性を確認できます。KPI について詳しくは、[このページ](../reporting/kpis.md)を参照してください。


ホームページの「**ラーニング**」セクションから、Campaign v8 web の主要ヘルプページにアクセスします。

### エクスプローラー {#user-interface-explorer}

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="エクスプローラー"
>abstract="**エクスプローラー**&#x200B;メニューには、クライアントコンソールのフォルダー階層と同じフォルダー階層を持つすべての Campaign コンポーネントとオブジェクトが表示されます。このメニューから、すべての Campaign v8 コンポーネント、フォルダーおよびスキーマを参照し、関連する権限を確認し、フォルダーとサブフォルダーを作成します。"

**エクスプローラー**&#x200B;メニューには、クライアントコンソールのフォルダー階層と同じフォルダー階層を持つすべての Campaign リソースとオブジェクトが表示されます。すべての Campaign v8 コンポーネント、フォルダーおよびスキーマを参照し、配信、ワークフローおよびキャンペーンを作成します。

**エクスプローラー**&#x200B;に表示される項目は、ユーザー権限によって異なります。また、適切な権限がある場合は、フォルダーやサブフォルダーを追加することもできます。権限について詳しくは、[この節](permissions.md)を参照してください。

必要な情報がすべて表示されるように、列を設定して表示をカスタマイズできます。[こちら](#list-screens)を参照してください。また、フォルダーやサブフォルダーを追加することもできます。詳しくは、[この節](permissions.md#folders)を参照してください。

Campaign エクスプローラー、フォルダー階層およびリソースについて詳しくは、この [Campaign v8（コンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/new/campaign-ui.html?lang=ja#ac-explorer-ui){target="_blank"}を参照してください。

### キャンペーン管理 {#user-interface-campaign-management}

「キャンペーン管理」セクションでは、マーケティングキャンペーン、配信およびワークフローにアクセスできます。

* **キャンペーン** - キャンペーンのリストとキャンペーンテンプレートです。デフォルトでは、各キャンペーンの開始日／終了日／作成日／最終変更日、現在のステータス、キャンペーンを作成した Campaign オペレーターの名前を表示できます。ステータス、開始日／終了日、フォルダーでリストをフィルタリングしたり、詳細フィルターを作成して独自のフィルタリング条件を定義したりできます。キャンケーンの詳細については、[この節](../campaigns/gs-campaigns.md)を参照してください。

* **配信** - 配信のリストを閲覧できます。デフォルトでは、配信の状態、最終変更日および主要 KPI を確認できます。リストは、ステータス、連絡日またはチャネルでフィルタリングできます。メール配信をクリックすると、その配信のダッシュボードが開くので、配信の詳細を大まかに確認できます。他のチャネルでの配信は読み取り専用です。配信について詳しくは、[この節](../msg/gs-messages.md)を参照してください。

  「**その他のアクション**」ボタンを使用すると、配信を削除または複製できます。

  ![](assets/more-actions.png){width="70%" align="left"}

* **ワークフロー** - この画面では、ワークフローとワークフローテンプレートの完全なリストにアクセスできます。ステータス、最後／次回の実行日を確認し、新しいワークフローまたは新しいワークフローテンプレートを作成できます。他のオブジェクトと同じ条件でリストをフィルタリングできます。さらに、キャンペーンに属するかどうかにかかわらず、ワークフローをフィルタリングできます。ワークフローについて詳しくは、[この節](../workflows/gs-workflows.md)を参照してください。


### 顧客管理 {#user-interface-customer-management}

「顧客管理」セクションでは、受信者、オーディエンスおよび購読を表示できます。これらのリストは読み取り専用です。

* **受信者** - 受信者データベースにアクセスできます。デフォルトでは、メールアドレス、名前（名）および名前（姓）が表示されます。受信者について詳しくは、[この節](../audience/about-recipients.md)を参照してください。
* **オーディエンス** - オーディエンスのリストです。デフォルトでは、オーディエンスのタイプ、接触チャネル、作成日／最終変更日およびラベルが表示されます。このリストは接触チャネルでフィルタリングできます。オーディエンスとリストについて詳しくは、[この節](../audience/about-recipients.md)を参照してください。
* **購読** - 購読リストを閲覧できます。デフォルトでは、購読リストのタイプ、モードおよびラベルが表示されます。購読と購読解除を管理する方法については、[Adobe Campaign v8（コンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/subscriptions.html?lang=ja){target="_blank"}を参照してください。

### 意思決定管理 {#decision-management}

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="オファー"
>abstract="**インタラクション**&#x200B;モジュールを使用して、コンソールで作成されたオファーとオファーテンプレートのリストを参照します。これらのリストは読み取り専用です。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/offers.html?lang=ja" text="配信へのオファーの追加"

「意思決定管理」セクションで、オファーとオファーテンプレートを表示できます。これらのリストは読み取り専用です。

* **オファー** - **インタラクション**&#x200B;モジュールを使用して、コンソールで作成されたオファーとオファーテンプレートのリストを参照します。デフォルトでは、オファーのステータス、開始日／終了日および環境が表示されます。このリストは、ステータスや開始日／終了日でフィルタリングできます。オファーテンプレートも使用できます。

メールと SMS でオファーを作成して送信する方法については、[この節](../msg/offers.md)を参照してください。



## コンテキストヘルプ {#user-interface-help}

コンテキストヘルプは、インターフェイスで利用できます。使用可能な場合は、「`?`」アイコンをクリックすると、ヘルプ情報や関連ドキュメントのリンクが表示されます。

![](assets/context-help.png){width="40%" align="left"}

新しいベータ版では、**AI を活用したナレッジアシスタント**&#x200B;がコンテキストヘルプに組み込まれており、膨大なドキュメントリポジトリを簡単に検索して、必要な正確な情報を即座に特定できるので、ドキュメントの検索と操作方法に関する質問への回答に大変革をもたらします。

Campaign 生成 AI の機能により、このアシスタントでユーザーのエクスペリエンスが変革され、情報の検索と問題解決を簡単に行うことができます。複雑なタスクでガイダンスを求めている場合でも、膨大なドキュメントから必要な情報を探している場合でも、AI を活用したアドビのナレッジアシスタントは究極のコンパニオンとなり、あらゆるインタラクションにおいて比類のない効率性と正確さを提供します。

詳しくは、[こちら](using-ai.md)を参照してください。



## 詳細情報 {#learn-more}

Campaign 環境で使用可能なリストを参照、検索、フィルタリングする方法については、[このページ](list-filters.md)を参照してください。



<!--
######## This part stores the contextualHelp definition for WebUI BETA ###########
######## These blocks should be dispatched in the appropriate pages when available ###########
######## PLEASE DO NOT DELETE ###########
REFER TO 
https://wiki.corp.adobe.com/pages/viewpage.action?spaceKey=neolane&title=v8+WebUI+Contextual+Help+%3CALPHA%3E-+Official+list
-->


>[!CONTEXTUALHELP]
>id="acw_push_permission_for_segment"
>title="権限が必要です"
>abstract="セグメントを作成するには、管理者から権限が付与されている必要があります。"

>[!CONTEXTUALHELP]
>id="acw_push_overview_edit"
>title="権限が必要です"
>abstract="セグメントを作成するには、管理者から権限が付与されている必要があります。"

<!-- Workflows-->


<!-- delivery template settings-->


>[!CONTEXTUALHELP]
>id="acw_global_reporting_sending"
>title="グローバルレポートの送信"
>abstract="トラッキングレポート指標は、この画面に表示されます"

>[!CONTEXTUALHELP]
>id="acw_global_reporting_tracking"
>title="グローバルレポートのトラッキング"
>abstract="トラッキングレポート指標は、この画面に表示されます"

>[!CONTEXTUALHELP]
>id="acw_campaign_workflow_list"
>title="キャンペーンのワークフローリスト"
>abstract="キャンペーンのワークフローリスト"

<!-- delivery settings-->






<!-- FOR BETA (alignment) -->
<!--https://wiki.corp.adobe.com/display/neolane/v8+WebUI+Contextual+Help+%3CBETA%3E-+Official+list-->




<!-- FOR GA -->
<!-- Aligned with https://wiki.corp.adobe.com/display/neolane/v8+WebUI+Contextual+Help+%3CGA%3E-+Official+list -->

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_list"
>title="受信者の作成"
>abstract="受信者の作成"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_cardoverview"
>title="受信者のカードの概要"
>abstract="受信者のカードの概要"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_touchpoints"
>title="受信者のタッチポイント"
>abstract="受信者のタッチポイント"

>[!CONTEXTUALHELP]
>id="acw_recipients_subscription_selection"
>title="受信者の購読の選択"
>abstract="受信者の購読の選択"

>[!CONTEXTUALHELP]
>id="acw_recipients_offers_eligible_list"
>title="受信者の実施要件を満たすオファーのリスト"
>abstract="受信者の実施要件を満たすオファーのリスト"

>[!CONTEXTUALHELP]
>id="acw_recipients_offers_preview_proposition"
>title="受信者のオファーのプレビュー"
>abstract="受信者のオファーのプレビュー"

>[!CONTEXTUALHELP]
>id="acw_recipients_readonlyprofile"
>title="受信者の読み取り専用プロファイル"
>abstract="受信者の読み取り専用プロファイル"

>[!CONTEXTUALHELP]
>id="acw_subscriptions_delivery_template"
>title="購読の配信テンプレート"
>abstract="購読の配信テンプレート"

>[!CONTEXTUALHELP]
>id="acw_landingpages_menu"
>title="ランディングページ"
>abstract="ランディングページ"

>[!CONTEXTUALHELP]
>id="acw_landingpages_properties"
>title="ランディングページのプロパティ"
>abstract="ランディングページのプロパティ"

>[!CONTEXTUALHELP]
>id="acw_landingpages_pages_list"
>title="ランディングページのページ"
>abstract="ランディングページのページ"

>[!CONTEXTUALHELP]
>id="acw_landingpages_schedule"
>title="ランディングページのスケジュール"
>abstract="ランディングページのスケジュール"

>[!CONTEXTUALHELP]
>id="acw_landingpages_primarypage"
>title="ランディングページのプライマリページ"
>abstract="ランディングページのプライマリページ"

>[!CONTEXTUALHELP]
>id="acw_landingpages_subscription"
>title="ランディングページの購読"
>abstract="ランディングページの購読"

>[!CONTEXTUALHELP]
>id="acw_landingpages_calltoaction"
>title="ランディングページのコールトゥアクション"
>abstract="ランディングページのコールトゥアクション"

>[!CONTEXTUALHELP]
>id="acw_landingpages_simulate"
>title="ランディングページのシミュレート"
>abstract="ランディングページのシミュレート"




>[!CONTEXTUALHELP]
>id="acw_orchestration_query_enrichment_noneditable"
>title="編集不可のアクティビティ"
>abstract="編集不可のアクティビティ"




>[!CONTEXTUALHELP]
>id="acw_fragments_menu"
>title="フラグメント"
>abstract="フラグメント"

>[!CONTEXTUALHELP]
>id="acw_fragments_save"
>title="フラグメントの保存"
>abstract="フラグメントの保存"

>[!CONTEXTUALHELP]
>id="acw_fragments_create"
>title="フラグメントの作成"
>abstract="フラグメントの作成"

>[!CONTEXTUALHELP]
>id="acw_fragments_properties"
>title="フラグメントのプロパティ"
>abstract="フラグメントのプロパティ"

>[!CONTEXTUALHELP]
>id="acw_fragments_type"
>title="フラグメントの種類"
>abstract="フラグメントの種類"

>[!CONTEXTUALHELP]
>id="acw_fragments_list"
>title="フラグメントリスト"
>abstract="フラグメントリスト"

>[!CONTEXTUALHELP]
>id="acw_fragments_details"
>title="フラグメントの詳細"
>abstract="フラグメントの詳細"






>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_savefilter"
>title="条件付きコンテンツ保存フィルター"
>abstract="条件付きコンテンツ保存フィルター"

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_selectfilter"
>title="条件付きコンテンツ選択フィルター"
>abstract="条件付きコンテンツ選択フィルター"

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_subjectline"
>title="件名行の条件付きコンテンツ"
>abstract="件名行の条件付きコンテンツ"

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_subjectlinecondition"
>title="条件付きコンテンツの件名条件"
>abstract="条件付きコンテンツの件名条件"





>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_testprofiles"
>title="テストプロファイルをシミュレート"
>abstract="テストプロファイルをシミュレート"

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_profiles_selection"
>title="テストプロファイルの選択をシミュレート"
>abstract="テストプロファイルの選択をシミュレート"

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_send_testprofiles"
>title="テストプロファイルの送信をシミュレート"
>abstract="テストプロファイルの送信をシミュレート"

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_email_log"
>title="メールログをシミュレート"
>abstract="メールログをシミュレート"


>[!CONTEXTUALHELP]
>id="acw_subscriptions_totalnumber_subscribers"
>title="購読の合計数"
>abstract="購読の合計数"

>[!CONTEXTUALHELP]
>id="acw_subscriptions_overtheperiod_subscribers"
>title="期間中の購読"
>abstract="期間中の購読"

>[!CONTEXTUALHELP]
>id="acw_subscriptions_overallevolution_subscribers"
>title="購読の全体的な変化"
>abstract="購読の全体的な変化"


>[!CONTEXTUALHELP]
>id="acw_directmail_content"
>title="ダイレクトメールのコンテンツ"
>abstract="ダイレクトメールのコンテンツ"

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_file"
>title="ダイレクトメールのファイルプロパティ"
>abstract="ダイレクトメールのファイルプロパティ"

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_content"
>title="ダイレクトメールのコンテンツプロパティ"
>abstract="ダイレクトメールのコンテンツプロパティ"




<!--
Deprecated IDs - to remove in GA: -->

>[!CONTEXTUALHELP]
>id="acw_attributepicker_advancedfields"
>title="詳細属性を表示"
>abstract="デフォルトでは、最も一般的な属性のみが属性リストに表示されます。ルールビルダーの左側のパレットにある現在のリストで使用可能なすべての属性（ノード、グループ、1-1 リンク、1-N リンクなど）を表示するには、「**詳細属性を表示**」切替スイッチをアクティブ化します。"

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_advancedfields"
>title="ルールビルダーの詳細フィールド"
>abstract="デフォルトでは、最も一般的な属性のみが属性リストに表示されます。ルールビルダーの左側のパレットにある現在のリストで使用可能なすべての属性（ノード、グループ、1-1 リンク、1-N リンクなど）を表示するには、「**詳細属性を表示**」切替スイッチをアクティブ化します。"

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_properties_advanced"
>title="ルールビルダーの詳細属性"
>abstract="デフォルトでは、最も一般的な属性のみが属性リストに表示されます。ルールビルダーの左側のパレットにある現在のリストで使用可能なすべての属性（ノード、グループ、1-1 リンク、1-N リンクなど）を表示するには、「**詳細属性を表示**」切替スイッチをアクティブ化します。"