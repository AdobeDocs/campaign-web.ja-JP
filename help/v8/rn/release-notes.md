---
title: Campaign v8 web ユーザーインターフェイスリリースノート
description: 最新の Campaign web ユーザーインターフェイスリリースで提供される新機能について説明します
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 944fbbdd273cc402b88f2beaef5b15f2ce80cc6b
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 83%

---

# リリースノート {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="リリースノート"
>abstract="Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。これにより、Campaign リリースノートは月に数回更新され、最新の機能、改善点、修正が含まれます。定期的に確認することをお勧めします。"

Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。したがって、これらのリリースノートは月に数回更新されます。定期的に確認してください。

以前のリリースで利用可能な変更と改善点については、[このページ](release-notes-24.md)を参照してください。

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
<p>Campaign web インターフェイスで外部配信と外部配信テンプレートを定義できるようになりました。このモードでは、メッセージは出力ファイルにコンパイルされ、外部プロバイダーと共有できます。 デフォルトでは、ダイレクトメールチャネルには外部配信モードが使用されます。</p>
<img src="assets/do-not-localize/external-delivery.gif">
<p>詳しくは、<a href="../msg/send-external-deliveries.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<!--
<table>
<thead>
<tr>
<th><strong>Create business rules (typology rules)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now create typologies and typology rules in the Adobe Campaign web interface. A typology is a collection of typology rules that help control, filter, and prioritize deliveries. Typologies ensure that your deliveries always contain required elements (such as an unsubscribe link or subject line) and apply filtering rules to exclude specific groups from your target audience (such as unsubscribers, competitors, or non-loyalty customers).</p>
<img src="assets/do-not-localize/typology.gif">
<p>For more information, refer to the <a href="../administration/typologies.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>
-->

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
<th><strong>AI Assistant コンテンツアクセラレーターによるランディングページ生成</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>ランディングページ配信で AI アシスタントコンテンツアクセラレーターが使用できるようになり、テキストや画像を生成したり、完全なページレイアウトを作成できるようになりました。</p>
<img src="assets/do-not-localize/ai-lp.gif">
<p>AI アシスタント コンテンツ アクセラレータの詳細については、<a href="../email/generative-lp.md"> 詳細ドキュメント </a> を参照してください。</p>
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

* 外部アカウント：新しい外部アカウントを作成する際に、新しい **[!UICONTROL ルーティング]** タイプを選択できます。 外部配信で使用する特定の外部アカウントを設定できます。 [詳細情報](../administration/external-account.md#routing)