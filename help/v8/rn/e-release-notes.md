---
title: Campaign v8 web ユーザーインターフェイス早期リリースノート
description: 次の Campaign web ユーザーインターフェイスリリースで提供される新機能について説明します
hide: true
hidefromtoc: true
exl-id: a4c6ecb7-d657-46de-aa55-90c4cb45164b
source-git-commit: 202796bbaa26afb0741a5eb3947795ceff7e5414
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 21%

---

# 早期リリースノート {#e-release}

Adobe Campaign web ユーザーインターフェイスでは、新機能、既存機能の強化、バグ修正が継続的に提供されます。すべての変更は、毎月末の[リリースノート](release-notes.md)に統合されます。

**以下の早期リリースノートの内容は、リリースの公開日まで予告なく変更される場合があります**。リンク、画面、更新済みのドキュメントは、リリース日に[リリースノート](release-notes.md)に公開されます。

## 2025 年 1 月リリース {#25-1-release}

**リリース日**:2025 年 2 月 5 日（PT）

1 月リリース以降、次の機能および改善点が提供されます。

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
<p>ビジュアルフラグメントは、複数のメール配信またはコンテンツテンプレートで再利用できる、事前定義されたビジュアルブロックです。 この機能は、サーバービルド 8.6.4 以降で実行されているすべての顧客が利用できるようになりました。</p>
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
<p>Campaign web インターフェイスで、外部配信と外部配信テンプレートを定義できるようになりました。 このモードでは、メッセージは入力ファイルにコンパイルされ、外部プロバイダーと共有できます。 デフォルトでは、ダイレクトメールチャネルに外部配信モードが使用されます。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>ビジネスルールの作成（タイポロジルール）</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Campaign web インターフェイスでタイポロジとタイポロジルールを作成できるようになりました。 タイポロジは、配信の制御、フィルタリングおよび優先順位付けに役立つタイポロジルールのコレクションです。 タイポロジを使用すると、配信には必ず必要な要素（登録解除リンクや件名行など）が含まれ、フィルタリングルールを適用してターゲットオーディエンスから特定のグループ（非購読者、競合他社、非ロイヤルティ顧客など）を除外できます。</p>
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
<p>Adobe Campaign web ユーザーインターフェイスから直接列挙を作成できるようになりました。 列挙は、フィールドへの入力をシステムが推奨する値のリストです。 列挙を利用することでフィールドの値を統一することができ、データ入力時やクエリでの利用に便利です。</p>
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
<p>Adobe Campaign web ユーザーインターフェイス内のテクニカルオプションにアクセスし、ニーズに合わせて独自のカスタムオプションを作成できるようになりました。 これは、JavaScript コードワークフローアクティビティを使用して中間データを保存する場合に特に便利です。</p>
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
<p>Adobe Campaign web ユーザーインターフェイスでJavaScript コードを作成できるようになりました。 これにより、ライブラリと同様に、ワークフロー全体で利用できる再利用可能な関数を作成できます。</p>
<img src="assets/do-not-localize/javascript.gif">
<!--p>For more information, refer to the <a href="../administration/external-account.md">detailed documentation</a>.</p-->
</td>
</tr>
</tbody>
</table>

### 改善点 {#25-1-improvements}

* インターフェイスでのカスタムフィールドの表示をカスタマイズします。

   * インターフェイスに表示する追加のカスタムフィールドを選択できるようになりました
   * 他のフィールドの入力に基づいてリスト値を制限するなど、リンクタイプのカスタムフィールドを表示するためのルールを設定できるようになりました
   * インターフェイスのフィールドをより柔軟に並べ替えることができるようになりました。フィールドを 1 列に分散したり、より良い整理のためにサブセクションにグループ化したりできます
   * 特定のフィールドを読み取り専用として設定できるようになりました

* 最近使用したフィルターとお気に入りフィルター：頻繁に使用する属性をすばやく再利用するために、お気に入りに追加できるようになりました。 これにより、今後のタスクでも簡単にアクセスできるようになります。 お気に入りに加えて、最近選択した属性を表示および使用することもできます。


