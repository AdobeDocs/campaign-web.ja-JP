---
title: Campaign v8 web ユーザーインターフェイスリリースノート
description: 最新の Campaign web ユーザーインターフェイスリリースで提供される新機能について説明します
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 36d2b7a67ef087d628151199a223ceee54f84180
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 31%

---

# リリースノート {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="リリースノート"
>abstract="Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。これにより、Campaign リリースノートは月に数回更新され、最新の機能、改善点、修正が含まれます。定期的に確認することをお勧めします。"

Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。したがって、これらのリリースノートは月に数回更新されます。定期的に確認してください。

以前のリリースで利用可能な変更と改善点について詳しくは、[2024](release-notes-24.md) ページと [2025](release-notes-25.md) ページを参照してください。

## 2026 年 1 月リリース {#26-1-release}

_2026 年 1 月 27 日_

### 新機能 {#26-1-features}

<table>
<thead>
<tr>
<th><strong>多言語配信機能（GA）</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>すべての顧客（GA）が多言語配信機能を使用できるようになりました。 この機能を使用すると、Adobe Campaign web ユーザーインターフェイスで、異なる言語で複数のメッセージを送信できます。 配信のデフォルト言語だけでなく、配信を送信する様々な言語を選択できます。 また、選択した言語でこれらの配信をプレビューすることもできます。 
<p>詳しくは、<a href="../msg/multilingual.md">詳細ドキュメント</a>を参照してください。</p>
<p>多言語プッシュ通知が次のように改善されました。</p>
<ul>
<li>多言語コンテンツを含む CSV ファイルをアップロードすることで、すべての言語バリアントをすばやく入力できるようになりました。 <a href="../msg/multilingual.md#csv-upload">詳細を表示</a>
</li>
<li>リッチなプッシュ通知がサポートされるようになりました。</li>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>トランザクションメッセージ（GA）でのプロファイルのエンリッチメント</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>トランザクションメッセージ機能のプロファイルエンリッチメントを、すべてのお客様が利用できるようになりました（GA）。 メールに加えて、SMS およびプッシュ通知もサポートされるようになりました。 この機能を使用すると、Adobe Campaign データベースフィールドをメッセージのコンテンツにリンクして、トランザクションメッセージをパーソナライズできます。 ターゲットマッピング、エンリッチメント列および紐付けキーを選択して、パフォーマンスのしきい値を維持しながら、正確でリアルタイムのパーソナライゼーションを行うことができます。</p>
<p>詳しくは、<a href="../transactional-messaging/profile-enrichment.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Adobe Experience Managerのライブコピーと言語コピー</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Experience Managerのコンテンツ統合機能を使用すると、配信を作成する際に、Adobe Experience Managerで作成されたすべての言語とライブコピーに Campaign 内で直接アクセスできます。 コンテンツをリアルタイムに更新して、Adobe Experience Managerの最新バージョンを取得できます。 この統合により、Adobe Experience Managerと Campaign の間で手動によるコンテンツの同期が不要になり、多言語キャンペーンのワークフローが合理化されます。</p>
<p>詳しくは、<a href="../integrations/aem-multilingual.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>コンテンツ実験 – A/B テスト</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Campaign Web でのコンテンツ実験では、ターゲットオーディエンスに最適なパフォーマンスを発揮する製品を測定するために、複数の A/B テスト用の配信バリアントを定義できます。 配信コンテンツ、件名または送信者を変更して、様々なバージョンをテストし、どのバリアントが最適な結果を生み出すかを決定できます。 件名、送信者名、メール本文のコンテンツなど、様々なメール要素に対して A/B テストを実行できます。</p>
<p>詳しくは、<a href="../email/ab-testing.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>連続配信アクティビティ</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>連続配信アクティビティでは、既存の配信に新しい受信者を追加できます。 この配信タイプでは、毎回新しい配信を作成する必要がないので、必要に応じて送信される少量のアラートや通知の方が効率的です。 連続配信では、1 つの配信インスタンスが作成されます。 すべての配信ログ（broadLog）とトラッキングログは、この 1 つの配信を参照するので、監視とレポートがシンプルになります。</p>
<p>詳しくは、<a href="../workflows/activities/continuous-delivery.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>キャンペーン承認管理</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>承認プロセスは、複数の関係者の調整に役立ち、配信が送信される前の品質管理を確実にします。 組織が様々なチームからの検証を必要とする場合（マーケティングマネージャーによるコンテンツのレビューや、データアナリストによるターゲットオーディエンスの検証など）に、承認を使用します。</p>
<p>詳しくは、<a href="../campaigns/campaign-approvals.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

### 改善点 {#26-1-improvements}

* 動的レポートで、プッシュ通知と SMS がサポートされるようになりました。 [詳細情報](../reporting/dynamic-reporting/get-started-reporting.md)
* 定義済みフィルター – 新しい「共有フィルター」オプションを使用すると、組織内の他のユーザーが定義済みフィルターを使用できるようになります。 [詳細情報](../get-started/predefined-filters.md#share-filter)
* 名前、メール、日付、住所など、Adobe Experience Managerで作成されたパーソナライゼーションフィールドが含まれ、コンテンツテンプレートを使用する際に使用できるようになりました。
* コンテンツ品質評価では、ブランドガイドラインに関係なく、読みやすさ、凝集性、有効性の問題をチェックし、メッセージの不明瞭さ、トーンの不一致、構造ギャップを特定するようになりました。 [詳細情報](../content/brands-score.md)
