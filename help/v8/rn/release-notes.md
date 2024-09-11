---
title: Campaign v8 web ユーザーインターフェイスリリースノート
description: 最新の Campaign web ユーザーインターフェイスリリースで提供される新機能について説明します
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 166623c699aa1c91b2d4e7530f5b2ea1b54507b4
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 59%

---

# リリースノート {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="リリースノート"
>abstract="Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。これにより、Campaign リリースノートは月に数回更新され、最新の機能、改善点、修正が含まれます。定期的に確認することをお勧めします。"

Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。したがって、これらのリリースノートは月に数回更新されます。定期的に確認してください。

## 9 月の更新 {#9-2024}

<table>
<thead>
<tr>
<th><strong>AI アシスタント – コンテンツアクセラレーター</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>メッセージを作成してカスタマイズしたら、Adobe Campaign Web の AI アシスタントを使用してコンテンツを次のレベルに引き上げます。 この強力なツールを使用すると、魅力的なテキスト、メインタイトル、視覚的に魅力的な画像の範囲を生成することで、コンテンツの影響を最適化できます。</p>
<p>機能を直接探索し、その機能を完全に理解できるように設計された <a href="https://experienceleague.adobe.com/en/apps/journey-optimizer/ai-assistant-content-accelerator"> ライブ機能プレビュー </a> を使用して、実践的な体験に没頭してください。</a></p>
<p>詳しくは、<a href="../email/generative-gs.md">詳細なドキュメント</a>を参照してください。</p>
<img src="assets/do-not-localize/ai-content-webui.gif"/>
</td>
</tr>
</tbody>
</table>

## 8月リリースノート {#24-8-release}

**リリース日**：2024年9月3日（PT）

次の機能と改善点は、8月のリリース以降使用できます。

* **値の配分** - パーソナライゼーションのフィールド用のリストにアクセスすると、各フィールドに値がどのように配分されているかを確認できるようになりました。専用のポップアップウィンドウに、各値の数と割合が表示されます。 [詳細情報](../query/build-query.md#distribution-values-query)

* **SMTP パラメーター** - メール配信設定で SMTP 設定が使用できるようになりました。 [詳細情報](../advanced-settings/delivery-settings.md#smtp)

* **グローバル変数** - グローバル変数を定義して、配信の値を定義できるようになりました。 [詳細情報](../advanced-settings/delivery-settings.md#variables-delivery)

### 限定提供の新機能 {#acs-24-8}

>[!AVAILABILITY]
>
>次の機能は、限定提供（LA）です。**Adobe Campaign Standard から Adobe Campaign v8** に移行するお客様に限定され、他の環境にはデプロイできません。
>
>[Campaign v8 へのCampaign Standardの移行 ](../rn/acs-migration.md) および [Campaign Standardユーザー向けの機能 ](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=ja){target="_blank"} のドキュメントページを参照してください。

* **ダイレクトメールのブランディング** - 技術管理者が 1 つまたは複数のブランドを定義して、ブランドの ID に影響を与えるパラメーターを一元化できるようになりました。ブランドのロゴ、ランディングページのアクセス URL のドメイン、メッセージトラッキングの設定などが含まれます。これらのブランドを作成して、メッセージやランディングページにリンクできるようになりました。こうした設定はテンプレートで管理されます。[詳細情報](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/branding/branding-assign)

* **ランディングページの購読** - ランディングページをサービスにリンクし、ユーザーが検証した際に確認メッセージを送信できるようになりました。 [詳細情報](../landing-pages/lp-content.md#lp-message){target="_blank"}。

* **ビジュアルフラグメント** - ビジュアルコンテンツフラグメントをアーカイブできるようになりました。 [詳細情報](../content/create-fragment.md#archive)

* **ランディングページの Captcha** - Captcha を追加して、ボットによるスパムや不正使用からランディングページを保護できるようになりました。 このメカニズムは、ユーザーによる操作が不要で、お客様のサイトとのやり取りに基づいているので、ユーザーにとっては負担になりません。[詳細情報](../landing-pages/create-lp.md#captcha)

<!--
* **Rest APIs** - As a Campaign Standard migrated user, you can now use Rest APIs to work with transactional messages. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html){target="_blank"}.-->
