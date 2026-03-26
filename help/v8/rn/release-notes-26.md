---
title: Campaign v8 web ユーザーインターフェイスの以前のリリースノート
description: 2026 Campaign web ユーザーインターフェイスリリース
exl-id: 40735c57-94ae-4646-8c3d-68197569fbd4
source-git-commit: 0cc09a983d412889f2b734a5bfb30bf422247ec0
workflow-type: tm+mt
source-wordcount: '746'
ht-degree: 22%

---

# 2026 リリースノート {#2026-release}

このページには、**2026 リリース**&#x200B;で使用可能なすべての変更点と改善点が記載されています。最新のリリースノートは、[このページ ](release-notes.md)で入手できます。

## 26/2月リリース {#26-2-release}

_2026年2月17日_

### 新機能 {#26-2-features}

<!--table>
<thead>
<tr>
<th><strong>Delivery scheduling compute process</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now use a delivery scheduling compute process similar to the one available in Adobe Campaign Standard. This feature allows you to calculate sending dates based on recipient timezones, enabling you to send communications at the optimal time for each recipient. This is particularly useful for organizations operating across multiple timezones, as it allows you to target regions with different timezones using a single delivery configuration.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Themes in the Email Designer (Beta)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Themes provide an improved authoring experience for emails by allowing you to define reusable theme styles that fit your brand guidelines. You can now use theme variables in fragments, ensuring consistent styling across your email templates. This feature enables you to build emails faster with predefined modules that abstract content elements such as titles, descriptions, images, and links, while maintaining brand consistency.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<table>
<thead>
<tr>
<th><strong>キャンペーン在庫のタイムラインビュー</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>キャンペーンのインベントリに、時間の経過に沿ってキャンペーンを視覚化および管理できるタイムラインビューが含まれるようになりました。リストとタイムラインを切り替え、週、月、日ごとに移動し、「今日」ボタンを使用して現在の日付にジャンプし、キャンペーンの詳細（ステータス、ワークフロー、配信）を右側のパネルで開きます。フィルターと検索はリストビューと同じです。</p>
<p>詳しくは、<a href="../campaigns/manage-campaigns.md#timeline">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>スキーマオーサリング（LA）</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Campaign Web ユーザーインターフェイスから直接スキーマを作成および管理できるようになりました。 この機能を使用すると、新しいテーブルを作成したり、既存のスキーマを拡張したり、カスタムフォームを作成したりできます。 クライアントコンソールにアクセスしなくても、特定のビジネスニーズに対応するカスタムデータ構造を定義できます。</p>
<p>メモ：この機能は一連の組織でのみ使用でき（使用制限あり）、今後のリリースでグローバルにロールアウトされます。</p>
<p>詳しくは、<a href="../administration/schemas.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<!--

### Improvement {#26-2-improvements}

* Brand guidelines now include a Colors section that defines standards for your brand's color system, ensuring consistent use of primary, secondary, accent, and neutral colors across all experiences. 
[Learn more](../content/brands-personalize.md)-->

## 26年1月リリース {#26-1-release}

_2026年1月27日_

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
<p>多言語配信機能がすべての顧客（GA）で利用できるようになりました。 この機能を使用すると、Adobe Campaign Web ユーザーインターフェイスで異なる言語で複数のメッセージを送信できます。 配信のデフォルトの言語と、配信を送信できるさまざまな言語を選択できます。 また、選択した言語でこれらの配信をプレビューすることもできます。 
<p>詳しくは、<a href="../msg/multilingual.md">詳細ドキュメント</a>を参照してください。</p>
<p>多言語プッシュ通知に対して、次の改善が行われました。</p>
<ul>
<li>多言語コンテンツを含むCSV ファイルをアップロードして、すべての言語バリエーションをすばやく入力できるようになりました。 <a href="../msg/multilingual.md#csv-upload">詳細情報</a>
</li>
<li>リッチプッシュ通知がサポートされるようになりました。</li>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>トランザクションメッセージのプロファイル強化（GA）</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>トランザクションメッセージのプロファイルエンリッチメント機能が、すべての顧客（GA）で使用できるようになりました。 メールに加えて、SMSおよびプッシュ通知もサポートされるようになりました。 この機能を使用すると、Adobe Campaign データベースフィールドをメッセージコンテンツにリンクすることで、トランザクションメッセージをパーソナライズできます。 ターゲットマッピング、エンリッチメント列および紐付けキーを選択して、パフォーマンスのしきい値を維持しながら、正確でリアルタイムのパーソナライゼーションを行うことができます。</p>
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
<p>Adobe Experience Manager コンテンツ統合を使用すると、配信を構築する際に、Adobe Experience Managerで作成されたすべての言語およびライブコピーにCampaign内で直接アクセスできます。 コンテンツをリアルタイムで更新し、最新のAdobe Experience Managerバージョンを取得できます。 この統合により、Adobe Experience ManagerとCampaignの間で手作業でコンテンツを同期する必要がなくなり、多言語キャンペーンのワークフローが合理化されます。</p>
<p>詳しくは、<a href="../integrations/aem-multilingual.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>コンテンツ実験 - A/B テスト</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Campaign Webのコンテンツ実験では、ターゲットオーディエンスにとって最適なパフォーマンスを測定するために、複数のA/B テスト配信のバリエーションを定義できます。 配信コンテンツ、件名、送信者を変更して、さまざまなバージョンをテストし、どのバリエーションが最も優れた結果を生み出すのかを判断できます。 件名、送信者名、メール本文など、様々なメール要素に対してA/B テストを実施できます。</p>
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
<p>継続配信アクティビティを使用すると、既存の配信に新しい受信者を追加できます。 毎回新しい配信を作成する必要がないため、必要に応じて少量のアラートや通知を送信することで効率が向上します。 継続的な配信は、単一の配信インスタンスを作成します。 すべての配信ログ（broadLog）とトラッキングログがこの1つの配信を参照するため、監視とレポートが簡素化されます。</p>
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
<p>承認プロセスは、複数の関係者の調整を支援し、配送の送信前に品質管理を確保します。 マーケティングマネージャーがコンテンツをレビューしたり、データアナリストがターゲットオーディエンスを検証したりするなど、複数のチームによる検証が必要な場合に、承認を使用します。</p>
<p>詳しくは、<a href="../campaigns/campaign-approvals.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

### 改善点 {#26-1-improvements}

* Dynamic Reportingがプッシュ通知とSMSをサポートするようになりました。 [詳細情報](../reporting/dynamic-reporting/get-started-reporting.md)
* 定義済みフィルター – 新しい「共有フィルター」オプションを使用すると、定義済みフィルターを組織内の他のユーザーが利用できるようになります。 [詳細情報](../get-started/predefined-filters.md#share-filter)
* 名前、電子メール、日付、住所など、Adobe Experience Managerで作成されたパーソナライゼーションフィールドが含まれ、コンテンツテンプレートを使用する際に利用できるようになりました。
* コンテンツの品質評価では、ブランドガイドラインに依存しない、読みやすさ、まとまり、有効性の問題をチェックし、不明確なメッセージ、一貫性のないトーン、構造的なギャップを特定します。 [詳細情報](../content/brands-score.md)
