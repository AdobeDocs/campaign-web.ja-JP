---
audience: end-user
title: WhatsApp 配信の作成
description: Adobe Campaign web ユーザーインターフェイスで WhatsApp 配信を作成する方法について説明します。
feature: Whatsapp
topic: Content Management
role: User
level: Beginner
exl-id: cac6f675-59e0-431d-8c20-f24ef16d7bf2
hide: true
source-git-commit: aa1a7c48d1708e73e4d6c6bbe4decd2e5ca69102
workflow-type: ht
source-wordcount: '472'
ht-degree: 100%

---


# WhatsApp 配信の作成 {#create-whatsapp}

**Adobe Campaign Web ユーザーインターフェイス**&#x200B;を使用すると、Meta で承認されたテンプレートで WhatsApp メッセージをデザインし、各プロファイルに合わせてパーソナライズして、送信前にテストすることができます。


+++ サポートされているメッセージ要素と CTA の詳細

WhatsAppでは、次のメッセージタイプがサポートされています。

| メッセージ機能 | 説明 |
|-|-|
| ヘッダー | メッセージの本文の上に表示されるオプションのテキスト。 |
| テキスト | パラメーターによる動的コンテンツのサポート。 |
| ヘッダー画像 | メッセージの本文の上に表示されるオプションの画像。 |
| 本文 | パラメーターによる動的コンテンツのサポート。 |
| フッターテキスト | パラメーターによる動的コンテンツのサポート。 |

+++


## WhatsApp 配信の作成 {#create-whatsapp-journey-campaign}

>[!IMPORTANT]
>
>WhatsApp メッセージのフィードバックは現在サポートされていません。

Adobe Campaign Web ユーザーインターフェイスで、次の手順に従ってスタンドアロン WhatsApp 配信を作成します。

1. **[!UICONTROL 配信]**&#x200B;メニューを参照し、「**[!UICONTROL 配信を作成]**」をクリックします。

   ![](assets/whatsapp-create-1.png)

1. 「**[!UICONTROL WhatsApp]**」を選択し、配信テンプレートを選択します。[テンプレートの詳細情報はこちら](../msg/delivery-template.md)。

   ![](assets/whatsapp-create-2.png)

1. 「**[!UICONTROL 配信を作成]**」をクリックし、確定します。

1. 「**[!UICONTROL 設定]**」をクリックして、配信テンプレートに関連する詳細オプションにアクセスします。[詳細情報](../advanced-settings/delivery-settings.md)

   ![](assets/whatsapp-create-3.png)

1. 配信の&#x200B;**[!UICONTROL ラベル]**&#x200B;を入力します。内部の名前、フォルダー、配信コード、説明、または性質、または他のチャネルと同じパターンが必要な場合は、「**[!UICONTROL その他のオプション]**」を使用します。

1. 「**[!UICONTROL オーディエンスを選択]**」をクリックして、既存のオーディエンスをターゲットにするか、独自のオーディエンスを作成します。[詳しくは、オーディエンスを参照してください](../audience/about-recipients.md)。

1. 「**[!UICONTROL コンテンツを編集]**」をクリックして WhatsApp コンテンツエディターを開きます。[WhatsApp コンテンツの定義](#whatsapp-content)を参照してください。

   ![](assets/whatsapp-create-4.png)

1. 「**[!UICONTROL スケジュールを有効にする]**」をオンにすると、特定の日時に送信できます。[詳細情報](../msg/gs-deliveries.md#gs-schedule)


## WhatsApp コンテンツの定義{#whatsapp-content}

>[!BEGINSHADEBOX]

Adobe Campaign Web ユーザーインターフェイスで WhatsApp メッセージをデザインする前に、Meta でテンプレートを作成して送信します。[詳細情報](https://www.facebook.com/business/help/2055875911147364?id=2129163877102343)

WhatsApp テンプレートは、使用前に Meta による承認を受ける必要があります。承認には通常数時間かかりますが、最大 24 時間かかる場合もあります。[詳細情報](https://developers.facebook.com/docs/whatsapp/message-templates/guidelines/#approval-process)

>[!ENDSHADEBOX]

1. Adobe Campaign Web ユーザーインターフェイスの配信設定ページで「**[!UICONTROL コンテンツを編集]**」をクリックして、WhatsApp メッセージを設定します。

1. マーケティングを&#x200B;**テンプレートカテゴリ**&#x200B;として選択します。

   [テンプレートカテゴリについて詳しく見る](https://developers.facebook.com/docs/whatsapp/updates-to-pricing/new-template-guidelines/#template-category-guidelines)

   ![](assets/whatsapp-design-1.png)

1. **WhatsApp テンプレート**&#x200B;ドロップダウンから、Meta 承認済みテンプレートを選択します。

   [WhatsApp テンプレートの作成方法について詳しく見る](https://www.facebook.com/business/help/2055875911147364?id=2129163877102343)

   ![](assets/whatsapp-design-2.png)

1. Meta 承認済みテンプレートに画像が含まれる場合は、**[!UICONTROL 画像 URL]** を指定します。

   ![](assets/whatsapp-design-3.png)

1. 「**パーソナライゼーションプレースホルダー**」フィールドで、パーソナライゼーションエディターを使用して、プロファイルフィールドと式をテンプレートパラメーターにマッピングします。[詳細情報](../personalization/personalize.md)

   ![](assets/whatsapp-design-4.png)

メッセージの準備が整った場合：

* **スタンドアロン配信またはキャンペーン配信**：配信ダッシュボードの「**[!UICONTROL 確認して送信]**」と「**[!UICONTROL 送信]**」を使用します。

* **ワークフロー**：実行により配信が使用可能になった際に、ワークフローアクティビティから配信を開き、同じ方法で配信ダッシュボードを使用します。[詳細情報](../workflows/start-monitor-workflows.md)

次に、配信&#x200B;**[!UICONTROL レポート]**&#x200B;のエントリポイントと[配信レポー](../reporting/delivery-reports.md)トから結果を追跡できます。
