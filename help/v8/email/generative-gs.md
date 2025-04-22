---
audience: end-user
title: AI アシスタントの基本を学ぶ
description: AI アシスタントの基本を学ぶ
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
source-git-commit: 5f7fe214c1c89b1ee25cea6d512bd1a55b5522ec
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 18%

---

# AI アシスタントを使用する {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="AI アシスタント"
>abstract="配信を作成およびパーソナライズした後、AI アシスタントを使用してコンテンツを強化します。 この機能を使用すると、生成対象を説明することでコンテンツを微調整できるので、パーソナライゼーションとコンテンツの改善を簡略化できます。"

>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Campaign で AI アシスタントを使用してコンテキストを定義"
>abstract="選択したコンテンツをコンテンツ生成の入力として使用するには、「**現在のコンテンツで拡張** 切替スイッチをアクティブにします。 また、ブランドアセットをアップロードして、ソースとして使用することもできます。選択したコンテンツを使用しない場合、ブランドアセットのアップロードと選択は必須です。"

>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Adobe 生成 AI の用語"
>abstract="この機能へのアクセスは、Adobe Experience Cloud ジェネレーティブ AI ユーザーガイドラインへの同意によって異なります。 この機能から出力される精度をレビューし、ユースケースに適していることを確認します。"
>additional-url="https://www.adobe.com/jp/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe 生成 AI ユーザーガイドライン"

>[!INFO]
>
>[ライブ機能プレビュー](https://experienceleague.adobe.com/ja/apps/journey-optimizer/ai-assistant-content-accelerator)では、実際に体験して、その機能を直接探索し、その機能を完全に理解できるように設計されています。

マーケティング業界の競争力が高まるにつれて、ブランドは効果的なコンテンツを迅速に生成する効率的な方法を模索しています。 Microsoft Azure OpenAI とAdobe Fireflyを活用した、Adobe Campaign Web の AI アシスタントは、Adobeの AI コンテンツ生成機能です。この機能により、マーケターがメール、SMS、プッシュ通知などのチャネルをまたいで、プロフェッショナルでブランドと一貫したコンテンツを作成する方法が変わります。 高度な GenAI モデルとブランドガイドラインの深い理解により、AI アシスタントは、マーケティング目標に基づいてパーソナライズされた魅力的で効果的なコンテンツを自動生成し、ブランドの概要を説明したスタイル、レイアウト、トーンなどに合わせてコンテンツを最適化します。

AI アシスタントは、メール、SMS、プッシュ通知などのチャネルをまたいでマーケティングキャンペーンの作成と実行を簡素化し、時間を節約し、効率を向上させ、より良い結果を導きます。

>[!IMPORTANT]
>
>* この機能を使用する前に、関連する [ ガードレールと制限 ](#generative-guardrails) を確認してください。
>
>* Adobe Campaign Web で AI アシスタントを使用するには、[ ユーザー使用許諾契約 ](https://www.adobe.com/jp/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) に同意する必要があります。 詳しくは、アドビ担当者にお問い合わせください。

## AI アシスタントにアクセス {#generative-access}

メール、プッシュ通知、SMS 用の AI アシスタントが一般提供（GA）になり、すべてのユーザーが使用できるようになりました。 ユーザーにアクセス権を付与するのに必要な権限と手順について詳しくは、以下を参照してください。

+++ コンテンツ生成関連の権限を割り当てる方法を学ぶ

1. **製品プロファイルの作成** - [Admin Console](https://stage.adminconsole.adobe.com/) で、次のパターンに沿って製品プロファイルを作成します。
   `Campaign - <instance-name> - AIAssistant`

1. **ユーザーを追加** – 必要なユーザーをその製品プロファイルに追加します。\
   または\
   **ユーザーグループを作成** し、そのユーザーグループを製品プロファイルに追加してから、その製品プロファイルにユーザーを追加します。

Campaign で権限を定義する方法について詳しくは、[この節](../get-started/permissions.md)を参照してください。

+++

## ガードレールと制限 {#generative-guardrails}

メール生成にAdobe Campaign Web で AI アシスタントを使用する際の一般的なガイドラインを以下に示します。

* 生成されるコンテンツの品質は、定義したマーケティング目的やプロンプトによって大きく異なります。 GenAI モデルを正確に解釈するには、明確に定義されたプロンプトを使用します。
* ブランドアセットをアップロードして、ブランド上の正確なコンテンツを確保する。 それ以外の場合、コンテンツは、公開されている情報に基づいています。 アップロードされるコンテンツの形式は、PDF、JPEG、PNG、ZIP ファイル（サポートされているファイル形式）のいずれかです。
* アップロードされるブランドアセットの最大サイズは 50 MB です。 ファイルのサイズが大きい場合や画像の数が多い場合は、処理時間が長くなる可能性があります。
* [ 組み込みのメールテンプレート ](../email/create-email-templates.md)、ブランド固有のテンプレート、またはカスタムテンプレートを使用して、AI アシスタントを使用してメールコンテンツを作成します。 最大 8～10 個の画像を使用するメールテンプレートを推奨します。
* バリアントを選択する際に、サムズアップ、サムズダウンまたはフラグのアイコンを使用して、問題のある出力を報告します。
* AI アシスタントの使用には、Adobe Experience Cloud ジェネレーティブ AI ユーザーガイドラインが適用されます。 [詳細情報](https://www.adobe.com/jp/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html)。
* Fireflyは、メディア作成で生成 AI ツールを使用する際の透明性に対するAdobeの取り組みの一環として、Adobeで生成されたアセットを含むコンテンツやプロジェクトがダウンロードまたは書き出される際に、Content Credentialsを適用します。 [詳細情報](https://helpx.adobe.com/jp/firefly/using/content-credentials.html)。

Adobe Campaign web の AI アシスタントには、次の制限が適用されます。

* Adobe Campaign web の AI アシスタントは、現在、英語でのみサポートされています。英語以外の入力では、一貫性のない結果や誤った結果が生じる場合があります。現時点では、英語以外の回答に起因する問題は解決または改善されません。
* メール、プッシュ、SMS チャネルでのみ使用できます。
* GenAI コンテンツは常に正確とは限りません。 フィードバックを共有して、エンジニアがモデルを調整できるようにします。
* 複数のブランドアセットをアップロードできますが、特定の世代に利用できるのは 1 つのみです。

## AI アシスタントコンテンツ生成機能 {#generative-features}

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="[AI アシスタントによるメール生成 ]" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>AI アシスタントによるメール生成 </strong></a>
</div>
<p>
</td>
<td>
<a href="generative-sms.md">
<img alt="[AI アシスタントによる SMS 生成 ]" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-sms.md"><strong>AI アシスタントによる SMS 生成 </strong>
</div>
<p>
</td>
<td>
<a href="generative-push.md">
<img alt="[AI アシスタントによるプッシュ通知の生成 ]" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-push.md"><strong>AI アシスタントによるプッシュ通知の生成 </strong></a>
</div>
<p></td>
</tr></table>