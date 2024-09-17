---
title: マーケター向け Adobe Campaign v8 の基本を学ぶ
description: Campaign v8 の主な機能を確認します。 Campaign Standard から Campaign v8 に移行するマーケターを対象としています。
role: User
level: Beginner, Experienced
source-git-commit: e68ad7ca3368165feb534363c36b03b510291e8a
workflow-type: tm+mt
source-wordcount: '2453'
ht-degree: 22%

---


# マーケター向けの基本を学ぶ {#acs-gs-marketers}

このガイドでは、Campaign Standardから Campaign v8 に移行するマーケターを対象に、Campaign v8 の主な機能の概要を説明します。

Adobe Campaign v8 には、クライアントコンソールまたは web ユーザーインターフェイスからアクセスできます。 Web インターフェイスを使用すると、主要なマーケティングアクションを作成、管理および実行できます。 新しい Adobe Campaign Web インターフェイスは、マーケティングキャンペーンのデザインと配信を簡素化する、最新の直感的なユーザーエクスペリエンスを提供します。[詳細情報](../../v8/get-started/user-interface.md)。

移行に伴い、Campaign Standardのすべてのデータが Campaign v8 にインポートされるので、進行中の業務の中断を最小限に抑えながらスムーズに移行できます。

既存の資格情報を引き続き使用してログインし、新しいAdobe Campaign v8 インスタンスに接続できます。 ログインすると、すべてのプロファイルとワークフローが移行されているのを確認でき、キャンペーンで引き続き作業を行うことができます。

主な違いはユーザーインターフェイスです。 2 つのインターフェイスでの同じワークフローの比較を次に示します。

![](assets/transition_workflow.png){zoomable="yes"}


>[!NOTE]
> Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対して、よりスケーラブルで段階的なアプローチを実現できる継続的配信モデルに基づいて動作します。最新の更新については、定期的に[リリースノート](../../v8/rn/release-notes.md)を参照してください。

## Campaign web ユーザーインターフェイスの確認 {#acs-gs-marketers-ui}

次のビデオでは、Campaign web ユーザーインターフェイスにアクセスして操作する方法と、在庫リストをカスタマイズする方法について説明します。

>[!VIDEO](https://video.tv.adobe.com/v/3427278?quality=12&learn=on){transcript=true}

詳しくは、以下のドキュメントを参照してください。

1. [Campaign web ユーザーインターフェイスの確認](../../v8/get-started/user-interface.md)

1. [リストの参照とフィルタリング](../../v8/get-started/list-filters.md)


## プロファイルとオーディエンスの作成と管理 {#acs-gs-marketers-profiles-and-audiences}

Campaign v8 でのプロファイルとオーディエンスの作成および管理に関する一般的な概念は、Adobe Campaign Standardの場合と同じです。 プロファイルとオーディエンスの使用を開始する方法については、[ この節 ](../../v8/audience/gs-audiences-recipients.md) を参照してください。

開始するのに役立つリンクを以下にいくつか示します。

### プロファイルの管理 {#acs-gs-marketers-profiles}

Adobe Campaignでは、プロファイルはデータベースに保存されたレコードであり、配信用のオーディエンスを作成し、パーソナライゼーションデータをコンテンツに追加するための主要なコンポーネントとして機能します。

1. Campaign web ユーザーインターフェイスを使用してプロファイルにアクセス、管理、調査する方法については、次のビデオを参照してください。

   >[!VIDEO](https://video.tv.adobe.com/v/3427293?quality=12&learn=on){transcript=true}

   詳しくは、[ プロファイルの基本を学ぶ ](../../v8/audience/about-recipients.md) ドキュメントを参照してください。

1. Campaign v8 での [ テストプロファイルの作成と管理 ](../../v8/audience/test-profiles.md) 方法を説明します。

### オーディエンス管理 {#acs-gs-marketers-audiences}

オーディエンスは、類似の行動や特性を共有するプロファイルのセットです。 この人物のコレクションは、生成、選択、または読み込みが可能です。作成したオーディエンスは、配信のターゲット母集団として活用できます。

オーディエンスを作成および管理する方法、配信のオーディエンスを選択する方法、コントロール母集団を定義する方法については、このビデオを参照してください。

>[!VIDEO](https://video.tv.adobe.com/v/3425861?quality=12&learn=on){transcript=true}

詳しくは、[ オーディエンスの基本を学ぶ ](../../v8/audience/manage-audience.md){target="_blank"} を参照してください。

Campaign Standardと同様に、配信にコントロール母集団を追加できます。 コントロール母集団を定義して、オーディエンスの一部にメッセージを送信しないようにし、配信後の動作をメインターゲットと比較できます。このオプションは、キャンペーンの影響を測定するのに役立ちます。
[ コントロール母集団を設定 ](../../v8/audience/control-group.md){target="_blank"} する方法を説明します。

>[!AVAILABILITY]
>
>* Campaign Standardクエリ アクティビティを使用して作成されたすべてのオーディエンスは、移行中に Campaign v8 で定義済みフィルターに変換されます。 Campaign v8 は、クエリ アクティビティもサポートしています。
>
>* オーディエンスを読み取りは、（定義済みフィルター [ を使用してクエリアクティビティに変換 ](../../v8/query/build-query.md) れます
>
>* 定義済みフィルターは、オーディエンスが Campaign v8 に移行された後にのみ、最新の値を取ります。
>
>* Campaign Standardのファイルタイプオーディエンスは、ディメンションのないリストタイプとして移行されます。

### 購読を管理 {#acs-gs-marketers-sub}

ニュースレターなどのサービスを管理および作成し、これらのサービスの購読や購読解除を確認できます。 主な手順は、全体的にCampaign Standardの場合と同じです。 詳しくは、以下のページを参照してください。

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/ja/docs/campaign-web/v8/audiences/work-with-services/manage-services">
<img alt="低頻度" src="assets/lp-list.jpg">
</a>
<div>
<a href="https://experienceleague.adobe.com/ja/docs/campaign-web/v8/audiences/work-with-services/manage-services"><strong>購読サービスの作成</strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/ja/docs/campaign-web/v8/audiences/work-with-services/manage-subscribers">
<img alt="低頻度" src="assets/workflow-activities.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/ja/docs/campaign-web/v8/audiences/work-with-services/manage-subscribers"><strong>購読者の管理<strong></strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/ja/docs/campaign-web/v8/msg/send-to-subscribers">
<img alt="検証" src="assets/workflow-create.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/ja/docs/campaign-web/v8/msg/send-to-subscribers"><strong>メッセージをサービスのサブスクライバーに送信</strong></a>
</div>
<p>
</td>
</tr>
</table>

## プラン、プログラム、キャンペーンの使用 {#acs-gs-marketers-plans}

Adobe Campaign v8 では、マーケティングプランおよびプログラムのフォルダー階層を設定できます。 プラン、プログラム、キャンペーンの機能は、Campaign Standard と Campaign v8 とでは似ています。

詳しくは、[ プランとプログラムのドキュメント ](../../v8/administration/plans-programs.md) を参照してください。

開始するのに役立つリンクを以下に示します。 ユーザーエクスペリエンスに影響を与える可能性のある変更は、可用性メモでハイライト表示されます。


### キャンペーンの作成 {#acs-gs-marketers-campaign}

Adobe Campaignでは、組み込みのキャンペーン管理機能を使用して、ターゲットにするマーケティング活動を簡単に調整できます。 スケジュールを定義する機能を使用すると、戦略目標に合わせてキャンペーンの期間とタイミングを計画し、オーディエンスのエンゲージメントを最大化できます。

![キャンペーンフロー](assets/campaign-flow.png)

キャンペーンについて詳しくは、次のドキュメントに従います。

1. [キャンペーンの基本を学ぶ](../../v8/campaigns/gs-campaigns.md)
1. [キャンペーンへのアクセスと管理](../../v8/campaigns/manage-campaigns.md)
1. [最初のキャンペーンを作成](../../v8/campaigns/create-campaigns.md)


### ワークフローの作成 {#acs-gs-marketers-wf}

Campaign web ユーザーインターフェイスのワークフローユーザーインターフェイスが完全に刷新され、使用、設定、実行、トラブルシューティングが容易になりました。 Campaign Standardでの経験と同様に、ワークフローを使用すると、あらゆるプロセスとタスクを調整し、セグメントの作成やメッセージの準備から配信に至るまでの、マーケティングキャンペーンのあらゆる側面でスピードと規模を改善できます。 さらに、キャンペーンオーケストレーション用の使いやすい単一のインターフェイスでチャネルを同期させることができます。

このビデオでは、ワークフローの仕組みと、ターゲティングワークフローの作成方法について説明します。

>[!VIDEO](https://video.tv.adobe.com/v/3425873?quality=12&learn=on){transcript=true}

詳しくは、[ ワークフローのドキュメント ](../../v8/workflows/gs-workflows.md) を参照してください。

Adobe Campaignの web ユーザーインターフェイスは、ワークフローのクエリモデラーを備えており、様々な条件に基づいてデータベースをフィルタリングするプロセスを簡素化します。 [ クエリモデラーの詳細情報 ](../../v8/query/query-modeler-overview.md)

ワークフロー内の各アクティビティの目的と機能を理解するには、[ ワークフローアクティビティ ](../../v8/workflows/activities/about-activities.md) で使用できる詳細情報を調べます。

[ ワークフローのガードレールと制限 ](../../v8/get-started/guardrails.md) を確認して、ワークフローの効率を最大化します。

>[!AVAILABILITY]
>
>* ワークフローの実行 [ 履歴とログ ](../../v8/workflows/start-monitor-workflows.md#logs-tasks) は、Adobe Campaign v8 で利用できます。
>
>* Campaign Standardインスタンスで実行されたワークフローの履歴ログは、Campaign v8 に移行されません。
>
>* 組織単位は、マッピングおよび同様のアクセス制御を確保するために、フォルダーの概念にマッピングされます。
>

## 配信の作成と管理 {#acs-gs-marketers-deliveries}

Campaign web ユーザーインターフェイスを使用する場合、マーケターは、スタンドアロンの配信を **配信** の左側のメニューから作成したり、キャンペーンに含まれているかどうかに関係なく、ワークフローのコンテキストで配信を作成したりできます。 主な手順は、Campaign Standardにおける以前のエクスペリエンスと連携しています。 配信の作成方法については、[ 配信の作成と管理に関するドキュメント ](../../v8/msg/gs-deliveries.md) の節を参照してください。

参考になるリンク：

* **配信テンプレート** – 改善されて高速化した設計プロセスを実現するために、配信テンプレートを作成して、キャンペーン全体でカスタムコンテンツや設定を簡単に再利用できます。 この機能を使用すると、クリエイティブなルックアンドフィールを標準化して、キャンペーンの実行と開始をより迅速に行うことができます。詳しくは、[ 配信テンプレート ](../../v8/msg/delivery-template.md) ページを参照してください。

* **配信設定** – 配信設定は、配信テンプレートで定義される技術的な配信パラメーターです。 配信ごとに過負荷になる可能性があります。これらの設定は、配信または配信テンプレートの編集時に使用できる「設定」ボタンから使用できます。 詳しくは、[ 配信設定 ](../../v8/advanced-settings/delivery-settings.md) の節を参照してください。

* **動的コンテンツ** - Adobe Campaignの web 動的コンテンツ機能を使用すると、受信者について収集した情報に基づいてコンテンツをカスタマイズできます。 動的コンテンツを利用することで、マーケティング活動の関連性が高まり、不要な製品やサービスのマーケティングを回避できます。詳しくは、[ 動的コンテンツ ](../../v8/personalization/gs-personalization.md) の節を参照してください。

* **テストと配達確認** – 配信コンテンツを定義したら、メッセージを送信する前に、プロファイルとテストプロファイルを使用してプレビューとテストを行うことができます。 この手順は、正確であると同時に、コンテンツとパーソナライゼーション設定の両方にエラーがないことを確認するために重要です。 [ プレビューとテスト ](../../v8/preview-test/preview-test.md) を参照してください。

* **スケジュール** - メッセージを送信する日付と正確な時刻を設定できます。 マーケティングメッセージに最も適した時間を選択することで、開封率を最大化します。

   * 詳しくは、[ スタンドアロン配信をスケジュールする ](../../v8/msg/gs-deliveries.md#gs-schedule) を参照してください。
   * 詳しくは、[ ワークフローで配信をスケジュールする ](../../v8/monitor/schedule-sending.md#schedule-a-delivery-in-a-campaign-workflow) を参照してください。

* **オファーを追加** - Adobe Campaign web ユーザーインターフェイスを使用して、配信にオファーを追加できます。 これらのオファーは、オファーの左側のメニューから使用できます。このメニューから、オファーのリストにアクセスできます。  方法を学ぶ [ メッセージにオファーを追加する ](../../v8/msg/offers.md)

>[!AVAILABILITY]
>
>* ドラフト状態または完了状態の配信が移行されました。
>
>* 次のいずれかのステータスの配信はAdobe Campaign v8 に移行されましたが、再度準備する必要があります：送信中/処理中/キャンセル/再試行中/準備エラー。
>
>* 次のいずれかのステータスの配信がキャンセル済み配信として移行されました：キャンセル済み/再試行中
>
>* トラッキングリンク、ミラーページ URL リンク、購読/購読解除リンクはCampaign Standardと同様に機能します。
>
>Adobe Campaignの [ トラッキングとモニタリング ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/analytics/tracking){target="_blank"}、[ ブランディング ](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/branding/branding-gs){target="_blank"} の節も参照してください。

### メール配信 {#acs-gs-marketers-email}

ゼロからメール配信を作成する方法、オーディエンスを定義する方法、コンテンツをデザインする方法、プレビューをシミュレートする方法、配達確認を送信する方法を次のビデオで説明します。

>[!VIDEO](https://video.tv.adobe.com/v/3425866?quality=12&learn=on){transcript=true}

最初のターゲットメールを作成する方法については、[ 最初のメールの作成 ](../../v8/email/create-email.md) ドキュメントを参照してください

Campaign v8 では、メール配信を作成、テストおよび送信する詳細な手順はCampaign Standardと似ています。

1. **コンテンツの設計と定義**

   Campaign v8 の E メールデザイナーは、Campaign Standardで使用できる E メールデザイナーと似ています。 数年前に、Campaign Standard[ レガシーのメールエディターは非推奨 ](https://experienceleague.adobe.com/en/docs/campaign-standard/using/release-notes/deprecated-features#deprecated-features){target="_blank"} なりました。 メールコンテンツを作成およびパーソナライズするには、既に Campaign メールDesignerに移行しているはずです。

   E メールデザイナーの操作方法について説明します。次のビデオでは、メールをゼロから構成およびデザインする方法、メールをパーソナライズおよびテストする方法について説明します。

   >[!VIDEO](https://video.tv.adobe.com/v/3425867?quality=12&learn=on){transcript=true}

   E メールデザイナーを使用すると、直感的なドラッグ＆ドロップインターフェイスを通じて、個別にカスタマイズされた魅力的なメールを作成できます。詳しくは、[ メールDesignerのドキュメント ](../../v8/email/get-started-email-designer.md) を参照してください。

   HTMLをアップロードしてメールを作成する方法、メールDesignerと互換性を持たせる方法、テンプレートに変換する方法については、このビデオを参照してください。

   >[!VIDEO](https://video.tv.adobe.com/v/3427633?quality=12&learn=on){transcript=true}

   コンテンツフラグメントは、1 つ以上のメッセージで参照できる再利用可能なコンポーネントです。メール配信の作成を簡素化する [ コンテンツフラグメント ](../../v8/content/fragments.md) について説明します。

   高速で改善された設計プロセスを実現するために、スタンドアロンテンプレートを作成して、Adobe Campaign全体でカスタムコンテンツを簡単に再利用できます。 [ メールテンプレートの作成 ](../../v8/email/create-email-templates.md) を参照してください。

1. **プレビューとテスト**

   このビデオでは、メールメッセージのコンテンツとパーソナライゼーションをプレビューし、テスト配信（配達確認）を送信し、一般的なデスクトップ、モバイル、web ベースのクライアントでメールのレンダリングを確認する方法について説明します。

   >[!VIDEO](https://video.tv.adobe.com/v/3425862?quality=12&learn=on){transcript=true}

1. **メールの送信とログの確認**

   コンテンツ、オーディエンスおよびスケジュールを定義したら、メール配信の準備を始めます。 詳しくは、次の節を参照してください。

   * [メールの準備と送信](../../v8/monitor/prepare-send.md)
   * [配信ログの監視](../../v8/monitor/delivery-logs.md)


### SMS 配信 {#acs-gs-marketers-sms}

SMS 配信は、顧客のモバイルデバイスにテキストメッセージを送信する実用的で効率的な方法を提供します。この機能を使用すると、テキストベースのメッセージを作成、パーソナライズ、プレビューして、効果的な通信を実現できます。

Campaign v8 では、SMS 配信を作成、テストおよび送信する詳細な手順は、Campaign Standardの場合と同様です。


<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/ja/docs/campaign-web/v8/msg/sms/create-sms">
<img alt="リード" src="assets/create_sms.png">
</a>
<div><a href="https://experienceleague.adobe.com/ja/docs/campaign-web/v8/msg/sms/create-sms"><strong>SMS 配信を作成</strong>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/ja/docs/campaign-web/v8/msg/sms/content-sms">
<img alt="低頻度" src="assets/design_sms.png">
</a>
<div>
<a href="https://experienceleague.adobe.com/ja/docs/campaign-web/v8/msg/sms/content-sms"><strong>SMS 配信をデザイン<strong></strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/ja/docs/campaign-web/v8/msg/sms/send-sms">
<img alt="検証" src="assets/send_sms.png">
</a>
<div>
<a href="https://experienceleague.adobe.com/ja/docs/campaign-web/v8/msg/sms/send-sms"><strong>SMS 配信のプレビューと送信</strong></a>
</div>
<p>
</td>
</tr></table>

### プッシュ通知 {#acs-gs-marketers-push}

プッシュ通知は、モバイルアプリのユーザーが積極的にアプリを使用していない場合でも、そのユーザーに通知するために不可欠です。 更新の提供、特定のアクションの促進、お得な情報の通知など、様々な目的に対応します。

Campaign v8 では、プッシュ通知配信を作成、テストおよび送信する詳細な手順はCampaign Standardと似ています。


<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/ja/docs/campaign-web/v8/msg/push/create-push">
<img alt="リード" src="assets/push_create.jpeg">
</a>
<div><a href="https://experienceleague.adobe.com/ja/docs/campaign-web/v8/msg/push/create-push"><strong>プッシュ配信を作成</strong>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/ja/docs/campaign-web/v8/msg/push/content-push">
<img alt="低頻度" src="assets/push_design.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/ja/docs/campaign-web/v8/msg/push/content-push"><strong>プッシュ配信をデザイン<strong></strong></a>
</div>
<p></td>
<td>
<a href="https://experienceleague.adobe.com/ja/docs/campaign-web/v8/msg/push/send-push">
<img alt="検証" src="assets/push_send.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/ja/docs/campaign-web/v8/msg/push/send-push"><strong>プッシュ配信のプレビューと送信</strong></a>
</div>
<p>
</tr></table>

>[!AVAILABILITY]
>
>* Adobe Campaign v8 は、AndroidとiOS プッシュチャネルの両方をサポートしています。 プッシュチャネルを使用して既存のワークフローと配信を移行する場合は、Adobe Campaignのトランジションマネージャーに接続してください。 詳しくは、[ チャネル設定 ](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/send/push/push-data-collection){target="_blank"} を参照してください。
>
>* なお、モバイルアプリケーション用の SDK V4 は、数年前に [Campaign Standardで非推奨 ](https://experienceleague.adobe.com/en/docs/campaign-standard/using/release-notes/deprecated-features#deprecated-features){target="_blank"} になっていました。 Adobe Experience Platform SDK には既に移行している必要があります。これは、Campaign v8 で使用される SDK と同じです。
> 

### ダイレクトメール {#acs-gs-marketers-direct-mail}

ダイレクトメールは、はがき、チラシ、カタログなどのパーソナライズされたレターを顧客に一括配信するためのファイルを作成できるオフラインチャネルです。 ダイレクトメール配信の作成時に、Adobe Campaignでは、すべてのターゲットプロファイルと、選択したデータ（住所やプロファイル属性など）を含む抽出ファイルを自動的に生成します。

Campaign v8 では、ダイレクトメール配信の作成、テストおよび送信の詳細な手順はCampaign Standardの場合と同様です。


1. [ダイレクトメール配信の作成](../../v8/direct-mail/create-direct-mail.md)
1. [ 抽出ファイルの定義 ](../../v8/direct-mail/content-direct-mail.md)
1. [プレビューして送信](../../v8/direct-mail/send-direct-mail.md)

### アプリ内チャネル {#acs-gs-marketers-in-app}

アプリ内チャネルは、Campaign v8 では使用できません。 アプリ内通知を送信する必要がある場合は、Adobe担当者にお問い合わせください。

## ランディングページの作成と管理 {#acs-gs-marketers-lp}

Adobe Campaign v8 web ユーザーインターフェイスは、ランディングページのユーザーエクスペリエンスを刷新したものです。 Campaign では、ランディングページを作成、デザインおよび共有できます。 ランディングページでは、ユーザーをオンラインフォームに誘導して、データを更新したり、通信の受信をオプトイン／オプトアウトしたり、ニュースレターなどの特定のサービスを購読したりできます。

Campaign v8 に移行するCampaign Standardユーザーの場合、既存のランディングページは Campaign web ユーザーインターフェイスに移行されます。 同じ範囲の機能にアクセスできます。

ランディングページについて詳しくは、次の節を参照してください。

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/ja/docs/campaign-web/v8/landing-pages/create-lp">
<img alt="リード" src="assets/lp-subscription.jpeg">
</a>
<div><a href="https://experienceleague.adobe.com/ja/docs/campaign-web/v8/landing-pages/create-lp"><strong>ランディングページの作成</strong>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/ja/docs/campaign-web/v8/landing-pages/lp-content">
<img alt="検証" src="assets/lp-design.jpg">
</a>
<div>
<a href="https://experienceleague.adobe.com/ja/docs/campaign-web/v8/landing-pages/lp-content"><strong>ランディングページの設計</strong></a>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/ja/docs/campaign-web/v8/landing-pages/lp-templates">
<img alt="検証" src="assets/lp-reporting.jpg">
</a>
<div>
<a href="https://experienceleague.adobe.com/ja/docs/campaign-web/v8/landing-pages/lp-templates"><strong>ランディングページテンプレートの操作</strong></a>
</div>
<p>
</td>
</tr></table>


## レポート {#acs-gs-marketers-reporting}

Adobe Campaignには、一連の [ レポートツール ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/analytics/reports/gs-reporting){target="_blank"} が用意されています。 管理者は、レポートを作成および設定して、他の Campaign ユーザーと共有できます。

Adobe Campaign レポートツールスイートは、マーケティング活動の有効性に関する貴重なインサイトを提供し、最大の効果を得るためにキャンペーンを最適化できます。 詳しくは、[ レポートドキュメント ](../../v8/reporting/gs-reports.md) を参照してください。

さらに、Adobe Campaign Standardのエクスペリエンスと連携して、Campaign v8 ではメール配信に関する動的レポートを使用できます。 完全にカスタマイズ可能なリアルタイムのレポートを提供して、マーケティングアクティビティの影響を測定します。 プロファイルデータへのアクセスが追加され、開封数やクリック数などの機能的なメールキャンペーンデータに加えて、性別、市区町村、年齢などのプロファイルディメンション別のデモグラフィック分析を可能にします。詳しくは、[ 動的レポートドキュメント ](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/reporting/get-started-reporting){target="_blank"} を参照してください

>[!AVAILABILITY]
>
>* [ 動的レポート ](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/reporting/get-started-reporting){target="_blank"} は、メール配信のレポート、メール配信を含むキャンペーン、トランザクションメッセージに使用できます。 プロファイルディメンション別の人口統計学的分析も使用できます。
>
> * [Adobe Campaign web ユーザーインターフェイス レポート ](../../v8/reporting/campaign-reports.md) は、Adobe Campaign StandardからAdobe Campaign v8 への移行において、すべてのユーザーが使用できます。

Adobe Campaign には 3 つの異なるレポートがあります。

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="https://experienceleague.adobe.com/ja/docs/campaign-web/v8/reports/campaign-report/campaign-reports">
<img alt="検証" src="./assets/campaign_report.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/ja/docs/campaign-web/v8/reports/campaign-report/campaign-reports"><strong>キャンペーンレポート</strong></a>
</div>
<p>
<div>
<p>個々の配信のパフォーマンス、有効性、結果に関する詳細情報を提供し、包括的な概要を提供します。</p>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/ja/docs/campaign-web/v8/reports/delivery-report/delivery-reports">
<img alt="リード" src="assets/email_report.jpeg">
</a>
<div><a href="https://experienceleague.adobe.com/ja/docs/campaign-web/v8/reports/delivery-report/delivery-reports"><strong>配信レポート</strong>
</div>
<p>
<div>
<p>成功率、オーディエンスのエンゲージメント、その他の重要な指標など、チャネルごとの各配信のパフォーマンスを徹底的に分析します。 キャンペーンの全体的な有効性と影響を評価できます。</p>
</div>
<p>
</td>
<td>
<a href="https://experienceleague.adobe.com/ja/docs/campaign-web/v8/reports/global-report/global-reports">
<img alt="グローバルレポート" src="assets/push_report.jpeg">
</a>
<div>
<a href="https://experienceleague.adobe.com/ja/docs/campaign-web/v8/reports/global-report/global-reports"><strong> グローバルレポート</strong></a>
</div>
<p>
<div>
<p>Campaign インスタンス内の各チャネルのトラフィックおよびエンゲージメント指標の総合的な概要を提供します。 これらのレポートは様々なウィジェットで構成され、それぞれがキャンペーンや配信パフォーマンスに関する明確な観点を提供します。</p>
</div>
<p>
</td>
</tr>
</table>
