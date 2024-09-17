---
title: 管理者と開発者向けの Adobe Campaign v8 の基本を学びます。
description: このチュートリアルでは、Campaign v8 の主な管理機能とデータ管理機能の概要について説明します。Campaign Standard から Campaign v8 に移行する管理者とテクニカルマーケターを対象としています。
role: Admin, Developer
level: Beginner, Experienced
source-git-commit: 271fb8805e046c20fad824ba37b84be43638011a
workflow-type: tm+mt
source-wordcount: '2666'
ht-degree: 15%

---


# はじめに（管理者および開発者向け） {#acs-gs-admin}

このページでは、Campaign v8 の主な管理およびデータ管理機能の概要を説明します。 Campaign Standard環境から Campaign v8 に移行する管理者やテクニカルマーケターを対象としています。

主な変更点は、Adobe Campaign アプリケーションサーバーと通信するネイティブアプリケーションであるクライアントコンソールの導入です。

Campaign クライアントコンソールは、すべての機能と設定を一元化します。 Campaign web ユーザーインターフェイスと同期されるので、両方の環境で一貫性を確保できます。

![](assets/client_console.png){zoomable="yes"}

[Adobe Campaign v8 のクライアントコンソールユーザーインターフェイスの詳細を説明します ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/campaign-ui#ui-access){target="_blank"}。

## Campaign v8 アーキテクチャ {#acs-gs-admi-archi}

Campaign のアーキテクチャについて詳しくは、Campaign v8 （コンソール）ドキュメントを参照してください。 基本については、[ このページ ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/architecture/general-architecture){target="_blank"} を参照してください。

開始するのに役立つリンク：

* Adobe Campaignのコンポーネントとグローバルアーキテクチャについては、[ このページ ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/ac-components){target="_blank"} を参照してください。

* インスタンスの構築を開始する前に Campaign アーキテクチャについて理解するには、[Campaign アーキテクチャの基本を学ぶ ](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/config/architecture/architecture){target="_blank"} を参照してください。

<!--Two deployment models are available: **Campaign FDA deployment** (P1-P3) and **Campaign Enterprise (FFDA)** deployment (P4). As a customer transitioning from Campaign Standard, your deployment model is **Campaign FDA**.-->

* トランザクションメッセージ（Message Center）は、トリガーメッセージを管理するために設計された Campaign v8 モジュールです。 これは、特定のアーキテクチャモデルに依存します。詳しくは、[ この節 ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/architecture/architecture#transac-msg-archi){target="_blank"} を参照してください。

## Campaign クライアントコンソール {#acs-gs-console}

### クライアントコンソールのインストール {#acs-gs-admin-console}

管理タスクと設定タスクは、クライアントコンソールで実行します。 最初の手順は、環境を設定することです。

Campaign クライアントコンソールは、SOAPや HTTP などの標準のインターネットプロトコルを通じてAdobe Campaign アプリケーションサーバーと通信するネイティブアプリケーションです。 Campaign クライアントコンソールは、すべての機能と設定を一元化しています。また、ローカルキャッシュに依存することで、必要な帯域幅は最小限に抑えられます。簡単にデプロイできるように設計された Campaign クライアントコンソールは、インターネットブラウザーからデプロイし、自動的に更新できます。発生するトラフィックは HTTP （S）のみであり、特別なネットワーク設定は不要です。

次のビデオでは、Adobe Campaign クライアントコンソールをダウンロードしてインストールし、インスタンスへの接続を管理する方法について説明します。

>[!VIDEO](https://video.tv.adobe.com/v/335375?quality=12&learn=on){transcript=true}

詳しくは、[クライアントコンソールを使用した Campaign への接続](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/new/connect){target="_blank"}を参照してください。

クライアントコンソールは、サポートされている環境にインストールする必要があります。 詳しくは、[Campaign v8 （コンソール）互換性マトリックス ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/releases/compatibility-matrix#ClientConsoleoperatingsystems){target="_blank"} を参照してください。

### クライアントコンソールインターフェイスの確認  {#acs-gs-ui}

このチュートリアルビデオでは、Adobe Campaign V8 ユーザーインターフェイスと、主な機能の操作方法について説明します。

>[!VIDEO](https://video.tv.adobe.com/v/334496?quality=12&learn=on){transcript=true}

詳しくは [ クライアントコンソールの操作 ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/campaign-ui){target="_blank"} を参照してください。

## 環境の管理 {#acs-gs-admin-env}

クライアントコンソールをインストールしたら、次のドキュメントの手順に従ってアプリケーションサーバーへの接続を作成します。[ アプリケーションサーバーへの接続ドキュメント ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/connect#create-your-connection){target="_blank"}。

セキュリティ対策は、社内のソフトウェア開発および運用プロセスとツールに深く根付いており、インシデントを適切な方法で防止、検出、対応するために、部門の枠を超えたチームが厳しくフォローしています。 詳しくは、[Campaign セキュリティのベストプラクティス ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/privacy/security){target="_blank"} を参照してください。

### アクセス権限と権限 {#acs-gs-admin-rights}

Adobe Campaign では、ユーザーに割り当てる権限を定義し管理することができます。これらの権限は、オペレーターグループの権限、ネームド権限およびフォルダーに対する権限を組み合わせることで定義されます。

Campaign v8 に移行するCampaign Standardユーザーの権限とアクセス権は同じままです。 セキュリティ グループはAdobeによって Campaign v8 オペレーターグループに移動され、組織単位ごとのアクセス許可はフォルダーアクセス許可に移行されました。 Campaign ユーザー   Adobe IDを使用して Campaign v8 に接続すると、Campaign Standardと同じログイン名とパスワードを使用できます。

Campaign[ フォルダー ](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/config/configuration/folders-and-views){target="_blank"} は、クライアントコンソールのエクスプローラーツリー内のノードです。 タイプに基づいて、特定のタイプのデータが含まれます。 プログラムは、Campaign v8 のフォルダーによって実体化されます。 フォルダーを作成し、フォルダーへの権限を管理してアクセスを制限できます。 [詳細情報](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/admin/permissions/folder-permissions){target="_blank"}

詳しくは、[ ユーザー権限ドキュメント ](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/admin/permissions/gs-permissions){target="_blank"} を参照してください。


### Campaign コントロールパネル {#acs-gs-admin-cp}

Campaign Standardに関しては、Campaign コントロールパネルを使用して環境を管理できます。 v8 の場合、Campaign コントロールパネルにはさらに機能があります。

Campaign コントロールパネルを使用すると、各インスタンスの設定を管理したり使用状況をトラッキングしたりできるので、Adobe Campaign の製品管理者としての作業を効率化できます。 直感的なインターフェイスにより、主要なアセットの使用状況を簡単に監視できるうえ、IP アドレスの許可リスト登録、SFTP ストレージの監視、鍵の管理などの管理タスクを実行できます。

詳しくは、[ コントロールパネルのチュートリアル ](https://experienceleague.adobe.com/en/docs/control-panel-learn/tutorials/control-panel-overview){target="_blank"} と [ コントロールパネルのドキュメント ](https://experienceleague.adobe.com/docs/control-panel/using/control-panel-home.html?lang=ja){target="_blank"} を参照してください。

* **IP アドレスの追加** - Campaign Campaign コントロールパネルでは、許可リストに IP アドレスの範囲を追加することで、インスタンスへの新しい接続を設定できます。 詳しくは、[IP 許可リストへの登録に関するドキュメント ](https://experienceleague.adobe.com/en/docs/control-panel/using/instances-settings/ip-allow-listing-instance-access){target="_blank"} 参照してください。

* **サブドメイン設定** - Adobe Campaignで使用するために、ドメインのサブセクション（技術的には「DNS ゾーン」）を設定できます。
詳しくは、[ サブドメインデリゲーションのドキュメント ](https://experienceleague.adobe.com/en/docs/control-panel/using/subdomains-and-certificates/subdomains-branding){target="_blank"} を参照してください。

* **SFTP サーバーの管理** - Campaign コントロールパネルでは、アクセス権のある Campaign インスタンスに接続されているすべての SFTP サーバーとやり取りできます。 詳しくは、[SFTP 管理ドキュメント ](https://experienceleague.adobe.com/en/docs/control-panel/using/sftp-management/about-sftp-management){target="_blank"} を参照してください。


### 監査記録 {#acs-gs-admin-audit-trail}

Campaign Standardで既に使用可能な監査記録を Campaign v8 で使用すると、インスタンス内で行われた変更の全履歴にアクセスできます。

Adobe Campaign web ユーザーインターフェイスでは、監査記録機能を使用すると、インスタンス内の重要なエンティティ（通常、インスタンスのスムーズな操作に大きな影響を与えるエンティティ）に加えられたすべての変更を完全に可視化できます。 詳しくは、[ 監査記録ドキュメント ](../../v8/reporting/audit-trail.md) を参照してください

### データパッケージ {#acs-gs-admin-audit-packages}

Campaign Standardと同様に、構造化された XML ファイルを使用して様々なAdobe Campaign インスタンス間でリソースを交換するパッケージを定義できます。 これには設定パラメーターまたはデータを使用できます。

データパッケージを使用すると、プラットフォームのカスタム設定とデータをエクスポートおよびインポートできます。パッケージには、フィルタリングの有無に関わらず、様々なタイプの設定やコンポーネントを含めることができます。 Campaign v8 でのデータパッケージの使用方法については、[ このドキュメント ](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/developer/packages){target="_blank"} を参照してください。

<!--
MISSING LINKS: 

- System options
- Data Encryption/Decryption-->

### ユーザーインターフェイスのパーソナライズ {#acs-gs-admin-ui}

クライアントコンソールのユーザーインターフェイスをカスタマイズするには、次のようなオプションがあります。

* **リストとデータ表示** - リスト、ユニット、データ表示などのユーザーインターフェイス設定を管理するためのガイドラインについては、このドキュメントを参照してください。[ ユーザーインターフェイス設定ドキュメント ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/ui-settings){target="_blank"}

* **フォルダー管理** - フォルダーは、コンポーネントとデータを整理できるAdobe Campaign内のオブジェクトです。 また、権限の管理にも使用されます。 詳細情報 [ フォルダーの操作 ](../../v8/get-started/work-with-folders.md)。

* **カスタムフィールド** - カスタムフィールドは、Adobe Campaign コンソールを通じて標準スキーマに追加される追加の属性です。 これらのカスタムフィールドは、プロファイルやテストプロファイルの詳細など、様々な画面に表示されます。 詳しくは、[ カスタムフィールド設定ドキュメント ](../../v8/administration/custom-fields.md) を参照してください。

## ブランディングの設定 {#acs-gs-admin-branding}

どの会社にも、視覚的要素と技術的な詳細の両方を定義したブランドガイドラインがあります。 Adobe Campaign Standardの場合、Adobe Campaign v8 はこれらのガイドラインを一元的に管理するのに役立ちます。これにより、メールのロゴからキャンペーンで使用される URL やドメインに至るまで、すべての操作で一貫したブランドイメージを顧客に提示できます。 技術管理者は、Adobe Campaign内で複数のブランドを作成および管理できます。

詳しくは、[ ブランディングドキュメント ](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/branding/branding-gs){target="_blank"} を参照してください

## データモデルの作成について {#acs-gs-admin-data-model-creation}

Campaign Standardと同様に、Adobe Campaign v8 には事前定義済みのデータモデルが付属しています。 Adobe Campaignは、相互にリンクされたテーブルを含んだクラウドデータベースに基づいています。 詳しくは、[ データモデルのドキュメント ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/datamodel){target="_blank"} を参照してください。

スキーマは、データベーステーブルに関連付けられた XML ドキュメントです。データ構造を定義し、表の SQL 定義を記述します。[ スキーマ作成ドキュメント ](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"} を参照してください。

このビデオでは、Campaign v8 でスキーマを作成する方法と、既存のスキーマを拡張する方法について説明します。

>[!VIDEO](https://video.tv.adobe.com/v/337939?quality=12&learn=on){transcript=true}

Campaign Standardで使用可能な機能と同様に、カスタムリソースを作成できます。 Campaign v8 では、カスタムリソースはカスタムまたは拡張 **スキーマ** です。

* スキーマの操作方法については、[ このページ ](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"} を参照してください。

* 既存のスキーマを拡張する方法については、[ このページ ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema){target="_blank"} を参照してください。

* 新しいスキーマを作成する方法については、[ このページ ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/create-schema){target="_blank"} を参照してください。

* スキーマを作成または拡張する場合は、関連する入力フォームを作成または変更して、それらの変更をエンドユーザーに表示する必要があります。 入力フォームを使用すると、データスキーマに関連付けられたインスタンスを Adobe Campaign クライアントコンソールから編集できます。 フォームは名前と名前空間で識別されます。 詳しくは、[ 入力フォーム作成ドキュメント ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/forms){target="_blank"} を参照してください。

## ワークフローとデータ管理 {#acs-gs-admin-data-management}

Adobe Campaign Standardの場合と同様に、Adobe Campaign v8 には、アプリケーションサーバーのさまざまなモジュールにわたり、すべての範囲のプロセスとタスクを調整できるワークフローモジュールが含まれています。 包括的なグラフィカル環境により、セグメント化、キャンペーン実行、ファイル処理、人間の関与などを含むプロセスを設計できます。 これらのプロセスは、ワークフローエンジンが実行し、トラッキングします。 Campaign v8 でワークフローを開始する方法については、[ このドキュメント ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/data/workflows){target="_blank"} を参照してください。

以下のその他の役に立つリソースへのリンクを参照してください。

* このビデオでは、ターゲティングディメンションと作業用テーブルの概要と、Adobe Campaignで様々なデータソースにわたるデータを管理する方法について説明します。

  >[!VIDEO](https://video.tv.adobe.com/v/339992?quality=12&learn=on){transcript=true}

* Campaign を使用すると、クラウドデータベースに連絡先を追加できます。ファイルを読み込んだり、複数の連絡先の更新をスケジュールして自動化したり、web でデータを収集したり、プロファイル情報を受信者テーブルに直接入力したりできます。  詳しくは、[ データのインポート（コンソール）ドキュメント ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/data/import){target="_blank"} を参照してください。

* 様々なレポートをPDF形式や CSV 形式で簡単に書き出すことができます。これにより、レポートの共有、操作、印刷を行うことができます。 詳しくは、[ データの書き出しに関するドキュメント ](../../v8/reporting/export-reports.md) を参照してください。

## REST API {#acs-gs-admin-apis}

Campaign REST API は、Adobe Campaignと使用するテクノロジーのパネルをインターフェイスで接続することで、Adobe Campaignとの統合を作成し、独自のエコシステムを構築できることを目的としています。

Campaign v8 に移行するCampaign Standardユーザーは、REST API を使用できます。

詳しくは、[Rest API ドキュメント ](https://experienceleague.adobe.com/ja/docs/experience-cloud/campaign/apis/get-started-apis){target="_blank"} を参照してください。

Campaign Standard環境から Campaign v8 に移行する際には、REST API に適用される推奨事項と制限事項があることに注意してください。 これらは [ このページ ](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/apis/limitations){target="_blank"} に一覧表示されます。 以下の可用性に関するメモに示すように、Campaign v8 に移行する際には特定の制限も適用されます。

>[!AVAILABILITY]
>
>* PKEY の値は、既存のCampaign Standardインスタンスと移行された Campaign v8 インスタンスの間で変化します。 PKEY が外部データベースに保存されている場合は、PKEY と pkeys/hrefs リンクを提供するAdobe Campaign v8 のメイン API を呼び出すように実装を変更する必要があります。また、後続の API 呼び出しは、以前の API 呼び出しの pkeys/hrefs を使用して動的に作成する必要があり&#x200B;す。
>
>* Campaign v8 では、車両がプロファイルにリンクしたのと同じ本文に対して&#x200B;firstName プロパティは `cusVehicle` に対して無効ですが、リンクのない属性のみを含むリクエスト本文は正常に機能するというエラーが発生します。`{ "vehicleNumber": "20009", "vehicleName": "Model E", "vehicleOwner":{   "firstName":"tester 11", "lastName":"Smith 11" } }&#x200B;`
>
>* タイムゾーンは、データ移行の一環とし `profileAndServicesExt/profile` 拡張スキーマで追加されるので、REST API 呼び出しの `profileAndServices/profile` 部ではなく、REST API 呼び出しの一部としてユーザーに表示されます&#x200B;
>
>* `ccpaOptOut` は、データ移行の一環として拡張スキーマ `profileAndServicesExt/profile` 追加されるので、REST API 呼び出し `profileAndServices/profile` 含まれず、REST API 呼び出しの一部としてユーザーにのみ表示されます。
>


<!--
## Working with templates - TO REMOVE?



Workflow templates contain pre-configured settings and activities which can be reused for creating new workflows.
[Workflow template documentation](../../v8/workflows/create-workflow.md)


You can design your landing page content, and save it for future reuse. See the [landing page template documentation](../../v8/landing-pages/lp-templates.md).

Each event can trigger a personalized message. For this to happen, you need to create a message template to match each event type. Templates contain the necessary information for personalizing the transactional message. See the [Transactional messaging template documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/real-time/transactional-template)

Using a workflow template is a best practice if you need to regularly import files with the same structure. See the [Import template documentation](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/use-cases/data-management/recurring-import-workflow){target="_blank"}
-->

## 購読サービス {#acs-gs-admin-sub}

Campaign Standardと同様、管理者は購読サービスを作成でき、マーケターは購読者にメッセージを送信できます。 主要な概念と実装の手順は、Campaign Standardに沿っています。 以下に役立つリンクとビデオを示します。

購読とターゲット購読者を設定し管理する方法について説明します。

>[!VIDEO](https://video.tv.adobe.com/v/334305?quality=12&learn=on){transcript=true}

* 購読サービス [web ユーザーインターフェイスのドキュメント ](../../v8/audience/manage-subscribers.md) を参照してください。

* クライアントコンソールで購読サービスを設定するためのドキュメントについては、[ この節 ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/audience/subscriptions){target="_blank"} も参照してください。

## メッセージと配信{#acs-gs-msg}

### 配信チャネルの設定 {#acs-gs-admin-channels}

Adobe Campaign v8 をCampaign Standardとして使用すると、メール、SMS、プッシュ通知、ダイレクトメールなどのクロスチャネルキャンペーンを送信し、各種の専用レポートを使用してその効果を測定できます。 これらのメッセージは、デザインし、配信を介して送信します。また、受信者ごとにパーソナライズすることができます。コア機能には、ターゲティング、メッセージの定義とパーソナライゼーション、通信の実行、関連する運用可能なレポートなどがあります。主な機能のアクセスポイントは、配信ウィザードです。このアクセスポイントから、Adobe Campaign で提供される複数の機能を使用できます。

管理者は、チャネル設定を定義する必要があります。 詳しくは、以下のリンクを参照してください。

* **メール** - メールの設定について詳しくは、[ このページ ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/emails/email-parameters){target="_blank"} を参照してください。
* **SMS** - SMS チャネルの設定方法については、[ このドキュメント ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/sms/sms){target="_blank"} を参照してください。
* **プッシュ通知** - プッシュ通知チャネルを設定する手順について詳しく説明します [ この節 ](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/send/push/push-data-collection){target="_blank"}。
* **トランザクションメッセージ** - Campaign v8 で [ トランザクションメッセージ ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/real-time/transactional){target="_blank"} の設定手順について詳しくは、[ この節 ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/transactional-msg-settings) を参照してください

### 外部アカウント {#acs-gs-ext-accounts}

管理者は、Campaign の外部アカウントの設定と保守を担当します。 Campaign Standardと同様、外部アカウントは、テクニカルワークフローやキャンペーンワークフローなどの技術プロセスで使用されます。

Campaign v8 への移行プロセスでは、既存のCampaign Standard外部アカウントが処理され、クライアントコンソールで使用できるようになります。

詳しくは、[ 外部アカウント設定 ](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/config/configuration/external-accounts){target="_blank"} を参照してください。


<!--
**Email**

MISSING LINKS :
- general email channel parameters 
- email routing accounts 
- email processing rules 
- email properties
-->

<!--
MISSING LINKS: 
- Setting external account 
- Adding vender details etc. -->

<!--
**Mobile app**
MISSING LINKS: 
- Configuring a mobile application using AEP SDKs 
- Sync Mobile app AEPSDK  
- Setting up your application in Adobe Campaign 
- Channel-specific application configuration
-->

### 動的コンテンツ {#acs-gs-dyn-content}

Campaign を使用して動的コンテンツを作成し、パーソナライズされたメッセージを送信します。パーソナライゼーション機能を組み合わせて、メッセージを改善し、カスタムなユーザーエクスペリエンスを実現することができます。

このビデオでは、Campaign v8 を管理者として使用する場合の、動的コンテンツブロックと、動的コンテンツブロックを使用してメール配信のコンテンツをパーソナライズする方法を定義できます。

>[!VIDEO](https://video.tv.adobe.com/v/342088?quality=12&learn=on){transcript=true}

参考になるリンク：

* [ パーソナライゼーションの概要 ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/personalize/personalize){target="_blank"}
* [ パーソナライゼーションブロックの使用 ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/personalize/personalization-blocks){target="_blank"}
* [ 条件付きコンテンツの作成 ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/personalize/conditions){target="_blank"}
* [Personalizationのデータソース ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/personalize/personalization-data){target="_blank"}

### 配信テンプレート {#acs-gs-templates}

Campaign Standardの場合と同様に、配信テンプレートの使用は、Campaign v8 では必須です。

設計プロセスを加速し改善するために、配信テンプレートを作成して、キャンペーン全体でカスタムコンテンツや設定を簡単に再利用できます。 この機能を使用すると、クリエイティブなルックアンドフィールを標準化して、キャンペーンの実行と開始をより迅速に行うことができます。 [Campaign web ユーザーインターフェイス ](../../v8/msg/delivery-template.md) で配信テンプレートを作成する方法を説明します。 クライアントコンソールで配信テンプレートを作成する方法については、[ この節 ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/create-templates){target="_blank"} も参照してください。

### タイポロジルール {#acs-gs-admin-rules}

管理者は、配信のタイポロジルールの作成と管理を担当します。 Adobe Campaign Standardと同様、Campaign v8 では、タイポロジルールはメッセージを送信する前にチェックとフィルタリングを行うことができるビジネスルールです。

Campaign Standard環境から Campaign v8 に移行すると、タイプオリジールールが Campaign v8 に移行されます。

Campaign v8 では、タイポロジルールにキャンペーンの最適化のアドオンが付属しています。 このモジュールでは、配信の送信を制御、フィルタリングおよび監視できます。 キャンペーン間の競合を回避するために、Adobe Campaign では特定の制限ルールを適用して、様々な組み合わせをテストできます。これにより、送信されるメッセージが、顧客や会社の通信ポリシーのニーズと期待に応えることが保証されます。 詳しくは、[ タイポロジルールのドキュメント ](https://experienceleague.adobe.com/en/docs/campaign/automation/campaign-optimization/campaign-typologies){target="_blank"} を参照してください。

### 強制隔離の管理 {#acs-gs-admin-quarantine}

すべての強制隔離アドレスと強制隔離ルールがCampaign Standard環境から Campaign v8 に移行されました。 強制隔離管理には、特定のアクションは必要ありません。

管理者は、[ このページ ](../../v8/audience/quarantine.md) 以降、Campaign v8 での強制隔離管理について理解します。 [ この節 ](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/send/failures/quarantines#access-quarantined-addresses){target="_blank"} の強制隔離管理に関するクライアントコンソールの詳細なドキュメントも参照してください。


## Adobe Campaign統合の管理 {#acs-gs-integrations}

Campaign インスタンスをAdobe Experience Cloud ソリューションに接続して、機能を組み合わせることができます。 Adobe Campaign にはいくつかのコネクタが付属しており、それらを使用して、外部アプリケーションとの通信、データベースエンジンへの接続、データの共有と同期などを行うことができます。ソリューションを組み合わせる方法については、[ このドキュメント ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/integration){target="_blank"} を参照してください。

Campaign v8 に移行するCampaign Standardユーザーには、次の点が適用されます。

* Campaign Standardでこれらの統合を使用していた場合、**Adobe Analytics** および **Audience Manager** の設定とデータはAdobeによって移行されています。
* Campaign Standard環境が **Adobe Experience Manager** と統合されている場合、Campaign web ユーザーインターフェイスでメールをデザインする際にこの機能を使用でき、メール配信コンテンツとフォームをAdobe Experience Manager内で直接効率的に管理できるように、AdobeAdobe Experience Manager as a Cloud Serviceでは **2}Campaign} に移行することをお勧めします。**&#x200B;詳しくは、[ このページ ](../../v8/integrations/aem-content.md) を参照してください。
Campaign はAdobe Experience Manager 6.5 と統合することもできます。この統合を設定するには、[ このドキュメント ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-aem){target="_blank"} を参照してください。
* Campaign Standard環境が **トリガー** と統合された場合は、[ このページ ](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/connect/ac-triggers){target="_blank"} を参照して、Campaign v8 でこの統合を設定する必要があります。
* Campaign Standard環境が **Adobe Target** と統合された場合は、[ このページ ](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/connect/ac-at){target="_blank"} を参照して、Campaign v8 でこの統合を設定する必要があります。

