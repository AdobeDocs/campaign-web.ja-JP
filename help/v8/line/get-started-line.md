---
audience: end-user
title: LINE メッセージの基本を学ぶ
description: Adobe Campaign Web ユーザーインターフェイスを使用してLINE メッセージを作成および送信する方法について説明します
feature: Line App
topic: Content Management
role: User
level: Beginner
source-git-commit: 1c4cdd5164d0cf572e9b88881bbe240b06308866
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 22%
---
# LINE メッセージの基本を学ぶ {#get-started-line}

LINE は、無料のインスタントメッセージ、音声およびビデオ通話用のアプリケーションで、すべてのモバイルデバイスと PC で利用できます。 Adobe Campaign を使用して、LINE メッセージを送信できます。 スタンドアロン配信またはワークフローで、他のチャネルと並行してLINEを使用します。

![&#x200B; モバイルデバイスで受信したLINE メッセージの例](assets/line-message.png)

* **[!UICONTROL 配信]**: SMSまたはプッシュ通知と同様に、左側のパネルの&#x200B;**[!UICONTROL 配信]** メニューからスタンドアロンのLINE配信を作成します。 [詳細情報](send-line.md)。

* **[!UICONTROL ワークフロー]**: ワークフローキャンバスで、**[!UICONTROL LINE]** チャネルアクティビティを追加し、配信テンプレートを選択してから、配信ダッシュボードでコンテンツと設定を定義します。 チャネルアクティビティについて詳しくは、[このセクション](../workflows/activities/channels.md)を参照してください。

  >[!NOTE]
  >
  >**[!UICONTROL LINE]** チャネルアクティビティをフィードする&#x200B;**[!UICONTROL オーディエンスの作成]** アクティビティで、ターゲティングディメンションを&#x200B;**[!UICONTROL 訪問者サブスクリプション]**&#x200B;に変更します。 サイドパネルで「**[!UICONTROL すべてのスキーマを表示]**」を有効にしてください。 配信テンプレートセレクターは、このターゲティングディメンションが設定されている場合にのみ使用できます。
