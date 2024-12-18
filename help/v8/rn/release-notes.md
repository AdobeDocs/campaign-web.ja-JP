---
title: Campaign v8 web ユーザーインターフェイスリリースノート
description: 最新の Campaign web ユーザーインターフェイスリリースで提供される新機能について説明します
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 344d38239df96d570a93aff9674d38b6fd375830
workflow-type: ht
source-wordcount: '418'
ht-degree: 100%

---

# リリースノート {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="リリースノート"
>abstract="Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。これにより、Campaign リリースノートは月に数回更新され、最新の機能、改善点、修正が含まれます。定期的に確認することをお勧めします。"

Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。したがって、これらのリリースノートは月に数回更新されます。定期的に確認してください。

以前のリリースで利用可能な変更と改善点については、[このページ](release-notes-24.md)を参照してください。

## 2024年10月リリース {#24-10-release}

**リリース日**：2024年10月29日（PT）

次の機能と改善点は、10月のリリース以降使用できます。

### 機能

<table>
<thead>
<tr>
<th><strong>外部アカウント</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Campaign web ユーザーインターフェイスを通じて外部アカウントを直接設定および管理できるようになりました。この新機能により、バウンスメール（POP3）や実行インスタンスなど、様々なタイプの外部アカウントを簡単に設定できます。</p>
<p>詳しくは、<a href="../administration/external-account.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>トランザクションメッセージ</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>トランザクションメッセージ（Message Center）が Campaign web ユーザーインターフェイスで使用できるようになりました。このアドオンは、情報システムからトリガーされたイベントから生成されるメッセージをトリガーする目的で設計され、請求書、注文確認、出荷確認、パスワード変更、製品入手不可通知、アカウントステートメント、web サイトアカウント作成などが含まれます。</p>
<p>詳しくは、<a href="../transactional-messaging/transactional.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>External deliveries</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now define External deliveries, and External delivery templates, in Campaign web user interface. With this mode, messages are generated in an input file which can be shared with your external provider. The External delivery mode is the default mode for the direct mail channel.</p>
</td>
</tr>
</tbody>
</table-->


### 改善点

* **ワークフローアクティビティ** - アクティビティとそのすべての子ノードをワークフロー内のトランジションから別のトランジションに移動できるようになりました。これを実行するには、アクティビティのプロパティパネルにある専用の「**移動**」ボタンを使用できます。[詳細情報](../workflows/orchestrate-activities.md#move)

* **ワークフローエンリッチメントアクティビティ**

   * **エンリッチメント**&#x200B;アクティビティで新しいフィールドを作成する際に、エイリアスとラベルを定義できるようになりました。[詳細情報](../workflows/activities/enrichment.md#collection-settings)
   * **エンリッチメント**&#x200B;アクティビティで各プロファイルに対してオファーを追加できるようになりました。[詳細情報](../workflows/activities/enrichment.md##add-offers)

* **値の配分** - パーソナライゼーション用のフィールドリストにアクセスすると、各フィールドに値がどのように配分されているかを確認できるようになりました。専用のポップアップウィンドウに、各値の数と割合が表示されます。[詳細情報](../query/build-query.md#distribution-values-query)

* **バージョンおよびシステム情報** - クライアントコンソールと web ユーザーインターフェイスの両方で、インスタンスバージョンに関する詳細にアクセスできるようになりました。この新しいセクションには、環境にインストールされているすべてのビルトインパッケージも一覧表示されます。[詳細情報](../get-started/user-interface.md#user-interface-about)

* **リスト** - リストの値を簡単に並べ替えることができるようになりました。[詳細情報](../get-started/work-with-folders.md)

* **配信** - 配信変数にパーソナライゼーションフィールドからアクセスできるようになりました。[詳細情報](../personalization/conditions.md#use-variables-for-conditional-content-variables-conditional)