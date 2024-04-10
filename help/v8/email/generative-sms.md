---
audience: end-user
title: Campaign の AI アシスタントを使用した SMS
description: Campaign の AI アシスタントの基本を学ぶ
badge: label="Beta"
hide: true
hidefromtoc: true
exl-id: db0459e5-8759-42d9-8945-8c9667450527
source-git-commit: 886fd47b52d08b0a1bfcbeca03929d48b5bc2a3f
workflow-type: ht
source-wordcount: '433'
ht-degree: 100%

---

# AI アシスタントを使用した SMS の生成 {#generative-sms}

>[!BEGINSHADEBOX]

**目次**

* [AI アシスタントの基本を学ぶ](generative-gs.md)
* [AI アシスタントを使用したメールの生成](generative-content.md)
* **[AI アシスタントを使用した SMS の生成](generative-sms.md)**
* [AI アシスタントを使用したプッシュ通知の生成](generative-push.md)

>[!ENDSHADEBOX]

SMS メッセージをオーディエンスに合わせて作成してパーソナライズしたら、革新的な AI テクノロジーを利用した Campaign の AI アシスタントを利用して、コミュニケーションを次のレベルに引き上げます。

この便利なツールは、コンテンツを絞り込むためのインテリジェントな提案を提供し、メッセージが効果的に共感を呼び、エンゲージメントを最大化します。

>[!NOTE]
>
>この機能の使用を開始する前に、関連する[ガードレールと制限](generative-gs.md#guardrails-and-limitations)のトピックに目を通してください。

1. SMS 配信を作成および設定した後、「**[!UICONTROL コンテンツを編集]**」をクリックします。

   SMS 配信の設定方法について詳しくは、[このページ](../sms/create-sms.md)を参照してください。

1. 配信の&#x200B;**[!UICONTROL 基本的な詳細]**&#x200B;を入力します。完了したら、「**[!UICONTROL コンテンツを編集]**」をクリックします。

1. 必要に応じて、SMS メッセージをパーソナライズします。[詳細情報](../sms/content-sms.md)

1. **[!UICONTROL AI アシスタントを表示]**&#x200B;メニューにアクセスします。

   ![](assets/sms-genai-1.png){zoomable=&quot;yes&quot;}

1. 「**[!UICONTROL プロンプト]**」フィールドで生成する内容を記述して、コンテンツを微調整します。

   プロンプトの作成に関するサポートが必要な場合は、配信を改善するための様々なプロンプトのアイデアを提供する&#x200B;**[!UICONTROL プロンプトライブラリ]**&#x200B;にアクセスしてください。

   ![](assets/sms-genai-2.png){zoomable=&quot;yes&quot;}

1. 「**[!UICONTROL 現在のコンテキストで拡張]**」オプションを有効にして、AI アシスタントで、配信、配信名、選択したオーディエンスに基づいて新しいコンテンツをパーソナライズします。

   >[!IMPORTANT]
   >
   > ブランドアセットをアップロードするか、「**[!UICONTROL 現在のコンテンツで拡張]**」オプションを有効にして、プロンプトを常に特定のコンテキストに関連付ける必要があります。

1. 「**[!UICONTROL ブランドアセットをアップロード]**」を選択し、AI アシスタントに追加のコンテキストを提供できるコンテンツを含むブランドアセットを追加します。

1. ニーズに最も合う&#x200B;**[!UICONTROL コミュニケーション戦略]**&#x200B;を選択します。これは、生成されるテキストのトーンとスタイルに影響を与えます。

1. 生成されるテキストの&#x200B;**[!UICONTROL 言語]**&#x200B;および&#x200B;**[!UICONTROL トーン]**&#x200B;を選びます。これにより、テキストがオーディエンスと目的に適したものになります。

   ![](assets/sms-genai-3.png){zoomable=&quot;yes&quot;}

1. スライダーコントロールを使用して、生成されるテキストの長さを設定します。

1. プロンプトの準備が整ったら、「**[!UICONTROL 生成]**」をクリックします。

1. 生成された&#x200B;**[!UICONTROL バリエーション]**&#x200B;を参照して、適切なコンテンツが見つかったら、「**[!UICONTROL 適用]**」をクリックします。

   「**[!UICONTROL プレビュー]**」をクリックして、選択したバリエーションのフルスクリーンバージョンを表示します。

   ![](assets/sms-genai-4.png){zoomable=&quot;yes&quot;}

1. パーソナライゼーションフィールドを挿入して、プロファイルデータに基づいて SMS コンテンツをカスタマイズします。[コンテンツのパーソナライゼーションの詳細情報](../personalization/personalize.md)

   ![](assets/sms-genai-5.png){zoomable=&quot;yes&quot;}

1. メッセージコンテンツを定義したら、「**[!UICONTROL コンテンツをシミュレート]**」ボタンをクリックして、レンダリングを制御し、テストプロファイルでパーソナライゼーション設定を確認します。[詳細情報](../preview-test/preview-content.md)

   ![](assets/sms-genai-6.png){zoomable=&quot;yes&quot;}

1. コンテンツ、オーディエンスおよびスケジュールを定義したら、SMS 配信の準備が整います。[詳細情報](../monitor/prepare-send.md)
