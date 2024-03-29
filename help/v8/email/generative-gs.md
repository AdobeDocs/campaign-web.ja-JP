---
audience: end-user
title: AI アシスタントの概要
description: AI アシスタントの概要
badge: label="ベータ版"
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
hide: true
hidefromtoc: true
source-git-commit: af67094638cfc3c5c64385203340918f0f8f2482
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 63%

---

# AI アシスタントの概要 {#generative-gs}

>[!BEGINSHADEBOX]

**目次**

* **[AI アシスタントの概要](generative-gs.md)**
* [AI アシスタントを使用した E メールの生成](generative-content.md)
* [AI アシスタントを使用した SMS の生成](generative-sms.md)
* [AI アシスタントを使用したプッシュ通知の生成](generative-push.md)

>[!ENDSHADEBOX]

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="AI アシスタント"
>abstract="配信を作成し、パーソナライズしたら、AI Assistant を使用してコンテンツを強化できます。 この機能を使用すると、生成する内容を記述してコンテンツを微調整できるので、パーソナライゼーションとコンテンツ改善のプロセスが簡素化されます。"


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Campaign で AI アシスタントを使用してコンテキストを定義"
>abstract="選択したコンテンツをコンテンツ生成の入力として使用するには、「**現在のコンテンツを使用して強化**」切替スイッチをオンにします。また、ブランドアセットをアップロードして、ソースとして使用することもできます。選択したコンテンツを使用しない場合は、ブランドアセットのアップロードと選択が必須です。"


>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Adobe 生成 AI の用語"
>abstract="この機能へアクセスするには、Adobe Experience Cloud 生成 AI ユーザーガイドラインへの同意が必要です。この機能に対して提供するプロンプト、コンテキスト、補足情報、またはその他の入力は、特定のコンテキストに関連付ける必要があります。特定のコンテキストには、ブランディング資料、web サイトコンテンツ、データ、そのようなデータのスキーマ、テンプレート、その他の信頼できるドキュメントが含まれますが、個人情報を含めることはできません (個人情報には、特定の個人に関連付けられる可能性のあるすべての情報が含まれます)。この機能からの出力が正確であるかどうかを確認し、ユースケースに適していることを確認する必要があります。"
>additional-url="https://www.adobe.com/jp/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe 生成 AI ユーザーガイドライン"

AI Assistant は、E メールの内容を改善するための貴重なツールです。 パーソナライゼーションとコンテンツ強化が簡素化され、メール配信を最適化してオーディエンスの共感を深めることができます。

この機能を利用すると、完全なメールコンテンツが自動的に生成されるので、時間を節約し一貫した品質を確保できます。生成 AI を使用すると、魅力的なメールを簡単に作成して、コミュニケーションの効果と効率を高めることができます。

>[!NOTE]
>
>この機能はアルファ版で使用でき、予告なく変更される場合があります。10 月初旬にはアクティブ化されます。

## ガードレールと制限 {#generative-guardrails}

E メール生成に Campaign で AI アシスタントを使用する際の一般的なガイドラインを次に示します。

* 生成されるコンテンツの品質は、定義したマーケティング目的やプロンプトに大きく左右されます。生成 AI モデルで正確に解釈できるように、適切に定義されたプロンプトを使用します。 
* ブランドアセットをアップロードして、正確なオンブランドコンテンツを確保します。それ以外の場合は、公開されている情報に基づいたコンテンツになります。アップロードされるコンテンツは、PDF、JPEG、PNG または ZIP ファイル（サポートされているファイル形式のもの）の形式です。
* アップロードされたブランドアセットの推奨サイズは 50MB 未満です。これより大きなファイルや多数の画像の場合でも動作しますが、処理時間が長くなります。
* Adobe Campaignで作成した電子メールテンプレートを使用します。できれば [組み込みの電子メールテンプレート](../email/create-email-templates.md)、E メールコンテンツを作成するためのブランド固有のテンプレートまたはカスタムテンプレート。 最大 8～10 個の画像を含むメールテンプレートをお勧めします。


Campaign の AI Assistant には次の制限が適用されます。

* サポートされている言語は英語のみです。
* E メール、プッシュ、SMS の各チャネルでのみ使用できます。
* GenAI のコンテンツは、必ずしも正確ではない場合があります。エンジニアがモデルを改善できるよう、お客様のフィードバックを共有してください。
* 複数のブランドアセットをアップロードできますが、特定の世代に使用できるブランドアセットは 1 つだけです。



<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="メール生成" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>AI アシスタントを使用した E メールの生成</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-sms.md">
<img alt="SMS の生成" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-sms.md"><strong>AI アシスタントを使用した SMS の生成</strong>
</div>
<p>
</td>
<td>
<a href="generative-push.md">
<img alt="プッシュ生成" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-push.md"><strong>AI アシスタントを使用したプッシュ通知の生成</strong></a>
</div>
<p></td>
</tr></table>
