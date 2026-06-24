---
audience: end-user
title: WhatsApp メッセージの基本を学ぶ
description: Adobe Campaign Web ユーザーインターフェイスでの WhatsApp メッセージの作成方法や送信方法を学ぶ
feature: Whatsapp
topic: Content Management
role: User
level: Beginner
hide: true
source-git-commit: f0c22710efcda2f59f75ea26cf239d549ff34f96
workflow-type: ht
source-wordcount: '248'
ht-degree: 100%

---

# WhatsApp メッセージの基本を学ぶ {#get-started-whatsapp}

Meta の [Cloud API](https://developers.facebook.com/docs/whatsapp/cloud-api/) を使用して、**Adobe Campaign Web ユーザーインターフェイス**&#x200B;から WhatsApp メッセージを送信できます。スタンドアロン配信、キャンペーンワークフロー、マーケティングキャンペーン内などで、他のチャネルと並行して WhatsApp を使用します。

* **[!UICONTROL 配信]**：Adobe Campaign Web ユーザーインターフェイスで、左側のパネルの&#x200B;**[!UICONTROL 配信]**&#x200B;メニューから、SMS やプッシュ通知と同様に、スタンドアロン WhatsApp 配信を作成します。[詳細情報](create-whatsapp.md)

* **[!UICONTROL キャンペーン]**：Adobe Campaign Web ユーザーインターフェイスでキャンペーンを開き、「**[!UICONTROL 配信]**」タブから WhatsApp 配信を追加するか、キャンペーンにワークフローを添付して送信を調整します。[詳細情報](../campaigns/create-campaigns.md)

* **[!UICONTROL ワークフロー]**：Adobe Campaign Web ユーザーインターフェイスのワークフローキャンバスで、**[!UICONTROL WhatsApp]** チャネルアクティビティを追加し、配信テンプレートを選択してから、配信ダッシュボードでコンテンツと設定を定義します。チャネルアクティビティについて詳しくは、[このセクション](../workflows/activities/channels.md)を参照してください。

## 前提条件 {#prereq}

WhatsApp を統合するには、次が必要です。

* Meta Business Manager アカウント
* [送信者名と電話番号が確認済みの WhatsApp ビジネスアカウント](https://developers.facebook.com/docs/whatsapp/overview/business-accounts/)
* [適切な権限を持つユーザー認証トークン](https://developers.facebook.com/blog/post/2022/12/05/auth-tokens/)
* [承認済み Meta テンプレート](https://developers.facebook.com/docs/whatsapp/message-templates/guidelines/)

また、続行するには、次の点を確認する必要があります。

* [WhatsApp コンテンツルール](https://www.whatsapp.com/legal/messaging-guidelines)
* [Meta ポリシーの準拠](https://www.whatsapp.com/legal)
* [24 時間の会話の上限](https://developers.facebook.com/docs/whatsapp/messaging-limits/)


