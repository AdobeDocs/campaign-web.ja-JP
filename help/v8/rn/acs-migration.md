---
audience: end-user
title: Campaign Standard から Adobe Campaign web への移行
description: Campaign web ユーザーインターフェイスの確認
exl-id: 4cf406af-4cf5-434d-b1c7-a7c102f8dc2f
source-git-commit: 448b002a284b05000da80fd165b300bc24178c78
workflow-type: ht
source-wordcount: '716'
ht-degree: 100%

---

# Campaign v8 への Campaign Standard の移行 {#welcome}

<!--
We are thrilled to annonce that you, as a Campaign Standard user, can now benefit from the new version of Adobe Campaign Web User Interface. The migration is seemless and will allow you to use all the intuitive features designed to simplify the creation of personalized cross-channel campaigns. Campaign Web User Interface also brings a connected canvas with Adobe Experience Platform for a unified experience.
-->

Adobe Campaign Managed Cloud Services v8 へようこそ。

Adobe Campaign Standard ユーザーは、Adobe Campaign Managed Cloud Services v8 に移行できるようになりました。この移行には、次のような多くのメリットがあります。

* 堅牢な IT インフラストラクチャ：Managed Cloud Services v8 を使用すると、クライアントはより堅牢な IT インフラストラクチャを活用して、キャンペーンのパフォーマンス、信頼性、スケーラビリティを強化できます。
* サポートの強化：Managed Cloud Services チームは、お客様のプラットフォームのスムーズな移行と継続的なモニタリングを確保し、優れたサポートを提供することに全力を注いでいます。トラブルシューティングからプロアクティブなメンテナンスまで、お客様をサポートします。
* Adobe Experience Platform との統合：Managed Cloud Services v8 では、Adobe Experience Platform とシームレスに接続し、クライアントがデータの可能性を最大限に活用し、パーソナライズされた効果的なキャンペーンをチャネル全体で提供できるようにします。
* 一貫性の高いユーザーインターフェイスとエクスペリエンス：Managed Cloud Services v8 に移行しても、ワークフローが中断されることはありません。使い慣れたユーザーインターフェイスとユーザーエクスペリエンスを引き続き利用して、チームの学習曲線を最小限に抑えることができます。

## 主な機能 {#key-features}

Campaign v8 ユーザーには、新しい Campaign web インターフェイスと v8 コンソールの両方へのアクセス権があります。データと設定は、環境間で同期されます。クライアントコンソールで使用可能なすべてのデータと設定は、エクスプローラーの左側のナビゲーションから Campaign web ユーザーインターフェイスに表示されます。[詳細情報](../get-started/user-interface.md#user-interface-explorer)

Campaign web ユーザーインターフェイスは、マーケターがキャンペーンを簡単に作成および調整できるように設計されています。Campaign v8 web ユーザーインターフェイスが提供する主な機能を詳しく見てみましょう。

* 最新、わかりやすい、統一されたエクスペリエンス。[詳細情報](../get-started/connect-to-campaign.md)。
* 新しい強力な機能とシームレスなプロセス。[詳細情報](../get-started/user-interface.md)
* 新しい簡素化された直感的なクエリモデラー。[詳細情報](../query/query-modeler-overview.md)
* 組み込みのクロスチャネルキャンペーン管理機能。[詳細情報](../msg/gs-messages.md)
* 新しくデザインを変更したキャンペーンワークフローアクティビティ。[詳細情報](../workflows/gs-workflows.md)
* 簡単なプロファイルの作成と管理。[詳細情報](../audience/about-recipients.md)
* 定義済みフィルター。[詳細情報](../get-started/predefined-filters.md)
* メールデザイン用の HTML コンバーター。[詳細情報](../email/existing-content.md)
* オファー付きの SMS。[詳細情報](../msg/offers.md)

Campaign クライアントコンソールは、管理者と開発者が環境を設定およびカスタマイズできるように設計されています。Campaign クライアントコンソールで使用できる主な機能について詳しくは、[このドキュメント](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/new/whats-new){target="_blank"}を参照してください。

>[!NOTE]
>
>サポートされている機能とサポートされていない機能や、Campaign web ユーザーインターフェイスと Campaign クライアントコンソール間の相互運用性について詳しくは、[このページ](../get-started/capability-matrix.md)を参照してください。
>

## 用語 {#terminology}

ほとんどの概念は、Campaign v8 と Campaign Standard で類似しています。ただし、いくつかの違いがあります。Campaign Standard と Campaign v8 の用語の違いの例を以下に示します。

<!--
* Profiles are **Recipients** in the console. [Learn more](../audience/gs-audiences-recipients.md).
* Test profiles are **Seed addresses**. [Learn more](../preview-test/test-deliveries.md).
* The delivery preparation is the **Delivery analysis**. [Learn more](../monitor/prepare-send.md).
* Audiences are **Lists**. [Learn more](../audience/gs-audiences-recipients.md).
-->

* リソースとカスタムリソースは、**スキーマ**&#x200B;と&#x200B;**カスタムスキーマ**&#x200B;です
* メッセージは&#x200B;**配信**&#x200B;と呼ばれます
* 役割は&#x200B;**ネームド権限**&#x200B;で設定されます
* セキュリティグループは&#x200B;**オペレーターグループ**&#x200B;です
* 組織単位は&#x200B;**フォルダー権限**&#x200B;によって管理されます
* 製品ユーザーはクライアントコンソールの&#x200B;**オペレーター**&#x200B;です
* 配信準備はクライアントコンソールの&#x200B;**配信分析**&#x200B;です

## 特定の機能 {#new-features}

Campaign v8 への移行をスムーズに行うために、Campaign v8 に Campaign Standard の主な機能が追加されました。詳しくは、[このドキュメント](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=ja){target="_blank"}を参照してください。このドキュメントは、Campaign Standard から移行するユーザーのみが利用できます。

* **動的レポート**：動的レポートでは、マーケティングアクティビティの影響を測定する完全にカスタマイズ可能なリアルタイムのレポートを提供します。プロファイルデータへのアクセスを可能にし、開封数やクリック数などの機能的なメールキャンペーンデータに加えて、性別、市区町村、年齢などのプロファイルディメンション別のデモグラフィック分析を可能にします。[詳細情報](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html?lang=ja){target="_blank"}

* **一元化されたブランディング**：どの会社にも、ブランドの視覚的ガイドラインと技術的ガイドラインがあります。Adobe Campaign を使用すれば、ロゴからメール送信者、URL、ドメインなどの技術的側面に至るまで、一貫したブランドを顧客に提供する一連の仕様を定義できます。[詳細情報](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html?lang=ja)

* **Rest API** - Campaign Stardard で移行したユーザーは、Rest API を使用して Adobe Campaign の統合を作成し、使用するテクノロジーのパネルと Adobe Campaign をインターフェイスで接続することで独自のエコシステムを作成できます。[詳細情報](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html?lang=ja){target="_blank"}

* **ランディングページ** - Campaign v8 のランディングページにいくつかの改善が加えられ、Campaign Standard と同等の機能を実現しました。詳しくは、[リリースノート](../rn/release-notes.md#new-24-4)とランディングページ[ドキュメント](../landing-pages/get-started-lp.md)を参照してください。

* **ビジュアルフラグメント** - ビジュアルフラグメントは、1 つ以上のメール配信またはコンテンツテンプレートで参照できる再利用可能なビジュアルコンポーネントです。フラグメントを変更すると、そのフラグメントを使用するすべてのコンテンツが更新されます。この機能を使用すると、マーケティングユーザーが改善されたデザインプロセスでメッセージコンテンツを迅速に組み立てるために使用できる複数のカスタムコンテンツブロックを事前に作成できます。[詳細情報](../content/use-visual-fragments.md)

<!--
* Delivery Alerting: In addition to viewing notifications directly in Campaign, Adobe Campaign also provides an email alerting system to trigger email alerts to users or external stakeholders of important system activities. Create, manage, and receive customizable alerts and dashboards to keep track of delivery successes or failures. Adobe Campaign Delivery Alerting boosts efficiency by keeping all involved Adobe Campaign users in a company automatically informed about the delivery execution status, via email and dashboard. 

* Landing Pages: Landing pages are web forms that can be used to capture information on your audiences, offer subscriptions to a service, display data and grow your database. Landing pages can also be used for acquiring or updating existing profiles, and to set up a double opt-in mechanism, allowing you to to protect the platform from wrong or invalid email addresses, or spambots. [Learn more](../landing-pages/get-started-lp.md)
-->
