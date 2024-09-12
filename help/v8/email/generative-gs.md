---
audience: end-user
title: AI アシスタント コンテンツ アクセラレータの基本を学ぶ
description: AI アシスタント コンテンツ アクセラレータの基本を学ぶ
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
source-git-commit: 9d32344b5ee378588cedb003b80daac04ac3a26c
workflow-type: tm+mt
source-wordcount: '840'
ht-degree: 57%

---

# AI アシスタント コンテンツ アクセラレータを使用する  {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="AI アシスタント コンテンツ アクセラレータ"
>abstract="AI アシスタントを使用すると、メール、SMS、プッシュなどすべてのチャネルでマーケティングキャンペーンを、直感的でシンプルかつ手間のかからない方法で作成および実行でき、時間を節約し、効率を向上させ、より良い結果を導き出すことができます。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=ja" text="リリースノートを参照してください"


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
>abstract="この機能へアクセスするには、Adobe Experience Cloud 生成 AI ユーザーガイドラインへの同意が必要です。この機能からの出力が正確であるかどうかを見直し、ユースケースに適していることを確認してください。"
>additional-url="https://www.adobe.com/jp/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe 生成 AI ユーザーガイドライン"

>[!INFO]
>
>機能を直接探索して機能を完全に理解できるように設計された [ ライブ機能プレビュー ](https://experienceleague.adobe.com/en/apps/journey-optimizer/ai-assistant-content-accelerator) を使用して、実践的な体験に浸ってください。


マーケティング業界の競争が激化する中、ブランドは効果的なコンテンツを効率的かつ迅速に生成する効率的な方法を模索しています。Microsoft Azure OpenAI とAdobe Fireflyを活用した、Adobe Campaign Web のコンテンツアクセラレーション向け AI アシスタントは、マーケターがメール、SMS、プッシュなど、あらゆるチャネルで、プロフェッショナルでブランドに一貫したコンテンツを作成する方法に革命を起こす、Adobeの AI コンテンツ作成機能です。 高度な 生成 AI モデルとブランドガイドラインの深い理解により、AI アシスタントは、ブランドの概要を示したスタイル、レイアウト、トーンなどに最適化されたコンテンツを使用して、マーケティング目的に基づいてパーソナライズされた魅力的で効果的なコンテンツを自動生成します。

AI アシスタントを使用すると、メール、SMS、プッシュなどすべてのチャネルでマーケティングキャンペーンを、直感的でシンプルかつ手間のかからない方法で作成および実行でき、時間を節約し、効率を向上させ、より良い結果を導き出すことができます。

>[!IMPORTANT]
>
>* この機能の使用を開始する前に、関連する[ガードレールと制限](#generative-guardrails)のトピックに目を通してください。
>
>* コンテンツアクセラレーションのためにAdobe Campaign Web で AI アシスタントを使用するには、[ ユーザー使用許諾契約 ](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) に同意する必要があります。 詳しくは、アドビ担当者にお問い合わせください。

## AI Assistant コンテンツ アクセラレータにアクセスする {#generative-access}

メール、プッシュ通知、SMS 用の AI Assistant コンテンツアクセラレーターが一般提供（GA）になり、すべてのユーザーが利用できるようになりました。 ユーザーにアクセス権を付与するために必要な権限と手順について、以下で詳しく説明します。

+++  コンテンツ生成関連の権限を割り当てる方法を学ぶ

1. **製品プロファイルの作成** - [Admin Consoleで ](https://stage.adminconsole.adobe.com/) 次のパターンの製品プロファイルを作成します。
   `Campaign - <instance-name> - AIAssistant`

1. **ユーザーを追加** – 必要なユーザーをその製品プロファイルに追加します。
または
   **ユーザーグループを作成** し、そのユーザーグループを製品プロファイルに追加して、その製品プロファイルにユーザーを追加します。

Campaign で権限を定義する方法については、[ この節 ](../get-started/permissions.md) を参照してください。

+++

## ガードレールと制限 {#generative-guardrails}

メール生成のためのコンテンツアクセラレーションについて、Adobe Campaign Web で AI アシスタントを使用する際の一般的なガイドラインを以下に示します。

* 生成されるコンテンツの品質は、定義したマーケティング目的やプロンプトに大きく左右されます。生成 AI モデルで正確に解釈できるように、適切に定義されたプロンプトを使用します。 
* ブランドアセットをアップロードして、正確なオンブランドコンテンツを確保します。それ以外の場合は、公開されている情報に基づいたコンテンツになります。アップロードされるコンテンツは、PDF、JPEG、PNG または ZIP ファイル（サポートされているファイル形式のもの）の形式です。
* アップロードされたブランドアセットの最大サイズは 50MB です。これより大きなファイルや多数の画像の場合でも動作しますが、処理時間が長くなります。
* [ 組み込みのメールテンプレート ](../email/create-email-templates.md)、ブランド固有のテンプレートまたはカスタムテンプレートを使用して、コンテンツアクセラレーターを使用してメールコンテンツを作成します。 最大 8～10 個の画像を含むメールテンプレートを使用することをお勧めします。
* バリアントを選択する際は、サムアップ、サムダウンまたはフラグのアイコンを使用して、問題のある出力を報告してください。
* AI アシスタントの使用は、Adobe Experience Cloud 生成 AI ユーザーガイドラインの対象となります。[詳細情報](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html)
* メディア制作における生成 AI ツールの使用に関する透明性を高めるためのAdobeの取り組みの一環として、Adobeは、Firefly生成アセットを含むコンテンツまたはプロジェクトがダウンロードまたは書き出されたときにContent credentialsを適用します。 [詳細情報](https://helpx.adobe.com/firefly/using/content-credentials.html)

コンテンツアクセラレーションに関するAdobe Campaign Web の AI アシスタントには次の制限が適用されます。

* コンテンツアクセラレーション用Adobe Campaign Web の AI アシスタントは、現在、英語でのみサポートされています。 英語以外の入力では、一貫性のない結果や誤った結果が生じる場合があります。 英語以外の回答に起因する問題は、現時点では解決または改善されません。
* メール、プッシュ、SMS の各チャネルにのみ使用できます。
* 生成 AI のコンテンツは必ずしも正確でない場合があります。エンジニアがモデルを改善できるように、フィードバックを共有してください。
* 複数のブランドアセットをアップロードできますが、特定の生成に利用できるのは 1 つだけです。

## AI アシスタントのコンテンツ生成機能 {#generative-features}

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
