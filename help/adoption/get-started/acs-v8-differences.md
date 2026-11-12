---
title: Campaign StandardとCampaign v8の違い
description: Campaign StandardからCampaign v8に移行する際の変更点と、詳細を確認する場所について説明します
hide: true
robots: noindex
googlebot: noindex
role: User, Admin, Developer
level: Beginner
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
source-git-commit: 25814ce1c70a139c9727b3bfccccd3efe056b441
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 2%
---
# Campaign StandardとCampaign v8の違い {#acs-v8-differences}

ほとんどのコンセプトは、Campaign StandardとCampaign v8で同じです。 このページでは、移行後に影響を与える違いを収集し、それぞれの違いを説明するページにリンクします。 [&#x200B; マーケター](marketers.md)および[管理者と開発者](admin-developers.md)のガイドを補完します。

* 用語の変更については、[Campaign StandardとCampaign v8](overview.md#experiences)の主な違いを参照してください。
* 移行を実行するためのチェックと、移行後に報告された問題については、[移行後のチェックとトラブルシューティング &#x200B;](post-transition-checks.md)を参照してください。
* クライアントコンソールでのみ使用できる機能については、[Campaign WebおよびCampaign クライアントコンソール &#x200B;](../../v8/get-started/capability-matrix.md)を参照してください。

## チャネルとコンテンツ {#channels}

メッセージの作成と送信の手順は、両方の製品で似ています。詳しくは、[&#x200B; マーケター向けガイド &#x200B;](marketers.md)を参照してください。 以下の違いは、チャネルの可用性、テスト配信、ランディングページ、ダイレクトメールワークフローに関するものです。

| 変更点 | 詳細情報 |
|---|---|
| アプリ内チャネルは、Campaign v8では使用できません。 | [&#x200B; アプリ内チャネル &#x200B;](marketers.md#acs-gs-marketers-in-app) |
| 既存のプッシュワークフローと配信を移行するには、Adobe Campaign Transition Managerにお問い合わせください。 | [プッシュ通知](marketers.md#acs-gs-marketers-push) |
| Campaign Standardでは、テストプロファイルを&#x200B;**トラップ**&#x200B;としてマークして、最終送信を受け取ることができます。 Campaign v8で、配信のオーディエンス設定に&#x200B;**トラップグループ**&#x200B;を追加します。 | [&#x200B; トラップグループ &#x200B;](../../v8/audience/trap-group.md) |
| Campaign Web ユーザーインターフェイスで作成されたランディングページは、非表示の入力フィールドやカスタム JavaScriptをサポートしていません。 | [ランディングページ](../../v8/landing-pages/get-started-lp.md) |
| Campaign Standardでは、ダイレクトメールアクティビティのアウトバウンドトランジションにも、生成されたファイルが含まれています。 Campaign v8では、ターゲット母集団のみが取り込まれます。 ファイルをサーバーに送信するには、**データ抽出** アクティビティを追加してから、**ファイル転送** アクティビティを追加します。 | [&#x200B; ダイレクトメール &#x200B;](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/direct-mail){target="_blank"} |

## オーディエンス、ワークフロー、配信 {#data-and-workflows}

これらの違いは、Campaign Standardから移行されたオーディエンスとワークフロー、定期的な配信と&#x200B;**ファイル転送** アクティビティのオプション、動的レポートの範囲に影響します。

| 変更点 | 詳細情報 |
|---|---|
| オーディエンスは移行中に変換されます。 例えば、「クエリ」アクティビティで作成されたオーディエンスは定義済みのフィルターになり、ファイルタイプのオーディエンスはディメンションのないリストタイプのオーディエンスになります。 | [&#x200B; オーディエンスの管理](marketers.md#acs-gs-marketers-audiences) |
| Campaign Standardで実行されたワークフローの履歴ログは移行されません。 | [ワークフローの作成](marketers.md#acs-gs-marketers-wf) |
| Campaign Standardでは、定期的なメールの集計期間を選択できます。 このオプションは、Campaign v8では使用できません。 | [&#x200B; チャネルアクティビティ &#x200B;](../../v8/workflows/activities/channels.md) |
| 動的レポートでは、メール配信、メール配信を伴うキャンペーン、トランザクションメッセージを取り上げます。 | [レポート](marketers.md#acs-gs-marketers-reporting) |

## アクセスとセキュリティ {#access}

Campaign Standardのセキュリティグループ、ロール、組織単位は、移行時にオペレーターグループ、名前付き権限、フォルダー権限にマッピングされます。 特に、一部のユーザーが以前よりも広範または狭い権限を持っている場合は、以下の点を確認してください。

| 変更点 | 詳細情報 |
|---|---|
| セキュリティグループ、役割、組織単位は、オペレーターグループ、名前付き権限、フォルダー権限にマッピングされます。 カスタムの役割は移行されません。 | [&#x200B; ユーザーアクセス管理](user-management-acs.md) |
| **データモデル**&#x200B;の役割を持ち、**管理**&#x200B;の役割を持たないユーザーは、**管理**&#x200B;へのアクセス権を取得します。 | [&#x200B; ユーザーアクセス管理](user-management-acs.md#migration-approach-from-user-roles-to-named-rights) |
| 並列の組織単位を持つセキュリティ グループに割り当てられたユーザーは、Campaign v8でより広範なアクセス権を持つことができます。 | [組織ユニットの並列割り当て](user-management-acs.md#parallel-assignments) |
| 実行インスタンスからトランザクション APIにアクセスするには、新しい製品プロファイルが必要です。 | [製品プロファイルマッピング &#x200B;](user-management-acs.md#product-profile-mapping-to-access-rest-apis) |
| プライバシーリクエストは、Campaign Standard環境がアクティブな状態を維持している間に、Campaign StandardとCampaign v8の両方に送信されます。 | [プライバシーと同意](admin-developers.md#privacy-and-consent) |

## 管理、トラッキング、ミラーページ {#admin-tracking}

これらの違いは、移行前にCampaign Standardから送信される配信と、Campaign v8に引き継がれない管理情報に影響します。

| 変更点 | 詳細情報 |
|---|---|
| 移行前にCampaign Standardから送信された配信のミラーページは使用できません。 Campaign v8から送信された配信のミラーページは、通常どおり機能します。 | [&#x200B; ミラーページ &#x200B;](../../v8/email/mirror-page.md) |
| 移行前にCampaign Standardから送信されたリアルタイムのトランザクション配信のトラッキングデータがCampaign v8でキャプチャされない。 これらのメッセージのリンクは引き続きリダイレクトされます。 | [&#x200B; トランザクションメッセージの監視](../../v8/transactional-messaging/monitor-transactional.md) |
| 地理的単位は使用できません。 地理的単位に基づくアクセス制御が失われます。 | [&#x200B; アクセス制御](../../v8/get-started/connect-to-campaign.md#access-control) |

## APIと統合 {#apis-and-integrations}

これらの違いは、そのREST APIを介してCampaignを呼び出す統合機能、および他のAdobe ソリューションやツールとの統合機能に影響します。

| 変更点 | 詳細情報 |
|---|---|
| PKEY値は、移行後に変更されます。 Campaign以外でPKEYを保存する場合は、代わりにAPIから返されるhrefsに従います。 | [REST API](admin-developers.md#acs-gs-admin-apis) |
| タイムゾーンや`ccpaOptOut`などの一部の移行されたプロファイルフィールドは、`profileAndServicesExt/profile` APIによってのみ返されます。 | [REST API](admin-developers.md#acs-gs-admin-apis) |
| Campaign StandardのDreamweaverとAdobe Experience Platform Data Connectorの統合は、Campaign v8では使用できません。 | [Campaignおよびその他のAdobe ソリューションとの連携](../../v8/integrations/integration.md) |
| Adobeは、Adobe AnalyticsとAudience Managerの設定を移行します。 トリガーとAdobe Targetの統合を再度設定する必要があります。 | [Adobe Campaign統合の管理](admin-developers.md#acs-gs-integrations) |
