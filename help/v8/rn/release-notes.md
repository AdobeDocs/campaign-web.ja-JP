---
title: Campaign v8 web ユーザーインターフェイスリリースノート
description: 最新の Campaign web ユーザーインターフェイスリリースで提供される新機能について説明します
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: e9022e53ff8733ecdfcca1aec2ba31ca6c79c3ad
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 52%

---

# リリースノート {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="リリースノート"
>abstract="Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。これにより、Campaign リリースノートは月に数回更新され、最新の機能、改善点、修正が含まれます。定期的に確認することをお勧めします。"

Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。したがって、これらのリリースノートは月に数回更新されます。定期的に確認してください。

## 8 月のリリースノート {#24-8-release}

**リリース日**:2024 年 9 月 3 日（PT）

8 月のリリース以降、次の機能および改善点が提供されます。

* **値の配分** - パーソナライゼーションのフィールドのリストにアクセスする際に、各フィールドの値の配分方法を確認できるようになりました。 専用のポップアップウィンドウに、各値の数と割合が表示されます。 [詳細情報](../query/build-query.md#distribution-values-query)

* **SMTP パラメーター** - メール配信設定で SMTP 設定が使用できるようになりました。 [詳細情報](../advanced-settings/delivery-settings.md#smtp)

* **グローバル変数** - グローバル変数を定義して、配信の値を定義できるようになりました。 [詳細情報](../advanced-settings/delivery-settings.md#variables-delivery)

### 限定提供の新機能 {#acs-24-8}

>[!AVAILABILITY]
>
>次の機能は、限定提供（LA）です。**Adobe Campaign Standard から Adobe Campaign v8** に移行するお客様に限定され、他の環境にはデプロイできません。
>
>[Campaign v8 へのCampaign Standardの移行 ](../rn/acs-migration.md) および [Campaign Standardユーザー向けの機能 ](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=ja){target="_blank"} のドキュメントページを参照してください。

* **ダイレクトメールのブランディング** – 技術管理者は、1 つまたは複数のブランドを定義して、ブランドの ID に影響を与えるパラメーターを一元化できるようになりました。 ブランドのロゴ、ランディングページのアクセス URL のドメイン、メッセージトラッキングの設定などが含まれます。これらのブランドを作成し、メッセージやランディングページにリンクできるようになりました。 こうした設定はテンプレートで管理されます。[詳細情報](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/branding/branding-assign)

* **ランディングページの購読** - ランディングページをサービスにリンクし、ユーザーが検証した際に確認メッセージを送信できるようになりました。 [詳細情報](../landing-pages/lp-content.md#lp-message){target="_blank"}。

* **ビジュアルフラグメント** - ビジュアルコンテンツフラグメントをアーカイブできるようになりました。 [詳細情報](../content/create-fragment.md#archive)

* **ランディングページの Captcha** - Captcha を追加して、ボットによるスパムや不正使用からランディングページを保護できるようになりました。 このメカニズムは、ユーザーによる操作が不要で、お客様のサイトとのやり取りに基づいているので、ユーザーにとっては負担になりません。[詳細情報](../landing-pages/create-lp.md#captcha)

<!--
* **Rest APIs** - As a Campaign Standard migrated user, you can now use Rest APIs to work with transactional messages. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html){target="_blank"}.-->
