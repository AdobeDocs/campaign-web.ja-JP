---
audience: end-user
title: オーディエンスの基本を学ぶ
description: Campaign web UI でのオーディエンスの使用方法について説明します
badge: label="Alpha" type="Positive"
exl-id: 21bb5082-82ce-47d6-a4d4-becf44490f13
source-git-commit: bbebd9dc462a189618cbf6e71467bb0935e1317a
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 31%

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


オーディエンスは、配信のメインターゲットです。メッセージを受信した受信者。 オーディエンスのタイプは、配信テンプレートで定義されたターゲットマッピングによって異なります。配信テンプレートとは [この節](../msg/delivery-template.md).

オーディエンス母集団を定義するには、次の操作を実行します。

* クライアントコンソールでリストとして作成した既存のオーディエンスを選択します。 [詳細情報](add-audience.md)
* Adobe Experience Platformオーディエンスを選択します。 [詳細情報](aep-audience.md)
* フィルター条件を定義し組み合わせて、ルールビルダーを使用して新しいオーディエンスを作成します。 [詳細情報](segment-builder.md)
* 外部ファイルからオーディエンスを使用：このオプションは、スタンドアロンの e メール配信にのみ使用でき、campaign 配信では使用できません。 [詳細情報](file-audience.md)

キャンペーンワークフローのコンテキストでメッセージを送信する場合、オーディエンスは、特定の **オーディエンスの閲覧** ワークフローアクティビティ。 このコンテキストでは、E メール配信用のオーディエンスをファイルから読み込むことはできず、オーディエンスはこの専用アクティビティでのみ定義されます。 キャンペーンワークフローで配信のオーディエンスを定義する方法を説明します [この節](../workflows/orchestrate-activities.md).

また、コントロール母集団を定義すると、キャンペーンの影響を測定するために、オーディエンスの一部にメッセージを送信しないようにできます。[詳細情報](control-group.md)

![](assets/about-audience.png)

