---
title: Campaign v8 web ユーザーインターフェイスリリースノート
description: 最新の Campaign web ユーザーインターフェイスリリースで提供される新機能について説明します
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 62294ce1809caee8af770b376aad97bac71c942c
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 65%

---

# リリースノート {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="リリースノート"
>abstract="Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。これにより、Campaign リリースノートは月に数回更新され、最新の機能、改善点、修正が含まれます。定期的に確認することをお勧めします。"

Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。したがって、これらのリリースノートは月に数回更新されます。定期的に確認してください。

以前のリリースで利用可能な変更と改善点について詳しくは、[2024](release-notes-24.md) と [2025](release-notes-25.md) を参照してください。

## 2025 年 7 月の更新 {#25-7-updates}

>[!AVAILABILITY]
>
>これらのアップデートのメリットを享受するには、サーバーを 8.8.1 分にアップグレードする必要があります。 クライアントコンソール [ リリースノート ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=ja){target="_blank"} を参照してください。

以前リリースされた限定提供（LA）では、次の機能がすべての環境で利用できるようになりました（一般提供）。

* **多言語配信の作成** - Adobe Campaign web ユーザーインターフェイスで、複数のメール配信を異なる言語で送信できるようになりました。多言語配信機能を使用すると、配信のデフォルト言語と、配信を送信できる様々な言語を選択できます。また、選択した言語でこれらの配信をプレビューすることもできます。[詳細情報](../email/edit-content.md#multilingual-delivery)。

<!--
* **Visual fragments** - You can now create, use and archive content fragments. Visual fragments are pre-defined visual blocks that you can reuse across multiple email deliveries, or in content templates. [Learn more](https://experienceleague.adobe.com/docs/campaign-web/v8/content/manage-reusable-content/fragments/fragments.html?lang=ja){target="_blank"}
-->

* **配信アラート** – 配信アラート機能は、ユーザーのグループが配信の実行に関する情報を含んだ通知を自動的に受信できるアラート管理システムです。 [詳細情報](../msg/delivery-alerting.md)

* **ランディングページの改善** - ランディングページが次のように改善されました。

   * サービスの設定時に、デフォルトの購読／購読解除のランディングページを参照できるようになりました。メールのデザイン時に、そのランディングページへのリンクを定義すると、ランディングページフォームを送信したユーザーは、このサービスに自動的に購読または登録解除されます。[詳細情報](../audience/manage-services.md#create-service)
   * ランディングページ設定の新しいオプションでは、匿名訪問者がランディングページにアクセスできます。このオプションを選択解除すると、識別されたユーザーのみがフォームにアクセスして送信できます。[詳細情報](../landing-pages/create-lp.md#create-landing-page)
   * ランディングページ設定の新しいオプションでは、ランディングページの送信時に追加の内部データを保存できます。[詳細情報](../landing-pages/create-lp.md#create-landing-page)
   * 新しいオプションでは、複数のサービスにランディングページを使用し、動的にすることができます。メールへのリンクの追加時に、動的ランディングページを選択すると、任意のサービスを選択できます。特定のサービスが関連付けられているランディングページを選択すると、このサービスが自動的に使用されます（別のサービスは選択できません）。[詳細情報](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * ランディングページで条件付きコンテンツがサポートされるようになりました。[詳細情報](../landing-pages/lp-content.md)
   * ランディングページをサービスにリンクし、ユーザーが検証したときに確認メッセージを送信できます。 [詳細情報](../landing-pages/lp-content.md#lp-message)
   * Captcha を追加すると、ボットによるスパムや不正使用からランディングページを保護できます。 このメカニズムは、ユーザーによる操作が不要で、お客様のサイトとのやり取りに基づいているので、ユーザーにとっては負担になりません。[詳細情報](../landing-pages/create-lp.md#captcha)

以前は限定提供（LA）でリリースされていましたが、現在は次の機能が **オンデマンド** で利用できます。

* **動的レポート** – 完全にカスタマイズ可能なリアルタイムのレポートを提供する動的レポートにアクセスして、マーケティングアクティビティの影響を測定できるようになりました。 プロファイルデータへのアクセスが追加され、開封数やクリック数などの機能的なメールキャンペーンデータに加えて、性別、市区町村、年齢などのプロファイルディメンション別のデモグラフィック分析を可能にします。動的レポートは、多言語のメール配信とトランザクションメッセージにも使用できます。 [詳細情報](../reporting/dynamic-reporting/get-started-reporting.md)

* **ブランディングの一元化** – 技術管理者は、1 つまたは複数のブランドを定義して、ブランドの ID に影響を与えるパラメーターを一元化できるようになりました。 ブランドのロゴ、ランディングページのアクセス URL のドメイン、メッセージトラッキングの設定などが含まれます。これらのブランドを作成して、メッセージやランディングページにリンクできます。こうした設定はテンプレートで管理されます。ブランディングオプションは、SMS やダイレクトメールを含むすべてのチャネルで使用できます。 [詳細情報](../administration/branding/branding-gs.md){target="_blank"}

  >[!NOTE]
  >
  >この機能は、新規実装でのみ使用できます。

このリリースには、上記の機能に加えて、クライアントコンソールで使用できる一連の機能も付属しています。

* [ 新しい SMS 送信コネクタ ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html?lang=ja)。
* [Rest API](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html)

クライアントコンソール [ リリースノート ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=ja){target="_blank"} を参照してください。

<!--
ACC * **Branding** - Branding options are now available for all channels, including SMS and Direct mail. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html?lang=ja){target="_blank"}
web - * **Branding for Direct Mail** - Technical administrators can now define one or several brands to centralize the parameters that affect a brand's identity. This includes the brand logo, the domain of the landing pages' access URL, or message tracking settings. You can now create these brands and link them to messages or landing pages. This configuration is managed in templates. [Learn more](https://experienceleague.adobe.com/ja/docs/experience-cloud/campaign/branding/branding-assign)
ACC - Branding - As a Campaign Standard migrated user, your technical administrators can now define one or several brands to centralize the parameters that affect a brand’s identity. This includes the brand logo, the domain of the landing pages’ access URL, or message tracking settings. You can create these brands and link them to messages or landing pages. This configuration is managed in templates. Read more
Previously released in Limited Availability, the following capability is now available **on demand, only for [Campaign FDA deployments](../architecture/fda-deployment.md)**. To gain access, contact your Adobe representative.
Previously released in Limited Availability, the following capability is now available by default **for new implementations**, and available **on demand for existing environments**. To gain access, contact your Adobe representative.
Previously released in Limited Availability, the following capability is now available **on demand**. To gain access, contact your Adobe representative.
-->