---
title: Campaign v8 web ユーザーインターフェイスリリースノート
description: 最新の Campaign web ユーザーインターフェイスリリースで提供される新機能について説明します
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: c0a40e8c68b009b6803d8f24e6572c4ea359ba9f
workflow-type: ht
source-wordcount: '770'
ht-degree: 100%

---

# リリースノート {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="リリースノート"
>abstract="Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。これにより、Campaign リリースノートは月に数回更新され、最新の機能、改善点、修正が含まれます。定期的に確認することをお勧めします。"

Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。したがって、これらのリリースノートは月に数回更新されます。定期的に確認してください。

以前のリリースで利用可能な変更と改善点については、[このページ](release-notes-24.md)を参照してください。

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