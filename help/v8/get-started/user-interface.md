---
audience: end-user
title: インターフェイスについて説明します
description: Campaign v8 Web ユーザーインターフェイス
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
source-git-commit: 15ee9ea467f9243834374cfe1a3e411f929c2a77
workflow-type: ht
source-wordcount: '717'
ht-degree: 100%

---

# インターフェイスについて説明します {#user-interface}

>[!NOTE]
>
>このドキュメントは作成中で、頻繁に更新されています。 このコンテンツの最終バージョンは、2023年1月に用意できます。

>[!CONTEXTUALHELP]
>id="acw_homepage_learnmore"
>title="インターフェイス"
>abstract="TBC"

新しい Campaign v8 Web インターフェイスは、直感的で一貫性のある統合されたユーザーエクスペリエンスを提供します。

ユーザーインターフェイスを閲覧する際の主要な概念は、Adobe Experience Platform と共通です。詳しくは、[Adobe Experience Platform のドキュメント](https://experienceleague.adobe.com/docs/experience-platform/landing/platform-ui/ui-guide.html?lang=ja#adobe-experience-platform-ui-guide)を参照してください。

>[!NOTE]
>
>このドキュメントは、製品のユーザーインターフェイスに対する最新の変更を反映するために頻繁に更新されています。ただし、一部のスクリーンショットは、お使いのユーザーインターフェイスと多少異なる場合があります。


<!--
* console + web interface (overview, why use each of them)
* web UI made up of read-only lists that can be configured, show how to add columns
-->

## 左側のナビゲーションメニュー

左側のリンクを参照すると、Campaign v8 の web 機能にアクセスできます。

![](assets/home.png)

### ホームページ

Campaign v8 web ホームページには、出発点となる主要なリンクやリソースが含まれています。**最近使用したもの**&#x200B;リストには、最近作成した配信へのショートカットが一覧表示されます。このリストには、配信の作成日と変更日およびステータスが表示されます。

<!--
* Banner
* KPIs on email channel (cross-deliveries): open rate, delivery rate, etc
* Recent items
* Learning cards
-->

ホームページの下部のセクションから、Campaign v8 web の主要ヘルプページにアクセスします。

<!--
show global KPIs, recent items + left menu to access features)
CONTROL PANEL not alpha
Global report not alpha
-->

### エクスプローラー

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="エクスプローラー"
>abstract="TBC"

**エクスプローラー**&#x200B;メニューには、クライアントコンソールのフォルダー階層と同じフォルダー階層が表示されます。Campaign v8 のすべてのコンポーネント、フォルダーおよびスキーマを参照できます。メール配信リストを除く、すべてのリスト画面は読み取り専用です。

エクスプローラーに表示される項目は、ユーザー権限によって異なります。

リスト画面の場合と同様に、必要なすべての情報を表示するように列を設定できます。[こちら](#list-screens)を参照してください。
<!--
Explorer' menu in web UI to navigate through console content: console navtree second view in addition to the left menu lists with filters. The Explorer gives the real folder hierarchy from the console. Make sure you find your deliveries in sub-folders. All lists can be accessed in read-only. No Create/Edit. You can configure lists (colums). All schema fields, linked tables are available. 

If you need to view your lists of recipients (age, gender), transactions or live transactional messages. To view each/edit -> console.

Navtree view depends on permissions (same as console).
-->

### キャンペーン管理

>[!CONTEXTUALHELP]
>id="acw_campaigns_list"
>title="キャンペーン"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_deliveries_list"
>title="配信"
>abstract="TBC"

* **キャンペーン** - キャンペーンのリストです。キャンペーンの開始日／終了日／最終変更日やステータスなどの有用な情報を確認できます。リストは、ステータスまたは開始日／終了日でフィルタリングできます。キャンペーンテンプレートも使用できます。これらのリストは読み取り専用です。

* **配信** - 配信のリストを閲覧できます。配信の状態、最終変更日および主要 KPI を確認できます。リストは、状態、コンタクト日またはチャネルでフィルタリングできます。メール配信をクリックすると、その配信のダッシュボードが開きます。その他の項目は読み取り専用です。 配信テンプレートも使用できます。

### 顧客管理

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="受信者"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="オーディエンス"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="購読リスト"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_targeting_workflow_list"
>title="ターゲティングワークフロー"
>abstract="TBC"

* **受信者** - 受信者データベースにアクセスできます。メールアドレス、名、姓などの有用な情報を確認できます。このリストは読み取り専用です。
* **オーディエンス** - オーディエンスのリストです。 オーディエンスのタイプ、接触チャネル、作成日／最終変更日およびラベルを確認できます。このリストは接触チャネルでフィルタリングできます。このリストは読み取り専用です。
* **購読リスト** - 購読リストを閲覧できます。購読リストのタイプ、モードおよびラベルを確認できます。このリストは読み取り専用です。
* **ターゲティングワークフロー** - キャンペーンワークフローのリストにアクセスできます。ワークフローの状態、前回／次の処理日および環境を確認できます。リストは、状態、前回の処理日およびワークフロータイプでフィルタリングできます。ワークフローテンプレートも使用できます。これらのリストは読み取り専用です。

### 意思決定管理

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="オファー"
>abstract="TBC"

* **オファー** - インタラクションオファーのリストを閲覧できます。オファーのステータス、開始日／終了日および環境を確認できます。リストは、状態や開始日／終了日でフィルタリングできます。オファーテンプレートも使用できます。これらのリストは読み取り専用です。

## 統合シェル

Campaign v8 web は、統合シェルと統合されています。上部バーの右側には、いくつかのボタンが表示されます。

![](assets/unified-shell.png){width="70%" align="left"}

これらのボタンを使用すると、次のことができます。

* アルファ顧客としてのフィードバックの共有
* IMS 組織の切り替え
* Adobe Experience Cloud アプリケーションの切り替え
* ヘルプページへのアクセス、サポートへの問い合わせ、フィードバックの共有検索フィールドからヘルプ記事およびビデオを検索できます。

<!--
Org / Sub-org switcher to switch between instances. Only one for Alpha. Later: intermerdiate screen with Control Panel (beta). if v8 + ACS with one card per ACS instance. Maybe quickly explain the menu for Alpha?
-->

## コンテキストヘルプとオンボーディングガイド

コンテキストヘルプは、インターフェイスで利用できます。使用可能な場合、「**?**」アイコンをクリックすると、ヘルプ情報や関連ドキュメントのリンクが表示されます。

![](assets/context-help.png){width="70%" align="left"}

また、Campaign v8 web の基本を学ぶうえで役に立つオンボーディングガイドも利用できます。右下隅にあるアイコンをクリックし、利用できるステップバイステップ方式のシナリオの 1 つを選択し、指示に従うだけです。

![](assets/onboarding.png){width="70%" align="left"}

## リスト画面の設定 {#list-screens}

メール配信リストを除く、すべてのリスト画面は読み取り専用です。

項目をすばやく見つけるには、検索バーを使用するか、コンテキスト条件に基づいてリストをフィルタリングします。

![](assets/filter.png){width="70%" align="left"}

リストは複数の列で表示されます。 各列は、1 つずつ昇順または降順に並べ替えることができます。列の設定を変更して、追加情報を表示することもできます。それには、リストの右上隅にあるアイコンをクリックします。 列の追加または削除や表示順序の変更を行うことができます。

![](assets/columns.png){width="70%" align="left"}

<!--
## Supported browsers {#browsers}

Adobe [!DNL Journey Optimizer] interface is designed to work optimally in the latest version of Google Chrome. You might have trouble using certain features on older versions or other browsers.
-->