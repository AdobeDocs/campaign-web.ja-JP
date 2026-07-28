---
title: Campaign v8 web ユーザーインターフェイスリリースノート
description: 最新の Campaign web ユーザーインターフェイスリリースで提供される新機能について説明します
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
  - id: c309ee4e-82e4-4f7e-b608-ef345678c34e
  - id: d5ef99fa-df0c-4153-bf94-105ad0724167
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: d9d1733854bceac52d54e02125dac92b74872c77
workflow-type: tm+mt
source-wordcount: 716
ht-degree: 23%

---

# リリースノート {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="リリースノート"
>abstract="Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。 これにより、Campaign リリースノートは月に数回更新され、最新の機能、改善点、修正が含まれます。 定期的に確認することをお勧めします。"

Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。 したがって、これらのリリースノートは月に数回更新されます。 定期的に確認してください。

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
