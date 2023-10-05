---
audience: end-user
title: インターフェイスを確認
description: Campaign v8 Web ユーザーインターフェイス
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
badge: label="Beta"
source-git-commit: 86a343aae763e753bc63ca2cab3c22cda07d7c16
workflow-type: tm+mt
source-wordcount: '1253'
ht-degree: 92%

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

**最近使用したもの**&#x200B;リストには、最近作成および変更した配信へのショートカットが一覧表示されます。このリストには、チャネル、ステータス、所有者、作成日、変更日が表示されます。

**主要業績評価指標**&#x200B;では、一般的な KPI を通じてプラットフォームの有効性を確認できます。KPI について詳しくは、[このページ](../reporting/kpis.md)を参照してください。

ホームページの「**ラーニング**」セクションから、Campaign v8 web の主要ヘルプページにアクセスします。

### エクスプローラー {#user-interface-explorer}

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="エクスプローラー"
>abstract="**エクスプローラー**&#x200B;メニューには、クライアントコンソールのフォルダー階層と同じフォルダー階層を持つすべての Campaign コンポーネントとオブジェクトが表示されます。このメニューから、すべての Campaign v8 コンポーネント、フォルダーおよびスキーマを参照し、関連する権限を確認し、フォルダーとサブフォルダーを作成します。"

**エクスプローラー**&#x200B;メニューには、クライアントコンソールのフォルダー階層と同じフォルダー階層を持つすべての Campaign リソースとオブジェクトが表示されます。すべての Campaign v8 コンポーネント、フォルダーおよびスキーマを参照し、配信、ワークフローおよびキャンペーンを作成します。

**エクスプローラー**&#x200B;に表示される項目は、ユーザー権限によって異なります。また、適切な権限がある場合は、フォルダーやサブフォルダーを追加することもできます。権限について詳しくは、[この節](permissions.md)を参照してください。

列を設定して表示をカスタマイズし、必要なすべての情報を表示することができます。 [こちら](#list-screens)を参照してください。また、フォルダーやサブフォルダーを追加することもできます。詳しくは、 [この節](permissions.md#folders).

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

メールと SMS でオファーを作成して送信する方法については、[この節](../content/offers.md)を参照してください。

## 上部バー {#top-bar}

インターフェイスの上部バーを使用して、次の操作を実行できます。

* ベータ版テスターとしてのフィードバックの共有
* 組織とインスタンス間の切り替え
* Adobe Experience Cloud アプリケーションの切り替え
* ヘルプページへのアクセス、サポートへの問い合わせ、フィードバックの共有検索フィールドからヘルプ記事およびビデオを検索できます。

![](assets/unified-shell.png){width="50%" align="left"}
<!--
Org / Sub-org switcher to switch between instances. Only one for Alpha. Later: intermerdiate screen with Control Panel (beta). if v8 + ACS with one card per ACS instance. Maybe quickly explain the menu for Alpha?
-->


## コンテキストヘルプ {#user-interface-help}

コンテキストヘルプは、インターフェイスで利用できます。使用可能な場合は、「`?`」アイコンをクリックすると、ヘルプ情報や関連ドキュメントのリンクが表示されます。

![](assets/context-help.png){width="40%" align="left"}

新しいベータ版では、 **AI を利用したナレッジアシスタント** コンテキストヘルプ内に組み込まれ、膨大なドキュメントリポジトリを簡単に切り替え、必要な正確な情報を即座に特定し、ドキュメントの検索とハウツー質問への回答に革新的に対応します。

Campaign Gen AI の機能により、このアシスタントではユーザーのエクスペリエンスを変革し、情報の検索と問題解決を簡単に行うことができます。複雑なタスクでのガイダンスを求める場合でも、広範なドキュメントをナビゲートする場合でも、AI を活用したナレッジアシスタントは究極のコンパニオンで、すべてのインタラクションで卓越した効率と正確性を提供します。

詳しくは、[こちら](using-ai.md)を参照してください。

## サポートしているブラウザー {#browsers}

Campaign v8 Web は、最新バージョンの Google Chrome、Safari および Microsoft Edge で最適に動作するように設計されています。古いバージョンや他のブラウザーでは、特定の機能を使用する際に問題が発生する可能性があります。

## 言語環境設定 {#language-pref}

Campaign v8 Web は現在、次の言語で利用できます。

* 英語（米国）- EN-US
* フランス語 - FR
* ドイツ語 - DE
* イタリア語 - IT
* スペイン語 - ES
* ポルトガル語（ブラジル）- PTBR
* 日本語 - JP
* 韓国語 - KR
* 簡体字中国語 - CHS
* 繁体字中国語 - CHT


Campaign web のデフォルト言語は、ユーザープロファイルで指定された優先言語によって決まります。Campaign サーバーとクライアントコンソールの言語とは関係ありません。

言語を変更するには：

1. 右上のプロファイルアイコンをクリックし、 「**環境設定**」を選択します。
1. 次に、メールアドレスの下に表示されている言語リンクをクリックします。
1. 優先言語を選択し、「**保存**」をクリックします。使用しているコンポーネントが第一希望の言語にローカライズされていない場合に備えて、第二の言語を選択できます。

## ダークテーマ {#dark-theme}

プロファイルアイコンからダークテーマに切り替えることができます。**ダークテーマ**&#x200B;の切替スイッチを使用して有効／無効を切り替えます。

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


