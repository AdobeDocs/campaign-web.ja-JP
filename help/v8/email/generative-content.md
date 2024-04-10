---
audience: end-user
title: AI アシスタントを使用したテキスト
description: Campaign での AI アシスタントの基本を学ぶ
badge: label="ベータ版"
exl-id: d9d35c1d-13db-4d2c-82f8-1629fd1e5848
hide: true
hidefromtoc: true
source-git-commit: 396f52cfdb482e5afdf43b5729ef37b5a634be3d
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 46%

---

# AI アシスタントによるメール生成 {#generative-content}

>[!BEGINSHADEBOX]

**Table of content**

* [AI アシスタントの基本を学ぶ](generative-gs.md)
* **[AI アシスタントによるメール生成](generative-content.md)**
* [AI アシスタントによる SMS 生成](generative-sms.md)
* [AI アシスタントによるプッシュ通知の生成](generative-push.md)

>[!ENDSHADEBOX]

メールを作成してパーソナライズしたら、生成 AI を活用した Campaign のJourney Optimizer AI アシスタントを使用して、コンテンツを次のレベルに引き上げます。

AI アシスタントは、オーディエンスの共感を得られる可能性の高い様々なコンテンツを提案することで、配信の影響を最適化するのに役立ちます。

>[!NOTE]
>
>この機能の使用を開始する前に、関連する[ガードレールと制限](generative-gs.md#guardrails-and-limitations)のトピックに目を通してください。

## AI アシスタントによるコンテンツ生成 {#generative-text}

1. メール配信を作成および設定したら、「**[!UICONTROL コンテンツを編集]**」をクリックします。

   メール配信の設定方法について詳しくは、[こちらのページ](../email/create-email-content.md)を参照してください。

1. 配信の&#x200B;**[!UICONTROL 基本的な詳細]**&#x200B;を入力します。完了したら、 **[!UICONTROL コンテンツを編集]**.

1. 必要に応じてメールをパーソナライズします。 [詳細情報](content-components.md)

1. へのアクセス **[!UICONTROL AI アシスタント]** メニュー。

   以下を選択することもできます **[!UICONTROL テキストコンポーネント]** 特定のコンテンツのみをターゲットにします。

   ![](assets/text-genai-1.png){zoomable=&quot;yes&quot;}

1. で生成する内容を記述して、コンテンツを微調整します **[!UICONTROL プロンプト]** フィールド。

   プロンプトの作成に関する支援を探している場合は、 **[!UICONTROL プロンプトライブラリ]** を使用すると、配信を改善するための様々な迅速なアイデアを利用できます。

   ![](assets/text-genai-2.png){zoomable=&quot;yes&quot;}

1. を切り替え **[!UICONTROL 件名]** または **[!UICONTROL プリヘッダー]** をクリックして、バリアント生成に含めます。

1. コンテキストメニューで、 **[!UICONTROL 現在のコンテキストで拡張]** 配信、配信名、選択したオーディエンスに基づいて新しいコンテンツをパーソナライズするための AI アシスタントのオプション。

   >[!IMPORTANT]
   >
   > プロンプトは、ブランドアセットをアップロードするか、を有効にすることで、常に特定のコンテキストに結び付ける必要があります。 **[!UICONTROL 現在のコンテンツの拡張]** オプション。

1. クリック **[!UICONTROL ブランドアセットのアップロード]** AI アシスタントに追加のコンテキストを提供できるコンテンツを含むブランドアセットを追加します。

   ![](assets/text-genai-3.png){zoomable=&quot;yes&quot;}

1. ニーズに最も合う&#x200B;**[!UICONTROL コミュニケーション戦略]**&#x200B;を選択します。これは、生成されるテキストのトーンとスタイルに影響を与えます。

1. 生成されるテキストの&#x200B;**[!UICONTROL 言語]**&#x200B;および&#x200B;**[!UICONTROL トーン]**&#x200B;を選びます。これにより、テキストがオーディエンスと目的に適したものになります。

   ![](assets/text-genai-4.png){zoomable=&quot;yes&quot;}

1. プロンプトの準備が整ったら、「**[!UICONTROL 生成]**」をクリックします。

1. 生成された&#x200B;**[!UICONTROL バリエーション]**&#x200B;を参照して、適切なコンテンツが見つかったら、「**[!UICONTROL 適用]**」をクリックします。

   「**[!UICONTROL プレビュー]**」をクリックして、選択したバリエーションのフルスクリーンバージョンを表示します。

   ![](assets/text-genai-5.png){zoomable=&quot;yes&quot;}

1. パーソナライゼーションフィールドを挿入して、プロファイルデータに基づいてメールコンテンツをカスタマイズします。[詳しくは、コンテンツのパーソナライゼーションを参照してください](../personalization/personalize.md)

   ![](assets/text-genai-6.png){zoomable=&quot;yes&quot;}

1. メッセージコンテンツを定義したら、「**[!UICONTROL コンテンツをシミュレート]**」ボタンをクリックして、レンダリングを制御し、テストプロファイルでパーソナライゼーション設定を確認します。[詳細情報](../preview-test/preview-content.md)

   ![](assets/text-genai-7.png){zoomable=&quot;yes&quot;}

1. コンテンツ、オーディエンスおよびスケジュールを定義したら、メール配信の準備が整いました。[詳細情報](../monitor/prepare-send.md)

## AI アシスタントによる画像の生成 {#generative-image}

次の例では、AI アシスタントを活用してコンテンツを最適化および改善し、より使いやすいエクスペリエンスを確保する方法について説明します。 次の手順に従います。

1. メール配信を作成および設定したら、「**[!UICONTROL コンテンツを編集]**」をクリックします。

   メール配信の設定方法について詳しくは、[こちらのページ](../email/create-email-content.md)を参照してください。

1. 配信の&#x200B;**[!UICONTROL 基本的な詳細]**&#x200B;を入力します。完了したら、「**[!UICONTROL メールコンテンツを編集]**」をクリックします。

1. AI アシスタントで変更するアセットを選択します。

1. 右側のメニューから、 **[!UICONTROL AI アシスタント]**.

   ![](assets/image-genai-1.png){zoomable=&quot;yes&quot;}

1. で生成する内容を記述して、コンテンツを微調整します **[!UICONTROL プロンプト]** フィールド。

   プロンプトの作成に関する支援を探している場合は、 **[!UICONTROL プロンプトライブラリ]** を使用すると、配信を改善するための様々な迅速なアイデアを利用できます。

   ![](assets/image-genai-2.png){zoomable=&quot;yes&quot;}

1. クリック **[!UICONTROL ブランドアセットのアップロード]** AI アシスタントに追加のコンテキストを提供できるコンテンツを含むブランドアセットを追加します。

   >[!IMPORTANT]
   >
   > プロンプトは、常に特定のコンテキストに関連付ける必要があります。

1. アセットの「**[!UICONTROL 縦横比]**」を選択します。これにより、アセットの幅と高さが決まります。

   16:9、4:3、3:2、1:1 などの一般的な比率から選択することも、カスタムサイズを入力することもできます。

1. 「**[!UICONTROL カラーとトーン]**」、「**[!UICONTROL コンテンツタイプ]**」、「**[!UICONTROL 照明]**」および「**[!UICONTROL コンポジション]**」の設定を、目的のアセット特性に合わせてカスタマイズします。

   ![](assets/image-genai-3.png){zoomable=&quot;yes&quot;}

1. プロンプトの設定が完了したら、「**[!UICONTROL 生成]**」をクリックします。

1. を参照 **[!UICONTROL バリエーションの提案]** をクリックして目的のアセットを検索します。

   「**[!UICONTROL プレビュー]**」をクリックして、選択したバリエーションのフルスクリーンバージョンを表示します。

   ![](assets/image-genai-5.png){zoomable=&quot;yes&quot;}

1. を選択 **[!UICONTROL 類似を表示]** このバリアントに関連する画像を表示する場合。

1. 適切なコンテンツが見つかったら、「**[!UICONTROL 選択]**」をクリックします。

   ![](assets/image-genai-6.png){zoomable=&quot;yes&quot;}

1. メッセージコンテンツを定義したら、「**[!UICONTROL コンテンツをシミュレート]**」ボタンをクリックしてレンダリングを制御し、テストプロファイルでパーソナライゼーション設定を確認します。[詳細情報](../preview-test/preview-content.md)

   ![](assets/image-genai-7.png){zoomable=&quot;yes&quot;}

1. コンテンツ、オーディエンスおよびスケジュールを定義したら、メール配信の準備が整いました。[詳細情報](../monitor/prepare-send.md)
