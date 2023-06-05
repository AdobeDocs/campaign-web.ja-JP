---
audience: end-user
title: オーディエンスの基本を学ぶ
description: Campaign web UI でのオーディエンスの使用方法について説明します
badge: label="Alpha" type="Positive"
exl-id: 21bb5082-82ce-47d6-a4d4-becf44490f13
source-git-commit: 84ef79098494236d3ea2d3b46b72280603ad5c94
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 53%

---


# オーディエンスの基本を学ぶ {#about-audiences}

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


オーディエンスは、配信のメインターゲットです。メッセージを受信した受信者。 オーディエンスのタイプは、配信テンプレートで定義されたターゲットマッピングによって異なります。[こちら](../msg/delivery-template.md)を参照してください。

Campaign のルールビルダーを使用し、メッセージのオーディエンスを選択するためのフィルター条件を定義する方法について説明します。 外部ファイルのデータを簡単に使用したり、Adobe Experience Platformオーディエンスをターゲット設定したりできます。


オーディエンスを定義するには、次の操作を実行します。

* クライアントコンソールで作成した既存のオーディエンスを選択します。 [詳細情報](add-audience.md)
* ルールビルダーを使用して新しいオーディエンスを作成します。 [詳細情報](segment-builder.md)
* 外部ファイルのオーディエンスを使用します。 [詳細情報](file-audience.md)
* Adobe Experience Platform オーディエンスの使用。[詳細情報](aep-audience.md)

また、コントロール母集団を定義すると、キャンペーンの影響を測定するために、オーディエンスの一部にメッセージを送信しないようにできます。[詳細情報](control-group.md)

![](assets/about-audience.png)

