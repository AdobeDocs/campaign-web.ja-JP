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
source-git-commit: bf5ff77b695a5a8584bad7784597bf1521bcb23e
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 12%

---


# 動的コンテンツの基本を学ぶ

顧客に関連するコンテンツを配信することは、マーケティングコンテンツを読むために、様々な顧客にアピールし、顧客の興味を引くための重要な要素です。

Adobe Campaignでは、様々なグループや個人向けのカスタム動的コンテンツを、収集した情報を活用して顧客向けのレベルで配信し、様々なマーケティングキャンペーンを最大限に活用し、ユーザー向けのカスタムエクスペリエンスを作成できます。

* **メッセージをパーソナライズ** 特定の受信者に対して、姓、興味、住所、購入内容などのプロファイルデータを活用します。

  受信者、メッセージまたは配信に関連するパーソナライゼーションエディターから、データベースで使用可能な任意のフィールドを選択できます。 これらのパーソナライゼーション属性は、メッセージの件名行や本文に挿入できます。&lt;%= recipient.location.city %> の構文は、受信者の市区町村をコンテンツに挿入します。

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
