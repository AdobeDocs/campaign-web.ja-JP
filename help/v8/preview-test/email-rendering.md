---
audience: end-user
title: メールのレンダリングのテスト
description: Campaign web ユーザーインターフェイスでメールのレンダリングをテストする方法について説明します
exl-id: 5cdbce8b-3969-470d-8019-1edc58433146
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: ht
source-wordcount: '243'
ht-degree: 100%

---

# メールのレンダリングのテスト {#email-rendering}

メールを送信する前に、様々な web クライアントやデバイスの受信者に対してメッセージが最適に表示されることを確認します。

これを行うには、[!DNL Adobe Campaign] 内で **Litmus** アカウントを使用して、様々なコンテキストでメールのレンダリングを即座にプレビューします。これにより、主要なデスクトップアプリケーション、web メールサービス、モバイルデバイスなどとの互換性を確認できます。

>[!CAUTION]
>
>Campaign でメールのレンダリングを使用すると、本配信前確認がサードパーティのシステムに送信されます。Litmus アカウントを [!DNL Campaign] に接続することにより、お客様がサードパーティに送信するすべてのデータに対して、アドビが一切の責任を負わないことを認めるものとします。Litmus のメールデータ保持ポリシーは、これらの本配信前確認に含まれる可能性のあるパーソナライゼーションデータを含め、これらのメールに適用されます。このようなデータにアクセスしたり削除したりするには、Litmus に直接お問い合わせください。

メールのレンダリング機能にアクセスするには、次の前提条件を満たします。

* Litmus アカウントを持っていること。
* プロファイルやテストプロファイルを選択すること。詳しくは、[この節](preview-content.md)を参照してください。

次に、以下の手順に従います。

1. [コンテンツを編集](../email/edit-content.md)画面または [E メールデザイナー](../email/get-started-email-designer.md)で、「**[!UICONTROL コンテンツをシミュレート]**」ボタンをクリックします。

1. 「**[!UICONTROL メールをレンダリング]**」ボタンを選択します。

   ![メールエディターの「コンテンツをシミュレート」ボタン](assets/simulate-rendering-button.png){zoomable="yes"}

1. セクションの右上隅の「**Litmus アカウントを接続**」をクリックします。

   ![メールのレンダリングインターフェイスの Litmus アカウント接続オプション](assets/simulate-rendering-litmus.png){zoomable="yes"}

1. 資格情報を入力してログインします。

   ![Litmus アカウントログイン画面](assets/simulate-rendering-credentials.png){zoomable="yes"}

1. 「**テストを実行**」ボタンをクリックして、メールのプレビューを生成します。

1. 一般的なデスクトップ、モバイルおよび web ベースのクライアントでメールコンテンツを確認します。

   ![様々なクライアントでのメールのレンダリングプレビュー](assets/simulate-rendering-previews.png){zoomable="yes"}

<!--
TO CHECK IF user is directed to Litmus or if the email rendering is shown directly in the Campaign UI.

CONTENT ABOVE COPIED FROM AJO

If not redirecting to Litmus:

To test the email rendering, follow these steps:

1. Access the email content creation screen, then click **[!UICONTROL Simulate content]**.

1. Click the **[!UICONTROL Render email]** button.

    The left pane provides various desktop, mobile, and web-based email clients. Select the desired email client to display a preview of your email in the right pane. 

    ![Preview pane showing email rendering across selected clients](assets/render-context.png){zoomable="yes"}

    >[!NOTE]
    >
    >The email clients list provides a sample of the major mail clients. Additional email clients are available from the filter button next to the top search bar.

 -->