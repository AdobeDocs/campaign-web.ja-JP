---
title: 動的コンテンツの基本を学ぶ
description: パーソナライゼーション、条件付きコンテンツ、組み込みコンテンツブロックを使用して、コンテンツを動的にする方法を説明します。
audience: automating
content-type: reference
topic-tags: workflow-general-operation
context-tags: workflow,overview;workflow,main
feature: Workflows
role: Data Architect
level: Intermediate
source-git-commit: 323dc9ccb9d04d2d7085a26a17f6944e999b1dec
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 9%

---


# 動的コンテンツの基本を学ぶ

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_dashboard"
>title="パーソナライズ機能"
>abstract="式エディターでは、すべてのデータを選択、整理、カスタマイズおよび検証して、コンテンツに合わせてカスタマイズされたエクスペリエンスを作成できます。 プロファイルデータを活用して、各受信者に対するメッセージをパーソナライズし、条件付きコンテンツを作成して、各受信者にメッセージを適応させ、関連するコンテンツのみを表示できます。 さらに、パーソナライゼーションブロックを使用して、事前に定義されたパーソナライズされたコンテンツを配信に追加できます。"

マーケターは、お客様の製品に真に興味を持つ顧客をターゲットにし、効果的で関連性の高いコンテンツを提供して顧客を惹きつけることが重要です。 発生する様々な受信者の範囲を考えると、異なる人に訴える複数のマーケティングコンテンツを作成するのに時間がかかり、無駄が多くなる可能性があります。 動的コンテンツは、ここで利用できます。

Adobe Campaign web 動的コンテンツ機能を使用すると、収集した受信者に関する情報に基づいてコンテンツをカスタマイズできます。 動的コンテンツを利用することで、マーケティング活動の関連性を高め、不要な製品や不要な製品やサービスのマーケティングを避けることができます。 このアプローチは、コンテンツの魅力を高め、コンテンツが読まれる可能性を高めます。 さらに、コンテンツをパーソナライズして、受信者に機械ではなく人から情報を受け取ったように感じさせることもできます。

## コンテンツを動的にする方法は？

Campaign Web 式エディターで JavaScript 構成要素を挿入することで、メッセージのコンテンツを動的に設定できます。 メッセージの送信時に、次の式がAdobe Campaignによって解釈され、各受信者に正しいコンテンツが配信されます。

* **メッセージをパーソナライズ** 特定の受信者に対して、姓、興味、住所、購入内容などのプロファイルデータを活用します。 受信者、メッセージまたは配信に関連するパーソナライゼーションエディターから、データベースで使用可能な任意のフィールドを選択できます。 これらのパーソナライゼーション属性は、メッセージの件名行や本文に挿入できます。&lt;%= recipient.location.city %> の構文は、受信者の市区町村をコンテンツに挿入します。

  ![](assets/perso-subject-line.png){width="800" align="center"}

* **条件付きコンテンツの作成** ：配信を各受信者に合わせて調整し、顧客に関する既知の情報に基づいて、特定の顧客に関連するコンテンツのみを表示する場合。 これにより、条件に基づいて特定のテキストブロックや画像を表示できます。 例えば、特定のサービスに対する受信者の購読に基づいて E メールバナーを調整します。

  ![](assets/condition-sample.png){width="800" align="center"}

* **パーソナライゼーションブロックを使用** 時間を節約し、再利用が容易なパーソナライズされたコンテンツをメッセージに活用する。 Campaign には、配信に挿入できる特定のレンダリングを含んだ一連のパーソナライゼーションブロックが付属しています。例えば、電子メールメッセージのミラーページにロゴ、挨拶メッセージまたはリンクを追加できます。 コンテンツブロックは、パーソナライゼーションエディターの専用のエントリから使用できます。

  ![](assets/content-blocks.png){width="800" align="center"}

## 式エディターにアクセスする {#access}

Adobe Campaign V8 Web には式エディターが用意されており、すべてのデータを選択、整理、カスタマイズおよび検証して、コンテンツに合わせてカスタマイズされたエクスペリエンスを作成できます。 式エディターは、すべてのチャネルで、 **[!UICONTROL パーソナライゼーションダイアログを開く]** アイコン（件名フィールド、E メールリンク、テキスト/ボタンのコンテンツコンポーネントなど）

動的にするコンテンツに応じて式エディターにアクセスする方法の例を以下に示します。

* *「送信者名」フィールドから式エディターにアクセスする*

  ![](assets/expression-editor-access.png){width="800" align="center"}

* *E メールテキストコンポーネントから式エディターにアクセスする*

  ![](assets/expression-editor-access-email.png){width="800" align="center"}

* *E メール内のリンクから式エディターにアクセスする*

  ![](assets/perso-link-insert-icon.png){width="800" align="center"}

>[!NOTE]
>
>式エディターに加えて、E メールをデザインする際に、専用の条件付きコンテンツビルダーを利用することもできます。 [メールでの条件付きコンテンツの作成方法を説明します](conditions.md)

## さらに深く掘り下げましょう

コンテンツを動的にする方法を理解できたので、次にこれらのドキュメントの節をさらに詳しく調べて、この機能の使用を開始します。

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="personalize.md">
<img alt="コンテンツのパーソナライズ" src="assets/do-not-localize/dynamic-personalization.jpg">
</a>
<div>
<a href="personalize.md"><strong>パーソナライゼーションの追加</strong></a>
</div>
<p>
</td>
<td>
<a href="conditions.md">
<img alt="リード" src="assets/do-not-localize/dynamic-conditional.jpg">
</a>
<div><a href="conditions.md"><strong>条件付きコンテンツを追加</strong>
</div>
<p>
</td>
<td>
<a href="content-blocks.md">
<img alt="低頻度" src="assets/do-not-localize/dynamic-content-blocks.jpg">
</a>
<div>
<a href="content-blocks.md"><strong>組み込みコンテンツブロックを追加する</strong></a>
</div>
<p></td>
</tr></table>
