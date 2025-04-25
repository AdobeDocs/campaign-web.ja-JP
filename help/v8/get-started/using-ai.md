---
title: Campaign web での AI を活用したコンテキストヘルプの使用
description: Campaign web ヘルプのポップオーバーで質問する
badge: label="ベータ版"
hide: true
hidefromtoc: true
exl-id: 577f4652-b3e5-4fa1-9a98-91815fe92d83
source-git-commit: b2de0d0061e5c2b582c3e73ccaf2dab1490cc854
workflow-type: ht
source-wordcount: '508'
ht-degree: 100%

---

# AI を活用したコンテキストヘルプ {#using-ai}

Q&amp;A AI を活用したコンテキストヘルプを製品のコンテキストヘルプボックスで使用し、製品ドキュメントと現在の製品コンテキストに基づいて、AI が生成した回答を迅速に取得できます。

**生成 AI を活用したコンテキストヘルプ**&#x200B;がコンテキストヘルプに組み込まれており、膨大なドキュメントリポジトリを簡単に検索して、必要な正確な情報を即座に特定できるので、ドキュメントの検索や、操作方法に関する質問への回答に革新をもたらします。

Campaign 生成 AI の機能を活用したこのコンポーネントは、ユーザーのエクスペリエンスを向上させ、情報の取得と問題解決を簡素化します。複雑なタスクでガイダンスを求めている場合でも、膨大なドキュメントから必要な情報を探している場合でも、AI を活用したコンテキストヘルプは究極のコンパニオンとして、あらゆるインタラクションにおいて比類のない効率性と正確さを提供します。

<!--
[Animation showing AI-powered contextual help in action](assets/do-not-localize/CH+AI-BETA.gif)-->

>[!AVAILABILITY]
>
>* AI を活用したコンテキストヘルプは、ベータ版で使用でき、予告なく変更される場合があります。
>
>* この機能は、**英語**&#x200B;でのみ使用できます。このバージョンでは、他の言語はサポートされていません。そのため、この機能を使用する前に、[優先言語](connect-to-campaign.md#language-pref)が英語に設定されています。
>
>* AI を活用したコンテキストヘルプは、現時点では Campaign E メールデザイナーでは使用できません。

<!--
## Consent {#consent-ai}

Campaign knowledge assistant embedded in the contextual help boxes uses AI. Your use of this capability constitutes consent that the information you provide in your session will be collected, used, disclosed, and retained by Adobe in accordance with the terms of Adobe's Customer Feedback Program. Please do not provide any personal information about yourself or other parties (including your name or contact information) in the knowledge assistant.

## Privacy {#privacy-ai}

Your data is encrypted and private following our standard data protection practices. Learn more about [Adobe Privacy Policies](https://www.adobe.com/privacy/policy.html){target="_blank"}.

The knowledge assistant AI capability does not use your data to train our models. We do not allow any partners or third parties to use your data for training their models or any other purpose.

For information specific to Adobe AI policies in Experience Cloud apps and solutions, refer to [this page](https://business.adobe.com/products/sensei/adobe-sensei.html){target="_blank"}.
-->

## 推奨される質問 {#questions-ai}

入力フィールドから、Adobe Campaign AI を活用したコンテキストヘルプにより、3 つの質問候補が表示されます。これらの質問は AI によって生成され、ヘルプボックスに関連し、現在の製品コンテキストと一致しています。質問を選択すると回答が得られます。

[コンテキストヘルプの質問候補の例](assets/do-not-localize/suggested-questions.png){width="600" align="left"}{zoomable="yes"}

## 回答 {#answers-ai}

Adobe Campaign の AI を活用したコンテキストヘルプはサポートを提供しますが、ユーザーは事実を確認する必要があります。AI により、誤った情報や不正確な情報、誤解を招きかねない情報が出力される場合があります。すべてのヘルプボックスでリンクされている製品ドキュメントを必ず確認してください。

ヘルプポップオーバーの下部にある&#x200B;**コピー**&#x200B;アイコンを使用して、回答をクリップボードにコピーします。

[コンテキストヘルプで回答をコピーする例](assets/do-not-localize/copy-answer.png){width="600" align="left"}{zoomable="yes"}

## フィードバック {#feedback-ai}

時間が経つにつれて人工知能および機械学習モデルが改善され、特定のユースケースに適切に対応できるようになります。Campaign の AI を活用したコンテキストヘルプは、引き続き改善を行います。  <img src="assets/do-not-localize/thumb.png" width="10%"/> ボタンを使用してアドビのエンジニアに通知することを強くお勧めします。

## 推奨事項 {#recommendations-ai}

AI を活用したコンテキストヘルプで質問する場合、現在の製品のコンテキスト（現在の画面）と現在のヘルプボックスの内容が考慮されます。

そのため、ユーザーインターフェイスのコンテキストに関連する質問をすることがベストプラクティスです。例えば、ワークフローでプッシュ配信を送信する方法についての情報が必要な場合は、**ワークフロー**&#x200B;の左のメニューエントリを選択し、その特定のコンテキストでコンテキストヘルプボックスを使用します。レポート指標について詳しくは、キャンペーンまたは配信レポートを参照して、そこから始めます。

AI を活用したコンテキストヘルプのメリットを最大限に利用するには、次の推奨事項に従ってください。

* 質問を正確で具体的に記述し、曖昧さを避けます。正確な回答は、明確な質問によって異なります。
* AI を活用したコンテキストヘルプで正しい情報を見つけるのに役立つ、学習しようとしている内容に関する詳細な情報を提供します。
* 回答の精度を向上させるために、質問を言い換えたり絞り込んだりします。回答が役に立たない場合は、別のアプローチを試し、コンテキストを追加します。
* 中立的な語調で適切な用語と表現を使用します。
* 回答を評価し、エンジニアが結果を改善するのに役立つフィードバックを提供します。