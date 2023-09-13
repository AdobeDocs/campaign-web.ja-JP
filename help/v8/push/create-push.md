---
audience: end-user
title: プッシュ通知配信を作成
description: Adobe Campaign Web を使用してプッシュ通知配信を作成する方法を説明します
badge: label="Beta"
source-git-commit: e934bc041b76511c0f4fec22b6abc41c647e1cb3
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 97%

---

# プッシュ通知配信を作成 {#create-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_audience"
>title="プッシュオーディエンスの定義"
>abstract="プッシュメッセージに最適なオーディエンスを選択します。"

>[!CONTEXTUALHELP]
>id="acw_push_notification_template"
>title="プッシュ通知テンプレート"
>abstract="プッシュ通知テンプレートを選択して、プッシュ配信を開始します。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_properties"
>title="プッシュ配信プロパティ"
>abstract="プッシュ配信プロパティを管理します。"

1. **[!UICONTROL 配信]**&#x200B;ホームページで、「**[!UICONTROL 配信を作成]**」をクリックします。

1. 「**[!UICONTROL チャネル]**」セクションで、チャネルとして「プッシュ通知」を選択し、Android または iOS から選択したオペレーショナルシステムに応じてテンプレートを選択します。[テンプレートの詳細情報](../msg/delivery-template.md)

1. 「**[!UICONTROL 配信を作成]**」ボタンをクリックして、確定します。

   ![](assets/push_create_1.png)

1. 配信の&#x200B;**[!UICONTROL ラベル]**&#x200B;を入力し、**[!UICONTROL その他のオプション]**&#x200B;ドロップダウンにアクセスします。

   +++要件に基づいて次の設定を行います。
   * **[!UICONTROL 内部名]**：配信に一意の ID を割り当てます。
   * **[!UICONTROL フォルダー]**：配信を特定のフォルダーに保存します。
   * **[!UICONTROL 配信コード]**：独自の命名規則を使用して配信を整理します。
   * **[!UICONTROL 説明]**：配信の説明を指定します。
   * **[!UICONTROL 特性]**：分類目的でメールの特性を指定します。
+++

1. **[!UICONTROL オーディエンス]**&#x200B;メニューで、この配信に使用するアプリケーションを選択します。

1. 「**[!UICONTROL オーディエンスを選択]**」ボタンをクリックして、既存のオーディエンスをターゲットにするか、独自のユーザーを作成します。[詳細情報](../audience/about-audiences.md)

   デフォルトでは、プッシュ通知はアプリケーションのすべてのサブスクライバーに送信されます。

   ![](assets/push_create_2.png)

1. 「**[!UICONTROL コントロール母集団を有効にする]**」オプションをオンにして、配信の影響を測定するコントロール母集団を設定すると、メッセージを受信した母集団の行動と、受信しなかった連絡先の行動を比較できるようになります。[詳細情報](../audience/control-group.md)

1. 「**[!UICONTROL コンテンツを編集]**」をクリックして、プッシュ通知のコンテンツのデザインを開始します。[詳細情報](content-push.md)

   ![](assets/push_create_5.png)

   この画面から、[コンテンツをシミュレート](../preview-test/preview-test.md)したり、[オファーを設定](../content/offers.md)したりすることもできます。

1. 特定の日時に配信をスケジュールするには、「**[!UICONTROL スケジュールを有効にする]**」オプションをオンにします。配信を開始すると、メッセージは、その受信者に対して定義した、正確な日時に自動的に送信されます。配信スケジュールについて詳しくは、 [この節](../msg/gs-messages.md#gs-schedule)

   ![](assets/push_create_3.png)

1. 「**[!UICONTROL 配信設定を指定]**」をクリックして、配信テンプレートに関連する詳細オプションにアクセスします。[詳細情報](../advanced-settings/delivery-settings.md)

   ![](assets/push_create_4.png)
