---
audience: end-user
title: Campaign の AI アシスタントを使用したプッシュ通知
description: Campaign での AI アシスタントの概要
badge: label="ベータ版"
hide: true
hidefromtoc: true
source-git-commit: af67094638cfc3c5c64385203340918f0f8f2482
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 39%

---

# AI アシスタントを使用したプッシュ通知の生成 {#generative-push}

>[!BEGINSHADEBOX]

**目次**

* [AI アシスタントの概要](generative-gs.md)
* [AI アシスタントを使用した E メールの生成](generative-content.md)
* [AI アシスタントを使用した SMS の生成](generative-sms.md)
* **[AI アシスタントを使用したプッシュ通知の生成](generative-push.md)**

>[!ENDSHADEBOX]

E メールを作成し、パーソナライズしたら、生成 AI を利用した Campaign の AI Assistant を使用して、コンテンツを次のレベルに引き上げます。

AI Assistant は、オーディエンスの共感を呼ぶ可能性の高い様々なコンテンツを提案することで、配信の影響を最適化するのに役立ちます。

>[!NOTE]
>
>この機能の使用を開始する前に、関連する[ガードレールと制限](generative-gs.md#guardrails-and-limitations)のトピックに目を通してください。

1. プッシュ通知配信を作成および設定した後、 **[!UICONTROL コンテンツを編集]**.

   プッシュ配信の設定方法について詳しくは、 [このページ](../push/create-push.md).

1. 配信の&#x200B;**[!UICONTROL 基本的な詳細]**&#x200B;を入力します。完了したら、「 **[!UICONTROL コンテンツを編集]**.

1. 必要に応じて、プッシュ通知をパーソナライズします。 [詳細情報](../push/content-push.md)

1. 次にアクセス： **[!UICONTROL AI アシスタントを表示]** メニュー。

   ![](assets/push-genai-1.png){zoomable=&quot;yes&quot;}

1. コンテンツを微調整するには、 **[!UICONTROL プロンプト]** フィールドに入力します。

   プロンプトの作成に関するサポートを探している場合は、 **[!UICONTROL プロンプトライブラリ]** 配信を改善するための迅速なアイデアの多様な範囲を提供します。

   ![](assets/push-genai-2.png){zoomable=&quot;yes&quot;}

1. を有効にします。 **[!UICONTROL 現在のコンテキストで拡張]** 」オプションを使用します。

   >[!IMPORTANT]
   >
   > プロンプトは、ブランドアセットをアップロードするか、 **[!UICONTROL 現在のコンテンツを拡張]** オプション。

   ![](assets/push-genai-3.png){zoomable=&quot;yes&quot;}

1. 選択 **[!UICONTROL ブランドアセットをアップロード]** :AI Assistant に追加のコンテキストを提供できるコンテンツを含むブランドアセットを追加します。

1. 生成するフィールドを選択してください： **[!UICONTROL タイトル]**, **[!UICONTROL 字幕]** または **[!UICONTROL メッセージ]**.

1. ニーズに最も合う&#x200B;**[!UICONTROL コミュニケーション戦略]**&#x200B;を選択します。これは、生成されるテキストのトーンとスタイルに影響を与えます。

1. 生成されるテキストの&#x200B;**[!UICONTROL 言語]**&#x200B;および&#x200B;**[!UICONTROL トーン]**&#x200B;を選びます。これにより、テキストがオーディエンスと目的に適したものになります。

   ![](assets/push-genai-4.png){zoomable=&quot;yes&quot;}

1. プロンプトの準備が整ったら、「**[!UICONTROL 生成]**」をクリックします。

1. 生成された&#x200B;**[!UICONTROL バリエーション]**&#x200B;を参照して、適切なコンテンツが見つかったら、「**[!UICONTROL 適用]**」をクリックします。

   「**[!UICONTROL プレビュー]**」をクリックして、選択したバリエーションのフルスクリーンバージョンを表示します。

   ![](assets/push-genai-5.png){zoomable=&quot;yes&quot;}

1. パーソナライゼーションフィールドを挿入して、プロファイルデータに基づいてメールコンテンツをカスタマイズします。[詳しくは、コンテンツのパーソナライゼーションを参照してください](../personalization/personalize.md)

   ![](assets/push-genai-6.png){zoomable=&quot;yes&quot;}

1. メッセージコンテンツを定義したら、「**[!UICONTROL コンテンツをシミュレート]**」ボタンをクリックして、レンダリングを制御し、テストプロファイルでパーソナライゼーション設定を確認します。[詳細情報](../preview-test/preview-content.md)

   ![](assets/push-genai-7.png){zoomable=&quot;yes&quot;}

1. コンテンツ、オーディエンスおよびスケジュールを定義したら、メール配信の準備が整いました。[詳細情報](../monitor/prepare-send.md)
