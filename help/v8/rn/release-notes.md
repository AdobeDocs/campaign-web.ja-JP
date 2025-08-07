---
title: Campaign v8 web ユーザーインターフェイスリリースノート
description: 最新の Campaign web ユーザーインターフェイスリリースで提供される新機能について説明します
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 127c65a466c41e1aba8408aa9cf41c2d89c93801
workflow-type: ht
source-wordcount: '900'
ht-degree: 100%

---

# リリースノート {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="リリースノート"
>abstract="Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。これにより、Campaign リリースノートは月に数回更新され、最新の機能、改善点、修正が含まれます。定期的に確認することをお勧めします。"

Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。したがって、これらのリリースノートは月に数回更新されます。定期的に確認してください。

以前のリリースで利用可能な変更と改善点について詳しくは、[2024](release-notes-24.md) ページと [2025](release-notes-25.md) ページを参照してください。

## 2025年7月リリース {#25-7-release}

### 新機能 {#25-7-features}

次の機能は、7月のリリース以降使用できます。

<!--table>
<thead>
<tr>
<th><strong>Multilingual email and SMS</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now send multiple email and SMS deliveries in different languages in Adobe Campaign Web UI. The multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen.
</p>
<p>For Multilingual email, your server must be upgraded to 8.8.1 minimum. Refer to the Client Console <a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=ja" target="_blank">release notes</a>.
<p>For more information, refer to the <a href="../email/edit-content.md#multilingual-delivery">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Custom channel for API deliveries</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now, directly from Adobe Campaign Web UI, orchestrate and execute deliveries based on custom API channels. These deliveries can be standalone or part of a workflow. The configuration of the custom API channel is performed in the console.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<table>
<thead>
<tr>
<th><strong>E メールデザイナーでのカスタム CSS のサポート</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>メールをデザインする際に、E メールデザイナー内で独自のカスタム CSS を直接追加できるようになりました。この機能により、コンテンツの外観に対する柔軟性と制御を高めるのに、高度で特定のスタイルを適用できます。</p>
<p>詳しくは、<a href="../email/custom-css.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>ブランド</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>独自のブランドを作成およびカスタマイズし、コミュニケーション全体で視覚的および言語的な ID を明確に定義できるようになりました。ブランド整合性スコアを使用すると、コンテンツがブランドのトーン、スタイル、ガイドラインをどの程度反映しているかに関するフィードバックをリアルタイムで受信でき、送信するすべてのメッセージでブランドに即して一貫性を保つことができます。
</p>
<p>詳しくは、<a href="../content/brands.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>配信アラート</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>配信アラート機能は、配信の実行に関する情報を含んだ通知をユーザーグループが自動的に受信できるようにするアラート管理システムです。</p>
<p>詳しくは、<a href="../msg/delivery-alerting.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>Landing pages improvements</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The following improvements to landing pages are now available:</p>
<ul>
    <li>You can now reference a default subscription/unsubscription landing page when configuring a service. When designing an email, if you define a link to that landing page, users submitting the landing page form are automatically subscribed to or unsubscribed from this service. <a href="../audience/manage-services.md#create-service">Read more</a></li>
    <li>A new option in the landing page configuration allows anonymous visitors to access the landing page. If you unselect this option, only identified users can access and submit the form. <a href="../landing-pages/create-lp.md#create-landing-page">Read more</a></li>
    <li>A new option in the landing page configuration allows to store additional internal data when the landing page is being submitted. <a href="../landing-pages/create-lp.md#create-landing-page">Read more</a></li>
    <li>A new option enables to use a landing page for several services, making it dynamic. When adding a link to an email, if you select a dynamic landing page, you can select any service. If you select a landing page that has a specific service associated, this service will be automatically used (you cannot select another one). <a href="../landing-pages/create-lp.md#define-actions-on-form-submission">Read more</a></li>
    <li>Conditional content is now supported in landing pages. <a href="../landing-pages/lp-content.md">Read more</a></li>
    <li>You can link a landing page to a service, and send a confirmation message when users validate it. <a href="../landing-pages/lp-content.md#lp-message">Read more</a></li>
    <li>You can add captcha to protect your landing page from spam and abuse caused by bots. This is non-intrusive for your customers since it does not require any interaction from them and is based on interactions with your site. <a href="../landing-pages/create-lp.md#captcha">Read more</a></li>
</ul>
</td>
</tr>
</tbody>
</table-->


<table>
<thead>
<tr>
<th><strong>動的レポート</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>マーケティングアクティビティの影響を測定する完全にカスタマイズ可能なリアルタイムのレポートを提供する動的レポートにアクセスできるようになりました。プロファイルデータへのアクセスが追加され、開封数やクリック数などの機能的なメールキャンペーンデータに加えて、性別、市区町村、年齢などのプロファイルディメンション別のデモグラフィック分析が可能になります。また、動的レポートは、多言語のメール配信とトランザクションメッセージにも使用できます。</p>
<p>この機能は、オンデマンドでのみ使用できます。アクセスするには、アドビ担当者にお問い合わせください。サーバーは 8.8.1 以上にアップグレードする必要があります。詳しくは、クライアントコンソール<a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=ja" target="_blank">リリースノート</a>を参照してください。
<p>詳しくは、<a href="../reporting/dynamic-reporting/get-started-reporting.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>一元化されたブランディング</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>技術管理者が 1 つまたは複数のブランドを定義して、ブランドの ID に影響を与えるパラメーターを一元化できるようになりました。ブランドのロゴ、ランディングページのアクセス URL のドメイン、メッセージトラッキングの設定などが含まれます。これらのブランドを作成して、メッセージやランディングページにリンクできます。こうした設定はテンプレートで管理されます。ブランディングオプションは、SMS やダイレクトメールを含むすべてのチャネルで使用できます。</p>
<p>この機能は、新しい実装でのみオンデマンドで使用できます。アクセスするには、アドビ担当者にお問い合わせください。サーバーは 8.8.1 以上にアップグレードする必要があります。詳しくは、クライアントコンソール<a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=ja" target="_blank">リリースノート</a>を参照してください。
<p>詳しくは、<a href="../administration/branding/branding-gs.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

このリリースには、上記の機能に加えて、クライアントコンソールで使用できる一連の機能も付属しています。

* [新しい SMS 送信コネクタ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html?lang=ja)（FDA 環境）
* [Rest API](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=ja)（オンデマンド、FDA 環境）

詳しくは、クライアントコンソール[リリースノート](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=ja){target="_blank"}を参照してください。

<!--

### Features previously in Limited Availability {#25-7-limited} 

>[!AVAILABILITY]
>
>To benefit from these updates, your server must be upgrated to 8.8.1 mininum. Refer to the Client Console [release notes](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=ja){target="_blank"}.

Previously released in Limited Availability, the following capabilities are now available to all environments (General Availability):

* **Multilingual delivery creation** - You can now send multiple email deliveries in different languages in Adobe Campaign Web User Interface. The Multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen. [Read more](../email/edit-content.md#multilingual-delivery).


* **Visual fragments** - You can now create, use and archive content fragments. Visual fragments are pre-defined visual blocks that you can reuse across multiple email deliveries, or in content templates. [Learn more](https://experienceleague.adobe.com/docs/campaign-web/v8/content/manage-reusable-content/fragments/fragments.html?lang=ja){target="_blank"}

* **Delivery alerting** - The Delivery alerting feature is an alert management system that enables a group of users to automatically receive notifications containing information on the execution of their deliveries. [Read more](../msg/delivery-alerting.md)


* **Landing pages improvements** - The following improvements to landing pages are now available:

    * You can now reference a default subscription/unsubscription landing page when configuring a service. When designing an email, if you define a link to that landing page, users submitting the landing page form are automatically subscribed to or unsubscribed from this service. [Read more](../audience/manage-services.md#create-service)
    * A new option in the landing page configuration allows anonymous visitors to access the landing page. If you unselect this option, only identified users can access and submit the form. [Read more](../landing-pages/create-lp.md#create-landing-page)
    * A new option in the landing page configuration allows to store additional internal data when the landing page is being submitted. [Read more](../landing-pages/create-lp.md#create-landing-page)
    * A new option enables to use a landing page for several services, making it dynamic. When adding a link to an email, if you select a dynamic landing page, you can select any service. If you select a landing page that has a specific service associated, this service will be automatically used (you cannot select another one). [Read more](../landing-pages/create-lp.md#define-actions-on-form-submission)
    * Conditional content is now supported in landing pages. [Read more](../landing-pages/lp-content.md)
    * You can link a landing page to a service, and send a confirmation message when users validate it. [Learn more](../landing-pages/lp-content.md#lp-message)
    * You can add captcha to protect your landing page from spam and abuse caused by bots. This is non-intrusive for your customers since it does not require any interaction from them and is based on interactions with your site. [Learn more](../landing-pages/create-lp.md#captcha)

Previously released in Limited Availability, the following capabilities are now available **on demand**:

* **Dynamic Reporting** - You can now access Dynamic Reporting which provides fully customizable and real-time reports to measure the impact of your marketing activities. It adds access to profile data, enabling demographic analysis by profile dimensions such as gender, city and age in addition to functional email campaign data like opens and clicks. Dynamic reporting is also available for multilingual email deliveries and transactional messages. [Read more](../reporting/dynamic-reporting/get-started-reporting.md)

* **Centralized Branding** -  Your technical administrators can now define one or several brands to centralize the parameters that affect a brand's identity. This includes the brand logo, the domain of the landing pages' access URL, or message tracking settings. You can create these brands and link them to messages or landing pages. This configuration is managed in templates. Branding options are available for all channels, including SMS and Direct mail. [Read more](../administration/branding/branding-gs.md){target="_blank"}

    >[!NOTE]
    >
    >This feature is only available for new implementations.

In addition to the features listed above, this release also comes with a set of functionalities available in the Client Console:

* [New SMS sending connector](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html?lang=ja) (FDA environments)
* [Rest APIs](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=ja) (on demand, FDA environments)

Refer to the Client Console [release notes](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=ja){target="_blank"}.

-->

### 機能強化 {#25-7-improvements}

* ルールビルダーで、各条件とグループに対してターゲット母集団を直接計算できるようになりました。レコードの詳細なリストを表示するには、結果番号をクリックします。[詳細情報](../query/build-query.md#validate-query)

* 定義済みフィルターをルールビルダーから直接編集または削除できるようになりました。[詳細情報](../get-started/predefined-filters.md#manage-predefined-filter)

* SMS 配信を設定する際に、「**SMS**」セクションで&#x200B;**オプションの SMPP パラメーター（TLV）**&#x200B;にアクセスできるようになりました。このパラメーターは、クライアントコンソールの場合と同じです。[詳細情報](../advanced-settings/delivery-settings.md#sms-tab)

* iOS コンテンツ編集画面の「**詳細設定**」セクションにある新しい「**コンテンツ使用可能**」オプションを使用して、iOS でバックグラウンド通知を有効にできるようになりました。これにより、`aps` ペイロードに `content-available:1` フラグが追加されます。詳しくは、[このページ](../push/content-push.md)を参照してください。また、[このページ](../push/rich-push-ios.md)も参照してください

* ランディングページの次の機能強化が使用できるようになりました。

   * サービスの設定時に、デフォルトの購読／購読解除のランディングページを参照できるようになりました。メールのデザイン時に、そのランディングページへのリンクを定義すると、ランディングページフォームを送信したユーザーは、このサービスに自動的に購読または登録解除されます。[詳細情報](../audience/manage-services.md#create-service)
   * ランディングページ設定の新しいオプションでは、匿名訪問者がランディングページにアクセスできます。このオプションを選択解除すると、識別されたユーザーのみがフォームにアクセスして送信できます。[詳細情報](../landing-pages/create-lp.md#create-landing-page)
   * ランディングページ設定の新しいオプションでは、ランディングページの送信時に追加の内部データを保存できます。[詳細情報](../landing-pages/create-lp.md#create-landing-page)
   * 新しいオプションでは、複数のサービスにランディングページを使用し、動的にすることができます。メールへのリンクの追加時に、動的ランディングページを選択すると、任意のサービスを選択できます。特定のサービスが関連付けられているランディングページを選択すると、このサービスが自動的に使用されます（別のサービスは選択できません）。[詳細情報](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * ランディングページで条件付きコンテンツがサポートされるようになりました。[詳細情報](../landing-pages/lp-content.md)
   * ランディングページをサービスにリンクして、ユーザーが検証する際に確認メッセージを送信できます。[詳細情報](../landing-pages/lp-content.md#lp-message)
   * Captcha を追加して、ボットによるスパムや不正使用からランディングページを保護できます。このメカニズムは、ユーザーによる操作が不要で、お客様のサイトとのやり取りに基づいているので、ユーザーにとっては負担になりません。[詳細情報](../landing-pages/create-lp.md#captcha)
