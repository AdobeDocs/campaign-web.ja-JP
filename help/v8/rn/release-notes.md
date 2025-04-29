---
title: Campaign v8 web ユーザーインターフェイスリリースノート
description: 最新の Campaign web ユーザーインターフェイスリリースで提供される新機能について説明します
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: e825b7859bff299906725eddf3ba014ed0b5e1b7
workflow-type: tm+mt
source-wordcount: '689'
ht-degree: 35%

---

# リリースノート {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="リリースノート"
>abstract="Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。これにより、Campaign リリースノートは月に数回更新され、最新の機能、改善点、修正が含まれます。定期的に確認することをお勧めします。"

Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。したがって、これらのリリースノートは月に数回更新されます。定期的に確認してください。

以前のリリースで使用可能な変更と改善点は、[2024](release-notes-24.md) および [2025](release-notes-25.md) に記載されています。

## 2025 年 4 月リリース {#25-4-release}

**リリース日**：2025年4月29日（PT）


### 新機能 {#25-4-features}

次の機能は、4月のリリース以降、すべてのユーザーが使用できます。

<table>
<thead>
<tr>
<th><strong>コールセンターチャネル</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>コールセンターチャネルを Campaign web ユーザーインターフェイスで使用できるようになりました。 このチャネルは、コールセンター（通常、エージェントによる顧客や見込み客への電話）を介して処理されるコミュニケーションやインタラクションを管理および追跡するために使用される通信方法を指します。</p>
<img src="assets/do-not-localize/call-center.gif">
<p>詳しくは、<a href="../call-center/gs-call-center.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>新規ルールビルダー</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>改善されたユーザーインターフェイスで複雑な条件を定義するのに役立つ、新しいルールビルダーが使用できるようになりました。 必要に応じて、古いルールビルダーから新しいルールビルダーに切り替えることができます。</p>
<img src="assets/do-not-localize/rule-builder-release.gif">
<p>詳しくは、<a href="../query/query-modeler-overview.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>外部アカウントのオーサリング</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Campaign 管理者は、Campaign web ユーザーインターフェイスから外部システムとの新しい接続を設定できるようになりました。
また、既存の外部アカウントを表示、更新、管理することもできます。</p>
<p>詳しくは、<a href="../administration/external-account.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

### 改善点 {#25-4-improvements}

**全般的なインターフェイスの改善**

* スキーマ属性のフィールドの説明、お気に入りに追加、値の配分のオプションがユーザーインターフェイスに表示されるようになりました。 詳しくは、[詳細なドキュメント](../get-started/attributes.md)を参照してください。
* Experience Leagueの環境設定で指定されたプライマリ言語に従って、日時がインターフェイスに表示されるようになりました。 この機能強化は、複数の言語でのみ使用できます。 サポートされる言語の完全なリストを確認するには、[ 詳細なドキュメント ](https://experienceleague.adobe.com/en/docs/core-services/interface/features/browser-language){target=_blank} を参照してください。

<!--
ko * Built-in options are now only visible in the list of options if the **Show advanced options** toggle is activated.
ko * The typology rules creation screen has been updated to facilitate the selection of the type of rule.
-->

**メールエディター**:Campaign web UI のアクセシビリティを強化するために、メールDesignerで 2 つの新しいフィールドが使用できるようになりました。これらは、メールコンテンツの `html` 要素の `title` 要素と lang 属性に対応しています。 「メール本文」セクションでは、プリヘッダーフィールドに加えて、これらの設定を定義できます。 詳しくは、[詳細なドキュメント](../email/metadata.md)を参照してください。

<!--
**Workflow**: You can now select an existing Javascript code in workflow properties or in a Javascript activity.    
-->

**スキーマ**

* Campaign web ユーザーインターフェイスからリストの一時スキーマを編集できるようになりました。 詳しくは、[詳細なドキュメント](../audience/manage-audience.md)を参照してください。
* サンプル画面でスキーマのカスタムフィールドをプレビューできるようになりました。 詳しくは、[詳細なドキュメント](../administration/custom-fields.md#add)を参照してください。
* ドラッグ&amp;ドロップを使用して、リスト内のカスタムフィールドを移動できるようになりました。 詳しくは、[詳細なドキュメント](../administration/custom-fields.md#add)を参照してください。


### 限定提供の新機能 {#25-4-features-la}

>[!AVAILABILITY]
>
>次の機能は、限定提供（LA）です。**Adobe Campaign StandardからAdobe Campaign v8 に** 移行するお客様に限定され、他の環境にデプロイすることはできません。 Campaign サーバーを v8.7.4 にアップグレードする必要があります。
>
>ドキュメントページの [Campaign v8 への Campaign Standard の移行](../rn/acs-migration.md)および [Campaign Standard ユーザー向けの機能](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=ja)を参照してください。

* **多言語配信の作成** - Adobe Campaign web ユーザーインターフェイスで、複数のメール配信を異なる言語で送信できるようになりました。 多言語配信機能を使用すると、配信のデフォルト言語と、配信を送信する様々な言語を選択できます。 また、選択した言語でこれらの配信をプレビューすることもできます。 詳しくは、[詳細なドキュメント](../email/edit-content.md)を参照してください。

* **多言語用の動的レポート** – 動的レポートが多言語メール配信で使用できるようになりました。 詳しくは、[詳細なドキュメント](../reporting/global-reports.md)を参照してください。

* **SMS REST API サポート（LA）** - トランザクションメッセージ REST API を SMS チャネルで使用できるようになりました。 ペイロードにメールと携帯電話の両方が存在する場合は、「wishedChannel」フィールドを使用してチャネルを指定できます。 指定しない場合、wishedChannel が SMS を明示的にリクエストしない限り、メールがデフォルトで使用されます。 詳しくは、[詳細なドキュメント](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/apis/managing-transactional-messages){target=_blank}を参照してください。

