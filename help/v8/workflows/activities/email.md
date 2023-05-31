---
audience: end-user
title: E メールワークフローアクティビティの使用
description: E メールワークフローアクティビティの使用方法を説明します
badge: label="Alpha" type="Positive"
source-git-commit: 2172d159b9d43b18ebb56f5bbbb806884db14346
workflow-type: tm+mt
source-wordcount: '84'
ht-degree: 84%

---


# メール {#email}

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
