---
audience: end-user
title: プッシュ通知配信の作成
description: Adobe Campaign Web を使用してプッシュ通知配信を作成する方法を説明します
badge: label="Alpha" type="Positive"
source-git-commit: 0463bc48bcee20b9f97d5b98053b77956dc4ef53
workflow-type: tm+mt
source-wordcount: '317'
ht-degree: 68%

---

# プッシュ通知配信の作成 {#create-push}

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

1. 以下 **[!UICONTROL チャネル]** 「 」セクションで、チャネルとして「プッシュ通知」を選択し、選択したオペレーショナルシステムに応じてテンプレートを選択します。Android またはiOS。 [テンプレートの詳細情報](../msg/delivery-template.md)

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

1. 次の **[!UICONTROL 対象ユーザ]** メニューで、この配信に使用するアプリケーションを選択します。

1. 「**[!UICONTROL オーディエンスを選択]**」ボタンをクリックして、既存のオーディエンスをターゲットにするか、独自のユーザーを作成します。[詳細情報](../audience/about-audiences.md)

   デフォルトでは、プッシュ通知はアプリケーションのすべての購読者に送信されます。

   ![](assets/push_create_2.png)

1. 「**[!UICONTROL コントロール母集団を有効にする]**」オプションをオンにして、配信の影響を測定するコントロール母集団を設定すると、メッセージを受信した母集団の行動と、受信しなかった連絡先の行動を比較できるようになります。[詳細情報](../audience/control-group.md)

1. クリック **[!UICONTROL コンテンツを編集]** プッシュ通知のコンテンツのデザインを開始します。

1. 特定の日時に配信をスケジュールするには、「**[!UICONTROL スケジュールを有効にする]**」オプションをオンにします。配信を開始すると、メッセージは、その受信者に対して定義した、正確な日時に自動的に送信されます。

1. クリック **[!UICONTROL 配信設定の指定]** をクリックして、配信テンプレートに関連する詳細オプションにアクセスします。 [詳細情報](../advanced-settings/delivery-settings.md)

   ![](assets/push_create_3.png)
