---
audience: end-user
title: AI アシスタントの基本を学ぶ
description: AI アシスタントの基本を学ぶ
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
source-git-commit: 5f7fe214c1c89b1ee25cea6d512bd1a55b5522ec
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 100%

---

# AI アシスタントの操作 {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="AI アシスタント"
>abstract="配信を作成してパーソナライズしたら、AI アシスタントを使用してコンテンツを強化します。この機能を使用すると、生成する内容を記述してコンテンツを微調整できるので、パーソナライゼーションとコンテンツ改善が簡素化されます。"

>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Campaign で AI アシスタントを使用してコンテキストを定義"
>abstract="選択したコンテンツをコンテンツ生成の入力として使用するには、「**現在のコンテンツを使用して強化**」切替スイッチをオンにします。また、ブランドアセットをアップロードして、ソースとして使用することもできます。選択したコンテンツを使用しない場合は、ブランドアセットのアップロードと選択が必須です。"

>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Adobe 生成 AI の用語"
>abstract="この機能へアクセスするには、Adobe Experience Cloud 生成 AI ユーザーガイドラインへの同意が必要です。この機能からの出力が正確であるかどうかを見直し、ユースケースに適していることを確認します。"
>additional-url="https://www.adobe.com/jp/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe 生成 AI ユーザーガイドライン"

>[!INFO]
>
>[ライブ機能プレビュー](https://experienceleague.adobe.com/ja/apps/journey-optimizer/ai-assistant-content-accelerator)では、実際に体験して、その機能を直接探索し、その機能を完全に理解できるように設計されています。

マーケティング業界の競争が激化する中、ブランドは、影響力のあるコンテンツを迅速に生成する効率的な方法を模索しています。Microsoft Azure OpenAI と Adobe Firefly を活用した Adobe Campaign web の AI アシスタントは、アドビの AI コンテンツ生成機能です。メール、SMS、プッシュ通知など、あらゆるチャネルで、マーケターがプロフェッショナルでブランドに即したコンテンツの作成方法を変革します。高度な 生成 AI モデルを用い、ブランドガイドラインを深く理解している AI アシスタントは、ブランドの概要を示したスタイル、レイアウト、トーンなどに合わせてコンテンツを最適化し、マーケティング目標に基づいてパーソナライズされた魅力的かつ効果的なコンテンツを自動生成します。

AI アシスタントを使用すると、メール、SMS、プッシュ通知などすべてのチャネルでのマーケティングキャンペーンの作成と実行が簡素化され、時間を節約し、効率を向上させ、より良い結果を導き出すことができます。

>[!IMPORTANT]
>
>* この機能を使用する前に、関連する[ガードレールと制限](#generative-guardrails)を参照してください。
>
>* Adobe Campaign web の AI アシスタントを使用する前に、[ユーザー契約](https://www.adobe.com/jp/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html)に同意する必要があります。詳しくは、アドビ担当者にお問い合わせください。

## AI アシスタントへのアクセス {#generative-access}

メール、プッシュ通知、SMS 用の AI アシスタントが一般公開（GA）になり、すべてのユーザーが使用できるようになりました。ユーザーにアクセス権を付与するのに必要な権限と手順について詳しくは、以下を参照してください。

+++ コンテンツ生成関連の権限を割り当てる方法について説明します。

1. **製品プロファイルを作成** - [Admin Console](https://stage.adminconsole.adobe.com/) で、次の特定のパターンを使用して製品プロファイルを作成します。
   `Campaign - <instance-name> - AIAssistant`

1. **ユーザーを追加** - 必要なユーザーをその製品プロファイルに追加します。\
   または\
   **ユーザーグループを作成**&#x200B;し、そのユーザーグループを製品プロファイルに追加して、その製品プロファイルにユーザーを追加します。

Campaign で権限を定義する方法について詳しくは、[この節](../get-started/permissions.md)を参照してください。

+++

## ガードレールと制限 {#generative-guardrails}

メールの生成に Adobe Campaign web の AI アシスタントを使用する際の一般的なガイドラインは次のとおりです。

* 生成されるコンテンツの品質は、定義したマーケティング目的やプロンプトに大きく依存します。生成 AI モデルで正確に解釈できるように、適切に定義されたプロンプトを使用します。
* ブランドアセットをアップロードして、正確なオンブランドコンテンツを確保します。それ以外の場合は、公開されている情報に基づいたコンテンツになります。アップロードされるコンテンツは、PDF、JPEG、PNG または ZIP ファイル（サポートされているファイル形式のもの）の形式です。
* アップロードされたブランドアセットの最大サイズは 50MB です。これより大きなファイルや多数の画像の場合は、処理時間が長くなることがあります。
* [ビルトインのメールテンプレート](../email/create-email-templates.md)、ブランド固有のテンプレートまたはカスタムテンプレートを使用して、AI アシスタントでメールコンテンツを作成します。最大 8～10 個の画像を含むメールテンプレートをお勧めします。
* バリアントを選択する際は、親指を立てる、親指を下げるまたはフラグのアイコンを使用して、問題のある出力を報告します。
* AI アシスタントの使用は、Adobe Experience Cloud 生成 AI ユーザーガイドラインの対象となります。[詳細情報](https://www.adobe.com/jp/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html)。
* メディア作成における生成 AI ツールの使用の透明性に対するアドビの取り組みの一環として、アドビでは、Firefly で生成されたアセットを含むコンテンツまたはプロジェクトがダウンロードまたはエクスポートされる際に、コンテンツ資格情報を適用します。[詳細情報](https://helpx.adobe.com/jp/firefly/using/content-credentials.html)。

Adobe Campaign web の AI アシスタントには、次の制限が適用されます。

* Adobe Campaign web の AI アシスタントは、現在、英語でのみサポートされています。英語以外の入力では、一貫性のない結果や誤った結果が生成される場合があります。英語以外の応答から生じる問題は、現時点では対処または改善されません。
* メール、プッシュ、SMS の各チャネルにのみ使用できます。
* 生成 AI コンテンツは必ずしも正確ではない可能性があります。エンジニアがモデルを改善できるよう、フィードバックを共有してください。
* 複数のブランドアセットをアップロードできますが、特定の生成に利用できるのは 1 つだけです。

## AI アシスタントコンテンツ生成機能 {#generative-features}

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="[AI アシスタントを使用したメールの生成]" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>AI アシスタントを使用したメールの生成</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-sms.md">
<img alt="[AI アシスタントを使用した SMS の生成]" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-sms.md"><strong>AI アシスタントを使用した SMS の生成</strong>
</div>
<p>
</td>
<td>
<a href="generative-push.md">
<img alt="[AI アシスタントを使用したプッシュ通知の生成]" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-push.md"><strong>AI アシスタントを使用したプッシュ通知の生成</strong></a>
</div>
<p></td>
</tr></table>