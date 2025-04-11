---
audience: end-user
title: Campaign web ユーザーインターフェイス／クライアントコンソール機能マトリックス
description: Campaign web ユーザーインターフェイスでサポートされる機能のリスト
exl-id: 4bcac01f-be1d-497c-937d-0c82f0d6b17d
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '2102'
ht-degree: 50%

---

# Campaign web および Campaign クライアントコンソール {#capabilities-matrix}

Campaign の主な機能は、Campaign web ユーザーインターフェイスから確認できます。 このインターフェイスは、主に、マーケターがマーケティングキャンペーンの計画、開始、測定をおこなうために設計されています。 すべての機能の一覧が [ このページ ](../rn/whats-new.md) に記載されています。

ビジネスおよびデータのニーズに基づく Campaign プラットフォームのカスタマイズと、他のシステムへの接続は、Campaign クライアントコンソールで管理されます。 その結果、一部の設定や機能は、Campaign クライアントコンソールからのみアクセス、作成または管理できます。 一部は、後の Campaign web ユーザーインターフェイスの更新で利用できるようになります。

<!--
**Homepage**

* Home page dashboard
* Home page customization-->

## キャンペーン管理 {#campaign-mgt-capabilities}

Campaign web ユーザーインターフェイスを使用すると、（この節 [ で説明しているように ](../campaigns/gs-campaigns.md) クロスチャネルキャンペーンを作成できます。 次の機能は、Campaign クライアントコンソールでのみ使用できます。 Campaign の web ユーザーインターフェイスからはアクセスできませんが、一部の機能は [ エクスプローラーメニュー ](user-interface.md#user-interface-explorer) から表示できます。

提供されたリンクを使用して、Campaign v8（クライアントコンソール）ドキュメントを参照し、これらの機能の使用方法の詳細を確認してください。

* **マーケティングカレンダー**。キャンペーンカレンダーでは、すべてのプログラム、プラン、キャンペーンおよび配信がグローバルタイムラインに表示されます。 この機能は、クライアントコンソールでのみ使用できます。[詳細情報](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html?lang=ja#campaign-calendar){target="_blank"}
* **プログラムとプラン**。各キャンペーンは 1 つのプログラムに属し、プログラムはプランに属します。 Campaign web ユーザーインターフェイスでは、すべてのキャンペーンがデフォルトのビルトインプランおよびプログラムに関連付けられます。 クライアントコンソールで作成および管理できるのは、プランとプログラムのみです。[詳細情報](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html?lang=ja#work-with-plan-and-program){target="_blank"}
* **プロバイダー、予算、コスト管理**。 キャンペーン内で実行されるジョブに関係するサービスプロバイダー（コスト構造など）を設定し、各プログラムとキャンペーン内の予算を管理できます。この機能は、クライアントコンソールでのみ使用できます。[詳細情報](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/providers--stocks-and-budgets.html?lang=ja){target="_blank"}
* **分散型マーケティング**（セントラル／ローカルマーケティング）Adobe Campaignは、セントラルエンティティ（本社、マーケティング部門など）とローカルエンティティ（販売店、地域代理店など）の間で協調キャンペーンを実装するための分散型マーケティングアプリを提供します。 この機能は、クライアントコンソールでのみ使用できます。[詳細情報](https://experienceleague.adobe.com/docs/campaign/automation/distributed-marketing/about-distributed-marketing.html?lang=ja){target="_blank"}
* **マーケティングリソース管理**（MRM）、目標、シミュレーションおよびコスト管理Adobe Campaignは、関係するタスク、予算およびマーケティングリソースの完全な管理とリアルタイムトラッキングにより、マーケティングアクションを協調的に制御できるマーケティングリソース管理（MRM）アプリを提供します。 この機能は、クライアントコンソールでのみ使用できます。[詳細情報](https://experienceleague.adobe.com/docs/campaign/automation/mrm/about-marketing-resource-management.html?lang=ja){target="_blank"}
* **タスク管理** MRM アプリの一部として、キャンペーンダッシュボードから Campaign タスクを作成、割り当て、トラッキングおよび監視できます。この機能は、クライアントコンソールでのみ使用できます。[詳細情報](https://experienceleague.adobe.com/docs/campaign/automation/mrm/creating-and-managing-tasks.html?lang=ja){target="_blank"}

## 通信チャネル {#channels-capabilities}

Campaign の web ユーザーインターフェイスを使用すると、**メール**、**SMS**、**プッシュ通知**、**ダイレクトメール** を作成、デザイン、送信したり、様々な専用レポートを使用して影響を測定したりできます。詳しくは、[ この節 ](../msg/gs-messages.md) を参照してください。 ただし、アプリ内、LINE、コールセンター／カスタムチャネル、X によるソーシャルマーケティング（Twitter）などのチャネルは現在利用でき&#x200B;**ません**。

提供されたリンクを使用して、Campaign v8（クライアントコンソール）ドキュメントを参照し、これらのチャネルの詳細を確認してください。

* **LINE メッセージ**。LINE は、無料のインスタントメッセージ、音声、ビデオ通話のためのアプリケーションで、すべてのモバイルデバイスと PC で利用できます。 Adobe Campaign では、クライアントコンソールからのみ LINE メッセージを送信できます。[詳細情報](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/line.html?lang=ja){target="_blank"}
* **コールセンターとカスタムチャネル**。コールセンターやその他のカスタムチャネルは、Campaign 環境に実装できます。これらのチャネルは、クライアントコンソールでのみ使用できます。[詳細については、Campaign Classic v7 ドキュメントを参照してください](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/communication-channels.html?lang=ja#other-channels){target="_blank"}
* X（Twitter）を使用した&#x200B;**ソーシャルマーケティング**。X（Twitter）を通じてメッセージを投稿したり、ダイレクトメッセージを送信したりしてお客様とやり取りします。この機能は、ソーシャルマーケティング アドオンに付属しており、クライアントコンソールからのみ使用できます。 [詳細情報](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-tw.html?lang=ja){target="_blank"}

## ランディングページと web アプリケーション {#Webapps-capabilities}

Adobe Campaign では、ランディングページを作成、設計および共有できます。ランディングページのエクスペリエンスが、新しいインターフェイスで完全に再考されました。Campaign web ユーザーインターフェイスでランディングページを作成、デザインおよび公開する方法については、[ この節 ](../landing-pages/get-started-lp.md) を参照してください。

その結果、Campaign クライアントコンソールでは、web インターフェイスで作成したランディングページを編集、更新、変更することはできません。また、その逆も同様です。 次のタイプの web アプリケーションは、Campaign web ユーザーインターフェイスでは使用できません。 ただし、ランディングページのリストには表示されます。提供されたリンクを使用して、Campaign Classic v7 ドキュメントを参照し、これらの web アプリの詳細を確認してください。

* **Web アプリケーション**。Adobe Campaignでは、データベースから事前に読み込まれたデータと、接続ユーザーの権限に応じたコンテンツを使用して、動的でインタラクティブな web アプリケーションを作成して公開できます。 この機能は、クライアントコンソールでのみ使用できます。[詳細については、Campaign Classic v7 ドキュメントを参照してください](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-applications/about-web-applications.html?lang=ja){target="_blank"}
* **Web フォーム**。クライアントコンソールで設計した web ページとランディングページは、Campaign Web ユーザーインターフェイスに表示されますが、編集または変更できません。一部のオプションは、クライアントコンソール web ページデザイナーと、Campaign web ユーザーインターフェイスに付属するランディングページデザイナーでは異なる場合があります。 [詳細については、Campaign Classic v7 ドキュメントを参照してください](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-forms/about-web-forms.html?lang=ja){target="_blank"}
* **オンライン調査**。オンライン調査を作成し、クライアントコンソールからのみ回答を収集できます。この機能は、Campaign web ユーザーインターフェイスでは使用できません。 [詳細については、Campaign Classic v7 ドキュメントを参照してください](https://experienceleague.adobe.com/docs/campaign-classic/using/online-surveys/about-surveys.html?lang=ja){target="_blank"}

## プロファイル、テストプロファイルおよびオーディエンス {#profiles-audiences-capabilities}

Campaign クライアントコンソールと Campaign web ユーザーインターフェイスの両方で、プロファイルとテストプロファイルを作成、管理および更新できます。 一方のインターフェイスで実行されたすべての変更が、もう一方のインターフェイスにも表示されます。 ただし、一部の受信者設定や詳細設定パラメーターが、新しい Campaign web ユーザーインターフェイスに表示されない場合があります。

新しい web ユーザーインターフェイスでは、「受信者」という用語が「プロファイル」に変更され、「シードアドレス」は「テストプロファイル」になりました。

<!--Audience composition is a new capability coming with Campaign Web user interface. As a consequence, in Campaign client console, you cannot edit, update or modify an [audience created with the Query modeler](../query/query-modeler-overview.md). -->

Campaign クライアントコンソールまたはAdobe Experience Platformで作成されたすべてのオーディエンスは、Campaign web ユーザーインターフェイスで使用できます。

[Campaign v8 （クライアントコンソール）ドキュメント ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/import-profiles.html?lang=ja#import-jobs){target="_blank"} で説明しているように、1 回限りのインポート/エクスポートジョブは、Campaign web ユーザーインターフェイスでは使用できません。<!--To import profiles into Campaign Web user interface, you must create a workflow as detailed in [this section]().-->

<!--
## Transactional messaging {#mc-capabilities}

Transactional messaging capabilities coming with the Message Center product package are currently not available in the new Campaign Web user interface. 

Browse the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/real-time/transactional.html){target="_blank"} and learn more about real-time messaging capabilities, such as:

* Realtime message authoring and execution on email, SMS and push
* Message enrichment and personalization
* Reporting and monitoring on transactional messaging
-->

## コンテンツデザイン {#content-capabilities}

Adobe Campaign Web ユーザーインターフェイスに付属する新しいメールデザイナーを使用すると、直感的なドラッグ＆ドロップインターフェイスを通じて、個別にカスタマイズされた魅力的なメールを簡単に作成できます。空白の状態から開始する場合でも、既存のコンテンツを読み込む場合でも、既存のテンプレートを活用する場合でも、メールごとに、すべてのコンテンツをデザインして調整できます。 [詳細情報](../email/edit-content.md)

この新しいユーザーインターフェイスを使用すると、Adobe Experience Managerでメールテンプレートの同期を管理し、Adobe Experience Manager as a Cloud Serviceと統合できます。

Campaign web ユーザーインターフェイスでは、現在、次の機能は使用できません。 提供されたリンクを使用して、Campaign v8（クライアントコンソール）ドキュメントを参照し、これらの機能の詳細を確認してください。

* **カスタムパーソナライゼーションブロックの作成**。デフォルトのパーソナライゼーションブロックに加えて、クライアントコンソールからカスタムブロックを作成できます。この機能は、Campaign web ユーザーインターフェイスでは使用できません。 [詳細情報](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/personalize/personalization-blocks.html?lang=ja#create-custom-personalization-blocks){target="_blank"}
* **カスタムフォームからのコンテンツ**。コンテンツ管理モジュールを使用すると、ユーザーが Campaign でコンテンツを作成する際に役立つフォームを作成および管理できます。この機能は、クライアントコンソールでのみ使用できます。[詳細については、Campaign Classic v7 ドキュメントを参照してください](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/content-management/about-content-management.html?lang=ja){target="_blank"}
* **AMP for Email**。AMP for Email フォーマットを使用すると、メッセージに AMP コンポーネントを組み込み、アクションにつながるリッチコンテンツでメールエクスペリエンスを向上させることができます。 この機能は、クライアントコンソールでのみ使用できます。[詳細については、Campaign Classic v7 ドキュメントを参照してください](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/sending-emails/defining-interactive-content.html?lang=ja){target="_blank"}
<!--
* Content from a URL`*`
* Email fragments`*`
* Multivariant / Multilingual use case`*`-->

## タイポロジとタイポロジルール {#rules-capabilities}

タイポロジとは、準備フェーズで実行され、複数のフィルタールールを 1 回の配信に容易に適用するための一連のタイポロジルールです。 マーケターは、配信の送信を制御、フィルタリングおよび優先順位付けすることで、すべての配信にわたってビジネスプラクティスを標準化できます。

[ この節 ](../advanced-settings/delivery-settings.md#typology) で説明しているように、タイポロジルールは、Campaign web ユーザーインターフェイスで配信または配信テンプレートに対して選択することができます。 ただし、ルールとタイポロジルールの作成、管理、カスタマイズは、Campaign クライアントコンソールでのみ使用できます。

提供されたリンクを使用して、Campaign v8（クライアントコンソール）ドキュメントを参照し、タイポロジルールの詳細を確認してください。

* コントロールルールの作成。[詳細情報](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html?lang=ja){target="_blank"}
* 疲労/圧力ルールの作成 [詳細情報](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=ja){target="_blank"}
* フィルタリングルールの作成。[詳細情報](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/filtering-rules.html?lang=ja){target="_blank"}
* タイポロジルール管理。[詳細情報](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/apply-rules.html?lang=ja){target="_blank"}
* キャンペーンのシミュレーション。[詳細情報](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/campaign-simulations.html?lang=ja){target="_blank"}
* タイポロジルールのオーサリング用の JavaScript コーディング。[詳細情報](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=ja#use-cases-on-pressure-rules){target="_blank"}

## ワークフロー {#wf-capabilities}

新しい Campaign Web ユーザーインターフェイスでは、プロセスを設計および管理するための再考されたワークフローキャンバスインターフェイスが導入されます。主要なワークフローアクティビティは、新しいデザインで既に使用可能で、一部は今後のアップデートで提供される予定です。 ガードレールや制限事項など、ワークフロー機能について詳しくは、[ この節 ](../get-started/guardrails.md) を参照してください。

以下の機能は、Campaign クライアントコンソールでのみ使用できます。

* ワークフローでのスクリプティング
* ETL アクティビティ：書き出し、スキーマ編集、データ読み込み、データ抽出、SQL コード

使用可能なワークフローアクティビティについて詳しくは、[こちら](https://experienceleague.adobe.com/docs/campaign/automation/workflows/wf-activities/activities.html?lang=ja){target="_blank"}にある Adobe Campaign v8（コンソール）ワークフロードキュメントを参照してください。

## オファー管理 {#offer-capabilities}

オファーは、Adobe Campaign Web ユーザーインターフェイスで作成した配信で送信できます。これらのオファーは、**[!UICONTROL インタラクション]**&#x200B;モジュールを使用してクライアントコンソールで作成している必要があります。オファーデザイン、実施要件ルール、オファー管理は、Campaign クライアントコンソールでのみ使用できます。 [詳細情報](../msg/offers.md)

オファーカタログを管理する方法については、[Campaign v8（クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=ja){target="_blank"}を参照してください。

## Adobe Experience Cloud ソリューションとの統合 {#exc-capabilities}

新しい Campaign の最新 UI は、マーケティングキャンペーンのデザインと配信を簡素化し、Adobe Experience PlatformやAdobe Experience Managerなどの他のAdobe ソリューションとの一貫性を保ちます。

次の統合機能はAdobe Campaign クライアントコンソールから利用できますが、Campaign web ユーザーインターフェイスではまだ使用できません。 提供されたリンクを使用して、Campaign v8（クライアントコンソール）ドキュメントを参照し、これらの統合について詳細を確認してください。

* Adobe Analytics データの使用と KPI の共有。[詳細情報](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aa.html?lang=ja){target="_blank"}
* Adobe Experience Cloud（Adobe Audience Manager）とのオーディエンスの共有。[詳細情報](https://experienceleague.adobe.com/docs/campaign-classic/using/integrating-with-adobe-experience-cloud/audience-sharing/sharing-audiences-with-adobe-experience-cloud.html?lang=ja){target="_blank"}
* Adobe Target との統合。[詳細情報](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-at.html?lang=ja){target="_blank"}
* Adobe Experience Cloud トリガーとの統合。[詳細情報](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-triggers.html?lang=ja){target="_blank"}

## レポート {#reporting-capabilities}

新しい Campaign web ユーザーインターフェイスには、すべてのチャネル（配信レポート、キャンペーンレポート、グローバルレポート）の一連の新しいレポートと KPI が付属しています。 詳しくは、[この節](../reporting/gs-reports.md)を参照してください。

一部の機能は、クライアントコンソールからのみ使用できます。[Campaign v8 （クライアントコンソール）ドキュメントへのリンクを参照し ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaign-home.html?lang=ja){target="_blank"} 詳細を確認してください。

* ビルトインの配信品質レポートと受信ボックスレンダリング。 [詳細情報](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/inbox-rendering.html?lang=ja){target="_blank"}
* レポートのカスタマイズ。[詳細情報](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/creating-a-new-report.html?lang=ja){target="_blank"}
* 記述的分析。[詳細情報](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/analyzing-populations/about-descriptive-analysis.html?lang=ja){target="_blank"}
* キャンペーン分析/キューブレポート。 [詳細情報](https://experienceleague.adobe.com/docs/campaign/campaign-v8/analytics/reports/cubes/gs-cubes.html?lang=ja){target="_blank"}
* スケジュールに従った PDF および CSV またはリンクとしてのレポート共有。[詳細情報](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/configuring-access-to-the-report.html?lang=ja){target="_blank"}

## データモデリングおよびデータ取り込み {#data-capabilities}

Campaign web ユーザーインターフェイスは、次の機能を表示しません。これらは、クライアントコンソールでのみ使用できます。

### 外部アカウント {#external}

Adobe Campaign には、外部システムと接続する事前定義済みの外部アカウントのセットが付属します。Campaign システム管理者は、外部アカウントを作成および管理できます。[詳細情報](../administration/external-account.md)

### スキーマの作成と拡張 {#schema}

スキーマの作成、変更および拡張は、上級ユーザーに制限されます。これらの機能は、クライアントコンソールからのみ使用できます。[詳細情報](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/schemas.html?lang=ja){target="_blank"}

### ワークフローのデータ管理機能 {#data}

データ管理は、データの読み込み、抽出（ファイル）、データの更新、スキーマの編集、テクニカルワークフローのインポート／エクスポートなど、より効率的で柔軟なツールを提供することで、複雑なターゲティングの問題を解決するための一連のアクティビティを組み合わせます。[詳しくは、クライアントコンソールでのワークフローのデータ管理機能の確認を参照してください](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html?lang=ja#data-management){target="_blank"}

>[!NOTE]
>
>これらのアクティビティの一部はクライアントコンソールでのみ使用できますが、一部は Campaign web ユーザーインターフェイスで使用できます（**エンリッチメント**、**ファイルを読み込み**、**データソースを変更**、**ディメンションを変更** などのアクティビティです）。 [Campaign web ユーザーインターフェイスでのターゲティングおよびデータ管理アクティビティの詳細を説明します ](../workflows/activities/about-activities.md#targeting)

### Federated Data Access の設定 {#fda}

Campaign の設定と外部システムへの接続は、上級ユーザーに制限され、クライアントコンソールからのみ使用できます。[詳細情報](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html?lang=ja){target="_blank"}

## 承認 {#approvals-capabilities}

>[!CONTEXTUALHELP]
>id="acw_deliveries_approval"
>title="承認管理"
>abstract="承認管理は、クライアントコンソールからのみ使用できます。 "

Campaign web ユーザーインターフェイスには、コンテンツ、配信、ワークフロー、キャンペーンおよびターゲットの承認管理は表示されません。 これらは、クライアントコンソールでのみ使用できます。

ワークフローでの承認を管理する方法については、[Campaign v8（クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/automation/workflows/executing-a-workflow/define-approvals.html?lang=ja){target="_blank"}を参照してください。

キャンペーンで配信、コンテンツ、ターゲットの承認を管理する方法については、[Campaign v8 （クライアントコンソール）ドキュメント ](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-approval.html?lang=ja){target="_blank"} を参照してください。

## 権限 {#permissions-capabilities}

Campaign ユーザーは、Adobe Identity Management System （IMS）を介してのみ、Adobe IDで Campaign web ユーザーインターフェイスにアクセスできます。 ユーザーに付与された権限も Campaign web ユーザーインターフェイスに適用されます。

権限の定義については、Adobe Admin ConsoleおよびAdobe Campaign クライアントコンソールを参照してください [ この節を参照 ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/gs-permissions.html?lang=ja)。 Adobe Campaign Web ユーザーインターフェイスから権限に対するアクションを実行することはできません。

## 監視 {#monitoring-capabilities}

Campaign プラットフォームの監視機能は、クライアントコンソールと Campaign コントロールパネルでのみ使用できます。 これらは、Campaign web ユーザーインターフェイスには表示されません。

詳しくは、Campaign v8（クライアントコンソール）ドキュメントおよびコントロールパネルドキュメントへの提供されたリンクを参照してください。

* [ワークフローの監視](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/monitor-technical-workflows.html?lang=ja){target="_blank"}
* [ワークフローヒートマップ](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/heatmap.html?lang=ja){target="_blank"}
* [パフォーマンスの監視](https://experienceleague.adobe.com/docs/control-panel/using/performance-monitoring/about-performance-monitoring.html?lang=ja){target="_blank"}
* [ 配信品質の監視 ](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/monitoring-deliverability.html?lang=ja){target="_blank"}