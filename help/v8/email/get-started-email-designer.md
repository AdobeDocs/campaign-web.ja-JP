---
audience: end-user
title: メールコンテンツを編集する
description: Campaign Web ユーザーインターフェイスのメールデザイナーを使用して、コンテンツ作成を開始する方法を学ぶ
exl-id: a5b966bb-09da-4a50-98d4-010fdfbb75cf
source-git-commit: eccd1ce6f95682d3dcfc224061f747f7da0b6681
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 45%

---


# E メールデザイナーの基本を学ぶ {#get-started-email-designer}

Adobe Campaignでメールを作成したら、そのコンテンツを定義する必要があります。

E メールデザイナーを使用すると、直感的なドラッグ＆ドロップインターフェイスを通じて、個別にカスタマイズされた魅力的なメールを作成できます。空白の状態から開始する場合でも、既存のコンテンツを読み込む場合でも、既存のテンプレートを活用する場合でも、プロモーションやトランザクションなど、あらゆるメールコンテンツのデザインと強化に対応します。

<!--Built to deliver HTML optimized for responsive design, the Email Designer allows you to easily define and apply visibility conditions and dynamic content to an email, template, or content fragment directly through the user interface. You can seamlessly switch between the drag and drop interface and HTML code at the click of a button.

The Email Designer allows you to create email content and email content templates. It is compatible with simple emails, transactional emails, A/B test emails, multilingual emails, and recurring emails.-->

* [!DNL Campaign] のメールデザイン機能を使用すると、レスポンシブなメールを簡単に作成できます。[詳細情報](create-email-content.md)

* プロファイル属性に基づいてパーソナライズされたメールを作成し、顧客体験を強化します。 [詳細情報](../personalization/personalize.md)

* 条件付きコンテンツフィールドを設定して、受信者のプロファイルに基づいて動的パーソナライゼーションを作成します。[詳細情報](../personalization/conditions.md)

## メールデザインのベストプラクティス {#best-practices}

メールを送信する際は、受信者がメールを転送する可能性を考慮してください。これにより、メールのレンダリングで問題が発生する可能性があります。 これは特に、転送に使用するメールプロバイダーでサポートされていない可能性のある CSS クラスを使用する場合に当てはまります。 例えば、「is-desktop-hidden」 CSS クラスを使用してモバイルデバイスで画像を非表示にすると、正しくレンダリングされない場合があります。

これらのレンダリングの問題を最小限に抑えるには、メールのデザイン構造をできるだけシンプルにします。 デスクトップとモバイルデバイスの両方で適切に機能する単一のデザインを使用し、複雑な CSS クラスや、すべてのメールクライアントで完全にはサポートされない他のデザイン要素を使用しないでください。 これらのベストプラクティスに従うと、受信者による表示や転送の方法に関係なく、一貫してメールをレンダリングできます。

## コンテンツの作成を開始 {#start-authoring}

メール配信ダッシュボードから、[コンテンツを編集](edit-content.md)画面に移動して、E メールデザイナーのホームページを開きます。ここで、次のオプションからメールのデザイン方法を選択します。

* **メールをゼロからデザイン** - E メールデザイナーのインターフェイスを使用します。メールコンテンツのデザイン方法については、[この節](create-email-content.md)を参照してください。

* **Raw HTML をコーディングまたはペースト** - E メールデザイナーで直接行います。独自のコンテンツのコーディング方法については、[この節](code-content.md)を参照してください。

* **既存の HTML コンテンツをインポート** - ファイルまたは .zip フォルダーから行います。メールコンテンツの読み込み方法については、[ この節 ](existing-content.md) を参照してください。

* **既存のコンテンツを選択** - 組み込みテンプレートまたはカスタムテンプレートのリストから行います。メールテンプレートの使用方法については、[ この節 ](create-email-templates.md) を参照してください。

  ![ メールコンテンツを作成するために E メールDesignerインターフェイスで使用できるオプション ](assets/email_designer_create_options.png){zoomable="yes"}
