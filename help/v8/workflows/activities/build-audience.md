---
audience: end-user
title: オーディエンスの作成ワークフローアクティビティの使用
description: オーディエンスの作成ワークフローアクティビティの使用方法を説明します
badge: label="Alpha" type="Positive"
source-git-commit: 2172d159b9d43b18ebb56f5bbbb806884db14346
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 14%

---


# オーディエンスを作成 {#build-audience}

このアクティビティを使用すると、オーディエンスを定義できます。 既存の Campaign オーディエンスを選択するか、ルールビルダーを使用して独自のクエリを定義できます。

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

次の手順に従って、 **オーディエンスの構築** アクティビティ：

1. 「オーディエンスを作成」アクティビティを追加します。
1. ラベルを定義します。
1. オーディエンスタイプを定義します。 **独自の** または **オーディエンスの閲覧**.

独自のクエリを作成するには、次の追加の手順に従います。

1. 選択 **独自の（クエリ）を作成**.
1. を選択します。 **ターゲティングディメンション**. ターゲティングディメンションを使用して、操作のターゲティング対象となる母集団を定義できます。受信者、契約受益者、オペレーター、購読者など デフォルトでは、ターゲットが受信者から選択されます。詳しくは、 [v8 ドキュメント](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html#targeting-and-filtering-dimensions){target="_blank"}.
1. 「**続行**」をクリックします。
1. ルールビルダーを使用してクエリを定義します。これは、新しい E メールをデザインする際にオーディエンスを作成するのと同じ方法です。 [こちら](../../audience/segment-builder.md)を参照してください。

既存のオーディエンスを選択するには、次の手順に従います。

1. 選択 **オーディエンスの閲覧**.
1. 「**続行**」をクリックします。
1. 新しい E メールをデザインする際にオーディエンスを使用するのと同じ方法で、オーディエンスを選択します。 [こちら](../../audience/add-audience.md)を参照してください。
