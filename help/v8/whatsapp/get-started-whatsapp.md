---
audience: end-user
title: WhatsApp メッセージの基本を学ぶ
description: Adobe Campaign Web ユーザーインターフェイスでの WhatsApp メッセージの作成方法や送信方法を学ぶ
feature: Whatsapp
topic: Content Management
role: User
level: Beginner
hide: true
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
source-git-commit: 4fa6c49fb2456ef2edeb3f609b77c0cc5d33b95e
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 100%
---
# WhatsApp メッセージの基本を学ぶ {#get-started-whatsapp}

Meta の [Cloud API](https://developers.facebook.com/docs/whatsapp/cloud-api/) を使用して、**Adobe Campaign Web ユーザーインターフェイス**&#x200B;から WhatsApp メッセージを送信できます。 スタンドアロン配信、キャンペーンワークフロー、マーケティングキャンペーン内などで、他のチャネルと並行して WhatsApp を使用します。

* **[!UICONTROL 配信]**：Adobe Campaign Web ユーザーインターフェイスで、左側のパネルの&#x200B;**[!UICONTROL 配信]**&#x200B;メニューから、SMS やプッシュ通知と同様に、スタンドアロン WhatsApp 配信を作成します。 [詳細情報](create-whatsapp.md)

* **[!UICONTROL キャンペーン]**：Adobe Campaign Web ユーザーインターフェイスでキャンペーンを開き、「**[!UICONTROL 配信]**」タブから WhatsApp 配信を追加するか、キャンペーンにワークフローを添付して送信を調整します。 [詳細情報](../campaigns/create-campaigns.md)

* **[!UICONTROL ワークフロー]**：Adobe Campaign Web ユーザーインターフェイスのワークフローキャンバスで、**[!UICONTROL WhatsApp]** チャネルアクティビティを追加し、配信テンプレートを選択してから、配信ダッシュボードでコンテンツと設定を定義します。 チャネルアクティビティについて詳しくは、[このセクション](../workflows/activities/channels.md)を参照してください。

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


