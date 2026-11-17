---
title: Campaign v8への移行後のチェックとトラブルシューティング
description: Campaign StandardからCampaign v8に移行した後に確認する方法と、一般的な問題を修正する方法について説明します
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
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
source-git-commit: 8b78a8494223fbcd3def29c955e6171cbb643fef
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 2%
---
# 移行後のチェックとトラブルシューティング {#post-transition-checks}

Campaign StandardからCampaign v8に移行すると、一部の配信、ワークフロー、ランディングページが、想定とは異なる動作を示す場合があります。 次の表に、遷移したユーザーによって報告された症状と、その原因と対処方法を示します。 相違点の一覧については、「[Campaign StandardとCampaign v8](acs-v8-differences.md)の相違点」を参照してください。

| 症状 | 原因と実行すべきアクション | 詳細情報 |
|---|---|---|
| 配信内のリンクは直接URLで、クリックデータは収集されません。 | トラッキングは、配信またはそのベースとなる配信テンプレートでは無効になっています。 特に定期的な配信のテンプレートで&#x200B;**Activate tracking**&#x200B;が有効になっていることを確認してください。 | [設定のトラッキング &#x200B;](../../v8/advanced-settings/delivery-settings.md#tracking-tab) |
| 「mailto」のList-Unsubscribe メソッドを通じて購読を解除した受信者は強制隔離されていません。 | 今期待されているものです。 これらの受信者は強制隔離には送信されません。 配信に関連付けられているサービスの購読を解除するか、配信にサービスがない場合は配信ブロックリストに追加されます。 これらの購読解除を追跡するには、サービスの購読またはプロファイルの「**もう連絡できません**」セクションを確認します。 | [強制隔離](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/send/failures/quarantines){target="_blank"} |
| ランディングページは、スクリプトによって計算された値や、非表示のフィールドに格納された値を保存しません。 | Campaign Web ユーザーインターフェイスで作成されたランディングページは、非表示の入力フィールドやカスタム JavaScriptをサポートしていません。 代わりに、クライアントコンソールでweb アプリケーションとしてフォームを作成します。 | [ランディングページ](../../v8/landing-pages/get-started-lp.md) |
| **ファイル転送**&#x200B;は、ダイレクトメールアクティビティによって生成されたファイルを見つけません。 | ダイレクトメールアクティビティのアウトバウンドトランジションでは、抽出ファイルではなく、ターゲット母集団が取り込まれます。 **データ抽出** アクティビティを追加してから、**ファイル転送** アクティビティを追加します。 | [&#x200B; ダイレクトメール &#x200B;](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/send/direct-mail){target="_blank"} |
| 配信の複数の波が一緒に送信されます。 | ウェーブは、配信の連絡日からスケジュールされます。 一部のウェーブの予定時刻の後に配信が開始された場合、それらのウェーブは間隔を空けずに一緒に送信されます。 | [&#x200B; ウェーブを使用して送信](../../v8/advanced-settings/send-using-waves.md) |
| アスタリスクの後に文字が付いたファイルマスクは、Azure Blob Storageにファイルを見つけません。 | Azure Blob Storageは、ファイルを名前のプレフィックスでフィルタリングします。 末尾のアスタリスクのみがサポートされます。 | [外部アカウントの転送](../../v8/administration/transfer-external-account.md) |
| カスタム JavaScriptを使用するランディングページやコンテンツブロックは、動作が異なります。 | カスタム JavaScriptは、移行中に変換されますが、特に`queryDef`、Campaign JavaScript API、セッション書き込み、組織単位の処理、カスタム URL生成を使用している場合は、検証および調整します。 | [ランディングページ](../../v8/landing-pages/get-started-lp.md) |
| REST API呼び出しは、空の値、エラー、または予期しない応答を返します。 | 一部のデータベースフィールドは移行中に削除され、空白の値が返されます。 空のPATCHは204を返し、場所のPATCHは500を返します。 リンクされたリソースを含むPOSTは、リンクを無視するか、エラーを返します。 無効なPKEYは404を返します。 | [REST APIの制限](acs-v8-differences.md#rest-api-limitations) |
| 保存されたPKEYは、API呼び出しでは機能しなくなりました。 | PKEY値は、移行後に変更されます。 Campaign以外では保存しないでください。 前の呼び出しによって返されたhrefsから各呼び出しを作成します。 | [&#x200B; キーの使用状況](acs-v8-differences.md#key-usage) |
| プロファイル応答にタイムゾーンまたは`ccpaOptOut`がありません。 | これらのフィールドは、`profileAndServices/profile`ではなく、`profileAndServicesExt/profile`によってのみ返されます。 拡張エンドポイントを呼び出します。 | [&#x200B; プロファイルタイムゾーンとccpaOptOut](acs-v8-differences.md#profile-timezone) |
| カスタムフィルターは、REST API呼び出しでエラーを返します。 | Campaign v8では、フィルターに「**Filter name in REST API**」フィールドに名前を付け、「by」プレフィックスなしで、この名前をリクエスト内で使用します。 | [&#x200B; フィルタリング &#x200B;](acs-v8-differences.md#rest-filtering) |
| ワークフロー外部信号をトリガーする呼び出しは、そのリクエスト本文を構築できません。 | ワークフローGET APIがワークフロー変数を返さなくなりました。 ワークフローに関する自分の知識から、POST リクエスト本文のパラメーターを作成します。 | [&#x200B; ワークフローの外部シグナル &#x200B;](acs-v8-differences.md#workflow-signals) |
| トランザクション APIへのアクセスは拒否されます。 | 実行インスタンスからトランザクション APIにアクセスするには、新しい製品プロファイルが必要です。 テクニカルアカウントの製品プロファイルマッピングを確認します。 | [製品プロファイルマッピング &#x200B;](user-management-acs.md#product-profile-mapping-to-access-rest-apis) |
| 移行されたオーディエンスには最新の値のみが表示されるか、ファイルオーディエンスにはディメンションがありません。 | 今期待されているものです。 事前定義されたフィルターは、オーディエンスの移行後に最新の値のみを取り込み、ファイルタイプのオーディエンスはディメンションを持たないリストタイプのオーディエンスになります。 | [&#x200B; オーディエンスの管理](marketers.md#acs-gs-marketers-audiences) |
| Campaign Standardで実行されたワークフローの履歴が空です。 | Campaign Standardで実行されたワークフローの履歴ログは移行されません。 Campaign v8で実行されるワークフローには、独自の履歴とログがあります。 | [ワークフローの作成](marketers.md#acs-gs-marketers-wf) |
| 一部のユーザーは、以前よりも多くの表示や操作を行うことができます。 | **データモデル**&#x200B;の役割を持つが&#x200B;**管理**&#x200B;の役割を持たないユーザーは&#x200B;**管理** アクセスを得ることができ、並行する組織単位を持つセキュリティグループは、より広範なアクセス権を持つことができます。 オペレーターグループ、名前付き権限、フォルダー権限を確認します。 | [&#x200B; ユーザーアクセス管理](user-management-acs.md) |
| 「**トラップ**」としてマークされたテストプロファイルは、最終的な送信を受け取りません。 | Campaign v8で、配信のオーディエンス設定に&#x200B;**トラップグループ**&#x200B;を追加します。 | [&#x200B; トラップグループ &#x200B;](../../v8/audience/trap-group.md) |
| 定期的なメールには集計期間のオプションがありません。 | このオプションは、Campaign v8では使用できません。 | [&#x200B; チャネルアクティビティ &#x200B;](../../v8/workflows/activities/channels.md) |
| 動的レポートでは、配信のデータは表示されません。 | 動的レポートでは、メール配信、メール配信を伴うキャンペーン、トランザクションメッセージを取り上げます。 | [レポート](marketers.md#acs-gs-marketers-reporting) |
