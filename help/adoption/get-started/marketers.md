---
title: マーケター向け Adobe Campaign v8 の基本を学ぶ
description: Campaign v8 の主な機能を確認Campaign Standard から Campaign v8 に移行するマーケターを対象としています。
role: User
level: Beginner, Experienced
exl-id: 514da15d-325b-4d28-9a58-50c1ae2e4925
source-git-commit: 09794df17632df243bf736d08a5a53319d79bf5f
workflow-type: tm+mt
source-wordcount: '2453'
ht-degree: 95%

---

# マーケター向けの基本を学ぶ {#acs-gs-marketers}

このガイドでは、Campaign Standard から Campaign v8 に移行するマーケターを対象に、Campaign v8 の主な機能の概要を説明します。

Adobe Campaign v8 には、クライアントコンソールまたは web ユーザーインターフェイスからアクセスできます。Web インターフェイスを使用すると、主なマーケティングアクションを作成、管理、実行できます。新しい Adobe Campaign web インターフェイスは、マーケティングキャンペーンのデザインと配信を簡素化する、最新の直感的なユーザーエクスペリエンスを提供します。[詳細情報](../../v8/get-started/user-interface.md)。

移行に伴い、Campaign Standard のすべてのデータが Campaign v8 に読み込まれるので、進行中の業務の中断を最小限に抑えながらスムーズに移行できます。

既存の資格情報を引き続き使用してログインし、新しい Adobe Campaign v8 インスタンスに接続できます。ログインすると、移行中のすべてのプロファイルとワークフローを確認でき、キャンペーンで引き続き作業を行うことができます。

主な違いはユーザーインターフェイスです。2 つのインターフェイスでの同じワークフローの比較を次に示します。

![](assets/transition_workflow.png){zoomable="yes"}


>[!NOTE]
> Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対して、よりスケーラブルで段階的なアプローチを実現できる継続的配信モデルに基づいて動作します。最新の更新については、定期的に[リリースノート](../../v8/rn/release-notes.md)を参照してください。

## Campaign web ユーザーインターフェイスの確認 {#acs-gs-marketers-ui}

以下のビデオでは、Campaign web ユーザーインターフェイスにアクセスして操作する方法と、在庫リストをカスタマイズする方法について説明します。

>[!VIDEO](https://video.tv.adobe.com/v/3427278?quality=12&learn=on){transcript=true}

詳しくは、以下のドキュメントを参照してください。

1. [Campaign web ユーザーインターフェイスの確認](../../v8/get-started/user-interface.md)

1. [リストの参照とフィルタリング](../../v8/get-started/list-filters.md)


## プロファイルとオーディエンスの作成と管理 {#acs-gs-marketers-profiles-and-audiences}

Campaign v8 でプロファイルとオーディエンスを作成および管理する一般的な概念は、Adobe Campaign Standard と同じです。プロファイルとオーディエンスを開始する方法について詳しくは、[この節](../../v8/audience/gs-audiences-recipients.md)を参照してください。

開始するのに役立つリンクを以下に示します。

### プロファイルの管理 {#acs-gs-marketers-profiles}

Adobe Campaign では、プロファイルはデータベースに保存されるレコードであり、配信のオーディエンスを作成し、コンテンツにパーソナライゼーションデータを追加する際に重要なコンポーネントとして機能します。

1. このビデオでは、Campaign web ユーザーインターフェイスを使用してプロファイルにアクセス、管理および探索する方法について説明します。

   >[!VIDEO](https://video.tv.adobe.com/v/3427293?quality=12&learn=on){transcript=true}

   詳しくは、[プロファイルの基本を学ぶ](../../v8/audience/about-recipients.md)ドキュメントを参照してください。

1. Campaign v8 でテストプロファイルを作成および管理する方法を学ぶ

   >[!VIDEO](https://video.tv.adobe.com/v/3442844?quality=12&learn=on){transcript=true}

### オーディエンス管理 {#acs-gs-marketers-audiences}

オーディエンスとは、類似した行動や特性を共有する一連のプロファイルです。この人物のコレクションは、生成、選択、または読み込みが可能です。作成したオーディエンスは、配信のターゲット母集団として活用できます。

このビデオでは、オーディエンスの作成と管理方法、配信用のオーディエンスの選択方法、コントロール母集団の定義方法について説明します。

>[!VIDEO](https://video.tv.adobe.com/v/3425861?quality=12&learn=on){transcript=true}

詳しくは、[&#x200B; オーディエンスの基本を学ぶ](../../v8/audience/manage-audience.md){target="_blank"}を参照してください。

Campaign Standard と同様に、配信にコントロール母集団を追加できます。コントロール母集団を定義して、オーディエンスの一部にメッセージを送信しないようにし、配信後の動作をメインターゲットと比較できます。このオプションは、キャンペーンの影響を測定するのに役立ちます。
[コントロール母集団の設定](../../v8/audience/control-group.md){target="_blank"}方法について説明します。

>[!AVAILABILITY]
>
>* Campaign Standard クエリアクティビティを使用して作成されたすべてのオーディエンスは、移行中に Campaign v8 で定義済みフィルターに変換されます。Campaign v8 は、クエリアクティビティもサポートしています。
>
>* 「オーディエンスを読み取り」では、[定義済みフィルター](../../v8/query/build-query.md)を使用してクエリアクティビティに変換されます。
>
>* 定義済みフィルターでは、オーディエンスを Campaign v8 に移行した後、最新の値のみを取得します。
>
>* Campaign Standard のファイルタイプのオーディエンスは、ディメンションのないリストタイプとして移行されます。

### 購読を管理 {#acs-gs-marketers-sub}

ニュースレターなどのサービスの管理と作成を行ったり、それらのサービスの購読または購読解除を確認したりできます。主な手順は、Campaign Standard とグローバルに同じです。詳しくは、以下のページを参照してください。

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

Adobe Campaign v8 では、マーケティングのプランとプログラムに関するフォルダー階層構造を設定できます。プラン、プログラム、キャンペーンの機能は、Campaign Standard および Campaign v8 と似ています。

詳しくは、[プランとプログラムのドキュメント](../../v8/administration/plans-programs.md)を参照してください。

開始するのに役立つリンクを以下に示します。ユーザーエクスペリエンスに影響を与える可能性のある変更は、可用性に関するメモでハイライト表示されます。


### キャンペーンの作成 {#acs-gs-marketers-campaign}

Adobe Campaign では、ビルトインのキャンペーン管理機能を使用して、ターゲットにするマーケティング活動を簡単に調整できます。スケジュールを定義する機能を使用すると、戦略目標に合わせてキャンペーンの期間とタイミングを計画し、オーディエンスのエンゲージメントを最大化できます。

![キャンペーンフロー](assets/campaign-flow.png)

キャンペーンについて詳しくは、次のドキュメントを参照してください。

1. [キャンペーンの基本を学ぶ](../../v8/campaigns/gs-campaigns.md)
1. [キャンペーンへのアクセスと管理](../../v8/campaigns/manage-campaigns.md)
1. [最初のキャンペーンを作成](../../v8/campaigns/create-campaigns.md)


### ワークフローの作成 {#acs-gs-marketers-wf}

Campaign web ユーザーインターフェイスでは、ワークフローユーザーインターフェイスが完全に再考され、使用、設定、実行、トラブルシューティングが容易になりました。Campaign Standard で既に経験したように、ワークフローを使用すると、あらゆるプロセスとタスクを調整し、セグメントの作成やメッセージの準備から配信に至るまでの、マーケティングキャンペーンのあらゆる側面でスピードと規模を改善できます。さらに、キャンペーンオーケストレーション用の使いやすい単一のインターフェイスでチャネルを同期させることができます。

このビデオでは、ワークフローの仕組みと、ターゲティングワークフローの作成方法について説明します。

>[!VIDEO](https://video.tv.adobe.com/v/3425873?quality=12&learn=on){transcript=true}

詳しくは、[ワークフローのドキュメント](../../v8/workflows/gs-workflows.md)を参照してください。

Adobe Campaign web ユーザーインターフェイスには、様々な基準に基づいてデータベースをフィルタリングするプロセスを簡素化するワークフローのクエリモデラーが備わっています。[詳しくは、クエリモデラーを参照してください](../../v8/query/query-modeler-overview.md)。

ワークフロー内の各アクティビティの目的と機能について詳しくは、[ワークフローアクティビティ](../../v8/workflows/activities/about-activities.md)に関する詳細情報を参照してください。

[ワークフローのガードレールと制限](../../v8/get-started/guardrails.md)を確認して、ワークフローの効率を最大化します。

>[!AVAILABILITY]
>
>* ワークフローの実行の[履歴とログ](../../v8/workflows/start-monitor-workflows.md#logs-tasks)は、Adobe Campaign v8 で使用できます。
>
>* Campaign Standard インスタンスで実行されたワークフローの履歴ログは、Campaign v8 に移行されません。
>
>* 組織単位は、マッピングと同様のアクセス制御を確保するフォルダーの概念にマッピングされます。
>

## 配信の作成と管理 {#acs-gs-marketers-deliveries}

Campaign web ユーザーインターフェースを使用すると、マーケターは、**配信**&#x200B;の左メニューからスタンドアロンの配信を作成したり、キャンペーンに含まれるかどうかに関係なく、ワークフローのコンテキストで配信を作成したりできます。主な手順は、Campaign Standard での以前のエクスペリエンスと一致しています。配信の作成方法について詳しくは、[配信の作成と管理に関するドキュメント](../../v8/msg/gs-deliveries.md)の節を参照してください。

役立つリンク：

* **配信テンプレート** - 設計プロセスを加速して改善するには、配信テンプレートを作成することで、キャンペーン全体でカスタムコンテンツと設定を簡単に再利用できます。この機能を使用すると、クリエイティブなルックアンドフィールを標準化して、キャンペーンの実行と開始をより迅速に行うことができます。詳しくは、[配信テンプレート](../../v8/msg/delivery-template.md)ページを参照してください。

* **配信設定** - 配信設定は、配信テンプレートで定義される技術的な配信パラメーターです。配信ごとに過負荷になる可能性があります。これらの設定は、配信または配信テンプレートの編集時に使用できる「設定」ボタンから利用できます。詳しくは、[配信設定](../../v8/advanced-settings/delivery-settings.md)の節を参照してください。

* **動的コンテンツ** - Adobe Campaign web 動的コンテンツ機能を使用すると、受信者について収集した情報に基づいてコンテンツをカスタマイズできます。動的コンテンツを利用することで、マーケティング活動の関連性が高まり、不要な製品やサービスのマーケティングを回避できます。詳しくは、[動的コンテンツ](../../v8/personalization/gs-personalization.md)の節を参照してください。

* **テストと配達確認** - 配信コンテンツを定義したら、メッセージを送信する前に、プロファイルとテストプロファイルを使用してプレビューとテストを行うことができます。この手順は、コンテンツが正確であると同時に、コンテンツとパーソナライゼーション設定の両方にエラーがないことを確認するのに重要です。詳しくは、[プレビューとテスト](../../v8/preview-test/preview-test.md)を参照してください。

* **スケジュール設定** - メッセージを送信する日付と正確な時刻を設定できます。マーケティングメッセージに最も適した時間を選択することで、開封率を最大化します。

   * 詳しくは、[スタンドアロン配信のスケジュール設定](../../v8/msg/gs-deliveries.md#gs-schedule)方法を参照してください。
   * 詳しくは、[ワークフローでの配信のスケジュール設定](../../v8/monitor/schedule-sending.md#schedule-a-delivery-in-a-campaign-workflow)方法を参照してください。

* **オファーを追加** - Adobe Campaign web ユーザーインターフェイスで、配信にオファーを追加できます。 これらのオファーは、オファーのリストにアクセスできる左側のオファーメニューから使用できます。詳しくは、[メッセージへのオファーの追加](../../v8/msg/offers.md)方法を参照してください。

>[!AVAILABILITY]
>
>* ドラフト状態または完了状態の配信は移行されました。
>
>* 転送中／処理中／キャンセル済み／再試行中／準備エラーのいずれかのステータスにある配信は Adobe Campaign v8 に移行されましたが、再度準備する必要があります。
>
>* キャンセル済み／再試行中のいずれかのステータスにある配信は、キャンセル済み配信として移行されました。
>
>* トラッキングリンク、ミラーページ URL リンク、購読／購読解除リンクは Campaign Standard と同様に機能します。
>
>Adobe Campaignの [&#x200B; トラッキングとモニタリング &#x200B;](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/analytics/tracking){target="_blank"}、[&#x200B; ブランディング &#x200B;](https://experienceleague.adobe.com/ja/docs/experience-cloud/campaign/branding/branding-gs){target="_blank"} の節も参照してください。

### メール配信 {#acs-gs-marketers-email}

このビデオでは、メール配信をゼロから作成、オーディエンスの定義、コンテンツの設計、プレビューのシミュレート、配達確認を送信する方法について説明します。

>[!VIDEO](https://video.tv.adobe.com/v/3425866?quality=12&learn=on){transcript=true}

最初のターゲットメールを作成する方法について詳しくは、[最初のメールの作成に関するドキュメント](../../v8/email/create-email.md)を参照してください。

Campaign v8 でのメール配信の作成、テスト、送信の詳細な手順は Campaign Standard と似ています。

1. **コンテンツの設計と定義**

   Campaign v8 の E メールデザイナーは、Campaign Standard で使用できるE メールデザイナーと似ています。備考：数年前、Campaign Standard[&#x200B; 従来のメールエディターは非推奨 &#x200B;](https://experienceleague.adobe.com/ja/docs/campaign-standard/using/release-notes/deprecated-features#deprecated-features){target="_blank"} なりました。 メールコンテンツを作成およびパーソナライズするには、既に Campaign E メールデザイナーに移行している必要があります。

   メールデザイナーの操作方法について説明します。次のビデオでは、メールをゼロから構築して設計する方法とメールをパーソナライズしてテストする方法ついて説明します。

   >[!VIDEO](https://video.tv.adobe.com/v/3425867?quality=12&learn=on){transcript=true}

   E メールデザイナーを使用すると、直感的なドラッグ＆ドロップインターフェイスを通じて、個別にカスタマイズされた魅力的なメールを作成できます。詳しくは、[E メールデザイナーのドキュメント](../../v8/email/get-started-email-designer.md)を参照してください。

   このビデオでは、HTML をアップロードしてメールを作成する方法、E メールデザイナーと互換性を持たせる方法、テンプレートに変換する方法について説明します。

   >[!VIDEO](https://video.tv.adobe.com/v/3427633?quality=12&learn=on){transcript=true}

   コンテンツフラグメントは、1 つ以上のメッセージで参照できる再利用可能なコンポーネントです。メール配信の作成の簡素化について詳しくは、[コンテンツフラグメント](../../v8/content/fragments.md)を参照してください。

   設計プロセスを加速し改善するのに、スタンドアロンのテンプレートを作成すると、Adobe Campaign 全体でカスタムコンテンツを簡単に再利用できます。詳しくは、[メールテンプレートの作成](../../v8/content/create-email-templates.md)を参照してください。

1. **プレビューとテスト**

   このビデオでは、メールメッセージのコンテンツとパーソナライゼーションをプレビューし、テスト配信（配達確認）を送信し、一般的なデスクトップ、モバイル、web ベースのクライアントでメールのレンダリングを確認する方法について説明します。

   >[!VIDEO](https://video.tv.adobe.com/v/3425862?quality=12&learn=on){transcript=true}

1. **メールの送信とログの確認**

   コンテンツ、オーディエンスおよびスケジュールを定義したら、メール配信の準備が整いました。詳しくは、次の節を参照してください。

   * [メールの準備と送信](../../v8/monitor/prepare-send.md)
   * [配信ログの監視](../../v8/monitor/delivery-logs.md)


### SMS 配信 {#acs-gs-marketers-sms}

SMS 配信は、顧客のモバイルデバイスにテキストメッセージを送信する実用的で効率的な方法を提供します。この機能を使用すると、テキストベースのメッセージを作成、パーソナライズ、プレビューして、効果的な通信を実現できます。

Campaign v8 では、SMS 配信の作成、テスト、送信の詳細な手順は Campaign Standard と似ています。


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

プッシュ通知は、モバイルアプリのユーザーが積極的にアプリを使用していない場合でも、そのユーザーへ通知するのに不可欠です。更新の提供、特定のアクションの促進、お得な情報の通知など、様々な目的に対応します。

Campaign v8 では、プッシュ通知配信の作成、テスト、送信の詳細な手順は Campaign Standard と似ています。


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
>* Adobe Campaign v8 では、Android と iOS の両方のプッシュチャネルをサポートしています。プッシュチャネルを使用した既存のワークフローと配信の移行について詳しくは、Adobe Campaign トランジションマネージャーにお問い合わせください。詳細情報 [&#x200B; チャネル設定 &#x200B;](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/send/push/push-data-collection){target="_blank"}。
>
>* なお、モバイルアプリケーション用のSDK V4 は、数年前に [Campaign Standardで非推奨 &#x200B;](https://experienceleague.adobe.com/ja/docs/campaign-standard/using/release-notes/deprecated-features#deprecated-features){target="_blank"} になっていました。 Campaign v8 で使用されているものと同じ Adobe Experience Platform SDK に既に移行している必要があります。
> 

### ダイレクトメール {#acs-gs-marketers-direct-mail}

ダイレクトメールは、はがき、チラシ、カタログなどのパーソナライズされたレターを顧客に大量に配信するファイルを作成できるオフラインチャネルです。ダイレクトメール配信を作成する際、Adobe Campaign では、すべてのターゲットプロファイルと選択したデータ（郵送先住所やプロファイル属性など）を含む抽出ファイルを自動的に生成します。

>[!VIDEO](https://video.tv.adobe.com/v/3433316/?learn=on)

Campaign v8 では、ダイレクトメール配信の作成、テスト、送信の詳細な手順は Campaign Standard と似ています。

1. [ダイレクトメール配信の作成](../../v8/direct-mail/create-direct-mail.md)
1. [抽出ファイルの定義](../../v8/direct-mail/content-direct-mail.md)
1. [プレビューと送信](../../v8/direct-mail/send-direct-mail.md)

>[!VIDEO](https://video.tv.adobe.com/v/3425867?quality=12&learn=on){transcript=true}

### アプリ内チャネル {#acs-gs-marketers-in-app}

アプリ内チャネルは、Campaign v8 では使用できません。アプリ内通知を送信する必要がある場合は、アドビ担当者にお問い合わせください。

## ランディングページの作成と管理 {#acs-gs-marketers-lp}

Adobe Campaign v8 web ユーザーインターフェイスには、ランディングページの再考されたユーザーエクスペリエンスが付属しています。Campaign では、ランディングページを作成、設計および共有できます。ランディングページでは、ユーザーをオンラインフォームに誘導して、データを更新したり、通信の受信をオプトイン／オプトアウトしたり、ニュースレターなどの特定のサービスを購読したりできます。

Campaign Standard ユーザーが Campaign v8 に移行する場合は、既存のランディングページが Campaign web ユーザーインターフェイスに移行されます。同じ範囲の機能にアクセスできます。

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

Adobe Campaignには、一連の [&#x200B; レポートツール &#x200B;](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/analytics/reports/gs-reporting){target="_blank"} が用意されています。 管理者は、レポートを作成および設定し、他の Campaign ユーザーと共有できます。

Adobe Campaign のレポートツールスイートは、マーケティング活動の有効性に関する貴重なインサイトを提供し、最大の効果を得るのにキャンペーンを最適化できます。詳しくは、[レポートのドキュメント](../../v8/reporting/gs-reports.md)を参照してください。

また、Adobe Campaign Standard エクスペリエンスに合わせて、メール配信用の動的レポートが Campaign v8 で使用できます。マーケティングアクティビティの影響を測定する完全にカスタマイズ可能なリアルタイムのレポートを提供します。プロファイルデータへのアクセスが追加され、開封数やクリック数などの機能的なメールキャンペーンデータに加えて、性別、市区町村、年齢などのプロファイルディメンション別のデモグラフィック分析が可能になります。詳しくは、[&#x200B; 動的レポートドキュメント &#x200B;](https://experienceleague.adobe.com/ja/docs/experience-cloud/campaign/reporting/get-started-reporting){target="_blank"} を参照してください

>[!AVAILABILITY]
>
>* [&#x200B; 動的レポート &#x200B;](https://experienceleague.adobe.com/ja/docs/experience-cloud/campaign/reporting/get-started-reporting){target="_blank"} は、メール配信のレポート、メール配信を含むキャンペーン、トランザクションメッセージに使用できます。 また、プロファイルディメンション別のデモグラフィック分析も使用できます。
>
> * また、[Adobe Campaign web ユーザーインターフェイスレポート](../../v8/reporting/campaign-reports.md)は、Adobe Campaign Standard から Adobe Campaign v8 に移行するすべてのユーザーが使用することもできます。

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
<p>個々の配信のパフォーマンス、有効性、結果に関する詳細情報が提供され、包括的な概要が得られます。</p>
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
<p>成功率、オーディエンスのエンゲージメント、その他の重要な指標など、各配信のチャネルごとのパフォーマンスを完全に分析します。キャンペーンの全体的な有効性と影響を評価できます。</p>
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
<p>Campaign インスタンス内の各チャネルについて、トラフィックとエンゲージメント指標を連結した全体的な概要を提供します。これらのレポートは様々なウィジェットで構成され、それぞれがキャンペーンや配信パフォーマンスに関する明確な観点を提供します。</p>
</div>
<p>
</td>
</tr>
</table>
