---
audience: end-user
title: WhatsApp メッセージの基本を学ぶ
description: Adobe Campaign Web ユーザーインターフェイスを使用してWhatsApp メッセージを作成および送信する方法について説明します
feature: Whatsapp
topic: Content Management
role: User
level: Beginner
hide: true
source-git-commit: f0c22710efcda2f59f75ea26cf239d549ff34f96
workflow-type: tm+mt
source-wordcount: '210'
ht-degree: 2%

---

# WhatsApp メッセージの基本を学ぶ {#get-started-whatsapp}

Metaの&#x200B;**Cloud API**&#x200B;を使用して、[Adobe Campaign Web ユーザーインターフェイス ](https://developers.facebook.com/docs/whatsapp/cloud-api/)からWhatsApp メッセージを送信できます。 スタンドアロン配信、キャンペーンワークフロー、マーケティングキャンペーン内などで、他のチャネルと並行してWhatsAppを使用します。

* **[!UICONTROL 配信]**: Adobe Campaign Web ユーザーインターフェイスで、左側のパネルの&#x200B;**[!UICONTROL 配信]** メニューから、SMSまたはプッシュ通知と同様に、スタンドアロン WhatsApp配信を作成します。 [詳細情報](create-whatsapp.md)。

* **[!UICONTROL キャンペーン]**: Adobe Campaign Web ユーザーインターフェイスでキャンペーンを開き、「**[!UICONTROL 配信]**」タブからWhatsApp配信を追加するか、キャンペーンにワークフローを添付して送信を調整します。 [詳細情報](../campaigns/create-campaigns.md)。

* **[!UICONTROL ワークフロー]**: Adobe Campaign Web ユーザーインターフェイスのワークフローキャンバスで、**[!UICONTROL WhatsApp]** チャネルアクティビティを追加し、配信テンプレートを選択してから、配信ダッシュボードでコンテンツと設定を定義します。 [このセクション ](../workflows/activities/channels.md)のチャネルアクティビティについて詳しく説明します。

## 前提条件 {#prereq}

WhatsAppを統合するには、次の操作が必要です。

* Meta Business Manager アカウント
* [送信者名と電話番号が確認されたWhatsApp ビジネス アカウント ](https://developers.facebook.com/docs/whatsapp/overview/business-accounts/)
* [適切な権限を持つユーザー認証トークン ](https://developers.facebook.com/blog/post/2022/12/05/auth-tokens/)
* [承認済みMeta テンプレート ](https://developers.facebook.com/docs/whatsapp/message-templates/guidelines/)

次の点を確認してから、作業を進める必要があります。

* [WhatsApp コンテンツルール ](https://www.whatsapp.com/legal/messaging-guidelines)
* [Meta ポリシーへの準拠](https://www.whatsapp.com/legal)
* [24時間の会話の制限](https://developers.facebook.com/docs/whatsapp/messaging-limits/)


