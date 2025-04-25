---
audience: end-user
title: メールコンテンツを編集する
description: Campaign Web ユーザーインターフェイスのメールデザイナーを使用して、コンテンツ作成を開始する方法を学ぶ
exl-id: a5b966bb-09da-4a50-98d4-010fdfbb75cf
source-git-commit: d7fc756b2e1d94b43c76ced748e1bf7c7ae5da0d
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 95%

---


# E メールデザイナーの基本を学ぶ {#get-started-email-designer}

Adobe Campaign でメールを作成したら、そのコンテンツを定義する必要があります。

E メールデザイナーを使用すると、直感的なドラッグ＆ドロップインターフェイスを通じて、個別にカスタマイズされた魅力的なメールを作成できます。空白の状態から開始する場合でも、既存のコンテンツをインポートする場合でも、既存のテンプレートを活用する場合でも、プロモーションやトランザクションなど、あらゆるメールコンテンツのデザインと強化に対応します。

<!--Built to deliver HTML optimized for responsive design, the Email Designer allows you to easily define and apply visibility conditions and dynamic content to an email, template, or content fragment directly through the user interface. You can seamlessly switch between the drag and drop interface and HTML code at the click of a button.

The Email Designer allows you to create email content and email content templates. It is compatible with simple emails, transactional emails, A/B test emails, multilingual emails, and recurring emails.-->

* [!DNL Campaign] のメールデザイン機能を使用すると、レスポンシブなメールを簡単に作成できます。[詳細情報](create-email-content.md)

* プロファイル属性に基づいてパーソナライズされたメールを作成することで、顧客体験を向上させます。[詳細情報](../personalization/personalize.md)

* 条件付きコンテンツフィールドを設定して、受信者のプロファイルに基づいて動的パーソナライゼーションを作成します。[詳細情報](../personalization/conditions.md)

## メールデザインのベストプラクティス {#best-practices}

メールを送信する際は、受信者がメールを転送する可能性があることを考慮してください。転送すると、メールのレンダリングで問題が発生する可能性があります。これは、転送に使用するメールプロバイダーでサポートされていない可能性のある CSS クラスを使用する場合に特に当てはまります。例えば、&quot;is-desktop-hidden&quot; CSS クラスを使用してモバイルデバイスで画像を非表示にすると、画像が正しくレンダリングされない場合があります。

これらのレンダリングの問題を最小限に抑えるために、メールのデザイン構造をできるだけシンプルにすることをお勧めします。デスクトップとモバイルデバイスの両方で適切に機能する単一のデザインを使用し、すべてのメールクライアントで完全にはサポートされていない可能性がある、複雑な CSS クラスやその他のデザイン要素を使用しないようにします。メールで画像を使用する場合は、2 MB を超える画像を使用しないか、エンコードされた画像リンクを使用します。

これらのベストプラクティスに従うことで、受信者が使用しているメールの表示方法や転送方法に関係なく、メールは常に正しく表示されます。

## コンテンツの作成を開始 {#start-authoring}

メール配信ダッシュボードから、[コンテンツを編集](edit-content.md)画面に移動して、E メールデザイナーのホームページを開きます。ここで、次のオプションからメールのデザイン方法を選択します。

* **メールをゼロからデザイン** - E メールデザイナーのインターフェイスを使用します。メールコンテンツのデザイン方法については、[この節](create-email-content.md)を参照してください。

* **Raw HTML をコーディングまたはペースト** - E メールデザイナーで直接行います。独自のコンテンツのコーディング方法については、[この節](code-content.md)を参照してください。

* **既存の HTML コンテンツをインポート** - ファイルまたは .zip フォルダーから行います。メールコンテンツのインポート方法については、[この節](existing-content.md)を参照してください。

* **既存のコンテンツを選択** - 組み込みテンプレートまたはカスタムテンプレートのリストから行います。メールテンプレートの操作方法については、[この節](create-email-templates.md)を参照してください。

  ![メールコンテンツを作成するために E メールデザイナーインターフェイスで使用できるオプション](assets/email_designer_create_options.png){zoomable="yes"}
