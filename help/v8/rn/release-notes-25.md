---
title: Campaign v8 web ユーザーインターフェイスの以前のリリースノート
description: 2025 Campaign web ユーザーインターフェイスリリース
exl-id: eecb4b18-4826-47a6-88b2-f2ed7b576d3e
source-git-commit: 934a37cfebfacd2df0b7610285252d883611f252
workflow-type: tm+mt
source-wordcount: '2667'
ht-degree: 100%

---

# 2025 リリースノート {#2025-release}

このページには、**2025 リリース**&#x200B;で使用可能なすべての変更点と改善点が記載されています。最新のリリースノートについて詳しくは、[このページ](release-notes.md)を参照してください。

## 2025年9月リリース {#25-9-release}

_2025年9月23日（PT）_

次の機能は、9月のリリース以降使用できます。

<table>
<thead>
<tr>
<th><strong>API 配信のカスタムチャネル</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Campaign web UI から直接、カスタム API チャネルに基づいて配信を調整および実行できるようになりました。これらの配信は、スタンドアロンで行うか、ワークフローの一部として行うことができます。カスタム API チャネルの設定は、コンソールで実行します。</p>
<p>詳しくは、<a href="../call-center/gs-custom-channel.md">詳細なドキュメント</a>を参照してください。</p>
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
<p>Campaign 管理者は、Campaign web ユーザーインターフェイスから外部システムとの新しい接続を設定できるようになりました。また、既存の外部アカウントを表示、更新、管理することもできます。</p>
<p>詳しくは、<a href="../administration/create-external-account.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>メールコンテンツのロック</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Campaign では、テンプレート全体または特定の構造とコンポーネントをロックして、メールテンプレート内のコンテンツをロックできるようになりました。これにより、意図しない編集や削除を防ぎ、テンプレートのカスタマイズをより細かく制御して、メールキャンペーンの効率と信頼性を向上させることができます。</p>
<p>詳しくは、<a href="../content/content-locking.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>Integration with Adobe GenStudio</strong><br/></th>  LA? sort? Juliette
</tr>
</thead>
<tbody>
<tr>
<td>
<p>To enhance marketing efficiency and to maintain brand consistency, you can now seamlessly integrate GenStudio for Performance Marketing experiences with Campaign. This enables you to leverage GenStudio's AI-power content creation alongside Campaign's advanced orchestration capabilities.<p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Dark mode support in the Email designer</strong><br/></th> -> pas sept, modifier composant... -> Juliette
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The Email Designer now offers the ability to switch to dark mode view, where you can additionally define specific custom settings. Note that the final rendering depends on the recipient's email client, and not all email clients support dark mode.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>>
<thead>
<tr>
<th><strong>Multilingual capabilities for transactional messaging and push notifications (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now send multiple transactional messages and push notifications in different languages in Adobe Campaign Web User Interface. The Multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen.</p>
<p>Note: this capability is only available for a set of organizations (Limited Availability), and will be rolled out globally in a future release.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Profile enrichment in Transactional Messages (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>This capability allows you to personalize transactional messages (Email, SMS, Push) by linking Adobe Campaign database fields to the message content. You can select target mappings, enrichment columns, and a reconciliation key to ensure accurate, real-time personalization while maintaining performance thresholds.</p>
<p>Note: this capability is only available for a set of organizations (Limited Availability), and will be rolled out globally in a future release.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Dynamic reporting for transactional messaging (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Note: this capability is only available for a set of organizations (Limited Availability), and will be rolled out globally in a future release.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->


### 機能強化 {#25-9-improvements}

* E メールデザイナーの条件付きコンテンツ機能を使用して条件を設定する際に、新しい演算子のセットが追加されました。
* フィルタリングディメンションが&#x200B;**オーディエンスを作成**&#x200B;ワークフローアクティビティで使用できるようになりました。表示または変更するには、ターゲティングディメンションの横にあるアイコンをクリックします。[詳細情報](../workflows/activities/build-audience.md#build-audience-configuration)。
<!--

NEO-84915 Stop button for deliveries???? ->>> met pas, juste bouton ajouté dans webUI meme comportement que console. bleu, marche, marche pas.
NEO-90345 WebUI - Extended operators for dynamic content ->>>> deja mis
NEO-88858 WebUI - Send proof from execution recurring delivery -> bug
NEO-89777 Content locking on create email template -> juliette
NEO-90365 Multi-lingual – Identify fields editable from variants???? -> fix pour SMS
query activity -> query ds workflow fitleting dimentsion 

-->

## 2025年8月リリース {#25-8-release}

このリリースには、次のような一連のバグ修正が含まれています。

* プロファイル複製プロセスがクライアントコンソールの動作と一致するように改善され、両方のインターフェイスで一貫性のあるエクスペリエンスが確保されます。これにより、重複したプロファイルの作成を妨げる可能性がある問題が修正されます。

* 配信設定画面の「**[!UICONTROL BCC でメールを送信]**」オプションが、Momentum（Enhanced MTA）で動作するようになりました。この機能は、以前はクライアントコンソールでのみ使用可能でした。

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

## 2025年6月リリース {#25-6-release}

### 機能強化 {#25-6-improvements}

* 配信概要レポートが、コールセンターチャネルとカスタムチャネルの両方で使用できるようになりました。[詳細情報](../reporting/direct-mail.md)

* SMS 配信を設定する際に、特定の SMS パラメーターにアクセスできるようになりました。これらは、クライアントコンソールで使用できるパラメーターと同じです。[詳細情報](../advanced-settings/delivery-settings.md#sms-tab)

* お気に入りフォルダーがエクスプローラーページの左側のパネルの上部に表示され、アクセスしやすくなりました。[詳細情報](../get-started/work-with-folders.md#favorite-folders)

* ルールビルダーでドラッグ＆ドロップがサポートされ、クエリのコンポーネントをより効率的に並べ替えることができるようになりました。[詳細情報](../query/build-query.md#drag-and-drop)

* ルールビルダーの「人間の状況」が改善されました。これは、画面の下部に表示される、ルールをわかりやすく記述したバージョンです。

   * 属性がハイライト表示されるようになり、関連するスキーマが表示されます。
   * これらの要素をクリックすると、より詳細な情報を表示できます。
   * 対応するボタンを使用して、人間の状況をコピーできるようになりました。

* テクニカルワークフローフォルダーおよび自動的に作成されたオブジェクトフォルダーへのアクセスが制限され、表示されなくなりました。[詳細情報](../get-started/work-with-folders.md#about-folders)

## 2025年5月リリース {#25-5-release}

次の機能は、5月のリリース以降、すべてのユーザーが使用できます。

<table>
<thead>
<tr>
<th><strong>ブランド整合性スコア（ベータ版）</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>ブランド整合性スコア機能は、E メールデザイナーで直接、明確なフィードバックを提供し、コンテンツがブランドのトーン、スタイル、ガイドラインと合っているかどうかを確認するのに役立ちます。この機能はベータ版で使用できます。</p>
<p>詳しくは、<a href="../content/brands-score.md">詳細なドキュメント</a>を参照してください。</p>
<img src="assets/do-not-localize/brand-score.gif">
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>外部配信のカスタムチャネル</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Campaign Web UI から直接、カスタム外部チャネルに基づいて配信を調整および実行できるようになりました。これらの配信は、スタンドアロンで行うか、ワークフローの一部として行うことができます。サードパーティと統合されたカスタム外部チャネルの作成は、コンソールで実行します。</p>
<p>メモ：カスタムチャネルの Web UI では、レポートは使用できません。レポートにアクセスするには、クライアントコンソールを参照する必要があります。</p>
<p>詳しくは、<a href="../call-center/gs-custom-channel.md">詳細なドキュメント</a>を参照してください。</p>
<img src="assets/do-not-localize/custom-channel.gif">
</td>
</tr>
</tbody>
</table>

### 機能強化 {#25-5-improvements}

タイポロジルールの作成画面が更新され、ルールのタイプを簡単に選択できるようになりました。

## 2025年4月リリース {#25-4-release}

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
<p>コールセンターチャネルを Campaign web ユーザーインターフェイスで使用できるようになりました。このチャネルは、コールセンター（通常、エージェントによる顧客や見込み客への電話）を通じて処理される通信やインタラクションを管理および追跡するのに使用される通信方法を指します。</p>
<p>メモ：レポートは、コールセンターチャネルの Web UI では使用できません。レポートにアクセスするには、クライアントコンソールを参照する必要があります。</p>
<img src="assets/do-not-localize/call-center.gif">
<p>詳しくは、<a href="../call-center/gs-call-center.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>新しいルールビルダー</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>改善されたユーザーインターフェイスで複雑な条件を定義するのに役立つ、新しいルールビルダーが使用できるようになりました。必要に応じて、古いルールビルダーから新しいルールビルダーに切り替えることができます。</p>
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

### 機能強化 {#25-4-improvements}

**一般的なインターフェイスの改善**

* スキーマ属性のフィールドの説明、お気に入りに追加、値の配分のオプションがユーザーインターフェイスでより見やすくなりました。詳しくは、[詳細なドキュメント](../get-started/attributes.md)を参照してください。
* Experience League の環境設定で指定したプライマリ言語に従って、日時がインターフェイスに表示されるようになりました。この改善は、複数の言語でのみ使用できます。サポートされる言語の完全なリストを確認するには、[詳細なドキュメント](https://experienceleague.adobe.com/ja/docs/core-services/interface/features/browser-language){target=_blank}を参照してください。

<!--
ko * Built-in options are now only visible in the list of options if the **Show advanced options** toggle is activated.
ko * The typology rules creation screen has been updated to facilitate the selection of the type of rule.
-->

**メールエディター**：Campaign web UI のアクセシビリティを強化することを目的に、E メールデザイナーで 2 つの新しいフィールドが使用できるようになりました。これらは、メールコンテンツの `html` 要素の `title` 要素と lang 属性に対応しています。これらの設定は、メールの「本文」セクションの「プリヘッダー」フィールドに加えて定義できます。詳しくは、[詳細なドキュメント](../email/metadata.md)を参照してください。

<!--
**Workflow**: You can now select an existing Javascript code in workflow properties or in a Javascript activity.    
-->

**スキーマ**

* Campaign web ユーザーインターフェイスからリストの一時スキーマを編集できるようになりました。詳しくは、[詳細なドキュメント](../audience/manage-audience.md)を参照してください。
* サンプル画面でスキーマのカスタムフィールドをプレビューできるようになりました。詳しくは、[詳細なドキュメント](../administration/custom-fields.md#add)を参照してください。
* ドラッグ＆ドロップを使用して、リストのカスタムフィールドを移動できるようになりました。詳しくは、[詳細なドキュメント](../administration/custom-fields.md#add)を参照してください。


### 限定提供の新機能 {#25-4-features-la}

>[!AVAILABILITY]
>
>次の機能は、限定提供（LA）です。**Adobe Campaign Standard から Adobe Campaign v8** に移行するお客様に限定され、他の環境にはデプロイできません。Campaign サーバーを v8.7.4 にアップグレードする必要があります。
>
>ドキュメントページの [Campaign v8 への Campaign Standard の移行](../rn/acs-migration.md)および [Campaign Standard ユーザー向けの機能](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=ja)を参照してください。

* **多言語配信の作成** - Adobe Campaign web ユーザーインターフェイスで、複数のメール配信を異なる言語で送信できるようになりました。多言語配信機能を使用すると、配信のデフォルト言語と、配信を送信できる様々な言語を選択できます。また、選択した言語でこれらの配信をプレビューすることもできます。詳しくは、[詳細なドキュメント](../email/edit-content.md)を参照してください。

* **多言語用の動的レポート** - 多言語メール配信で動的レポートが使用できるようになりました。詳しくは、[詳細なドキュメント](../reporting/global-reports.md)を参照してください。

* **SMS REST API サポート（LA）** - トランザクションメッセージング REST API が SMS チャネルで使用できるようになりました。ペイロードにメールと mobilePhone の両方が存在する場合は、「wishedChannel」フィールドを使用してチャネルを指定できます。指定しない場合は、wishedChannel で明示的に SMS をリクエストしない限り、デフォルトでメールが使用されます。詳しくは、[詳細なドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=ja){target=_blank}を参照してください。

## 2025年2月リリース {#25-2-release}

**リリース日**：2025年2月18日（PT）

次の機能と改善点は、2月のリリース以降使用できます。

### 機能 {#25-2-features}

<table>
<thead>
<tr>
<th><strong>ビジネスルール（タイポロジルール）の作成</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Campaign web ユーザーインターフェイスでタイポロジとタイポロジルールを作成できるようになりました。タイポロジでは、配信の送信を制御、フィルタリングおよび優先順位付けできます。タイポロジを使用すると、必須コンポーネント（登録解除リンクや件名など）や、オーディエンス（登録解除者、競合他社、非ロイヤルティ顧客など）からグループを除外するフィルタリングルールが配信に常に含まれていることを検証できます。</p>
<img src="assets/do-not-localize/typology.gif">
<p>詳しくは、<a href="../administration/typologies.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>ターゲットマッピング</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Campaign web ユーザーインターフェイスでターゲットマッピングを作成できるようになりました。ターゲットマッピングは、様々な配信チャネル（メール、SMS、プッシュ通知）からスキーマのデータフィールドへのリンク方法を定義します。ターゲットマッピングを使用すると、ターゲットオーディエンス（プロファイル、契約の受取人、オペレーター、サブスクライバーなど）を定義できます。</p>
<img src="assets/do-not-localize/target-mapping.gif">
<p>詳しくは、<a href="../administration/target-mappings.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>スキーマの詳細</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>リストで名前を選択して、スキーマの詳細にアクセスできるようになりました。カスタムフィールドの編集は、スキーマの詳細にある「<b>カスタムフィールドを編集</b>」ボタンからアクセスできるようになりました。</p>
<img src="assets/do-not-localize/schemas.gif">
<p>詳しくは、<a href="../administration/schemas.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

## 2025年1月リリース {#25-1-release}

**リリース日**：2025年2月5日（PT）

次の機能と改善点は、1月のリリース以降使用できます。

### 機能 {#25-1-features}


<table>
<thead>
<tr>
<th><strong>ビジュアルフラグメントの作成と使用</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>ビジュアルフラグメントは、複数のメール配信やコンテンツテンプレートをまたいで再利用できる、定義済みのビジュアルブロックです。この機能を、サーバービルド 8.6.4 以降を実行しているすべてのお客様が使用できるようになりました。</p>
<img src="assets/do-not-localize/visual-fragment.gif">
<p>詳しくは、<a href="../content/use-visual-fragments.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>サードパーティシステムを使用した配信の送信</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Campaign web インターフェイスで外部配信と外部配信テンプレートを定義できるようになりました。このモードでは、外部プロバイダーと共有できる出力ファイルにメッセージをコンパイルできます。デフォルトでは、ダイレクトメールチャネルには外部配信モードが使用されます。</p>
<img src="assets/do-not-localize/external-delivery.gif">
<p>詳しくは、<a href="../msg/send-external-deliveries.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>列挙の管理</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Campaign web ユーザーインターフェイスから列挙を直接作成できるようになりました。列挙とは、フィールドへの入力候補としてシステムによって表示される値のリストです。列挙を使用してフィールドの値を統一すると、データ入力やクエリ内での使用が簡単になります。</p>
<img src="assets/do-not-localize/enumerations.gif">
<p>詳しくは、<a href="../administration/enumerations.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>カスタムオプションの作成</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Campaign web ユーザーインターフェイス内のテクニカルオプションにアクセスし、ニーズに合わせて独自のカスタムオプションを作成できるようになりました。これは、JavaScript コードワークフローアクティビティを使用して中間データを保存する際に特に便利です。</p>
<img src="assets/do-not-localize/options.gif">
<p>詳しくは、<a href="../administration/options.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>Javascript コードの定義と呼び出し</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Campaign web ユーザーインターフェイスで JavaScript コードを作成できるようになりました。これにより、ライブラリと同様に、ワークフロー全体で利用できる再利用可能な関数を作成できます。</p>
<img src="assets/do-not-localize/javascript.gif">
<p>詳しくは、<a href="../administration/javascript-codes.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>AI アシスタントを使用したランディングページの生成</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>ランディングページ配信で AI アシスタントが使用できるようになりました。これにより、テキスト、画像または完全なページレイアウトを生成できます。</p>
<img src="assets/do-not-localize/ai-lp.gif">
<p>AI アシスタントについて詳しくは、<a href="../email/generative-lp.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>


### 改善点 {#25-1-improvements}

* インターフェイスでのカスタムフィールドの表示のカスタマイズ：

   * インターフェイスに表示する追加のカスタムフィールドを選択できるようになりました
   * リンクタイプのカスタムフィールドを表示するためのルールを設定できるようになりました（他のフィールドの入力に基づいてリスト値を制限するなど）
   * インターフェイスのフィールドをより柔軟に並べ替えられるようになりました（フィールドの幅を 1 つの列全体に広げる、より適切に整理するためにサブセクションにグループ化する）
   * 特定のフィールドを読み取り専用として設定できるようになりました

* 最近使用したフィルターとお気に入りフィルター：頻繁に使用する属性をすばやく再利用するために、お気に入りに追加できるようになりました。これにより、以降のタスクではすばやくアクセスできます。お気に入りに加えて、最近選択した属性を表示したり使用したりすることもできます。

* 外部アカウント：新しい外部アカウントを作成する際に、新しい&#x200B;**[!UICONTROL ルーティング]**&#x200B;タイプを選択できます。これにより、外部配信で使用する特定の外部アカウントを設定できます。[詳細情報](../administration/external-account.md#routing)
