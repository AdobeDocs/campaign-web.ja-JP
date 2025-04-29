---
audience: end-user
title: メールコンテンツを編集する
description: Campaign Web ユーザーインターフェイスでメールコンテンツを編集する方法を学ぶ
exl-id: b6316551-bebc-40e0-b75c-4408ce4d6c57
source-git-commit: 498162045a2a58a5326a3cf311a153cf9dfef5c3
workflow-type: tm+mt
source-wordcount: '687'
ht-degree: 48%

---

# メールコンテンツの設定 {#edit-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="メールコンテンツを定義"
>abstract="**コンテンツを編集** 画面では、送信者のアドレスや件名などのメッセージの基本要素を定義し、添付ファイルやオファーの追加などの追加アクションを実行し、メールDesignerにアクセスして洗練された外観をメッセージに設定できます。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_header"
>title="メールのプロパティを設定"
>abstract="「**基本の詳細**」セクションでは、送信者のアドレスと返信先アドレスを更新し、式エディターを使用して件名を定義できます。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_attachment"
>title="メールにファイルを添付"
>abstract="メッセージに挿入する 1 つまたは複数のファイルを選択します。 パフォーマンスの問題を回避するために、1 つのメールに複数の添付ファイルを含めないことをお勧めします。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_options"
>title="トラッキングの編集"
>abstract="デフォルトでは、配信のトラッキングが有効になっています。つまり、メッセージコンテンツに含まれるすべてのリンクが追跡されます。ここからこのオプションを無効にできます。"
>additional-url="https://experienceleague.adobe.com/ja/docs/campaign-web/v8/content/email-design/design-content/message-tracking" text="リンクの追加とメッセージのトラッキング"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_multilingual"
>title="言語を追加"
>abstract="このタブには、配信を送信する言語のリストがあります。 「言語を追加」ボタンをクリックするか、このタブから別の言語を複製して、さらに言語を追加できます。"

メールの&#x200B;**[!UICONTROL コンテンツを編集]**&#x200B;画面では、次の操作を実行できます。

* 送信者のアドレスや件名など、メッセージの基本要素を定義します。
* 添付ファイルの追加やオファーの設定など、追加のアクションを実行します。
* [ メールDesigner](get-started-email-designer.md#start-authoring) にアクセスして、適切なメールのコンテンツの作成を開始します。

>[!NOTE]
>
>この画面の編集可能なテキストフィールドはすべて、パーソナライゼーションフィールドを使用して入力できます。[コンテンツをパーソナライズする方法を学ぶ](../personalization/personalize.md)

メールのコンテンツを設定または編集するには、次の手順に従います。

1. [メール配信ダッシュボード](../email/create-email.md)画面で「**[!UICONTROL コンテンツを編集]**」ボタンをクリックします。

   ![ メール配信ダッシュボードの「コンテンツを編集」ボタンを示したスクリーンショット。](assets/email-edit-content-button.png){zoomable="yes"}

1. メールコンテンツ編集画面が開きます。

   ![ メールコンテンツ編集ダッシュボードを示したスクリーンショット。](assets/email-edit-content-dashboard.png){zoomable="yes"}

   >[!NOTE]
   >
   >新しいメールを設定している場合、「送信者名 **[!UICONTROL および]** 送信元メール **[!UICONTROL フィールドには既に値が入力されて]** ます。

1. 「**[!UICONTROL 送信者名]**」フィールドは、メールテンプレートで定義されます。変更する場合は、ブランド名など、受信者が容易に識別できる名前を使用して、配信の開封率を高めます。

   >[!NOTE]
   >
   >受信者のエクスペリエンスをさらに向上させるには、「Luma からの Eve」などの個人名を追加できます。

1. また、「**[!UICONTROL 送信元メール]**」アドレスフィールドもメールテンプレートで定義されます。アドレスドメインがAdobeにデリゲートしたサブドメインと一致することを確認します。

   >[!NOTE]
   >
   >「@」より前の部分は変更できますが、ドメインアドレスは変更できません。

1. 「**[!UICONTROL 返信先フィールド]**」セクションを展開します。送信者の名前とアドレスは、デフォルトで返信に使用されます。ただし、Adobeでは、ブランドのカスタマーケアなど、既存の実際のアドレスを使用することをお勧めします。 この場合、受信者が返信を送信すると、カスタマーケアチームが処理できます。

   ![ メールコンテンツエディターの「返信先フィールド」セクションを示すスクリーンショット。](assets/email-edit-content-reply-to.png){zoomable="yes"}

1. メールの「**[!UICONTROL 件名]**」を定義します。件名を専用フィールドに直接入力するか、式エディターを開いて、様々な属性、式フラグメントまたはオファーを使用して [ パーソナライゼーション ](../personalization/personalize.md) を追加します。

1. メールにファイルを添付する場合は、「**[!UICONTROL 添付ファイルを追加]** ボタンをクリックして、1 つまたは複数のファイルを選択します。

   >[!NOTE]
   >
   >パフォーマンスの問題を回避するために、1 つのメールに複数の添付ファイルを含めないことをお勧めします。

   <!--limitation on size + number of files?-->

1. メールでオファーを送信する場合は、「**[!UICONTROL オファーを設定]**」ボタンを使用して選択します。

   その後、パーソナライゼーションフィールドを使用してメールに挿入できます。 [オファーの送信方法を学ぶ](../msg/offers.md)

1. 「**[!UICONTROL メール本文を編集]**」ボタンをクリックし、[E メールデザイナー](get-started-email-designer.md#start-authoring)を使用して、メールのコンテンツを構成およびデザインします。メールコンテンツのデザイン方法に関する追加情報については、次の節を参照してください。

   * [新規でのメールの作成](create-email-content.md)
   * [コンテンツのスタイル設定](get-started-email-style.md)

   >[!NOTE]
   >
   >また、メールのプレビューにポインタを合わせて、「**[!UICONTROL E メールデザイナーを開く]**」を選択することもできます。

1. デフォルトでは、配信のトラッキングが有効になっています。このオプションは、「**[!UICONTROL オプション機能]**」セクションから無効にすることができます。[ リンクを追加しトラッキングを管理する方法を説明します ](message-tracking.md)。

1. メールのコンテンツを定義したら、「**[!UICONTROL コンテンツをシミュレート]**」ボタンを使用して、どのように表示されるかを送信前に確認します。[ メールのプレビューとテストの方法を説明します ](../preview-test/preview-test.md)。