---
title: Campaign v8 web ユーザーインターフェイスの以前のリリースノート
description: 2026 Campaign web ユーザーインターフェイスのリリース
exl-id: 40735c57-94ae-4646-8c3d-68197569fbd4
source-git-commit: 6ed3a17593d0dc7bda55d9f90fc27526c09d99ed
workflow-type: tm+mt
source-wordcount: '2025'
ht-degree: 72%

---

# 2026 リリースノート {#2026-release}

このページには、**2026 リリース**&#x200B;で提供されるすべての変更点と改善点が一覧表示されています。 最新のリリースノートについて詳しくは、[このページ](release-notes.md)を参照してください。

## 26/7/月リリース {#26-7-release}

_2026年7月28日_

### 新機能 {#26-7-features}

<table>
<thead>
<tr>
<th><strong>オファー管理</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Campaign Web ユーザーインターフェイスからエンドツーエンドでオファーを直接管理できるようになりました。 オファー環境とオファースペースの設定、オファーカタログとカテゴリーの作成、適格性ルールと優先度の重み付けを使用したオファーの作成、配信で使用するためのオファーの承認とデプロイを行います。 高度な設定は、クライアントコンソールで引き続き使用できます。</p>
<p>詳しくは、<a href="../offers/gs-offer-management.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>ブランド設定</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>技術管理者は、クライアントコンソールを使用せずに、Campaign Web ユーザーインターフェイスからブランドを直接作成および設定できるようになりました。 ID、サブドメインとプロトコル、メールヘッダーパラメーター、URL トラッキングパラメーターなど、すべてのブランド設定がWeb UIで使用できるようになりました。</p>
<p>詳しくは、<a href="../administration/branding/branding-configure.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>メールDesignerの公開リソース</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>メールに画像を追加する際、<strong>公開リソース </strong>を選択できるようになりました。 これにより、Adobe Campaign インスタンスで既に使用可能な画像（以前にメールDesignerに読み込まれたファイルや、クライアントコンソールからアップロードされたパブリックリソースなど）を選択できます。</p>
<p>詳しくは、<a href="../email/content-components.md#image">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>データ読み込み（RDBMS）ワークフローアクティビティ</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p><strong> データ読み込み（RDBMS） </strong> アクティビティが、Campaign Web ユーザーインターフェイスで使用できるようになりました。 このアクティビティを使用すると、外部リレーショナルデータベースからワークフローに直接データをロードできます。 抽出されたデータはワークフロー全体を通じて利用でき、ターゲティング、エンリッチメント、またはさらなるデータ処理に使用できます。</p>
<p>詳しくは、<a href="../workflows/activities/data-loading-rdbms.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>動的な JavaScript ページ</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>動的JavaScript ページ（JSSP）を使用すると、カスタム API、書き出し、web アプリケーションロジックなどのURLを介してアクセスしたときに動的コンテンツを生成するサーバーサイドページを構築できます。 これらのページをCampaign Web ユーザーインターフェイスから直接作成、変更、複製、削除できるようになりました。</p>
<p>詳しくは、<a href="../administration/dynamic-javascript-pages.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

### 改善点 {#26-7-improvements}

* **カスタムスキーマ設定**&#x200B;に対して、次の改善が行われました。
  * 新しい&#x200B;**アクションデータ** セクションでは、個々のフォルダーで設定されたセキュリティルールに関係なく、カスタムスキーマのレコードで使用できるアクションを制限できます。 [詳細情報](../administration/schemas-action-data.md)
  * **カスタムフィルター**&#x200B;が&#x200B;**在庫リスト設定** セクションに追加されました。 リストビューのフィルターペインで、クイックアクセスフィールドとして表示する属性を選択できます。 [詳細情報](../administration/schemas-custom-filters.md)

* **ワークフロー**&#x200B;に対して、次の改善が行われました。
  * ワークフローアクティビティの削除がより柔軟になりました。アクティビティに後続のアクティビティがある場合は、すべて削除するか、選択したアクティビティのみを削除するか、後続のアクティビティを新しいブランチに維持しながら削除するかを選択できます。 [詳細情報](../workflows/orchestrate-activities.md#delete-activity)
  * 2つのワークフローアクティビティ間のトランジションを削除せずに切断できるようになりました。 これにより、ワークフローダイアグラムを再整理できます。例えば、保存するアクティビティのグループを一時的に保存し、削除して再作成する必要はありません。 [詳細情報](../workflows/orchestrate-activities.md#disconnect-transition)
  * ワークフローキャンバスの周りに水平スクロールバーと垂直スクロールバーが表示され、表示する領域に直接ドラッグして大きなワークフローを移動できるようになりました。 [詳細情報](../workflows/orchestrate-activities.md)
  * ワークフローを保存または開始/再起動する際に、開いてから別のユーザーがWeb UIまたはクライアントコンソールでワークフローを変更した場合に、警告が表示されるようになりました。 他の変更を上書きするか、ワークフローをリロードして最新バージョンを取得するか、キャンセルするかを選択できます。

* **送信者の電子メールアドレス**: **NmsDelivery_senderAddressMask** オプションを使用して、配信の&#x200B;**送信者の電子メール** フィールドを事前定義されたアドレスのリストに制限できるようになりました。 [詳細情報](../administration/options.md#restrict-sender-address)
* **ログインエラーメッセージ**&#x200B;が改善されました。ログインが失敗した場合、Web UIに、いくつかのシナリオに対してより具体的なエラーメッセージが表示されるようになりました（例えば、ユーザーにセキュリティゾーンが割り当てられていないか、IP アドレスが制限されている場合）。

## 2026年6月リリース {#26-6-release}

_2026年6月16日（PT）_

### 改善点 {#26-6-improvements}

<!--
* Technical administrators can now create and configure brands directly from the Campaign Web User Interface, without using the Client Console. All brand settings, including identity, subdmain and protocols, email header parameters and URL tracking parameters, are now available in the Web UI. <!-- [Learn more](../administration/branding/branding-configure.md)
-->

* トラッキングログを含む任意のリスト画面からデータをエクスポートできるようになりました。 リストを見つけて、エクスポートボタンをクリックするだけです。 エクスポートでは、現在読み込まれている行が含まれ、画面に表示されている列やアクティブな検索またはフィルターが考慮されます。 [詳細情報](../get-started/list-filters.md)

* **重複排除 - 重複**&#x200B;および&#x200B;**終了**&#x200B;ワークフローアクティビティで、複数のインバウンドトランジションがサポートされるようになりました 複数のインバウンドトランジションが使用可能な場合は、アクティビティの「**結合に設定する**」セクションを使用します
接続するトランジションを選択します。 詳しくは、[重複排除 - 重複](../workflows/activities/deduplication.md)、[終了](../workflows/activities/end.md)の各ページを参照してください。

* **オーディエンスを作成**（クエリタイプ）および&#x200B;**エンリッチメント**&#x200B;ワークフローアクティビティの「**エンリッチメントデータ**」セクションで、詳細設定パラメーターが公開されるようになりました。 これらのパラメーターを使用すると、グループ化、重複排除 - 重複、プライマリキーの処理、インバウンドイベントデータなど、エンリッチメントデータの作成方法を微調整できます。 [詳細情報](../workflows/activities/enrichment.md)

<!--
* Delivery templates now allow you to define a time zone in the Schedule settings.
-->

## 2026年4月リリース {#26-4-release}

_2026年4月29日（PT）_

### 改善点 {#26-4-improvement}

「**エンリッチメントデータ**」セクションが&#x200B;**オーディエンスを作成**&#x200B;ワークフローアクティビティ（クエリタイプ）で使用できるようになりました。 Campaign web ユーザーインターフェイスから直接&#x200B;**追加データ**&#x200B;を表示、追加、編集、削除できます。 **エンリッチメント**&#x200B;アクティビティと同様に、単一のエンリッチメント属性、コレクションのリンクおよび式を追加できます。

[詳細情報](../workflows/activities/build-audience.md)

## 2026年3月リリース {#26-3-release}

2026年&#x200B;_3月_ 24日（PT）

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

## 2026年2月リリース {#26-2-release}

_2026年2月17日（PT）_

### 新機能 {#26-2-features}

<!--
table>
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
</table
-->

<!--
table>
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
</table
-->

<table>
<thead>
<tr>
<th><strong>キャンペーンのインベントリのタイムラインビュー</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>キャンペーンのインベントリに、キャンペーンの推移を視覚化および管理できるタイムラインビューが含まれるようになりました。リストとタイムラインの表示を切り替えたり、週、月、日ごとに移動したり、「今日」ボタンを使用して現在の日付にジャンプしたりすることができます。また、右側のパネルでキャンペーンの詳細（ステータス、ワークフロー、配信）を開くことができます。フィルターや検索機能はリスト表示のものと同じです。</p>
<p>詳しくは、<a href="../campaigns/manage-campaigns.md#timeline">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>スキーマ作成（LA）</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Campaign web ユーザーインターフェイスから直接スキーマを作成および管理できるようになりました。 この機能を使用すると、新しいテーブルの作成、既存のスキーマの拡張、カスタムフォームの作成ができます。 クライアントコンソールにアクセスすることなく、特定のビジネスニーズに合わせてカスタムデータ構造を定義できます。</p>
<p>メモ：この機能は一連の組織でのみ使用でき（使用制限あり）、今後のリリースでグローバルにロールアウトされます。</p>
<p>詳しくは、<a href="../administration/schemas.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<!--

### Improvement {#26-2-improvements}

* Brand guidelines now include a Colors section that defines standards for your brand's color system, ensuring consistent use of primary, secondary, accent, and neutral colors across all experiences. 
[Learn more](../content/brands-personalize.md)
-->

## 2026年1月リリース {#26-1-release}

_2026年1月27日（PT）_

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
<p>多言語配信機能は、すべてのお客様が利用できるようになりました（GA）。 この機能を使用すると、Adobe Campaign web ユーザーインターフェイスから異なる言語で複数のメッセージを送信できます。 配信のデフォルト言語と、配信に使用できる様々な言語を選択できます。 また、選択した言語でこれらの配信をプレビューすることもできます。 
<p>詳しくは、<a href="../msg/multilingual.md">詳細ドキュメント</a>を参照してください。</p>
<p>多言語プッシュ通知に対して、次の改善が行われました。</p>
<ul>
<li>多言語コンテンツを含む CSV ファイルをアップロードして、すべての言語バリアントをすばやく入力できるようになりました。 <a href="../msg/multilingual.md#csv-upload">詳細情報</a>
</li>
<li>リッチプッシュ通知がサポートされるようになりました。</li>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>トランザクションメッセージでのプロファイルエンリッチメント（GA）</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>トランザクションメッセージのプロファイルエンリッチメント機能は、すべてのお客様が利用できるようになりました（GA）。 メールに加えて、SMS とプッシュ通知もサポートされるようになりました。 この機能を使用して、Adobe Campaign データベースフィールドをメッセージのコンテンツにリンクすることによって、トランザクションメッセージをパーソナライズできます。 ターゲットマッピング、エンリッチメント列および紐付けキーを選択することで、パフォーマンスのしきい値を維持しながら、正確でリアルタイムのパーソナライゼーションを行うことができます。</p>
<p>詳しくは、<a href="../transactional-messaging/profile-enrichment.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Adobe Experience Manager のライブコピーと言語コピー</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Experience Manager コンテンツ統合機能により、配信を構築する際に、Adobe Experience Manager で作成されたすべての言語コピーとライブコピーに Campaign から直接アクセスできます。 コンテンツをリアルタイムで更新し、最新の Adobe Experience Manager バージョンを取得できます。 この統合により、Adobe Experience Manager と Campaign との間でコンテンツの同期を手作業で行う必要がなくなり、多言語キャンペーンのワークフローが合理化されます。</p>
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
<p>Adobe Campaign web のコンテンツ実験では、ターゲットオーディエンスにとって最適なパフォーマンスを測定するのに、複数の A/B テスト配信のバリアントを定義できます。 配信コンテンツ、件名、送信者を変更して、さまざまなバージョンをテストし、どのバリアントが最も優れた結果を生み出すのかを判断できます。 A/B テストは、件名、送信者名、メール本文など、様々なメール要素に対して実施できます。</p>
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
<p>連続配信アクティビティでは、既存の配信に新しい受信者を追加できます。 この配信タイプを使用すると、毎回新しい配信を作成する必要がなくなります。このモードは、容量不足のアラートや通知を必要に応じて送信する場合に、より効率的です。 連続配信では、単一の配信インスタンスが作成されます。 すべての配信ログ（broadLog）とトラッキングログがこの 1 つの配信を参照するため、監視とレポートが簡素化されます。</p>
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
<p>承認プロセスは、複数の関係者の連携を支援し、配信前の品質管理を確実に行うためのものです。 承認を使用するのは、マーケティングマネージャーがコンテンツをレビューしたり、データアナリストがターゲットオーディエンスを検証したりするなど、組織の複数のチームによる検証が必要になる場合です。</p>
<p>詳しくは、<a href="../campaigns/campaign-approvals.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

### 改善点 {#26-1-improvements}

* 動的レポートでプッシュ通知と SMS がサポートされるようになりました。 [詳細情報](../reporting/dynamic-reporting/get-started-reporting.md)
* 定義済みフィルター – 新しい「共有フィルター」オプションを使用すると、組織内の他のユーザーが定義済みフィルターを利用できるようになります。 [詳細情報](../get-started/predefined-filters.md#share-filter)
* コンテンツテンプレートを使用する際に、Adobe Experience Manager で作成された、名前、メール、日付、住所などのパーソナライゼーションフィールドを利用できるようになりました。
* コンテンツの品質評価では、ブランドのガイドラインに依存せずに、読みやすさ、まとまり、有効性の問題をチェックし、不明確なメッセージ、一貫性のないトーン、構造的なギャップを特定します。 [詳細情報](../content/brands-score.md)
