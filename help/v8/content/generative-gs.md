---
audience: end-user
title: コンテンツアシスタントの基本を学ぶ
description: コンテンツアシスタントの基本を学ぶ
badge: label="Beta"
source-git-commit: 2da9bdab7e8a5050d0e4e0531fc30f85870de70f
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 1%

---


# コンテンツアシスタントの基本を学ぶ {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="コンテンツアシスタント"
>abstract="配信を作成し、パーソナライズしたら、コンテンツアシスタントを使用してコンテンツを拡張できます。 この機能を使用すると、生成する内容を記述してコンテンツを微調整でき、パーソナライゼーションとコンテンツの改善のプロセスを簡素化できます。"


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="コンテンツ生成のコンテキストを定義"
>abstract="選択したコンテンツをコンテンツ生成の入力として使用するには、 **現在のコンテンツで拡張** 切り替え また、ブランドアセットをアップロードして、ソースとして使用することもできます。 選択したコンテンツを使用しない場合は、ブランドアセットのアップロードと選択が必須です。"

Content Assistant は、生成 AI を活用した、E メールコンテンツを改善するための貴重なツールです。 パーソナライゼーションとコンテンツの強化を簡素化し、E メール配信を最適化してオーディエンスの共感を深めます。

この機能により、完全な E メールコンテンツが自動的に生成され、時間を節約し、品質の一貫性を保ちます。 Generative AI を使用すると、魅力的なメールを簡単に作成し、コミュニケーションの効果と効率を高めることができます。

メール内の Campaign コンテンツアシスタントは次の目的で使用できます。 [画像を生成](generative-image.md), [テキストコンテンツを生成](generative-content.md), [完全なHTMLコンテンツを生成](generative-email.md).


## ガードレールと制限 {#generative-guardrails}

E メールの生成にコンテンツアシスタントを使用する際の一般的なガイドラインを次に示します。

* 生成されるコンテンツの品質は、定義したマーケティングの目的やプロンプトの影響を強く受けます。 GenAI モデルを正確に解釈するために、適切に定義されたプロンプトを使用します。 
* ブランドコンテンツに正確なブランドアセットをアップロードする。 それ以外の場合、コンテンツは公開されている情報に基づいています。 アップロードされるコンテンツは、PDFファイル、Microsoft Word ドキュメント、JPEG、PNG または ZIP ファイル（サポートされているファイル形式を含む）です。
* アップロードされたブランドアセットの推奨サイズは 10MB 未満です。 大きなファイルや画像の数が多い場合でも動作しますが、処理時間は長くなります。
* Adobe Campaignで作成した電子メールテンプレートを使用するか、できれば [組み込みの電子メールテンプレート](../content/email-sample-templates.md) 電子メールコンテンツを作成します。 最大 8 ～ 10 個の画像を含む E メールテンプレートをお勧めします。


Campaign コンテンツアシスタントには次の制限が適用されます。

* サポートされている言語は英語のみです
* E メールチャネルでのみ使用できます
* GenAI のコンテンツが正確でない場合があります。エンジニアがモデルを改善できるよう、フィードバックを共有してください。
* 複数のブランドアセットをアップロードできますが、特定の世代に利用できるのは 1 つだけです

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="テキストの生成" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>コンテンツアシスタントを使用したテキスト生成</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-image.md">
<img alt="画像の生成" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-image.md"><strong>コンテンツアシスタントを使用した画像の生成</strong>
</div>
<p>
</td>
<td>
<a href="generative-email.md">
<img alt="E メールの生成" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-email.md"><strong>コンテンツアシスタントを使用した E メールの生成</strong></a>
</div>
<p></td>
</tr></table>

