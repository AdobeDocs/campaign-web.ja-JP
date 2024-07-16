---
audience: end-user
title: AI アシスタントの基本を学ぶ
description: AI アシスタントの基本を学ぶ
badge: label="Beta"
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
hide: true
hidefromtoc: true
source-git-commit: 7de6d85036eac7289e7fcf3a82a7c11be12d9c6e
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 91%

---

# AI アシスタントの基本を学ぶ {#generative-gs}

>[!BEGINSHADEBOX]

**目次**

* AI アシスタントの基本を学ぶ
* [AI アシスタントを使用したメールの生成](generative-content.md)
* [AI アシスタントを使用した SMS の生成](generative-sms.md)
* [AI アシスタントを使用したプッシュ通知の生成](generative-push.md)

>[!ENDSHADEBOX]

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="AI アシスタント"
>abstract="配信を作成しパーソナライズしたら、AI アシスタントを使用してコンテンツを強化できます。 この機能を使用すると、生成する内容を記述してコンテンツを微調整できるので、パーソナライゼーションとコンテンツ改善のプロセスが簡素化されます。"


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Campaign で AI アシスタントを使用してコンテキストを定義"
>abstract="選択したコンテンツをコンテンツ生成の入力として使用するには、「**現在のコンテンツを使用して強化**」切替スイッチをオンにします。また、ブランドアセットをアップロードして、ソースとして使用することもできます。選択したコンテンツを使用しない場合は、ブランドアセットのアップロードと選択が必須です。"


>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Adobe 生成 AI の用語"
>abstract="この機能へアクセスするには、Adobe Experience Cloud 生成 AI ユーザーガイドラインへの同意が必要です。この機能からの出力が正確かどうかを確認し、ユースケースに適していることを確認してください。"
>additional-url="https://www.adobe.com/jp/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe 生成 AI ユーザーガイドライン"

マーケティング業界の競争が激化する中、ブランドは効果的なコンテンツを効率的かつ迅速に生成する効率的な方法を模索しています。Azure OpenAI を活用した Campaign の AI アシスタントは、マーケターがメール、SMS、プッシュなど、あらゆるチャネルで、プロフェッショナルでブランドに一貫性のあるコンテンツを作成する方法に革命を起こす、Adobeの AI コンテンツ生成機能です。 高度な 生成 AI モデルとブランドガイドラインの深い理解により、AI アシスタントは、ブランドの概要を示したスタイル、レイアウト、トーンなどに最適化されたコンテンツを使用して、マーケティング目的に基づいてパーソナライズされた魅力的で効果的なコンテンツを自動生成します。

AI アシスタントを使用すると、メール、SMS、プッシュなどすべてのチャネルでマーケティングキャンペーンを、直感的でシンプルかつ手間のかからない方法で作成および実行でき、時間を節約し、効率を向上させ、より良い結果を導き出すことができます。

>[!NOTE]
>
>この機能は、ベータ版で使用でき、予告なく変更される場合があります。

## ガードレールと制限 {#generative-guardrails}

メールの生成に Campaign の AI アシスタントを使用する際の一般的なガイドラインは次のとおりです。

* 生成されるコンテンツの品質は、定義したマーケティング目的やプロンプトに大きく左右されます。生成 AI モデルで正確に解釈できるように、適切に定義されたプロンプトを使用します。 
* ブランドアセットをアップロードして、正確なオンブランドコンテンツを確保します。それ以外の場合は、公開されている情報に基づいたコンテンツになります。アップロードされるコンテンツは、PDF、JPEG、PNG または ZIP ファイル（サポートされているファイル形式のもの）の形式です。
* アップロードされたブランドアセットの最大サイズは 50MB です。これより大きなファイルや多数の画像の場合でも動作しますが、処理時間が長くなります。
* Adobe Campaign で作成したメールテンプレートを使用するか、できれば[組み込みのメールテンプレート](../email/create-email-templates.md)、ブランド固有のテンプレートまたはカスタムテンプレートを使用して、メールコンテンツを作成します。最大 8～10 個の画像を含むメールテンプレートをお勧めします。
* バリアントを選択する際は、サムアップ、サムダウンまたはフラグのアイコンを使用して、問題のある出力を報告してください。
* AI アシスタントの使用は、Adobe Experience Cloud 生成 AI ユーザーガイドラインの対象となります。[詳細情報](https://www.adobe.com/jp/legal/licenses-terms/adobe-gen-ai-user-guidelines.html)

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
