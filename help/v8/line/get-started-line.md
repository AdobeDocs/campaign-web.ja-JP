---
audience: end-user
title: LINE メッセージの基本を学ぶ
description: Adobe Campaign Web ユーザーインターフェイスを使用してLINE メッセージを作成および送信する方法について説明します
feature: Line App
topic: Content Management
role: User
level: Beginner
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
feature_v2:
  - id: d5ef99fa-df0c-4153-bf94-105ad0724167
    internal-label: Integrations
subfeature_v2:
  - id: d9d413df-4e9e-4906-bbbc-28c06c2ccf59
    internal-label: LINE App
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
source-git-commit: 4fa6c49fb2456ef2edeb3f609b77c0cc5d33b95e
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
