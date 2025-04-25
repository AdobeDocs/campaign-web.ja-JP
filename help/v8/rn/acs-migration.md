---
audience: end-user
title: Campaign Standard から Adobe Campaign web への移行
description: Campaign web ユーザーインターフェイスの確認
exl-id: 4cf406af-4cf5-434d-b1c7-a7c102f8dc2f
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: ht
source-wordcount: '589'
ht-degree: 100%

---

# Campaign v8 への Campaign Standard の移行 {#acs-to-ac}

Adobe Campaign Standard ユーザーは、Adobe Campaign Managed Cloud Services v8 に移行できるようになりました。この移行には、次のようないくつかのメリットがあります。

* **堅牢な IT インフラストラクチャ**：Managed Cloud Services v8 では、より堅牢な IT インフラストラクチャを提供し、キャンペーンのパフォーマンス、信頼性、スケーラビリティを強化します。
* **サポートの強化**：Managed Cloud Services チームは、スムーズな移行と継続的なプラットフォームモニタリングを確保するために、優れたサポートを提供します。サポートには、トラブルシューティングとプロアクティブなメンテナンスが含まれます。
* **Adobe Experience Platform との統合**：Managed Cloud Services v8 では、Adobe Experience Platform とシームレスに接続し、ユーザーがデータを最大限に活用して、パーソナライズされた効果的なキャンペーンをチャネル全体で配信できるようにします。
* **一貫性の高いユーザーインターフェイスとエクスペリエンス**：Managed Cloud Services v8 への移行により、ワークフローが中断されることはありません。ユーザーは使い慣れたインターフェイスとエクスペリエンスを引き続き利用できるので、チームの学習曲線は最小限に抑えられます。

**Campaign Standard ユーザーが Campaign v8 に移行する場合の開始方法について詳しくは、[このドキュメント](../../adoption/home.md)を参照してください。**

<!--
As a Campaign Standard user, we now offer you a way to migrate to Adobe Campaign v8. You will benefit from both the new Campaign Web interface and the v8 console.
-->

## 主な機能 {#key-features}

Campaign v8 ユーザーには、新しい Campaign web インターフェイスと v8 コンソールの両方へのアクセス権があります。データと設定は、環境間で同期されます。クライアントコンソールで使用可能なすべてのデータと設定は、Campaign web ユーザーインターフェイスに表示され、エクスプローラーの左側のナビゲーションからアクセスできます。[詳細情報](../get-started/user-interface.md#user-interface-explorer)

Campaign web ユーザーインターフェイスは、マーケターがキャンペーンを簡単に作成および調整できるように設計されています。Campaign v8 web ユーザーインターフェイスの主な機能は次のとおりです。

* **現代的な、わかりやすく統一されたエクスペリエンス**。[詳細情報](../get-started/connect-to-campaign.md)。
* **新しい強力な機能とシームレスなプロセス**。[詳細情報](../get-started/user-interface.md)。
* **簡素化された直感的なクエリモデラー**。[詳細情報](../query/query-modeler-overview.md)。
* **組み込みのクロスチャネルキャンペーン管理機能**。[詳細情報](../msg/gs-messages.md)。
* **デザインを変更したキャンペーンワークフローアクティビティ**。[詳細情報](../workflows/gs-workflows.md)。
* **簡単なプロファイルの作成と管理**。[詳細情報](../audience/about-recipients.md)。
* **定義済みフィルター**。[詳細情報](../get-started/predefined-filters.md)。
* **メールデザイン用の HTML コンバーター**。[詳細情報](../email/existing-content.md)。
* **オファー付きの SMS**。[詳細情報](../msg/offers.md)。

Campaign クライアントコンソールは、管理者と開発者が環境を設定およびカスタマイズできるように設計されています。Campaign クライアントコンソールで使用できる主な機能について詳しくは、[このドキュメント](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/new/whats-new){target="_blank"}を参照してください。

>[!NOTE]
>
>サポートされている機能とサポートされていない機能や、Campaign web ユーザーインターフェイスと Campaign クライアントコンソール間の相互運用性について詳しくは、[このページ](../get-started/capability-matrix.md)を参照してください。

## 用語 {#terminology}

ほとんどの概念は、Campaign v8 と Campaign Standard で類似しています。ただし、いくつかの用語の違いがあります。例を次に示します。

<!--
* Profiles are **Recipients** in the console. [Learn more](../audience/gs-audiences-recipients.md).
* Test profiles are **Seed addresses**. [Learn more](../preview-test/test-deliveries.md).
* The delivery preparation is the **Delivery analysis**. [Learn more](../monitor/prepare-send.md).
* Audiences are **Lists**. [Learn more](../audience/gs-audiences-recipients.md).
-->

<!--
* Custom resources are **Schemas**
* Messages are referred to as **Deliveries**
* Roles are configured with **Named Rights**
* Security Groups are **Operator Groups**
* Organizational units are managed through **Folder Permissions**
* Product users are **Operators** in the client console
* Delivery preparation is the **Delivery analysis** in the client console
-->

## 特定の機能 {#new-features}

Campaign v8 へのスムーズな移行を行うために、Campaign v8 に Campaign Standard の主な機能が追加されました。これらの機能について詳しくは、[このドキュメント](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=ja){target=&quot;_blank} を参照してください。このドキュメントは、Campaign Standard から移行するユーザーのみが利用できます。

* **動的レポート**：動的レポートでは、マーケティングアクティビティの影響を測定する、カスタマイズ可能なリアルタイムのレポートを提供します。これには、開封数やクリック数などの機能的なメールキャンペーンデータに加えて、性別、市区町村、年齢などのディメンション別のデモグラフィック分析のためのプロファイルデータへのアクセスが含まれます。[詳細情報](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html?lang=ja){target="_blank"}。

* **一元化されたブランディング**：Adobe Campaign を使用すると、会社はブランドの視覚的ガイドラインと技術的ガイドラインを定義できます。ユーザーは、ロゴからメール送信者、URL、ドメインなどの技術的側面に至るまで、一貫したブランドを顧客に提供できます。[詳細情報](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html?lang=ja)。

* **REST API**：Campaign Standard に移行したユーザーは、REST API を使用して Adobe Campaign の統合を作成し、Adobe Campaign を他のテクノロジーと連携させてエコシステムを作成できます。[詳細情報](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html?lang=ja){target="_blank"}。

* **ランディングページ**：Campaign v8 ランディングページには、Campaign Standard と同等の機能を確保するための改善が含まれています。詳しくは、[リリースノート](../rn/release-notes.md#new-24-4)とランディングページ[ドキュメント](../landing-pages/get-started-lp.md)を参照してください。

* **ビジュアルフラグメント**：ビジュアルフラグメントは、1 つ以上のメール配信またはコンテンツテンプレートで参照される、再利用可能なビジュアルコンポーネントです。フラグメントを変更すると、そのフラグメントを使用するすべてのコンテンツが更新されます。この機能により、マーケティングユーザーは、改善されたデザインプロセスでメッセージを迅速に組み立てるために、複数のカスタムコンテンツブロックを事前に作成できます。[詳細情報](../content/use-visual-fragments.md)。

<!--
* Delivery Alerting: In addition to viewing notifications directly in Campaign, Adobe Campaign also provides an email alerting system to trigger email alerts to users or external stakeholders of important system activities. Create, manage, and receive customizable alerts and dashboards to keep track of delivery successes or failures. Adobe Campaign Delivery Alerting boosts efficiency by keeping all involved Adobe Campaign users in a company automatically informed about the delivery execution status, via email and dashboard. 

* Landing Pages: Landing pages are web forms that can be used to capture information on your audiences, offer subscriptions to a service, display data and grow your database. Landing pages can also be used for acquiring or updating existing profiles, and to set up a double opt-in mechanism, allowing you to protect the platform from wrong or invalid email addresses, or spambots. [Learn more](../landing-pages/get-started-lp.md)
-->