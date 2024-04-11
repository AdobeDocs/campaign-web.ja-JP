---
audience: end-user
title: AI アシスタントの基本を学ぶ
description: AI アシスタントの基本を学ぶ
badge: label="Beta"
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
hide: true
hidefromtoc: true
source-git-commit: f249a73e25857e65e200f3cbd9516206aab918f9
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 90%

---

# AI アシスタントの基本を学ぶ {#generative-gs}

>[!BEGINSHADEBOX]

**目次**

* **[AI アシスタントの基本を学ぶ](generative-gs.md)**
* [AI アシスタントを使用したメールの生成](generative-content.md)
* [AI アシスタントを使用した SMS の生成](generative-sms.md)
* [AI アシスタントを使用したプッシュ通知の生成](generative-push.md)

>[!ENDSHADEBOX]

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="AI アシスタント"
>abstract="配信を作成しパーソナライズしたら、AI アシスタントを使用してコンテンツを強化できます。この機能を使用すると、生成する内容を記述してコンテンツを微調整できるので、パーソナライゼーションとコンテンツ改善のプロセスが簡素化されます。"


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Campaign で AI アシスタントを使用してコンテキストを定義"
>abstract="選択したコンテンツをコンテンツ生成の入力として使用するには、「**現在のコンテンツを使用して強化**」切替スイッチをオンにします。また、ブランドアセットをアップロードして、ソースとして使用することもできます。選択したコンテンツを使用しない場合は、ブランドアセットのアップロードと選択が必須です。"


>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Adobe 生成 AI の用語"
>abstract="この機能へアクセスするには、Adobe Experience Cloud 生成 AI ユーザーガイドラインへの同意が必要です。この機能に対して提供するプロンプト、コンテキスト、補足情報、またはその他の入力は、特定のコンテキストに関連付ける必要があります。特定のコンテキストには、ブランディング資料、web サイトコンテンツ、データ、そのようなデータのスキーマ、テンプレート、その他の信頼できるドキュメントが含まれますが、個人情報を含めることはできません (個人情報には、特定の個人に関連付けられる可能性のあるすべての情報が含まれます)。この機能からの出力が正確であるかどうかを確認し、ユースケースに適していることを確認する必要があります。"
>additional-url="https://www.adobe.com/jp/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe 生成 AI ユーザーガイドライン"

Azure OpenAI と Azure AI ビジョンを活用した AI アシスタントは、メールコンテンツを改善するための貴重なツールとして機能します。 パーソナライゼーションとコンテンツ強化が簡素化され、メール配信を最適化してオーディエンスの共感を深めることができます。

この機能を利用すると、完全なメールコンテンツが自動的に生成されるので、時間を節約し一貫した品質を確保できます。生成 AI を使用すると、魅力的なメールを簡単に作成して、コミュニケーションの効果と効率を高めることができます。

>[!NOTE]
>
>この機能はアルファ版で使用でき、予告なく変更される場合があります。10 月初旬にはアクティブ化されます。

## ガードレールと制限 {#generative-guardrails}

メールの生成に Campaign の AI アシスタントを使用する際の一般的なガイドラインは次のとおりです。

* 生成されるコンテンツの品質は、定義したマーケティング目的やプロンプトに大きく左右されます。生成 AI モデルで正確に解釈できるように、適切に定義されたプロンプトを使用します。 
* ブランドアセットをアップロードして、正確なオンブランドコンテンツを確保します。それ以外の場合は、公開されている情報に基づいたコンテンツになります。アップロードされるコンテンツは、PDF、JPEG、PNG または ZIP ファイル（サポートされているファイル形式のもの）の形式です。
* アップロードされたブランドアセットの推奨サイズは 50MB 未満です。これより大きなファイルや多数の画像の場合でも動作しますが、処理時間が長くなります。
* Adobe Campaign で作成したメールテンプレートを使用するか、できれば[組み込みのメールテンプレート](../email/create-email-templates.md)、ブランド固有のテンプレートまたはカスタムテンプレートを使用して、メールコンテンツを作成します。最大 8～10 個の画像を含むメールテンプレートをお勧めします。
* バリアントを選択する際は、サムアップ、サムダウンまたはフラグアイコンを使用して、問題のある出力を報告してください。
* AI アシスタントの使用は、Adobe Experience Cloud ジェネレーティブ AI ユーザーガイドラインの対象となります。 [詳細情報](https://www.adobe.com/jp/legal/licenses-terms/adobe-gen-ai-user-guidelines.html)

Campaign の AI アシスタントには、次の制限が適用されます。

* サポートされている言語は英語のみです。
* メール、プッシュ、SMS の各チャネルにのみ使用できます。
* 生成 AI のコンテンツは必ずしも正確でない場合があります。エンジニアがモデルを改善できるように、フィードバックを共有してください。
* 複数のブランドアセットをアップロードできますが、特定の生成に利用できるのは 1 つだけです。

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="メール生成" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>AI アシスタントを使用したメールの生成</strong></a>
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
<img alt="プッシュの生成" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-push.md"><strong>AI アシスタントを使用したプッシュ通知の生成</strong></a>
</div>
<p></td>
</tr></table>
