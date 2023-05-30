---
audience: end-user
title: オーディエンスの基本を学ぶ
description: Campaign web UI でのオーディエンスの使用方法について説明します
badge: label="Alpha" type="Positive"
exl-id: 21bb5082-82ce-47d6-a4d4-becf44490f13
source-git-commit: 0703b872bb8f452773e76f2524d47bf774c687e0
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 83%

---


# オーディエンスの基本を学ぶ {#about-audiences}

>[!CONTEXTUALHELP]
>id="acw_homepage_card2"
>title="オーディエンスの基本を学ぶ"
>abstract="Campaign のルールビルダーを使用し、メッセージのオーディエンスを構築するためのフィルタリング条件を定義する方法について説明します。"

<!--
Audience only created for the delivery, not available later-->


<!--
Three ways:
* existing audience

Campaign or AEP Audiences

* create new on the fly

query like AEP segment builder (same component with campaign data)

* import from file

show use case with a new audience creation (or import from file?)

control groups like acc: exract, random, based on attribute
-->

この節では、メールのオーディエンスを定義する方法について説明します。オーディエンスは配信のメインターゲットであり、メールを受信する受信者となります。オーディエンスのタイプは、配信テンプレートで定義されたターゲットマッピングによって異なります。[こちら](../email/create-email.md)を参照してください。

オーディエンスを定義するには、次の操作を実行します。

* 既存のオーディエンスの使用。[詳細情報](add-audience.md)
* 新しいオーディエンスの作成。[詳細情報](segment-builder.md)
* 外部ファイルのオーディエンスを使用します。 [詳細情報](file-audience.md)
* Adobe Experience Platform オーディエンスの使用。[詳細情報](aep-audience.md)

また、コントロール母集団を定義すると、キャンペーンの影響を測定するために、オーディエンスの一部にメッセージを送信しないようにできます。[詳細情報](control-group.md)

![](assets/about-audience.png)
