---
audience: end-user
title: Campaign Web ユーザーインターフェイス/クライアントコンソール機能マトリックス
description: Campaign の Web ユーザーインターフェイスでサポートされる機能のリスト
exl-id: 4bcac01f-be1d-497c-937d-0c82f0d6b17d
source-git-commit: 45e5b528837614cdbd537d0a92e71265f65f97db
workflow-type: tm+mt
source-wordcount: '2151'
ht-degree: 11%

---

# Campaign Web および Campaign クライアントコンソール {#capabilities-matrix}

主要な Campaign 機能は、Campaign Web ユーザーインターフェイスで使用できます。 このインターフェイスは、マーケターがマーケティングキャンペーンを計画、開始、測定できるように主に設計されていました。 すべての機能が一覧表示されます [このページの](../rn/whats-new.md).

ビジネスやデータのニーズに基づく Campaign プラットフォームのカスタマイズと、他のシステムへの接続は、Campaign クライアントコンソールで管理されます。 その結果、一部の設定や機能は、Campaign クライアントコンソールからのみアクセス、作成または管理できます。 一部の機能は、今後の Campaign Web ユーザーインターフェイスのアップデートで利用できるようになります。

<!--
**Homepage**

* Home page dashboard
* Home page customization-->

## キャンペーン管理 {#campaign-mgt-capabilities}

Campaign Web ユーザーインターフェイスを使用すると、詳細な手順でクロスチャネルキャンペーンを作成できます [この節](../campaigns/gs-campaigns.md). 以下の機能は、Campaign クライアントコンソールでのみ使用できます。 Campaign Web ユーザーインターフェイスでアクセスできませんが、一部は [エクスプローラーメニュー](user-interface.md#user-interface-explorer).

提供されたリンクを使用して Campaign v8（クライアントコンソール）のドキュメントを参照し、これらの機能の使用方法を学びます。

* **マーケティングカレンダー**. キャンペーンカレンダーには、すべてのプログラム、プラン、キャンペーンおよび配信がグローバルタイムラインで表示されます。 この機能は、クライアントコンソールでのみ使用できます。 [詳細情報](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html#campaign-calendar){target="_blank"}
* **プログラムとプラン**. 各キャンペーンは 1 つのプログラムに属し、プログラムはプランに属します。Campaign Web ユーザーインターフェイスでは、すべてのキャンペーンがデフォルトの組み込みプランおよびプログラムに関連付けられます。 クライアントコンソールで作成および管理できるのは、プランとプログラムのみです。 [詳細情報](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-create.html#work-with-plan-and-program){target="_blank"}
* **プロバイダー、予算、コスト管理**. キャンペーン内で実行されるジョブに関係するサービスプロバイダーを設定し（コスト構造を含む）、各プログラムおよびキャンペーン内で予算を管理できます。 この機能は、クライアントコンソールでのみ使用できます。 [詳細情報](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/providers--stocks-and-budgets.html){target="_blank"}
* **分散型マーケティング** （セントラル/ローカルマーケティング）。 Adobe Campaignは、中央企業（本社、マーケティング部門など）間で協調的なキャンペーンを実装するための分散型マーケティングアプリを提供しています。 およびローカルエンティティ（販売店、地域代理店など）との共同作業によるキャンペーンを実装できます。この機能は、クライアントコンソールでのみ使用できます。 [詳細情報](https://experienceleague.adobe.com/docs/campaign/automation/distributed-marketing/about-distributed-marketing.html?lang=ja){target="_blank"}
* **マーケティングリソース管理** (MRM)、目標、シミュレーション、コスト管理。 Adobe Campaignにはマーケティングリソース管理 (MRM) アプリが用意されており、関連するタスク、予算およびマーケティングリソースの完全な管理とリアルタイムトラッキングにより、マーケティングアクションを協調モードで制御できます。 この機能は、クライアントコンソールでのみ使用できます。 [詳細情報](https://experienceleague.adobe.com/docs/campaign/automation/mrm/about-marketing-resource-management.html){target="_blank"}
* **タスク管理** MRM アプリの一部として、キャンペーンタスクは、キャンペーンダッシュボードから作成、割り当て、トラッキングおよび監視できます。 この機能は、クライアントコンソールでのみ使用できます。 [詳細情報](https://experienceleague.adobe.com/docs/campaign/automation/mrm/creating-and-managing-tasks.html){target="_blank"}

## 通信チャネル {#channels-capabilities}

Campaign Web ユーザーインターフェイスを使用して、作成、デザインおよび送信できます **電子メール**, **SMS** および **プッシュ通知**&#x200B;を参照し、詳細に示すように、様々な専用レポートを使用して影響を測定します。 [この節](../msg/gs-messages.md). ただし、現在、次のチャネルが存在します **not** 利用可能：アプリ内、ダイレクトメール、LINE、コールセンター/カスタムチャネル、X でのソーシャルマーケティング (Twitter)。

提供されたリンクを使用して Campaign v8（クライアントコンソール）のドキュメントを参照し、これらのチャネルの詳細を確認します。

* **ダイレクトメール**. ダイレクトメールチャネルを使用すると、顧客、クライアント、サプライヤーまたはその他に、通知、請求書、明細書、マーケティングオファーなどの物理的な通信を送信できます。 このチャネルは、クライアントコンソールでのみ使用できます。  [詳細情報](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/sending-direct-mail/about-direct-mail-channel.html?lang=ja){target="_blank"}
* **LINE メッセージ**. LINE は、無料のインスタントメッセージ、音声、ビデオ通話用のアプリケーションで、すべてのモバイルデバイスと PC で利用できます。Adobe Campaignでは、クライアントコンソールからのみ LINE メッセージを送信できます。 [詳細情報](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/line.html){target="_blank"}
* **コールセンターとカスタムチャネル**. コールセンターやその他のカスタムチャネルは、Campaign 環境に実装できます。 これらのチャネルは、クライアントコンソールでのみ使用できます。 [詳細については、Campaign Classic v7 ドキュメントを参照してください](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/communication-channels.html#other-channels){target="_blank"}
* **ソーシャルマーケティング** を X(Twitter) に置き換えます。 メッセージを投稿し、ダイレクトメッセージを送信することで、X(Twitter) を介して顧客とやり取りします。 Social Marketing アドオンに付属するこの機能は、クライアントコンソールからのみ使用できます。 [詳細情報](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-tw.html?lang=ja){target="_blank"}

## ランディングページと Web アプリケーション {#Webapps-capabilities}

Adobe Campaignでは、ランディングページを作成、デザイン、共有できます。 ランディングページのエクスペリエンスが、新しいインターフェイスで完全に再設計されました。 Campaign Web ユーザーインターフェイスでランディングページを作成、設計、公開する方法を説明します [この節](../landing-pages/get-started-lp.md).

その結果、Campaign クライアントコンソールでは、Web インターフェイスで作成したランディングページを編集、更新、変更することはできません。また、逆も同様です。 次の種類の Web アプリケーションは、Campaign Web ユーザーインターフェイスでは使用できません。 ただし、ランディングページのリストには表示されます。 提供されたリンクを使用してCampaign Classicv7 ドキュメントを参照し、これらの Web アプリの詳細を確認します。

* **Web アプリケーション**. Adobe Campaignを使用すると、データベースのプリロードされたデータと、接続ユーザーの権限に応じたコンテンツを使用して、動的でインタラクティブな Web アプリケーションを作成および公開できます。 この機能は、クライアントコンソールでのみ使用できます。 [詳細については、Campaign Classic v7 ドキュメントを参照してください](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-applications/about-web-applications.html){target="_blank"}
* **Web フォーム**. クライアントコンソールで設計された Web ページとランディングページは、Campaign Web ユーザーインターフェイスに表示されますが、編集や変更はできません。 一部のオプションは、クライアントコンソールの Web ページデザイナーと、Campaign Web ユーザーインターフェイスに付属するランディングページデザイナーで異なる場合があります。 [詳細については、Campaign Classic v7 ドキュメントを参照してください](https://experienceleague.adobe.com/docs/campaign-classic/using/designing-content/web-forms/about-web-forms.html?lang=ja){target="_blank"}
* **オンライン調査**. オンライン調査を作成し、回答を収集できるのはクライアントコンソールからのみです。 この機能は、Campaign Web ユーザーインターフェイスでは使用できません。  [詳細については、Campaign Classic v7 ドキュメントを参照してください](https://experienceleague.adobe.com/docs/campaign-classic/using/online-surveys/about-surveys.html){target="_blank"}


## プロファイル、テストプロファイル、オーディエンス {#profiles-audiences-capabilities}

Campaign クライアントコンソールと Campaign Web ユーザーインターフェイスの両方で、プロファイルおよびテストプロファイルを作成、管理および更新できます。 一方の UI で実行した変更はすべて他方の UI に表示されます。 ただし、新しい Campaign Web ユーザーインターフェイスでは、一部の特定の受信者設定や詳細設定パラメーターが欠落する場合があります。

新しい Web ユーザーインターフェイスでは、「受信者」という用語が「プロファイル」に変更され、「シードアドレス」が「テストプロファイル」に変更されました。

<!--Audience composition is a new capability coming with Campaign Web user interface. As a consequence, in Campaign client console, you cannot edit, update or modify an [audience created with the Query modeler](../query/query-modeler-overview.md). -->

Campaign のクライアントコンソールまたはAdobe Experience Platformで作成されたすべてのオーディエンスは、Campaign Web ユーザーインターフェイスで使用できます。

ワンショットの読み込み/書き出しジョブ ( [Campaign v8（クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/import-profiles.html#import-jobs){target="_blank"} は、Campaign Web ユーザーインターフェイスでは使用できません。 <!--To import profiles into Campaign Web user interface, you must create a workflow as detailed in [this section]().-->

## トランザクションメッセージ {#mc-capabilities}

現在、Message Center 製品パッケージに付属するトランザクションメッセージ機能は、新しい Campaign Web ユーザーインターフェイスでは使用できません。

次を参照： [Campaign v8（クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/real-time/transactional.html){target="_blank"} 次のようなリアルタイムメッセージング機能の詳細を説明します。

* メール、SMS およびプッシュに関するリアルタイムメッセージオーサリングと実行
* メッセージのエンリッチメントとパーソナライゼーション
* トランザクションメッセージングに関するレポートと監視

## コンテンツデザイン {#content-capabilities}

Adobe Campaign Web ユーザーインターフェイスに付属する新しい E メールデザイナーを使用すると、直感的なドラッグ&amp;ドロップインターフェイスで、個別にカスタマイズした魅力的な E メールを簡単に作成できます。 空白のスレートから始める場合でも、既存のコンテンツを読み込む場合でも、既存のテンプレートを活用する場合でも、すべての E メール用にすべてのコンテンツをデザインおよび調整できます。 [詳細情報](../email/edit-content.md)

この新しいユーザーインターフェイスを使用すると、Adobe Experience Managerから電子メールテンプレートの同期を管理し、Adobe Experience Manager as a Cloud Serviceと統合できます。

以下の機能は、Campaign Web ユーザーインターフェイスでは現時点では使用できません。 提供されたリンクを使用して Campaign v8（クライアントコンソール）のドキュメントを参照し、これらの機能の詳細を確認します。

* **カスタムパーソナライゼーションブロックの作成**. デフォルトのパーソナライゼーションブロックに加えて、クライアントコンソールからカスタムブロックを作成できます。 この機能は、Campaign Web ユーザーインターフェイスでは使用できません。 [詳細情報](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/personalize/personalization-blocks.html#create-custom-personalization-blocks){target="_blank"}
* **カスタムフォームのコンテンツ**. コンテンツ管理モジュールを使用すると、Campaign でコンテンツを作成する際にユーザーを支援するフォームを作成および管理できます。 この機能は、クライアントコンソールでのみ使用できます。 [詳細については、Campaign Classic v7 ドキュメントを参照してください](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/content-management/about-content-management.html){target="_blank"}
* **E メール用の AMP**. AMP for Email は、新しいフォーマットで、メッセージに AMP コンポーネントを含め、アクションにつながる豊富なコンテンツで E メールのエクスペリエンスを向上させることができます。 この機能は、クライアントコンソールでのみ使用できます。 [詳細については、Campaign Classic v7 ドキュメントを参照してください](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/sending-emails/defining-interactive-content.html){target="_blank"}
<!--
* Content from a URL`*`
* Email fragments`*`
* Multivariant / Multilingual use case`*`-->

## タイポロジとタイポロジルール {#rules-capabilities}

タイポロジとは、複数のフィルタールールを一度に配信に簡単に適用できるように、準備段階で実行される一連のタイポロジルールです。 これを使用すると、マーケターは、配信の送信を制御、フィルタリング、優先順位付けできるので、すべての配信でビジネスプラクティスを標準化できます。

タイポロジルールは、Campaign Web ユーザーインターフェイスで、詳細に従って、配信または配信テンプレートから選択できます [この節](../advanced-settings/delivery-settings.md#typology). ただし、ルールとタイポロジルールの作成、管理、カスタマイズは、Campaign クライアントコンソールでのみ使用できます。

提供されたリンクを使用して Campaign v8（クライアントコンソール）のドキュメントを参照し、タイポロジルールの詳細を確認します。

* コントロールルールの作成。 [詳細情報](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html?lang=ja){target="_blank"}
* 疲労/頻度ルールの作成。 [詳細情報](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=ja){target="_blank"}
* フィルタールールの作成。 [詳細情報](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/filtering-rules.html){target="_blank"}
* タイポロジルール管理。 [詳細情報](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/apply-rules.html){target="_blank"}
* キャンペーンのシミュレーション。 [詳細情報](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/campaign-simulations.html){target="_blank"}
* タイポロジルールのオーサリング用の JavaScript コーディング。 [詳細情報](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html#use-cases-on-pressure-rules){target="_blank"}

## ワークフロー {#wf-capabilities}

新しい Campaign Web ユーザーインターフェイスでは、新しいワークフローキャンバスインターフェイスが導入され、プロセスの設計と管理が可能になります。 主要なワークフローアクティビティは、新しいデザインで既に使用可能です。一部のワークフローアクティビティは、将来のアップデートで提供される予定です。 ガードレールや制限を含むワークフロー機能の詳細を説明します [この節](../get-started/guardrails.md).

以下の機能は、Campaign クライアントコンソールでのみ使用できます。

* ワークフローでのスクリプティング
* ETL アクティビティ：書き出し、スキーマ編集、データ読み込み、データ抽出、SQL コード

使用可能なワークフローアクティビティの詳細については、 Adobe Campaign v8（コンソール）ワークフロードキュメントを参照してください [ここ](https://experienceleague.adobe.com/docs/campaign/automation/workflows/wf-activities/activities.html?lang=ja){target="_blank"}.

## オファー管理 {#offer-capabilities}

オファーは、Adobe Campaign Web ユーザーインターフェイスで作成された配信で送信できます。 これらのオファーは、 **[!UICONTROL インタラクション]** モジュール。 オファーのデザイン、実施要件ルール、オファー管理は、Campaign クライアントコンソールでのみ使用できます。 [詳細情報](../msg/offers.md)

オファーカタログの管理方法については、 [Campaign v8（クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=ja){target="_blank"}.

## Adobe Experience Cloud ソリューションとの統合 {#exc-capabilities}

新しい Campaign の最新の UI は、マーケティングキャンペーンの設計と配信を簡素化し、Adobe Experience PlatformやAdobe Experience Managerなどの他のAdobeソリューションと共に一貫性を保ちます。

次の統合は、Adobe Campaignクライアントコンソールから使用でき、Campaign Web ユーザーインターフェイスではまだ使用できません。 提供されたリンクを使用して Campaign v8（クライアントコンソール）ドキュメントを参照し、これらの統合の詳細を確認します。

* Adobe Analyticsのデータ使用と KPI の共有。 [詳細情報](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aa.html){target="_blank"}
* Adobe Experience Cloud(Adobe Audience Manager) とオーディエンスを共有する。 [詳細情報](https://experienceleague.adobe.com/docs/campaign-classic/using/integrating-with-adobe-experience-cloud/audience-sharing/sharing-audiences-with-adobe-experience-cloud.html){target="_blank"}
* Adobe Targetとの統合。 [詳細情報](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-at.html){target="_blank"}
* Adobe Experience Cloud Triggersとの統合。 [詳細情報](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-triggers.html){target="_blank"}

## レポート {#reporting-capabilities}

新しい Campaign Web ユーザーインターフェイスには、配信レポート、キャンペーンレポート、グローバルレポートなど、すべてのチャネルに関する一連の新しいレポートと KPI が用意されています。 詳しくは、[この節](../reporting/gs-reports.md)を参照してください。

一部の機能は、クライアントコンソールからのみ使用できます。 提供されたリンクを参照して、 [Campaign v8（クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaign-home.html?lang=ja){target="_blank"} 詳細情報

* 配信品質レポートと受信ボックスレンダリングの組み込み。 [詳細情報](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/inbox-rendering.html){target="_blank"}
* レポートのカスタマイズ。 [詳細情報](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/creating-a-new-report.html?lang=ja){target="_blank"}
* 記述的分析。 [詳細情報](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/analyzing-populations/about-descriptive-analysis.html?lang=ja){target="_blank"}
* キャンペーン分析/キューブレポート。 [詳細情報](https://experienceleague.adobe.com/docs/campaign/campaign-v8/analytics/reports/cubes/gs-cubes.html?lang=ja){target="_blank"}
* スケジュールに従って、PDF、CSV、またはリンクとしてレポートを共有します。 [詳細情報](https://experienceleague.adobe.com/docs/campaign-classic/using/reporting/creating-new-reports/configuring-access-to-the-report.html?lang=ja){target="_blank"}

## データモデリングとデータ取り込み {#data-capabilities}

Campaign Web ユーザーインターフェイスは、次の機能を表示しません。 これらは、クライアントコンソールでのみ使用できます。

指定したリンクを [Campaign v8（クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaign-home.html?lang=ja){target="_blank"} を参照してください。

* **外部アカウント**. Adobe Campaignには、外部システムと接続するための事前定義済みの外部アカウントのセットが付属しています。 Campaign システム管理者は、外部アカウントの作成と管理をクライアントコンソールからのみおこなえます。[詳細情報](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/external-accounts.html){target="_blank"}
* **スキーマの作成と拡張**. スキーマの作成、変更および拡張は、上級ユーザーに制限されます。 これらの機能は、クライアントコンソールからのみ使用できます。 [詳細情報](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/schemas.html){target="_blank"}
* **データ管理** ワークフローアクティビティ。 データ管理は、より効率的で柔軟なツールを提供することで複雑なターゲティングの問題を解決するために、一連のアクティビティを組み合わせます。 これらのアクティビティには、データの読み込み、抽出（ファイル）、データの更新、スキーマの編集、インポート/エクスポートのテクニカルワークフローが含まれます。 これらは、クライアントコンソールでのみ使用できます。 [詳細情報](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html#data-management){target="_blank"}
* **Federated Data Access**. Campaign の設定と外部システムへの接続は、上級ユーザーに制限され、クライアントコンソールからのみ使用できます。 [詳細情報](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html?lang=ja){target="_blank"}

## 承認 {#approvals-capabilities}

Campaign Web ユーザーインターフェイスでは、コンテンツ、配信、ワークフロー、キャンペーンおよびターゲットの承認管理は表示されません。 これらは、クライアントコンソールでのみ使用できます。

ワークフローで承認を管理する方法については、 [Campaign v8（クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/automation/workflows/executing-a-workflow/define-approvals.html){target="_blank"}.


キャンペーンで配信、コンテンツ、ターゲットの承認を管理する方法については、 [Campaign v8（クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-approval.html?lang=ja){target="_blank"}.


## 権限 {#permissions-capabilities}

Campaign ユーザーは、AdobeIdentity Management System(IMS) を通じて、Adobe ID Web ユーザーインターフェイスにのみアクセスできます。 ユーザーに付与される権限は、Campaign Web ユーザーインターフェイスにも適用されます。

権限の詳細は、Adobe Admin ConsoleおよびAdobe Campaignクライアントコンソールで定義されます [この節](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/gs-permissions.html?lang=ja). Adobe Campaign Web ユーザーインターフェイスでは、権限に対するアクションは実行できません。


## 監視 {#monitoring-capabilities}

Campaign プラットフォームの監視機能は、クライアントコンソールと Campaign コントロールパネルでのみ使用できます。 Campaign の Web ユーザーインターフェイスに表示されません。

提供された Campaign v8（クライアントコンソール）ドキュメントへのリンクと、コントロールパネルのドキュメントを参照して詳細を確認します。

* [ワークフロー監視](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/monitor-technical-workflows.html){target="_blank"}
* [ワークフローヒートマップ](https://experienceleague.adobe.com/docs/campaign/automation/workflows/monitoring-workflows/heatmap.html){target="_blank"}
* [パフォーマンスの監視](https://experienceleague.adobe.com/docs/control-panel/using/performance-monitoring/about-performance-monitoring.html?lang=ja){target="_blank"}
* [配信品質の監視](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/deliverability-management/monitoring-deliverability.html){target="_blank"}




