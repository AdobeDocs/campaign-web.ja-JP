---
audience: end-user
title: メールコンテンツの編集
description: Campaign Web UI の E メールデザイナーを使用してコンテンツの作成を開始する方法を説明します
badge: label="Alpha" type="Positive"
source-git-commit: 97c65771f9302bb188de0a8dae05f0d607519d4a
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 9%

---

# 電子メールデザイナーの基本を学ぶ {#get-started-email-designer}

Adobe Campaign で E メールを作成したら、そのコンテンツを定義する必要があります。

E メールデザイナーを使用すると、個別にカスタマイズした魅力的な E メールを、直感的なドラッグ&amp;ドロップインターフェイスで作成できます。 新規のコンテンツから始める場合でも、既存のコンテンツの読み込みか既存のテンプレートの活用かに関わらず、プロモーションやトランザクションなど、あらゆる E メール用のすべてのコンテンツの設計と洗練を行います。

<!--Built to deliver HTML optimized for responsive design, the Email Designer allows you to easily define and apply visibility conditions and dynamic content to an email, template, or fragment directly through the user interface. You can seamlessly switch between the drag and drop interface and HTML code at the click of a button.

The Email Designer allows you to create email content and email content templates. It is compatible with simple emails, transactional emails, A/B test emails, multilingual emails, and recurring emails.-->

* 用途 [!DNL Campaign] e メールデザイン機能を使用して、レスポンシブ e メールを簡単に作成できます。 [詳細情報](create-email-content.md)

* プロファイル属性に基づいてパーソナライズされたを作成することで、顧客体験を強化します。 [詳細情報](../personalization/personalize.md)

* 条件付きコンテンツフィールドを設定して、受信者のプロファイルに基づいて動的なパーソナライゼーションを作成します。 [詳細情報](../personalization/conditions.md)

## E メールデザインのベストプラクティス {#best-practices}

E メールを送信する際は、受信者が E メールを転送する可能性を考慮することが重要です。E メールのレンダリングに問題が生じる場合があります。 これは特に、転送に使用される電子メールプロバイダーでサポートされていない可能性のある CSS クラスを使用する場合に当てはまります。例えば、「is-desktop-hidden」CSS クラスを使用してモバイルデバイスで画像を非表示にする場合です。

これらのレンダリングの問題を最小限に抑えるために、E メールのデザイン構造をできるだけ簡単に保つことをお勧めします。 デスクトップとモバイルデバイスの両方で適切に機能する単一のデザインを使用し、複雑な CSS クラスや、すべての電子メールクライアントで完全にはサポートされない他のデザイン要素を使用しないようにします。 これらのベストプラクティスに従うことで、受信者による表示や転送の方法に関係なく、E メールの一貫したレンダリングを正しくおこなうことができます。

## コンテンツのオーサリングを開始 {#start-authoring}

E メール配信ダッシュボードから、 [コンテンツを編集](edit-content.md) 画面を開いて E メールデザイナーのホームページを開きます。 ここから、次のオプションから E メールのデザイン方法を選択します。

* **メールをゼロからデザイン** 電子メールデザイナーのインターフェイスを使用する。 で E メールコンテンツをデザインする方法を説明します。 [この節](create-email-content.md).

* **コードまたは生のHTMLを貼り付け** を直接電子メールデザイナーに追加します。 で独自のコンテンツをコーディングする方法を学ぶ [この節](code-content.md).

* **既存のHTMLコンテンツの読み込み** ファイルまたは.zip フォルダーから。 電子メールコンテンツをにインポートする方法を説明します。 [この節](existing-content.md).

* **既存のコンテンツを選択** 組み込みテンプレートまたはカスタムテンプレートのリストから。 電子メールテンプレートの使用方法を説明します。 [この節](email-templates.md).

  ![](assets/email_designer_create_options.png)

