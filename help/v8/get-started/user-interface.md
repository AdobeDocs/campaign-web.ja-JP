---
audience: end-user
title: インターフェイスの確認
description: Adobe Campaign Web ユーザーインターフェイス
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
source-git-commit: c0a40e8c68b009b6803d8f24e6572c4ea359ba9f
workflow-type: ht
source-wordcount: '2003'
ht-degree: 100%

---

# インターフェイスの確認 {#user-interface}

新しい Adobe Campaign Web インターフェイスは、マーケティングキャンペーンのデザインと配信を簡素化する、最新の直感的なユーザーエクスペリエンスを提供します。この新しいインターフェイスは、Adobe Experience Cloud のアプリおよびソリューションと統合されています。

Adobe Campaign に接続する方法と、Experience Cloud ナビゲーションの基本については、[この記事](connect-to-campaign.md)を参照してください。

>[!NOTE]
>
>このドキュメントは、製品のユーザーインターフェイスに対する最新の変更を反映するために頻繁に更新されています。ただし、一部のスクリーンショットは、お使いのユーザーインターフェイスと多少異なる場合があります。

## Campaign ホームページ {#user-interface-home}

>[!CONTEXTUALHELP]
>id="acw_homepage_recent"
>title="最近使用したもの"
>abstract="**最近使用したもの**&#x200B;リストには、最近作成および変更した配信へのショートカットが一覧表示されます。このリストには、チャネル、ステータス、所有者、作成日、変更日が表示されます。"

Campaign ホームページでは、主要リソース、指標、コンポーネントをすばやく簡単に参照できます。

ホームページの上部セクションには、製品で使用可能な最新の更新と新機能の詳細が、リリースノートと詳細なドキュメントへのリンクと共に表示されます。機能カードをスクロールするには、左向き矢印を使用します。

![](assets/home.png){zoomable="yes"}

**主要業績評価指標**&#x200B;では、一般的な KPI を通じてプラットフォームの有効性を確認できます。KPI について詳しくは、[このページ](../reporting/kpis.md)を参照してください。

**最近使用したもの**&#x200B;リストには、最近作成および変更した配信へのショートカットが一覧表示されます。このリストには、チャネル、ステータス、所有者、作成日、変更日が表示されます。さらに配信を読み込むには、**詳細を表示**&#x200B;リンクをクリックします。

また、ホームページの「**ラーニング**」セクションから、Adobe Campaign Web の主要ヘルプページにアクセスすることができます。

### リンクについて {#user-interface-about}


>[!CONTEXTUALHELP]
>id="acw_about"
>title="ページについて"
>abstract="詳細ページには、Adobe Campaign インスタンスに関する詳細が表示されます。"

>[!CONTEXTUALHELP]
>id="acw_about_instance"
>title="インスタンスについて"
>abstract="「インスタンス」セクションには、バージョンと関連付けられたビルド番号の両方を含む、コンソールクライアントに関する主な情報が表示されます"

>[!CONTEXTUALHELP]
>id="acw_about_web"
>title="Web について"
>abstract="「Web」セクションには、Campaign web ユーザーインターフェイスのバージョンと、使用可能な場合は最終更新日が表示されます。"

>[!CONTEXTUALHELP]
>id="acw_about_packages"
>title="インストールしたパッケージについて"
>abstract="「インストールしたパッケージ」セクションには、インスタンスに存在するすべてのモジュール、機能、統合が一覧表示されます。"

ページの下部にある&#x200B;**[!UICONTROL 詳細]**&#x200B;リンクには、Adobe Campaign インスタンスに関する詳細が表示されます。これらの情報は読み取り専用モードです。

![](assets/about-link.png){zoomable="yes"}

「**インスタンス**」セクションには、**バージョン**&#x200B;と関連付けられた&#x200B;**ビルド**&#x200B;番号の両方を含む、コンソールクライアントに関する主な情報が表示されます。

* **バージョン**&#x200B;は、使用している公式リリースバージョンを指します。
* **ビルド**&#x200B;は、そのバージョンの特定の反復を指します。

バージョン番号とビルド番号は両方とも、環境内に存在する機能と修正を正確に特定するのに役立つので、トラブルシューティングには重要です。

「**Web**」セクションには、Campaign web ユーザーインターフェイスのバージョンと、使用可能な場合は最終更新日が表示されます。これは、Campaign web ユーザーインターフェイスに対して行われた変更や機能強化を追跡するのに役立ちます。

「**インストールしたパッケージ**」セクションには、インスタンスに存在するすべてのモジュール、機能、統合が一覧表示されます。これらのパッケージでは、Adobe Campaign の機能を拡張し、他のアドビソリューションとの統合や特定のワークフローの有効化などの特殊なタスクを実行できます。多数のパッケージがある場合は、このセクション内で調査を行って、特定のモジュールがインスタンスにインストールされているかどうかをすばやく確認できます。

![](assets/about.png){zoomable="yes"}

## 左側のナビゲーションメニュー {#user-interface-left-nav}

左側のリンクを参照すると、Adobe Campaign Web 機能にアクセスできます。いくつかのリンクを選択すると、並べ替えやフィルタリングが可能なオブジェクトのリストが表示されます。また、必要なすべての情報を表示するように列を設定することもできます。[こちら](#list-screens)を参照してください。一部のリスト画面は読み取り専用です。左側のナビゲーションメニューとリストに表示される項目は、ユーザーの権限によって異なります。権限について詳しくは、[この節](permissions.md)を参照してください。


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

  ![](assets/more-actions.png){zoomable="yes"}{width="70%" align="left"}

* **ワークフロー** - この画面では、ワークフローとワークフローテンプレートの完全なリストにアクセスできます。ステータス、最後／次回の実行日を確認し、新しいワークフローまたは新しいワークフローテンプレートを作成できます。他のオブジェクトと同じ条件でリストをフィルタリングできます。さらに、キャンペーンに属するかどうかにかかわらず、ワークフローをフィルタリングできます。ワークフローについて詳しくは、[この節](../workflows/gs-workflows.md)を参照してください。


### コンテンツ管理 {#user-interface-content-management}

「コンテンツ管理」セクションでは、コンテンツのテンプレートとフラグメントを表示できます。

* **コンテンツテンプレート** - 設計プロセスを加速し改善するために、スタンドアロンのテンプレートを作成すると、[!DNL Adobe Campaign] 全体でカスタムコンテンツを簡単に再利用できます。メールでのみ使用可能なこの機能により、コンテンツ指向のユーザーはスタンドアロンのテンプレートで操作でき、マーケティングユーザーは自分たちのメールキャンペーン内でテンプレートを再利用して適応させることができます。詳しくは、[こちら](../email/create-email-templates.md)を参照してください。

* **フラグメント** - フラグメントは、キャンペーン全体で 1 つ以上の配信で参照できる再利用可能なコンポーネントです。フラグメントを変更すると、そのフラグメントを使用するすべてのコンテンツが更新されます。[詳しくは、フラグメントの操作方法を参照してください](../content/fragments.md)

この機能を使用すると、マーケティングユーザーが改善されたデザインプロセスでメールコンテンツを迅速に組み立てるために使用できる複数のカスタムコンテンツブロックを事前に作成できます。

### 顧客管理 {#user-interface-customer-management}

「顧客管理」セクションでは、プロファイル、オーディエンスおよび購読を表示できます。これらのリストは読み取り専用です。

* **プロファイル** - プロファイルを作成および管理し、受信者データベースにアクセスします。 デフォルトでは、メールアドレス、名前（名）および名前（姓）が表示されます。プロファイルについて詳しくは、[この節](../audience/about-recipients.md)を参照してください。
* **オーディエンス** - オーディエンスのリストです。デフォルトでは、オーディエンスのタイプ、接触チャネル、作成日／最終変更日およびラベルが表示されます。このリストは接触チャネルでフィルタリングできます。オーディエンスとリストについて詳しくは、[この節](../audience/about-recipients.md)を参照してください。
* **購読サービス** - 購読リストを参照できます。デフォルトでは、購読リストのタイプ、モードおよびラベルが表示されます。購読と購読解除を管理する方法については、[Adobe Campaign v8（コンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/subscriptions.html?lang=ja){target="_blank"}を参照してください。
* **定義済みフィルター** - 定義済みフィルターは、後で使用できるように作成および保存されるカスタムフィルターです。これらは、例えば、データのリストをフィルタリングしたり、配信のオーディエンスを作成したりする場合に、クエリモデラーでの任意のフィルタリング操作でショートカットとして使用できます。詳しくは、[このセクション](predefined-filters.md)を参照してください。


### 意思決定管理 {#decision-management}

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="オファー"
>abstract="**インタラクション**&#x200B;モジュールを使用して、コンソールで作成されたオファーとオファーテンプレートのリストを参照します。これらのリストは読み取り専用です。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/offers.html?lang=ja" text="配信へのオファーの追加"

「意思決定管理」セクションで、オファーとオファーテンプレートを表示できます。これらのリストは読み取り専用です。

* **オファー** - **インタラクション**&#x200B;モジュールを使用して、コンソールで作成されたオファーとオファーテンプレートのリストを参照します。デフォルトでは、オファーのステータス、開始日／終了日および環境が表示されます。このリストは、ステータスや開始日／終了日でフィルタリングできます。オファーテンプレートも使用できます。

メールと SMS でオファーを作成して送信する方法については、[この節](../msg/offers.md)を参照してください。

### レポート {#left-nav-reporting}

* **レポート** - **レポート**&#x200B;エントリでは、Campaign 環境内の各チャネルのトラフィックとエンゲージメント指標の統合された全体的な概要が提供されます。これらのレポートは様々なウィジェットで構成され、それぞれがキャンペーンや配信パフォーマンスに関する明確な観点を提供します。詳しくは、[こちら](../reporting/global-reports.md)を参照してください。

### 管理 {#left-nav-admin}


* **監査記録** - **監査記録**&#x200B;エントリにより、インスタンス内の重要なエンティティに対して行われたすべての変更（通常、インスタンスのスムーズな操作に大きな影響を与える変更）を完全に表示できます。[詳細情報](../reporting/audit-trail.md)

* **外部アカウント** - Web ユーザーインターフェイスを使用して新しい外部アカウントを作成し、特定のニーズを満たし、シームレスなデータ転送を確実に行います。[詳細情報](../administration/external-account.md)

* **スキーマ** - カスタムフィールドは、Adobe Campaign コンソールを通じて標準スキーマに追加される追加属性です。[詳細情報](../administration/custom-fields.md)

* **配信アラート** - 配信アラートは、ユーザーのグループが配信実行に関する情報を含むメール通知を自動的に受信できるようにする、アラート管理システムです。[詳細情報](../msg/delivery-alerting.md)

<!--
## Contextual Help {#user-interface-help} 

A contextual help is available in the interface. When available, click on the `?` icon to display help information and related documentation links. 

![](assets/do-not-localize/context-help.png){zoomable="yes"}{width="40%" align="left"}

Currently released as a Beta version within the new Campaign Web user interface, the **AI-powered Knowledge Assistant** embedded within contextual help revolutionizes documentation searching and answering how-to questions with effortlessly sifting through vast documentation repositories, instantly pinpointing the precise information you need.

Thanks to Campaign Gen AI's capabilities, this assistant transforms your experience, making information retrieval and problem-solving a breeze. Whether you're seeking guidance in a complex task or navigating extensive documents, our AI-powered Knowledge Assistant is your ultimate companion, providing unmatched efficiency and accuracy in every interaction.

Learn more in [this section](using-ai.md).

-->

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

<!-- delivery template settings-->

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sending"
>title="グローバルレポートの送信"
>abstract="トラッキングレポート指標は、この画面に表示されます"

>[!CONTEXTUALHELP]
>id="acw_global_reporting_tracking"
>title="グローバルレポートのトラッキング"
>abstract="トラッキングレポート指標は、この画面に表示されます"


<!-- FOR BETA (alignment) -->
<!--https://wiki.corp.adobe.com/display/neolane/v8+WebUI+Contextual+Help+%3CBETA%3E-+Official+list-->


<!-- FOR GA -->
<!-- Aligned with https://wiki.corp.adobe.com/display/neolane/v8+WebUI+Contextual+Help+%3CGA%3E-+Official+list -->

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

<!--ML: not visible in UI-->

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_profiles_selection"
>title="テストプロファイルの選択をシミュレート"
>abstract="テストプロファイルの選択をシミュレート"

<!-- ML: beta wiki page - not visible in UI-->

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_send_testprofiles"
>title="テストプロファイルの送信をシミュレート"
>abstract="テストプロファイルの送信をシミュレート"

<!-- ML: beta wiki page - not visible in UI-->

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_email_log"
>title="メールログをシミュレート"
>abstract="メールログをシミュレート"

<!-- ML: beta wiki page - not visible in UI-->

<!-- FOR POST-GA -->

<!--Update file-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata"
>title="データを更新"
>abstract="**データを更新**&#x200B;アクティビティでは、データベースのフィールドを一括で更新します。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_operationtype"
>title="データの更新方法を選択"
>abstract="「**操作のタイプ**」フィールドで、データベース内のデータに実行する処理を選択します。最初のオプションを選択してデータを追加するか、既に追加されている場合は更新します。また、データの追加のみ、データの更新のみ、またはデータの削除を行うこともできます。「**コレクションを更新して結合**」を選択して、重複をリンクするプライマリレコードを選択し、これらの重複を安全に削除します。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_recordid"
>title="レコード識別"
>abstract="データベース内のレコードを識別する方法を指定します。データが既存のターゲティングディメンションに関連する場合は、「**ターゲティングディメンションを使用**」オプションを選択し、更新するターゲティングディメンションとフィールドを選択します。それ以外の場合は、データベース内のデータを識別する 1 つ以上のカスタムリンクを指定するか、紐付けキーを直接使用します。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_fieldsupdate"
>title="更新するフィールドを選択"
>abstract="更新するフィールドと紐付け設定を選択します。「**自動マッピング**」オプションを使用すると、更新するフィールドを自動的に識別できます。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_advancedoptions"
>title="データ更新の詳細オプション"
>abstract="「**詳細オプション**」セクションでは、データと重複を管理する追加設定を指定できます。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_outboundtransition"
>title="アウトバウンドトランジションを生成"
>abstract="「**アウトバウンドトランジションを生成**」オプションを切り替えて、**データを更新**&#x200B;アクティビティの実行の終了時にアクティブ化されるアウトバウンドトランジションを追加します。通常は、更新によってターゲティングワークフローの終了が示されるので、このオプションはデフォルトでは有効化されません。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_outboundtransition_rejects"
>title="却下に対するアウトバウンドトランジションを生成します。"
>abstract="「**却下に対するアウトバウンドトランジションを生成**」オプションを切り替えて、更新後に（例えば、重複レコードが存在するなどで）正しく処理されなかったレコードを含むアウトバウンドトランジションを追加します。通常は、更新によってターゲティングワークフローの終了が示されるので、このオプションはデフォルトでは有効化されません。"

<!-- Workflow settings -->

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_initscript"
>title="初期化スクリプト"
>abstract="初期化スクリプト"

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution_properties"
>title="実行プロパティ"
>abstract="実行プロパティ"

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution_error"
>title="実行エラー"
>abstract="実行エラー"

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution_initscript"
>title="実行初期化スクリプト"
>abstract="実行初期化スクリプト"

<!-- Schema creation -->

>[!CONTEXTUALHELP]
>id="acw_schema_type"
>title="スキーマタイプ"
>abstract="スキーマタイプ"

>[!CONTEXTUALHELP]
>id="acw_schema_properties"
>title="スキーマのプロパティ"
>abstract="スキーマ"

>[!CONTEXTUALHELP]
>id="acw_schema_existing"
>title="既存のスキーマを選択"
>abstract="スキーマ"

>[!CONTEXTUALHELP]
>id="acw_schema_external"
>title="外部データベースを選択"
>abstract="スキーマ"

>[!CONTEXTUALHELP]
>id="acw_schema_add_tables"
>title="テーブルを追加"
>abstract="スキーマ"

>[!CONTEXTUALHELP]
>id="acw_schema_logs_tasks"
>title="ワークフローログとタスク"
>abstract="スキーマ"

>[!CONTEXTUALHELP]
>id="acw_schema_update"
>title="データベースを更新"
>abstract="スキーマ"

>[!CONTEXTUALHELP]
>id="acw_schema_update_script"
>title="スクリプトを更新"
>abstract="スキーマ"

>[!CONTEXTUALHELP]
>id="acw_schema_start_update"
>title="データベース更新を開始"
>abstract="スキーマ"
