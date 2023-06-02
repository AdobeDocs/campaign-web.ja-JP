---
audience: end-user
title: メールコンテンツの編集
description: Campaign web UI でメールコンテンツを編集する方法を学ぶ
exl-id: b6316551-bebc-40e0-b75c-4408ce4d6c57
badge: label="Alpha" type="Positive"
source-git-commit: f04e8aa5ecb12fca02da640b0037441d4cd7d4d3
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 73%

---

# メールコンテンツの編集 {#configure-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="メールコンテンツの作成"
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

メールのコンテンツの作成を開始するには、メール作成画面から「**[!UICONTROL コンテンツを編集]**」ボタンをクリックします。[](../email/create-email.md)

![](assets/email-edit-content.png)

開いた画面では、基本的な詳細の定義、添付ファイルの追加やオファーの設定などの追加のアクションの実行、E メールデザイナーにアクセスしてコンテンツを作成できます。

![](assets/email-edit-content-dashboard.png)

E メールのコンテンツを編集する手順は次のとおりです。

1. 内 **[!UICONTROL 送信者名]** 「 」フィールドに値を入力する場合は、ブランド名など、受信者が容易に識別できる名前を使用して、配信の開封率を高めます。

1. メールの「**[!UICONTROL 件名]**」を定義します。これを行うには、件名を専用フィールドに直接入力するか、式エディターを開いて、様々な属性とコンテンツブロックまたはオファーを使用してパーソナライゼーションを追加するように定義します。[コンテンツをパーソナライズする方法を学ぶ](../personalization/personalize.md)受信者のエクスペリエンスの質を高めるために、「Megastore（担当：田中）」のように個人名を追加する方法もあります。

1. 内 **[!UICONTROL 送信元メール]** 住所フィールドで、住所ドメインが、Adobeにデリゲートしたサブドメインと同じであることを確認します。

   「@」より前の部分は変更できますが、ドメインアドレスは変更できません。

   <!--In the Reply address text fields, the sender's address is used by default for replies. However, Adobe recommends using an existing real address such as your brand's customer care. In this case, if a recipient sends a reply, the customer care will be able to handle it.-->

1. メールの「**[!UICONTROL 件名]**」を定義します。専用のフィールドに件名を直接入力するか、式エディターを開いて、様々な属性、コンテンツブロックまたはオファーを使用したパーソナライゼーションを追加します。 [コンテンツをパーソナライズする方法を学ぶ](../personalization/personalize.md)

1. メールにファイルを添付する場合は、「**[!UICONTROL 添付ファイルを追加]**」ボタンをクリックして、1 つまたは複数のファイルを選択します。

   >[!NOTE]
   >
   >    パフォーマンスの問題を回避するために、1 つのメールに複数の添付ファイルを含めないことをお勧めします。

   <!--limitation on size + number of files?-->

1. メールでオファーを送信する場合は、「**[!UICONTROL オファーを設定]**」ボタンを使用して選択します。

   その後、パーソナライゼーションフィールドを使用してメールに挿入できます。[オファーの送信方法を学ぶ](offers.md)

1. 「**[!UICONTROL メール本文を編集]**」ボタンをクリックして、メールのコンテンツを構成およびデザインします。メールコンテンツのデザイン方法に関する追加情報については、次の節を参照してください。

   * [メールのデザイン方法を説明します](create-email-content.md)
   * [コンテンツのスタイル設定](get-started-email-style.md)

1. デフォルトでは、配信のトラッキングが有効になっています。このオプションは、「**[!UICONTROL オプション機能]**」セクションから無効にすることができます。[リンクを追加してトラッキングを管理する方法を学ぶ](message-tracking.md)

1. メールのコンテンツを定義したら、「**[!UICONTROL コンテンツをシミュレート]**」ボタンを使用して、どのように表示されるかを送信前に確認します。[メールのプレビューとテストの方法を学ぶ](../preview-test/preview-test.md)
