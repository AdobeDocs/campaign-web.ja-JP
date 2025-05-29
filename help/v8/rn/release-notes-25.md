---
title: Campaign v8 web ユーザーインターフェイスの以前のリリースノート
description: 2025 Campaign web ユーザーインターフェイスリリース
exl-id: eecb4b18-4826-47a6-88b2-f2ed7b576d3e
source-git-commit: 8ec342d565bc8418c202cdba834d74a99cff3a47
workflow-type: tm+mt
source-wordcount: '1281'
ht-degree: 100%

---

# 2025 リリースノート {#2025-release}

このページには、**2025 リリース**&#x200B;で使用可能なすべての変更点と改善点が記載されています。最新のリリースノートについて詳しくは、[このページ](release-notes.md)を参照してください。

## 2025年4月リリース {#25-4-release}

**リリース日**：2025年4月29日（PT）

### 新機能 {#25-4-features}

次の機能は、4月のリリース以降、すべてのユーザーが使用できます。

<table>
<thead>
<tr>
<th><strong>コールセンターチャネル</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>コールセンターチャネルを Campaign web ユーザーインターフェイスで使用できるようになりました。このチャネルは、コールセンター（通常、エージェントによる顧客や見込み客への電話）を通じて処理される通信やインタラクションを管理および追跡するのに使用される通信方法を指します。</p>
<p>メモ：レポートは、コールセンターチャネルの Web UI では使用できません。レポートにアクセスするには、クライアントコンソールを参照する必要があります。</p>
<img src="assets/do-not-localize/call-center.gif">
<p>詳しくは、<a href="../call-center/gs-call-center.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>新しいルールビルダー</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>改善されたユーザーインターフェイスで複雑な条件を定義するのに役立つ、新しいルールビルダーが使用できるようになりました。必要に応じて、古いルールビルダーから新しいルールビルダーに切り替えることができます。</p>
<img src="assets/do-not-localize/rule-builder-release.gif">
<p>詳しくは、<a href="../query/query-modeler-overview.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>外部アカウントのオーサリング</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Campaign 管理者は、Campaign web ユーザーインターフェイスから外部システムとの新しい接続を設定できるようになりました。
また、既存の外部アカウントを表示、更新、管理することもできます。</p>
<p>詳しくは、<a href="../administration/external-account.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

### 改善点 {#25-4-improvements}

**一般的なインターフェイスの改善**

* スキーマ属性のフィールドの説明、お気に入りに追加、値の配分のオプションがユーザーインターフェイスでより見やすくなりました。詳しくは、[詳細なドキュメント](../get-started/attributes.md)を参照してください。
* Experience League の環境設定で指定したプライマリ言語に従って、日時がインターフェイスに表示されるようになりました。この改善は、複数の言語でのみ使用できます。サポートされる言語の完全なリストを確認するには、[詳細なドキュメント](https://experienceleague.adobe.com/ja/docs/core-services/interface/features/browser-language){target=_blank}を参照してください。

<!--
ko * Built-in options are now only visible in the list of options if the **Show advanced options** toggle is activated.
ko * The typology rules creation screen has been updated to facilitate the selection of the type of rule.
-->

**メールエディター**：Campaign web UI のアクセシビリティを強化することを目的に、E メールデザイナーで 2 つの新しいフィールドが使用できるようになりました。これらは、メールコンテンツの `html` 要素の `title` 要素と lang 属性に対応しています。これらの設定は、メールの「本文」セクションの「プリヘッダー」フィールドに加えて定義できます。詳しくは、[詳細なドキュメント](../email/metadata.md)を参照してください。

<!--
**Workflow**: You can now select an existing Javascript code in workflow properties or in a Javascript activity.    
-->

**スキーマ**

* Campaign web ユーザーインターフェイスからリストの一時スキーマを編集できるようになりました。詳しくは、[詳細なドキュメント](../audience/manage-audience.md)を参照してください。
* サンプル画面でスキーマのカスタムフィールドをプレビューできるようになりました。詳しくは、[詳細なドキュメント](../administration/custom-fields.md#add)を参照してください。
* ドラッグ＆ドロップを使用して、リストのカスタムフィールドを移動できるようになりました。詳しくは、[詳細なドキュメント](../administration/custom-fields.md#add)を参照してください。


### 限定提供の新機能 {#25-4-features-la}

>[!AVAILABILITY]
>
>次の機能は、限定提供（LA）です。**Adobe Campaign Standard から Adobe Campaign v8** に移行するお客様に限定され、他の環境にはデプロイできません。Campaign サーバーを v8.7.4 にアップグレードする必要があります。
>
>ドキュメントページの [Campaign v8 への Campaign Standard の移行](../rn/acs-migration.md)および [Campaign Standard ユーザー向けの機能](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=ja)を参照してください。

* **多言語配信の作成** - Adobe Campaign web ユーザーインターフェイスで、複数のメール配信を異なる言語で送信できるようになりました。多言語配信機能を使用すると、配信のデフォルト言語と、配信を送信できる様々な言語を選択できます。また、選択した言語でこれらの配信をプレビューすることもできます。詳しくは、[詳細なドキュメント](../email/edit-content.md)を参照してください。

* **多言語用の動的レポート** - 多言語メール配信で動的レポートが使用できるようになりました。詳しくは、[詳細なドキュメント](../reporting/global-reports.md)を参照してください。

* **SMS REST API サポート（LA）** - トランザクションメッセージング REST API が SMS チャネルで使用できるようになりました。ペイロードにメールと mobilePhone の両方が存在する場合は、「wishedChannel」フィールドを使用してチャネルを指定できます。指定しない場合は、wishedChannel で明示的に SMS をリクエストしない限り、デフォルトでメールが使用されます。詳しくは、[詳細なドキュメント](https://experienceleague.adobe.com/ja/docs/experience-cloud/campaign/apis/managing-transactional-messages){target=_blank}を参照してください。

## 2025年2月リリース {#25-2-release}

**リリース日**：2025年2月18日（PT）

次の機能と改善点は、2月のリリース以降使用できます。

### 機能 {#25-2-features}

<table>
<thead>
<tr>
<th><strong>ビジネスルール（タイポロジルール）の作成</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Campaign web ユーザーインターフェイスでタイポロジとタイポロジルールを作成できるようになりました。タイポロジでは、配信の送信を制御、フィルタリングおよび優先順位付けできます。タイポロジを使用すると、必須コンポーネント（登録解除リンクや件名など）や、オーディエンス（登録解除者、競合他社、非ロイヤルティ顧客など）からグループを除外するフィルタリングルールが配信に常に含まれていることを検証できます。</p>
<img src="assets/do-not-localize/typology.gif">
<p>詳しくは、<a href="../administration/typologies.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>ターゲットマッピング</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Campaign web ユーザーインターフェイスでターゲットマッピングを作成できるようになりました。ターゲットマッピングは、様々な配信チャネル（メール、SMS、プッシュ通知）からスキーマのデータフィールドへのリンク方法を定義します。ターゲットマッピングを使用すると、ターゲットオーディエンス（プロファイル、契約の受取人、オペレーター、サブスクライバーなど）を定義できます。</p>
<img src="assets/do-not-localize/target-mapping.gif">
<p>詳しくは、<a href="../administration/target-mappings.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>スキーマの詳細</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>リストで名前を選択して、スキーマの詳細にアクセスできるようになりました。カスタムフィールドの編集は、スキーマの詳細にある「<b>カスタムフィールドを編集</b>」ボタンからアクセスできるようになりました。</p>
<img src="assets/do-not-localize/schemas.gif">
<p>詳しくは、<a href="../administration/schemas.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

## 2025年1月リリース {#25-1-release}

**リリース日**：2025年2月5日（PT）

次の機能と改善点は、1月のリリース以降使用できます。

### 機能 {#25-1-features}


<table>
<thead>
<tr>
<th><strong>ビジュアルフラグメントの作成と使用</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>ビジュアルフラグメントは、複数のメール配信やコンテンツテンプレートをまたいで再利用できる、定義済みのビジュアルブロックです。この機能を、サーバービルド 8.6.4 以降を実行しているすべてのお客様が使用できるようになりました。</p>
<img src="assets/do-not-localize/visual-fragment.gif">
<p>詳しくは、<a href="../content/use-visual-fragments.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>サードパーティシステムを使用した配信の送信</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Campaign web インターフェイスで外部配信と外部配信テンプレートを定義できるようになりました。このモードでは、外部プロバイダーと共有できる出力ファイルにメッセージをコンパイルできます。デフォルトでは、ダイレクトメールチャネルには外部配信モードが使用されます。</p>
<img src="assets/do-not-localize/external-delivery.gif">
<p>詳しくは、<a href="../msg/send-external-deliveries.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>列挙の管理</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Campaign web ユーザーインターフェイスから列挙を直接作成できるようになりました。列挙とは、フィールドへの入力候補としてシステムによって表示される値のリストです。列挙を使用してフィールドの値を統一すると、データ入力やクエリ内での使用が簡単になります。</p>
<img src="assets/do-not-localize/enumerations.gif">
<p>詳しくは、<a href="../administration/enumerations.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>カスタムオプションの作成</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Campaign web ユーザーインターフェイス内のテクニカルオプションにアクセスし、ニーズに合わせて独自のカスタムオプションを作成できるようになりました。これは、JavaScript コードワークフローアクティビティを使用して中間データを保存する際に特に便利です。</p>
<img src="assets/do-not-localize/options.gif">
<p>詳しくは、<a href="../administration/options.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>Javascript コードの定義と呼び出し</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Campaign web ユーザーインターフェイスで JavaScript コードを作成できるようになりました。これにより、ライブラリと同様に、ワークフロー全体で利用できる再利用可能な関数を作成できます。</p>
<img src="assets/do-not-localize/javascript.gif">
<p>詳しくは、<a href="../administration/javascript-codes.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>AI アシスタントを使用したランディングページの生成</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>ランディングページ配信で AI アシスタントが使用できるようになりました。これにより、テキスト、画像または完全なページレイアウトを生成できます。</p>
<img src="assets/do-not-localize/ai-lp.gif">
<p>AI アシスタントについて詳しくは、<a href="../email/generative-lp.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>


### 改善点 {#25-1-improvements}

* インターフェイスでのカスタムフィールドの表示のカスタマイズ：

   * インターフェイスに表示する追加のカスタムフィールドを選択できるようになりました
   * リンクタイプのカスタムフィールドを表示するためのルールを設定できるようになりました（他のフィールドの入力に基づいてリスト値を制限するなど）
   * インターフェイスのフィールドをより柔軟に並べ替えられるようになりました（フィールドの幅を 1 つの列全体に広げる、より適切に整理するためにサブセクションにグループ化する）
   * 特定のフィールドを読み取り専用として設定できるようになりました

* 最近使用したフィルターとお気に入りフィルター：頻繁に使用する属性をすばやく再利用するために、お気に入りに追加できるようになりました。これにより、以降のタスクではすばやくアクセスできます。お気に入りに加えて、最近選択した属性を表示したり使用したりすることもできます。

* 外部アカウント：新しい外部アカウントを作成する際に、新しい&#x200B;**[!UICONTROL ルーティング]**&#x200B;タイプを選択できます。これにより、外部配信で使用する特定の外部アカウントを設定できます。[詳細情報](../administration/external-account.md#routing)
