---
title: Campaign web での AI を活用したコンテキストヘルプの使用
description: Campaign web ヘルプのポップオーバーで質問する
badge: label="ベータ版"
hide: true
hidefromtoc: true
exl-id: 577f4652-b3e5-4fa1-9a98-91815fe92d83
source-git-commit: b2de0d0061e5c2b582c3e73ccaf2dab1490cc854
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 14%

---

# AI を活用したコンテキストヘルプ {#using-ai}

製品コンテキストヘルプボックスで使用できる Q&amp;A AI を利用したコンテキストヘルプを使用して、製品ドキュメントと現在の製品コンテキストに基づいて、AI が生成した回答をすばやく取得します。

**Gen AI を使用したコンテキストヘルプ** は、コンテキストヘルプに組み込まれており、膨大なドキュメントリポジトリを簡単に調べて、必要な正確な情報を即座に特定することで、ドキュメントの検索とハウツー質問への回答に革命をもたらします。

Campaign Gen AI の機能により、このコンポーネントはエクスペリエンスを強化し、情報の取得と問題解決を簡単にします。 複雑なタスクのガイダンスを求める場合でも、大量のドキュメントをナビゲートする場合でも、AI を活用したコンテキストヘルプは、あらゆるインタラクションで比類のない効率と精度を提供する究極のコンパニオンとして機能します。

<!--
[Animation showing AI-powered contextual help in action](assets/do-not-localize/CH+AI-BETA.gif)-->

>[!AVAILABILITY]
>
>* AI を利用したコンテキストヘルプは、Beta版で利用でき、予告なく変更される場合があります。
>
>* この機能は、**英語**&#x200B;でのみ使用できます。このバージョンでは、他の言語はサポートされていません。その結果、この機能を使用する前に [ 優先言語 ](connect-to-campaign.md#language-pref) が英語に設定されていることを確認します。
>
>* 現時点では、AI を活用したコンテキストヘルプは Campaign メールDesignerでは使用できません。

<!--
## Consent {#consent-ai}

Campaign knowledge assistant embedded in the contextual help boxes uses AI. Your use of this capability constitutes consent that the information you provide in your session will be collected, used, disclosed, and retained by Adobe in accordance with the terms of Adobe's Customer Feedback Program. Please do not provide any personal information about yourself or other parties (including your name or contact information) in the knowledge assistant.

## Privacy {#privacy-ai}

Your data is encrypted and private following our standard data protection practices. Learn more about [Adobe Privacy Policies](https://www.adobe.com/privacy/policy.html){target="_blank"}.

The knowledge assistant AI capability does not use your data to train our models. We do not allow any partners or third parties to use your data for training their models or any other purpose.

For information specific to Adobe AI policies in Experience Cloud apps and solutions, refer to [this page](https://business.adobe.com/products/sensei/adobe-sensei.html){target="_blank"}.
-->

## 推奨される質問 {#questions-ai}

入力フィールドから、Adobe Campaign AI を活用したコンテキストヘルプが 3 つの提案された質問を提供します。 これらの質問は AI によって生成され、ヘルプボックスに関連し、現在の製品コンテキストに合わせられます。 質問を選択すると回答が得られます。

[ コンテキストヘルプで提案される質問の例 ](assets/do-not-localize/suggested-questions.png){width="600" align="left"}{zoomable="yes"}

## 回答 {#answers-ai}

Adobe Campaign の AI を活用したコンテキストヘルプはサポートを提供しますが、ユーザーは事実を確認する必要があります。誤った、不正確、または誤解を招く情報が出力される場合があります。 すべてのヘルプボックスにリンクされている製品ドキュメントを必ず確認してください。

ヘルプポップオーバーの下部にある **コピー** アイコンを使用して、回答をクリップボードにコピーします。

[ コンテキストヘルプで回答をコピーする例 ](assets/do-not-localize/copy-answer.png){width="600" align="left"}{zoomable="yes"}

## フィードバック {#feedback-ai}

時間が経つにつれて人工知能および機械学習モデルが改善され、特定のユースケースに適切に対応できるようになります。Campaign AI を活用したコンテキストヘルプは、引き続き改善されます。 の使用 当社のエンジニアに対して不適切な回答にフラグを立てるために、回答を読むたびにボタンを <img src="assets/do-not-localize/thumb.png" width="10%"/> きます。

## 推奨事項 {#recommendations-ai}

AI を利用したコンテキストヘルプで質問するときは、現在の画面や現在のヘルプボックスの内容など、現在の製品のコンテキストが考慮されます。

そのため、ベストプラクティスはユーザーインターフェイスのコンテキストに関する質問をすることです。 例えば、ワークフローでのプッシュ配信の送信方法を学習する必要がある場合、左側のメニューエントリ **ワークフロー** を参照し、その特定のコンテキストでコンテキストヘルプボックスを使用します。 レポート指標の詳細については、キャンペーンまたは配信レポートを参照し、そこから開始します。

AI を利用したコンテキストヘルプのメリットを最大化するには、次の推奨事項に従います。

* 曖昧さを避け、正確で具体的であること。 正確な回答は、明確な質問によって異なります。
* AI を活用したコンテキストヘルプで正しい情報を見つけるのに役立つ、学びようとしている内容に関する詳細情報を提供します。
* 質問のフレーズを変更して絞り込み、回答の精度を向上させます。 答えが役に立たない場合は、別のアプローチを試してコンテキストを追加します。
* ニュートラルなトーンで適切な用語と表現を使用します。
* 回答を評価し、エンジニアが結果を改善するのに役立つフィードバックを提供します。