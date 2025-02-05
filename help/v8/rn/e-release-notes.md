---
title: Campaign v8 web ユーザーインターフェイス早期リリースノート
description: 次の Campaign web ユーザーインターフェイスリリースで提供される新機能について説明します
hide: true
hidefromtoc: true
exl-id: a4c6ecb7-d657-46de-aa55-90c4cb45164b
source-git-commit: 202796bbaa26afb0741a5eb3947795ceff7e5414
workflow-type: ht
source-wordcount: '511'
ht-degree: 100%

---

# 早期リリースノート {#e-release}

Adobe Campaign web ユーザーインターフェイスでは、新機能、既存機能の強化、バグ修正が継続的に提供されます。すべての変更は、毎月末の[リリースノート](release-notes.md)に統合されます。

**以下の早期リリースノートの内容は、リリースの公開日まで予告なく変更される場合があります**。リンク、画面、更新済みのドキュメントは、リリース日に[リリースノート](release-notes.md)に公開されます。

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
<p>Campaign web インターフェイスで外部配信と外部配信テンプレートを定義できるようになりました。このモードでは、外部プロバイダーと共有できる入力ファイルにメッセージをコンパイルできます。デフォルトでは、ダイレクトメールチャネルには外部配信モードが使用されます。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>ビジネスルール（タイポロジルール）の作成</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Campaign web インターフェイスでタイポロジとタイポロジルールを作成できるようになりました。タイポロジとは、配信の制御、フィルタリング、および優先順位付けに役立つタイポロジルールのコレクションです。タイポロジは、配信に常に必須の要素（登録解除リンクや件名行など）を含め、フィルタリングルールを適用し、ターゲットオーディエンスから特定のグループ（登録解除者、競合他社、非ロイヤルティ顧客など）を除外できるようにします。</p>
<img src="assets/do-not-localize/typology.gif">
<!--p>For more information, refer to the <a href="../administration/external-account.md">detailed documentation</a>.</p-->
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
<p>Adobe Campaign web ユーザーインターフェイスから列挙を直接作成できるようになりました。 列挙とは、フィールドへの入力候補としてシステムによって表示される値のリストです。列挙を利用することでフィールドの値を統一することができ、データ入力時やクエリでの利用に便利です。</p>
<img src="assets/do-not-localize/enumerations.gif">
<!--p>For more information, refer to the <a href="../administration/external-account.md">detailed documentation</a>.</p-->
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
<!--p>For more information, refer to the <a href="../administration/external-account.md">detailed documentation</a>.</p-->
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
<!--p>For more information, refer to the <a href="../administration/external-account.md">detailed documentation</a>.</p-->
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


