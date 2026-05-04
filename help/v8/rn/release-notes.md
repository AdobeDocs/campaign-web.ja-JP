---
title: Campaign v8 web ユーザーインターフェイスリリースノート
description: 最新の Campaign web ユーザーインターフェイスリリースで提供される新機能について説明します
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: f1f207785ad25ceb8f9891bfad74193768cb2937
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 91%

---

# リリースノート {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="リリースノート"
>abstract="Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。 これにより、Campaign リリースノートは月に数回更新され、最新の機能、改善点、修正が含まれます。 定期的に確認することをお勧めします。"

Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。 したがって、これらのリリースノートは月に数回更新されます。 定期的に確認してください。

## 26年4月リリース {#26-4-release}

_2026年4月29日_

### 改善点 {#26-4-improvement}

**エンリッチメントデータ** セクションが、**オーディエンスの構築** ワークフローアクティビティ（クエリタイプ）で利用できるようになりました。 Campaign Web ユーザーインターフェイスから直接&#x200B;**追加データ**&#x200B;を表示、追加、編集、削除できます。 「**エンリッチメント**」アクティビティと同様に、単一のエンリッチメント属性、コレクションのリンクおよび式を追加できます。

[詳細情報](../workflows/activities/build-audience.md)

## 2026年3月リリース {#26-3-release}

_2026年3月1日（PT） 24_

### 新機能 {#26-3-features}

<table>
<thead>
<tr>
<th><strong>スキーマ作成（GA）</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>スキーマ作成機能は、すべてのお客様が利用できるようになりました（GA）。 この機能を使用すると、Campaign web ユーザーインターフェイスから直接スキーマを作成および管理できます。 新しいテーブルの作成、既存のスキーマの拡張、カスタムフォームの作成ができます。 クライアントコンソールにアクセスすることなく、特定のビジネスニーズに合わせてカスタムデータ構造を定義できます。</p>
<p>詳しくは、<a href="../administration/schemas.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>E メールデザイナー（LA）のテーマ</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>テーマを使用すると、ブランドガイドラインに沿って再利用可能なテーマスタイルを定義できるため、メールの作成エクスペリエンスが向上します。 フラグメントでテーマ変数を使用できるようになり、メールテンプレート全体でスタイルを統一できます。 この機能を使用すると、ブランドの一貫性を維持しながら、タイトル、説明、画像、リンクなどのコンテンツ要素を抽象化する定義済みのモジュールを使用して、メールをより迅速に構築できます。</p>
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
<p>標準およびカスタムの Firefly モデルと承認済みのサードパーティ画像モデルとのシームレスな統合によって、画像を生成する際の柔軟性、コントロール、ブランドの整合性を高めます。</p>
<p>ニーズに適したモデルの選択：</p>
<ul><li> <strong>Adobe モデル</strong> （Firefly Image Model 4 搭載）追加設定なしで即座に画像を生成</li><li> <strong> パートナーモデル </strong> （Gemini 2.5 Flash を搭載）特殊機能を提供</li><li><strong>カスタムモデル</strong> （独自のアセットでトレーニングされたブランド固有のモデル）ブランドアイデンティティ、スタイル、ビジュアルガイドラインに正確に一致する、ブランドに即したコンテンツを生成</li></ul>
<p>詳しくは、<a href="../content/generative-models.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>自動配信アクティビティ</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p><strong>自動配信</strong> ワークフローアクティビティがワークフローパレットで利用可能になりました。 配信アクションの作成または実行（準備、配達確認の送信、準備と開始など）に使用できます。 ワークフローに直接組み込むことができます。 ワークフローの外部で作成された既存の配信を選択して、実行のたびに再利用するか、アクティビティが実行されるたびにテンプレートから新しい配信を作成します。</p>
<p><img src="assets/do-not-localize/workflow-automated-delivery.gif"/></p>
<p>詳しくは、<a href="../workflows/activities/automated-delivery.md">詳細なドキュメントを参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>ワークフローの複数の分岐と結合アクティビティ</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>

<p><strong>複数の分岐</strong>がサポートされるようになりました。 <strong>分岐</strong>を使用する代わりに、ツールバーの「<strong>分岐を追加</strong>」をクリックできます。 <strong>AND 結合</strong>アクティビティも改善されました。 現在は、AND と OR の結合オプションを選択できる汎用的な<strong>結合</strong>アクティビティになりました。</p>
<p><img src="assets/do-not-localize/workflow-branches-join.gif"/></p>
<p>詳しくは、<a href="../workflows/orchestrate-activities.md#toolbar">アクティビティのオーケストレーション</a>および<a href="../workflows/activities/join.md">結合</a>のドキュメントページを参照してください。</p>
</td>
</tr>
</tbody>
</table>

### 改善点 {#26-3-improvements}

* クライアントコンソールとの互換性を向上させるために、ワークフローの&#x200B;**開始**アクティビティが追加されました。 このアクティビティはオプションであるため、新しいワークフローにはデフォルトで挿入されません。 ただし、既存のワークフローには自動的に追加されます。
  [詳細情報](../workflows/activities/about-activities.md#flow-control)
* 配信の「**スケジュール**」設定のタイムゾーン選択フィールドが、「**連絡日**」フィールドの下に移動しました。 [詳細情報](../msg/create-deliveries.md#gs-schedule)