---
audience: end-user
title: ワークフローのチャネルアクティビティの操作
description: チャネルアクティビティを Adobe Campaign Web ワークフローに使用する方法を学ぶ
badge: label="Alpha" type="Positive"
exl-id: 6f9be348-6138-470c-8c40-750dc0311424
source-git-commit: dd006d1e161dec49d9a1a6bcb8cb67503178479b
workflow-type: ht
source-wordcount: '219'
ht-degree: 100%

---

# チャネルアクティビティ {#channel}

Adobe Campaign Web を使用すると、メール、SMS、プッシュなど複数のチャネルをまたいでマーケティングキャンペーンを自動化および実行できます。Adobe Campaign のワークフローを使用すると、チャネルアクティビティをキャンバスに組み合わせて、顧客の行動に基づいてアクションをトリガーできるクロスチャネルワークフローを作成できます。

例えば、メール、SMS、プッシュなど、様々なチャネルをまたいだ一連のメッセージを含むようこそメールキャンペーンを作成できます。また、顧客が購入を完了した後や、SMS を使用してパーソナライズされた誕生日メッセージを顧客に送信した後に、フォローアップメールを送信することもできます。

チャネルアクティビティを使用すると、複数のタッチポイントで顧客を引きつけてコンバージョンを促進する、包括的でパーソナライズされたキャンペーンを作成できます。

チャネルアクティビティは、パレットの画面左側にある「チャネル」セクションで使用できます。

## メール {#email}

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