---
audience: end-user
title: メールコンテンツの編集
description: Campaign web UI でメールコンテンツを編集する方法を学ぶ
exl-id: b6316551-bebc-40e0-b75c-4408ce4d6c57
badge: label="Beta"
source-git-commit: 9fb4a5057ec05877ffbadc85d1198ab24faf8972
workflow-type: ht
source-wordcount: '505'
ht-degree: 100%

---

# メールコンテンツを設定 {#edit-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="メールコンテンツを作成"
>abstract="この節では、メールのコンテンツを作成し、電子メールデザイナーを使用して洗練された外観にすることができます。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_header"
>title="メールパラメーター"
>abstract="送信者名と送信元メールの値は、メールテンプレートで定義します。件名は、式エディターを使用してパーソナライズできます。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_attachment"
>title="メール添付ファイル"
>abstract="メッセージに挿入する 1 つ以上のファイルを選択します。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_options"
>title="トラッキングオプション"
>abstract="デフォルトでは、配信のトラッキングが有効になっています。ここからこのオプションを無効にできます。"

メールの&#x200B;**[!UICONTROL コンテンツを編集]**&#x200B;画面では、次の操作を実行できます。
* 送信者のアドレスや件名など、メッセージの基本要素を定義する
* 添付ファイルの追加やオファーの設定など、追加のアクションを実行する
* [メールデザイナー](get-started-email-designer.md#start-authoring)にアクセスして、適切なメールのコンテンツの作成を開始する

メールのコンテンツを設定または編集するには、次の手順に従います。

1. [メール配信ダッシュボード](../email/create-email.md)画面で「**[!UICONTROL コンテンツを編集]**」ボタンをクリックします。

   ![](assets/email-edit-content-button.png)

1. メールコンテンツ編集画面が開きます。

   ![](assets/email-edit-content-dashboard.png)

   >[!NOTE]
   >
   >新しいメールを設定している場合、「**[!UICONTROL 送信者名]** 」フィールドと「**[!UICONTROL 送信元メール]**」フィールドには既に値が入力されています。

1. 「**[!UICONTROL 送信者名]**」フィールドは、メールテンプレートで定義されます。変更する場合は、ブランド名など、受信者が容易に識別できる名前を使用して、配信の開封率を高めます。

   >[!NOTE]
   >
   >受信者のエクスペリエンスの質を高めるために、「Luma（担当：田中）」のように個人名を追加する方法もあります。

1. また、「**[!UICONTROL 送信元メール]**」アドレスフィールドもメールテンプレートで定義されます。アドレスドメインがアドビにデリゲートしたサブドメインと同じであることを確認します。

   >[!NOTE]
   >
   >「@」より前の部分は変更できますが、ドメインアドレスは変更できません。

   <!--In the Reply address text fields, the sender's address is used by default for replies. However, Adobe recommends using an existing real address such as your brand's customer care. In this case, if a recipient sends a reply, the customer care will be able to handle it.-->

1. メールの「**[!UICONTROL 件名]**」を定義します。件名を専用フィールドに直接入力するか、式エディターを開いて、様々な属性とコンテンツブロックまたはオファーを使用してパーソナライゼーションを追加します。[コンテンツをパーソナライズする方法を学ぶ](../personalization/personalize.md)

1. メールにファイルを添付する場合は、「**[!UICONTROL 添付ファイルを追加]**」ボタンをクリックして、1 つまたは複数のファイルを選択します。

   >[!NOTE]
   >
   >    パフォーマンスの問題を回避するために、1 つのメールに複数の添付ファイルを含めないことをお勧めします。

   <!--limitation on size + number of files?-->

1. メールでオファーを送信する場合は、「**[!UICONTROL オファーを設定]**」ボタンを使用して選択します。

   その後、パーソナライゼーションフィールドを使用してメールに挿入できます。[オファーの送信方法を学ぶ](offers.md)

1. 「**[!UICONTROL メール本文を編集]**」ボタンをクリックし、[メールデザイナー](#start-authoring) を使用して、メールのコンテンツを構成およびデザインします。メールコンテンツのデザイン方法に関する追加情報については、次の節を参照してください。

   * [新規でのメールの作成](create-email-content.md)
   * [コンテンツのスタイル設定](get-started-email-style.md)

   >[!NOTE]
   >
   >また、メールのプレビューにポインタを合わせて、「**[!UICONTROL メールデザイナーを開く]**」を選択することもできます。

1. デフォルトでは、配信のトラッキングが有効になっています。このオプションは、「**[!UICONTROL オプション機能]**」セクションから無効にすることができます。[リンクを追加してトラッキングを管理する方法を学ぶ](message-tracking.md)

1. メールのコンテンツを定義したら、「**[!UICONTROL コンテンツをシミュレート]**」ボタンを使用して、どのように表示されるかを送信前に確認します。[メールのプレビューとテストの方法を学ぶ](../preview-test/preview-test.md)

