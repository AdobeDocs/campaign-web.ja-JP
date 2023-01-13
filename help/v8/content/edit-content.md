---
audience: end-user
title: メールコンテンツの編集
description: Campaign Web UI で E メールコンテンツを編集する方法を説明します
exl-id: b6316551-bebc-40e0-b75c-4408ce4d6c57
source-git-commit: 045025367a826eece052367be557e47aaf37dc99
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 68%

---

# メールコンテンツの編集 {#configure-content}

![](../assets/do-not-localize/badge.png)

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="メールコンテンツの作成"
>abstract="このセクションでは、E メール用のコンテンツを作成し、E メールデザイナーを使用して洗練された外観を設定できます。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_header"
>title="メールヘッダー"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_attachment"
>title="メール添付ファイル"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_options"
>title="トラッキングオプション"
>abstract="TBC"

E メールのコンテンツの作成を開始するには、 **[!UICONTROL コンテンツを編集]** ボタンをクリックします。

![](assets/edit-content.png)

この画面では、メールのコンテンツを定義し、電子メールデザイナーにアクセスしてデザインできます。

![](assets/content-dashboard.png)

メールのコンテンツを定義する手順は次のとおりです。

1. 「**[!UICONTROL 送信者名]**」と「**[!UICONTROL 送信元電子メール]**」の情報を確認します。これらのフィールドは読み取り専用で、メールの作成時に選択したメールテンプレートで設定されます。

1. メールの「**[!UICONTROL 件名]**」を定義します。これをおこなうには、専用のフィールドに件名を直接入力するか、式エディターを開いて、様々な属性、コンテンツブロックまたはオファーを使用してパーソナライゼーションを追加するように定義します。 詳しくは、[コンテンツをパーソナライズする方法](../personalization/personalize.md)を参照してください。

1. メールでオファーを送信する場合は、「**[!UICONTROL オファー]**」ボタンを使用して選択します。 その後、パーソナライゼーションフィールドを使用してメールに挿入できます。詳しくは、[オファーの送信方法](offers.md)を参照してください。

1. 「**[!UICONTROL 電子メールデザイナー]**」ボタンをクリックして、メールのコンテンツを構造化しデザインします。メールコンテンツのデザイン方法に関する追加情報については、次の節を参照してください。

   * [メールのデザイン方法を説明します](create-email-content.md)
   * [コンテンツのスタイル設定](get-started-email-style.md)

1. メールにファイルを添付する場合は、「**[!UICONTROL 添付ファイルを追加]**」ボタンをクリックして、1 つまたは複数のファイルを選択します。

   <!--limitation on size + number of files?-->

1. デフォルトでは、配信に対してトラッキングが有効になっています。 このオプションは、 **[!UICONTROL オプション機能]** 」セクションに入力します。 詳しくは、[リンクを追加しトラッキングを管理する方法](message-tracking.md)を参照してください。

メールのコンテンツを定義したら、「**[!UICONTROL コンテンツをシミュレート]**」ボタンを使用して、どのように表示されるかを送信前に確認します。詳しくは、[メールのプレビューとテストの方法](../preview-test/preview-test.md)を参照してください。

<!-- show screenshot showing an email fully configured + highlight the simulate content button-->
