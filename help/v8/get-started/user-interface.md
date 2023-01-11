---
audience: end-user
title: インターフェイスについて説明します
description: Campaign v8 Web ユーザーインターフェイス
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
source-git-commit: 1157113798f95329651e71b726d6132f9d8c7544
workflow-type: tm+mt
source-wordcount: '1153'
ht-degree: 54%

---

# インターフェイスについて説明します {#user-interface}

![](../assets/do-not-localize/badge.png)

>[!CONTEXTUALHELP]
>id="acw_homepage_learnmore"
>title="インターフェイス"
>abstract="新しい Campaign v8 Web インターフェイスは、統合され、直感的で一貫性のあるユーザーエクスペリエンスを提供します。"

新しい Campaign v8 Web インターフェイスは、マーケティングキャンペーンの設計と配信をシンプル化する、最新で直感的なユーザーエクスペリエンスを提供します。 この新しいインターフェイスは、Adobe Experience Platformと統合されています。

<!--
Key concepts when browsing the user interface are common with Adobe Experience Platform. Refer to [Adobe Experience Platform documentation](https://experienceleague.adobe.com/docs/experience-platform/landing/platform-ui/ui-guide.html#adobe-experience-platform-ui-guide) for more details.
-->

>[!NOTE]
>
>このドキュメントは、製品のユーザーインターフェイスに対する最新の変更を反映するために頻繁に更新されています。ただし、一部のスクリーンショットは、お使いのユーザーインターフェイスと多少異なる場合があります。


<!--
* console + web interface (overview, why use each of them)
* web UI made up of read-only lists that can be configured, show how to add columns
-->

## 左側のナビゲーションメニュー

左側のリンクを参照して、Campaign v8 Web 機能にアクセスします。 複数のリンクには、並べ替えやフィルタリングが可能なオブジェクトのリストが表示されます。 また、必要なすべての情報を表示するように列を設定することもできます。 [こちら](#list-screens)を参照してください。メール配信リストを除く、すべてのリスト画面は読み取り専用です。編集/表示用のリスト項目をクリックすると、アルファでは利用できません。 すべてのリストは、ベータ版および GA 版で編集可能になります。 左側のナビゲーションメニューに表示される項目は、ユーザー権限によって異なります。

![](assets/home.png)

### ホーム

この画面には、Campaign v8 の主な Web 機能にすばやくアクセスするための主要なリンクやリソースが含まれています。 この **最近** リストには、最近作成および変更された配信へのショートカットが表示されます。 このリストには、配信の作成日と変更日およびステータスが表示されます。

<!--
* Banner
* KPIs on email channel (cross-deliveries): open rate, delivery rate, etc
* Recent items
* Learning cards
-->

ホームページの下部のセクションから、Campaign v8 Web キーのヘルプページにアクセスします。

<!--
show global KPIs, recent items + left menu to access features)
CONTROL PANEL not alpha
Global report not alpha
-->

### エクスプローラー

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="エクスプローラー"
>abstract="**エクスプローラー**&#x200B;メニューには、クライアントコンソールのフォルダー階層と同じフォルダー階層が表示されます。Campaign v8 のすべてのコンポーネント、フォルダーおよびスキーマを参照できます。メール配信リストを除く、すべてのリスト画面は読み取り専用です。"

**エクスプローラー**&#x200B;メニューには、クライアントコンソールのフォルダー階層と同じフォルダー階層が表示されます。Campaign v8 のすべてのコンポーネント、フォルダーおよびスキーマを参照できます。メール配信リストを除く、すべてのリスト画面は読み取り専用です。

エクスプローラーに表示される項目は、ユーザー権限によって異なります。

他のリスト画面と同様に、列を設定して表示をパーソナライズし、必要なすべての情報を表示できます。 [こちら](#list-screens)を参照してください。

Campaign エクスプローラーについて詳しくは、 [ドキュメント](https://experienceleague.adobe.com/docs/campaign-classic/using/getting-started/starting-with-adobe-campaign/campaign-workspace/adobe-campaign-explorer.html).
<!--
Explorer' menu in web UI to navigate through console content: console navtree second view in addition to the left menu lists with filters. The Explorer gives the real folder hierarchy from the console. Make sure you find your deliveries in sub-folders. All lists can be accessed in read-only. No Create/Edit. You can configure lists (colums). All schema fields, linked tables are available. 

If you need to view your lists of recipients (age, gender), transactions or live transactional messages. To view each/edit -> console.

Navtree view depends on permissions (same as console).
-->

### キャンペーン管理

>[!CONTEXTUALHELP]
>id="acw_campaigns_list"
>title="キャンペーン"
>abstract="キャンペーンのリストです。 キャンペーンの開始日／終了日／最終変更日やステータスなどの有用な情報を確認できます。リストは、ステータスまたは開始日／終了日でフィルタリングできます。キャンペーンテンプレートも使用できます。これらのリストは読み取り専用です。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_list"
>title="配信"
>abstract="配信のリストを参照します。 配信の状態、最終変更日および主要 KPI を確認できます。リストは、状態、コンタクト日またはチャネルでフィルタリングできます。メール配信をクリックすると、その配信のダッシュボードが開きます。その他の項目は読み取り専用です。 配信テンプレートも使用できます。"

* **キャンペーン** - キャンペーンのリストです。デフォルトでは、変更の開始日/終了日/最終日とステータスを表示できます。 リストは、ステータスまたは開始日／終了日でフィルタリングできます。キャンペーンテンプレートも使用できます。これらのリストは読み取り専用です。

* **配信** - 配信のリストを閲覧できます。デフォルトでは、状態、最終変更日および主要 KPI を表示できます。 リストは、状態、コンタクト日またはチャネルでフィルタリングできます。E メール配信をクリックして、ダッシュボードを開き、配信の詳細の概要を確認します。 他のチャネルでの配信は読み取り専用です。 配信テンプレートは、読み取り専用モードでも使用できます。 クライアントコンソールを使用して編集できます。 参照 [ドキュメント](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/using-delivery-templates/about-templates.html?lang=ja).

### 顧客管理

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="受信者"
>abstract="受信者データベースにアクセスします。 メールアドレス、名、姓などの有用な情報を確認できます。このリストは読み取り専用です。"

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="オーディエンス"
>abstract="これはオーディエンスのリストです。 オーディエンスのタイプ、接触チャネル、作成日／最終変更日およびラベルを確認できます。このリストは接触チャネルでフィルタリングできます。このリストは読み取り専用です。"

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="購読リスト"
>abstract="購読リストを閲覧します。 購読リストのタイプ、モードおよびラベルを確認できます。このリストは読み取り専用です。"

>[!CONTEXTUALHELP]
>id="acw_targeting_workflow_list"
>title="ターゲティングワークフロー"
>abstract="キャンペーンワークフローのリストにアクセスします。 ワークフローの状態、前回／次の処理日および環境を確認できます。リストは、状態、前回の処理日およびワークフロータイプでフィルタリングできます。ワークフローテンプレートも使用できます。これらのリストは読み取り専用です。"

* **受信者** - 受信者データベースにアクセスできます。デフォルトでは、メールアドレス、名および姓を表示できます。 このリストは読み取り専用です。
* **オーディエンス** - オーディエンスのリストです。 デフォルトでは、タイプ、接触チャネル、作成日/最終変更日およびラベルを表示できます。 このリストは接触チャネルでフィルタリングできます。このリストは読み取り専用です。
* **購読リスト** - 購読リストを閲覧できます。デフォルトでは、タイプ、モードおよびラベルを表示できます。 このリストは読み取り専用です。
* **ターゲティングワークフロー** - キャンペーンワークフローのリストにアクセスできます。デフォルトでは、その状態、最終/次の処理日および環境を表示できます。 リストは、状態、前回の処理日およびワークフロータイプでフィルタリングできます。ワークフローテンプレートも使用できます。これらのリストは読み取り専用です。

### 意思決定管理

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="オファー"
>abstract="インタラクションオファーのリストを参照します。 デフォルトでは、ステータス、開始日/終了日および環境を表示できます。 リストは、状態や開始日／終了日でフィルタリングできます。オファーテンプレートも使用できます。これらのリストは読み取り専用です。"

* **オファー** - インタラクションオファーのリストを閲覧できます。デフォルトでは、ステータス、開始日/終了日および環境を表示できます。 リストは、状態や開始日／終了日でフィルタリングできます。オファーテンプレートも使用できます。これらのリストは読み取り専用です。

## 上部バー

インターフェイスの上部のバーでは、次の操作を実行できます。

* フィードバックをアルファテスターとして共有
* 組織とインスタンスの切り替え
* Adobe Experience Cloud アプリケーションの切り替え
* ヘルプページへのアクセス、サポートへの問い合わせ、フィードバックの共有検索フィールドからヘルプ記事およびビデオを検索できます。

![](assets/unified-shell.png){width="70%" align="left"}
<!--
Org / Sub-org switcher to switch between instances. Only one for Alpha. Later: intermerdiate screen with Control Panel (beta). if v8 + ACS with one card per ACS instance. Maybe quickly explain the menu for Alpha?
-->

## コンテキストヘルプとオンボーディングガイド

コンテキストヘルプは、インターフェイスで利用できます。使用可能な場合、「**?**」アイコンをクリックすると、ヘルプ情報や関連ドキュメントのリンクが表示されます。

![](assets/context-help.png){width="70%" align="left"}

また、Campaign v8 Web の使用を開始する際に役立つオンボーディングガイドも利用できます。 右下隅にあるアイコンをクリックし、利用できるステップバイステップ方式のシナリオの 1 つを選択し、指示に従うだけです。

![](assets/onboarding.png){width="70%" align="left"}

## リスト画面の設定 {#list-screens}

左側のナビゲーションメニューからの複数のリンク（例： ） **配信** または **キャンペーン**、オブジェクトのリストを表示します。 これらのリスト画面は、E メール配信リストを除き、読み取り専用です。

項目をすばやく見つけるには、検索バーを使用するか、コンテキスト条件に基づいてリストをフィルタリングします。

![](assets/filter.png){width="70%" align="left"}

リストは複数の列で表示されます。 列の設定を変更して、追加情報を表示できます。 それには、リストの右上隅にあるアイコンをクリックします。 列の追加または削除や表示順序の変更を行うことができます。

![](assets/columns.png){width="70%" align="left"}

任意の列見出しをクリックして、リスト内の項目を並べ替えることができます。 リストがその列で並べ替えられていることを示す矢印が（上または下）表示されます。 数値列または日付列の場合、上向き矢印はリストが昇順で並べ替えられていることを示し、下向き矢印は降順であることを示します。 文字列列または英数字列の場合、値はアルファベット順に表示されます。

<!--
## Supported browsers {#browsers}

Adobe [!DNL Journey Optimizer] interface is designed to work optimally in the latest version of Google Chrome. You might have trouble using certain features on older versions or other browsers.
-->