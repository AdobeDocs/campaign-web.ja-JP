---
audience: end-user
title: コンテンツアシスタントの基本を学ぶ
description: コンテンツアシスタントの基本を学ぶ
badge: label="アルファ版"
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
source-git-commit: bc1b4186b5869d104c6b14e09160f28bf3e28f95
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 99%

---

# コンテンツアシスタントの基本を学ぶ {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_homepage_rn5"
>title="メールコンテンツ用生成 AI"
>abstract="アドビの生成 AI テクノロジーは、高度なアルゴリズムを利用して、非常に魅力的でパーソナライズされたコンテンツを生成します。生成 AI のインテリジェントなコンテンツ生成により、開封率、クリックスルー率、コンバージョン率の向上を推進します。競合他社に先んじて、メールコンテンツに対する生成 AI を使用してメールマーケティングゲームを向上させます。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html" text="リリースノートを参照"



>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="コンテンツアシスタント"
>abstract="配信を作成しパーソナライズしたら、コンテンツアシスタントを使用してコンテンツを強化できます。この機能を使用すると、生成する内容を記述してコンテンツを微調整できるので、パーソナライゼーションとコンテンツ改善のプロセスが簡素化されます。"


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="コンテンツ生成のコンテキストの定義"
>abstract="選択したコンテンツをコンテンツ生成の入力として使用するには、「**現在のコンテンツを使用して強化**」切替スイッチをオンにします。また、ブランドアセットをアップロードして、ソースとして使用することもできます。選択したコンテンツを使用しない場合は、ブランドアセットのアップロードと選択が必須です。"

コンテンツアシスタントは、生成 AI を活用したツールで、メールコンテンツの改善に役立ちます。パーソナライゼーションとコンテンツ強化が簡素化され、メール配信を最適化してオーディエンスの共感を深めることができます。

この機能を利用すると、完全なメールコンテンツが自動的に生成されるので、時間を節約し一貫した品質を確保できます。生成 AI を使用すると、魅力的なメールを簡単に作成して、コミュニケーションの効果と効率を高めることができます。


メールで Campaign コンテンツアシスタントを使用して、[画像の生成](generative-image.md)、[テキストコンテンツの生成](generative-content.md)、[完全な HTML コンテンツの生成](generative-email.md)を行えます。

>[!NOTE]
>
>この機能はアルファ版で使用でき、予告なく変更される場合があります。10 月初旬にはアクティブ化されます。

## ガードレールと制限 {#generative-guardrails}

メールの生成にコンテンツアシスタントを使用する際の一般的なガイドラインは次のとおりです。

* 生成されるコンテンツの品質は、定義したマーケティング目的やプロンプトに大きく左右されます。生成 AI モデルで正確に解釈できるように、適切に定義されたプロンプトを使用します。 
* ブランドアセットをアップロードして、正確なオンブランドコンテンツを確保します。それ以外の場合は、公開されている情報に基づいたコンテンツになります。アップロードされるコンテンツは、PDF、JPEG、PNG または ZIP ファイル（サポートされているファイル形式のもの）の形式です。
* アップロードされたブランドアセットの推奨サイズは 10 MB 未満です。これより大きなファイルや多数の画像の場合でも動作しますが、処理時間が長くなります。
* Adobe Campaign で作成したメールテンプレートを使用するか、できれば[組み込みのメールテンプレート](../content/email-sample-templates.md)を使用して、メールコンテンツを作成します。最大 8～10 個の画像を含むメールテンプレートをお勧めします。


Campaign コンテンツアシスタントには、次の制限が適用されます。

* サポートされている言語は英語のみです
* メールチャネルにのみ使用できます
* 生成 AI のコンテンツは必ずしも正確でない場合があります。エンジニアがモデルを改善できるように、フィードバックを共有してください
* 複数のブランドアセットをアップロードできますが、特定の生成に利用できるのは 1 つだけです



<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="テキスト生成" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>コンテンツアシスタントを使用したテキスト生成</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-image.md">
<img alt="画像生成" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-image.md"><strong>コンテンツアシスタントを使用した画像生成</strong>
</div>
<p>
</td>
<td>
<a href="generative-email.md">
<img alt="メール生成" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-email.md"><strong>コンテンツアシスタントを使用したメール生成</strong></a>
</div>
<p></td>
</tr></table>
