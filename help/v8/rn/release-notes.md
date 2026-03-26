---
title: Campaign v8 web ユーザーインターフェイスリリースノート
description: 最新の Campaign web ユーザーインターフェイスリリースで提供される新機能について説明します
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 304e3771ee55777d2eaf7a6c83ee4af3c97aa3b6
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 28%

---

# リリースノート {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="リリースノート"
>abstract="Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。これにより、Campaign リリースノートは月に数回更新され、最新の機能、改善点、修正が含まれます。定期的に確認することをお勧めします。"

Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。したがって、これらのリリースノートは月に数回更新されます。定期的に確認してください。

## 26年3月リリース {#26-3-release}

### 新機能 {#26-3-features}

<table>
<thead>
<tr>
<th><strong>スキーマオーサリング（GA）</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>スキーマオーサリング機能は、すべての顧客（GA）で使用できるようになりました。 この機能を使用すると、Campaign Web ユーザーインターフェイスから直接スキーマを作成および管理できます。 新しいテーブルを作成したり、既存のスキーマを拡張したり、カスタムフォームを作成したりできます。 クライアントコンソールにアクセスしなくても、特定のビジネスニーズに対応するカスタムデータ構造を定義できます。</p>
<p>詳しくは、<a href="../administration/schemas.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>メールDesigner（LA）のテーマ</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>テーマは、ブランドガイドラインに沿って再利用可能なテーマスタイルを定義できるため、メールのオーサリング体験を向上させます。 テーマ変数をフラグメントで使用できるようになり、メールテンプレート全体で一貫したスタイル設定を実現できます。 この機能を使用すると、ブランドの一貫性を維持しながら、タイトル、説明、画像、リンクなどのコンテンツ要素を抽象化する定義済みのモジュールを使用して、メールをより迅速に構築できます。</p>
<p>メモ：この機能は一連の組織でのみ使用でき（使用制限あり）、今後のリリースでグローバルにロールアウトされます。</p>
<p>詳しくは、<a href="../email/apply-email-themes.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>カスタム Firefly モデルとサードパーティの画像生成モデルの統合</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>標準Fireflyモデルとカスタム Adobe Target モデルを、承認済みのサードパーティ画像モデルとシームレスに統合することで、画像を生成する際の柔軟性、コントロール、ブランドの整合性を向上できます。</p>
<p>ニーズに適したモデルの選択：</p>
<ul><li> <strong>Adobe モデル </strong> （Firefly Image Model 4を利用）は、追加設定なしで即座に画像を生成できます</li><li> <strong> パートナーモデル </strong> （Gemini 2.5 Flashを搭載）を使用した特殊機能</li><li>ブランドに即した生成を可能にする<strong> カスタムモデル </strong> （独自のアセットでトレーニングされたブランド固有のモデル）は、ブランドアイデンティティ、スタイル、ビジュアルガイドラインに正確に一致します。</li></ul>
<p>詳しくは、<a href="../content/generative-models.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>配信アクティビティの自動化</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p><strong>自動配信</strong> ワークフローアクティビティがワークフローパレットで使用できるようになりました。 ワークフロー内で配信アクション（準備、プルーフの送信、準備、開始など）を直接作成または実行するために使用できます。 ワークフローの外部で作成された既存の配信を選択して、実行するたびに再利用するか、アクティビティが実行されるたびにテンプレートから新しい配信を作成します。</p>
<p><img src="assets/do-not-localize/workflow-automated-delivery.gif"/></p>
<p>詳しくは、<a href="../workflows/activities/automated-delivery.md">詳細ドキュメントを参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>複数のワークフローブランチと結合アクティビティ</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>

<p><strong>複数の分岐</strong>がサポートされるようになりました。 <strong>Fork</strong>を使用する代わりに、ツールバーの「<strong>分岐を追加</strong>」をクリックできます。 <strong>AND-join</strong> アクティビティも改善されました。 現在は、ANDとORの結合オプションを選択できる汎用的な<strong>結合</strong> アクティビティです。</p>
<p><img src="assets/do-not-localize/workflow-branches-join.gif"/></p>
<p>詳しくは、<a href="../workflows/orchestrate-activities.md#toolbar"> アクティビティのオーケストレーション </a>および<a href="../workflows/activities/join.md">参加</a>のドキュメントページを参照してください。</p>
</td>
</tr>
</tbody>
</table>

### 改善点 {#26-3-improvements}

* クライアントコンソールとの互換性を向上させるために、**開始** ワークフローアクティビティが追加されました。 このアクティビティはオプションであり、新しいワークフローにはデフォルトでは挿入されません。 ただし、既存のワークフローには自動的に追加されます。
  [詳細情報](../workflows/activities/about-activities.md#flow-control)
* 配信の&#x200B;**スケジュール**&#x200B;設定のタイムゾーン選択フィールドが、**連絡日** フィールドの下に移動されました。 [詳細情報](../msg/create-deliveries.md#gs-schedule)