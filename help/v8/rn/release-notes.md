---
title: Campaign v8 web ユーザーインターフェイスリリースノート
description: 最新の Campaign web ユーザーインターフェイスリリースで提供される新機能について説明します
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: ef040ec079961771b734208ecf8ac9e510b38104
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 69%

---

# リリースノート {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="リリースノート"
>abstract="Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。これにより、Campaign リリースノートは月に数回更新され、最新の機能、改善点、修正が含まれます。定期的に確認することをお勧めします。"

Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。したがって、これらのリリースノートは月に数回更新されます。定期的に確認してください。

## 10 月リリース {#24-10-release}

**リリース日**: 2024 年 10 月 29 日（PT）

10 月のリリース以降、次の機能および機能強化が利用可能になります。

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
<p>Adobe Campaign web ユーザーインターフェイスから直接外部アカウントを設定および管理できるようになりました。 この新機能により、バウンスメール（POP3）や実行インスタンスなど、様々なタイプの外部アカウントを簡単に設定できます。</p>
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
<p>Campaign web ユーザーインターフェイスで、トランザクションメッセージを作成および監視できるようになりました。 トランザクションメッセージは、Adobe Campaignの特殊なモジュールで、トリガーメッセージを処理するために設計されています。 これらのメッセージは、情報システムからのイベントに応答して自動的に生成されます。 このようなイベントの一般的な例としては、ボタンやリンクのクリック、買い物かごの放棄、製品可用性アラートのリクエスト、アカウントの作成や変更などがあります。</p>
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

* **ワークフローアクティビティ** - アクティビティとそのすべての子ノードをワークフロー内のトランジションから別のトランジションに移動できるようになりました。 アクティビティのプロパティパネルに、これを実行するための専用の **移動** ボタンが表示されます。 [詳細情報](../workflows/orchestrate-activities.md#move)

* **ワークフローエンリッチメントアクティビティ**

   * **エンリッチメント** アクティビティで新しいフィールドを作成する際に、エイリアスとラベルを定義できるようになりました。 [詳細情報](../workflows/activities/enrichment.md#collection-settings)
   * **エンリッチメント** アクティビティの各プロファイルにオファーを追加できるようになりました。 [詳細情報](../workflows/activities/enrichment.md##add-offers)

* **値の配分** - パーソナライゼーション用のフィールドリストにアクセスすると、各フィールドに値がどのように配分されているかを確認できるようになりました。専用のポップアップウィンドウに、各値の数と割合が表示されます。[詳細情報](../query/build-query.md#distribution-values-query)


## 9月の更新 {#9-2024}

<table>
<thead>
<tr>
<th><strong>AI アシスタントコンテンツアクセラレータ</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>メッセージを作成してカスタマイズしたら、Adobe Campaign Web の AI アシスタントコンテンツアクセラレーターを使用して次のレベルに進めます。 この強力なツールを使用すると、様々な魅力的なテキスト、メインタイトル、視覚的に魅力的な画像を生成することで、コンテンツの影響を最適化できます。</p>
<p><a href="https://experienceleague.adobe.com/ja/apps/journey-optimizer/ai-assistant-content-accelerator">ライブ機能プレビュー</a>は、実際に体験して、その機能を直接探索し、その機能を完全に理解できるように設計されています。</a></p>
<p>詳しくは、<a href="../email/generative-gs.md">詳細なドキュメント</a>を参照してください。</p>
<img src="assets/do-not-localize/ai-content-webui.gif"/>
<p>公開日：9月12日（PT）</p>
</td>
</tr>
</tbody>
</table>

## 8 月リリース {#24-8-release}

**リリース日**：2024年9月3日（PT）

次の機能と改善点は、8月のリリース以降使用できます。

* **SMTP パラメーター** - メール配信設定で SMTP 設定が使用できるようになりました。[詳細情報](../advanced-settings/delivery-settings.md#smtp)

* **グローバル変数** - グローバル変数を定義して、配信の値を定義できるようになりました。[詳細情報](../advanced-settings/delivery-settings.md#variables-delivery)

### 限定提供の新機能 {#acs-24-8}

>[!AVAILABILITY]
>
>次の機能は、限定提供（LA）です。**Adobe Campaign Standard から Adobe Campaign v8** に移行するお客様に限定され、他の環境にはデプロイできません。
>
>ドキュメントページの [Campaign v8 への Campaign Standard の移行](../rn/acs-migration.md)および [Campaign Standard ユーザー向けの機能](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=ja){target="_blank"}を参照してください。

* **ダイレクトメールのブランディング** - 技術管理者が 1 つまたは複数のブランドを定義して、ブランドの ID に影響を与えるパラメーターを一元化できるようになりました。ブランドのロゴ、ランディングページのアクセス URL のドメイン、メッセージトラッキングの設定などが含まれます。これらのブランドを作成して、メッセージやランディングページにリンクできるようになりました。こうした設定はテンプレートで管理されます。[詳細情報](https://experienceleague.adobe.com/ja/docs/experience-cloud/campaign/branding/branding-assign)

* **ランディングページによるサブスクリプション** - ランディングページをサービスにリンクして、ユーザーが検証する際に確認メッセージを送信できるようになりました。[詳細情報](../landing-pages/lp-content.md#lp-message){target="_blank"}。

* **ビジュアルフラグメント** - ビジュアルコンテンツフラグメントをアーカイブできるようになりました。[詳細情報](../content/create-fragment.md#archive)

* **ランディングページの Captcha** - Captcha を追加して、ボットによるスパムや不正使用からランディングページを保護できるようになりました。このメカニズムは、ユーザーによる操作が不要で、お客様のサイトとのやり取りに基づいているので、ユーザーにとっては負担になりません。[詳細情報](../landing-pages/create-lp.md#captcha)

<!--
* **Rest APIs** - As a Campaign Standard migrated user, you can now use Rest APIs to work with transactional messages. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html){target="_blank"}.-->
