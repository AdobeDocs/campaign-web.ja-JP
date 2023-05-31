---
audience: end-user
title: ワークフローアクティビティの操作
description: ワークフローアクティビティの方法を説明します
badge: label="Alpha" type="Positive"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: acc3f2cdc50fc8727a472d427c2f8077775a8744
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 98%

---


# ワークフローアクティビティ {#workflow-activities}

## ターゲティングアクティビティ {#targeting}

コンテンツ未定

<!--à reformuler-->これらのアクティビティでは、セットを定義するか、積集合、和集合、除外の各操作を使用して分割または結合することで、1 つまたは複数のターゲットを作成できます。

### オーディエンスを作成 {#build-audience}

### 結合 {#combine}

## チャネルアクティビティ {#channel}

Adobe Campaign Web を使用すると、メール、SMS、プッシュなど複数のチャネルをまたいでマーケティングキャンペーンを自動化および実行できます。Adobe Campaign のワークフローを使用すると、チャネルアクティビティをキャンバスに組み合わせて、顧客の行動に基づいてアクションをトリガーできるクロスチャネルワークフローを作成できます。

例えば、メール、SMS、プッシュなど、様々なチャネルをまたいだ一連のメッセージを含むようこそメールキャンペーンを作成できます。また、顧客が購入を完了した後や、SMS を使用してパーソナライズされた誕生日メッセージを顧客に送信した後に、フォローアップメールを送信することもできます。

チャネルアクティビティを使用すると、複数のタッチポイントで顧客を引きつけてコンバージョンを促進する、包括的でパーソナライズされたキャンペーンを作成できます。

チャネルアクティビティは、パレットの画面左側にある「チャネル」セクションで使用できます。

### メール {#email}

説明、実行できるユースケース（アクティビティの後に、前にリンクできるその他の一般的なアクティビティ）

アクティビティの追加と設定方法

ワークフロー内の設定済みアクティビティの例


メール配信アクティビティでは、ワークフローでメールの送信を設定できます。

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.-->

メール受信者は、オーディエンスのターゲティングアクティビティを通じて、同じワークフロー内のアクティビティの上流で定義されます。

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->


### SMS {#sms}

### プッシュ通知 (Android) {#push-android}

### プッシュ通知 (iOS) {#push-ios}

## フロー制御アクティビティ {#flow-control}

コンテンツ未定

<!--à reformuler-->これらのアクティビティでは、セットを定義するか、積集合、和集合、除外の各操作を使用して分割または結合することで、1 つまたは複数のターゲットを作成できます。

フロー制御アクティビティは、ワークフローアクティビティを調整するために使用します。

### 分岐 {#fork}

### AND 結合 {#end}


### 待機 {#end}

### 終了 {#end}

## データ管理アクティビティ {#data-management}

概要：これらを使用して
実行できるユースケース

使用可能なアクティビティのリスト + 短い説明 + 節への参照

### エンリッチメント {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="エンリッチメント アクティビティ"
>abstract="エンリッチメントアクティビティでは、データベースからの追加情報を使用してターゲットデータを強化できます。これは、一般的に、ターゲティングアクティビティの後のワークフローで使用します。<br/>エンリッチメントデータをワークフローに追加すると、エンリッチメントアクティビティ後に追加されたアクティビティで使用して、行動、好み、ニーズに基づいて顧客を個別のグループにセグメント化したり、ターゲットオーディエンスの共感を呼ぶ可能性が高いパーソナライズされたマーケティングメッセージとキャンペーンを作成したりできます。"

エンリッチメントアクティビティでは、データベースからの追加情報を使用してターゲットデータを強化できます。これは、一般的に、ターゲティングアクティビティの後のワークフローで使用します。

エンリッチメントデータは次のいずれかを実行できます。

* ワークフローのターゲットと&#x200B;**同じ作業用テーブルから**：

   *顧客のグループをターゲットにし、「生年月日」フィールドを現在の作業用テーブルに追加します*

* **別の作業用テーブルから**：

   *顧客のグループをターゲットにし、「購入」テーブルから取得した「金額」フィールドと「製品のタイプ」フィールドを追加します*。

ワークフローに追加されたエンリッチメントデータは、エンリッチメントアクティビティ後に追加されたアクティビティで使用して、行動、好み、ニーズに基づいて顧客を個別のグループにセグメント化したり、ターゲットオーディエンスの共感を呼ぶ可能性が高いパーソナライズされたマーケティングメッセージやキャンペーンを作成したりできます。

例えば、顧客の購入に関する情報をワークフローの作業用テーブルに追加し、このデータを使用して、最新の購入または購入金額に応じてメールをパーソナライズできます。

エンリッチメントアクティビティをワークフローに追加するには、次の手順に従います。

1. アクティビティを追加します
1. エンリッチメントデータとして使用する属性を選択します

   「詳細フィールドを表示」オプション
「i」ボタン

   メモ：ターゲットディメンションからの属性です

1. データの収集方法を選択します
1. 複数のレコードのコレクションを取得する場合に取得するレコードの数
1. フィルターの適用と、ルールの作成

   既存のフィルターを選択します
再利用できるようにフィルターを保存します
フィルターの結果を視覚的にまたはコードビューで表示します

1. 属性を使用してレコードを並べ替えます

Campaign でのエンリッチメントデータの活用

エンリッチメントデータの使用先：電子メールのパーソナライズ、その他のユースケース？
