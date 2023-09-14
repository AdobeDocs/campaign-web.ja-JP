---
audience: end-user
title: SMS 配信を作成
description: Adobe Campaign Web で SMS を作成して送信する方法を学ぶ
badge: label="Beta"
exl-id: 89c9da76-1e04-41cd-9636-0d3b957875b6
source-git-commit: a67a692cf9b74015323954eca5b4c554f7fe8eb6
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 82%

---

# SMS 配信を作成 {#create-sms}

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_properties"
>title="SMS 配信プロパティ"
>abstract="プロパティには、配信の名前付けと分類の両方に役立つ一般的な配信パラメーターが含まれています。配信が拡張スキーマに基づいている場合は、特定のカスタムオプションフィールドを使用できます。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_audience"
>title="SMS オーディエンスの定義"
>abstract="SMS メッセージに最適なオーディエンスを選択します。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_template_selection"
>title="SMS テンプレートの選択"
>abstract="事前定義済みのテンプレートを選択して SMS 配信を開始します。"

スタンドアロンの SMS 配信を作成することも、キャンペーンワークフローのコンテキストで SMS を作成することもできます。 以下の手順では、スタンドアロン（ワンショット）の SMS 配信の手順について説明します。 キャンペーンワークフローのコンテキストで作業している場合、作成手順の詳細は [この節](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).


スタンドアロンの新しい SMS 配信を作成するには、次の手順に従います。

1. 左側のナビゲーションの&#x200B;**[!UICONTROL 配信]**&#x200B;メニューを参照し、「**[!UICONTROL 配信を作成]**」ボタンをクリックします。

1. 「**[!UICONTROL チャネル]**」セクションで、チャネルとして SMS を選択し、テンプレートを選択します。[テンプレートの詳細情報](../msg/delivery-template.md)

1. 「**[!UICONTROL 配信を作成]**」ボタンをクリックして、確定します。

   ![](assets/sms_create_1.png)

1. 配信の&#x200B;**[!UICONTROL ラベル]**&#x200B;を入力し、**[!UICONTROL その他のオプション]**&#x200B;ドロップダウンにアクセスします。

   +++要件に基づいて次の設定を行います。
   * **[!UICONTROL 内部名]**：配信に一意の ID を割り当てます。
   * **[!UICONTROL フォルダー]**：配信を特定のフォルダーに保存します。
   * **[!UICONTROL 配信コード]**：独自の命名規則を使用して配信を整理します。
   * **[!UICONTROL 説明]**：配信の説明を指定します。
   * **[!UICONTROL 特性]**：分類目的でメールの特性を指定します。
+++

1. 「**[!UICONTROL オーディエンスを選択]**」ボタンをクリックして、既存のオーディエンスをターゲットにするか、独自のユーザーを作成します。[詳細情報](../audience/about-audiences.md)

   ![](assets/sms_create_2.png)

1. 「**[!UICONTROL コントロールグループを有効にする]**」オプションをオンにして、配信の影響を測定するコントロール母集団を設定すると、メッセージを受信した母集団の行動と、受信しなかった連絡先の行動を比較できるようになります。[詳細情報](../audience/control-group.md)

1. 「**[!UICONTROL コンテンツの編集]**」をクリックして、SMS メッセージのコンテンツのデザインを開始します。[詳細情報](content-sms.md)

   ![](assets/sms_create_4.png)

   この画面から、[コンテンツをシミュレート](../preview-test/preview-test.md)したり、[オファーを設定](../content/offers.md)したりすることもできます。

1. 特定の日時に配信をスケジュールするには、「**[!UICONTROL スケジュールを有効にする]**」オプションをオンにします。配信を開始すると、メッセージは、その受信者に対して定義した、正確な日時に自動的に送信されます。配信スケジュールについて詳しくは、 [この節](../msg/gs-messages.md#gs-schedule).

1. 「**[!UICONTROL 配信設定を指定]**」をクリックして、配信テンプレートに関連する詳細オプションにアクセスします。[詳細情報](../advanced-settings/delivery-settings.md)

   ![](assets/sms_create_3.png)
