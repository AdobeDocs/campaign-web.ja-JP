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
source-git-commit: 071900a6c0b717161ae123097aeae8bf9e97898c
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 3%
---
# 移行後のチェックとトラブルシューティング {#post-transition-checks}

Campaign StandardからCampaign v8に移行すると、一部の配信、ワークフロー、ランディングページが、想定とは異なる動作を示す場合があります。 次の表に、遷移したユーザーによって報告された症状と、その原因と対処方法を示します。 相違点の一覧については、「[Campaign StandardとCampaign v8](acs-v8-differences.md)の相違点」を参照してください。

| 症状 | 原因と実行すべきアクション | 詳細情報 |
|---|---|---|
| 配信内のリンクは直接URLで、クリックデータは収集されません。 | トラッキングは、配信またはそのベースとなる配信テンプレートでは無効になっています。 特に定期的な配信のテンプレートで&#x200B;**Activate tracking**&#x200B;が有効になっていることを確認してください。 | [設定のトラッキング &#x200B;](../../v8/advanced-settings/delivery-settings.md#tracking-tab) |
| 「mailto」のList-Unsubscribe メソッドを通じて購読を解除した受信者は強制隔離されていません。 | 今期待されているものです。 これらの受信者は強制隔離には送信されません。 配信に関連付けられているサービスの購読を解除するか、配信にサービスがない場合は配信ブロックリストに追加されます。 これらの購読解除を追跡するには、サービスの購読またはプロファイルの「**もう連絡できません**」セクションを確認します。 | [強制隔離](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/send/failures/quarantines){target="_blank"} |
| ランディングページは、スクリプトによって計算された値や、非表示のフィールドに格納された値を保存しません。 | Campaign Web ユーザーインターフェイスで作成されたランディングページは、非表示の入力フィールドやカスタム JavaScriptをサポートしていません。 代わりに、クライアントコンソールでweb アプリケーションとしてフォームを作成します。 | [ランディングページ](../../v8/landing-pages/get-started-lp.md) |
| **ファイル転送**&#x200B;は、ダイレクトメールアクティビティによって生成されたファイルを見つけません。 | ダイレクトメールアクティビティのアウトバウンドトランジションでは、抽出ファイルではなく、ターゲット母集団が取り込まれます。 **データ抽出** アクティビティを追加してから、**ファイル転送** アクティビティを追加します。 | [&#x200B; ダイレクトメール &#x200B;](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/direct-mail){target="_blank"} |
| 配信の複数の波が一緒に送信されます。 | ウェーブは、配信の連絡日からスケジュールされます。 一部のウェーブの予定時刻の後に配信が開始された場合、それらのウェーブは間隔を空けずに一緒に送信されます。 | [&#x200B; ウェーブを使用して送信](../../v8/advanced-settings/send-using-waves.md) |
| アスタリスクの後に文字が付いたファイルマスクは、Azure Blob Storageにファイルを見つけません。 | Azure Blob Storageは、ファイルを名前のプレフィックスでフィルタリングします。 末尾のアスタリスクのみがサポートされます。 | [外部アカウントの転送](../../v8/administration/transfer-external-account.md) |
| カスタム JavaScriptを使用するランディングページやコンテンツブロックは、動作が異なります。 | カスタム JavaScriptは、移行中に変換されますが、特に`queryDef`、Campaign JavaScript API、セッション書き込み、組織単位の処理、カスタム URL生成を使用している場合は、検証および調整します。 | [ランディングページ](../../v8/landing-pages/get-started-lp.md) |
