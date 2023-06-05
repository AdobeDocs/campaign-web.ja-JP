---
audience: end-user
title: オーディエンスの作成ワークフローアクティビティの使用
description: オーディエンスの作成ワークフローアクティビティの使用方法を説明します
badge: label="Alpha" type="Positive"
source-git-commit: bdf569913dfcf9bee549c6ae3252f5a92a5f34e8
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 9%

---


# オーディエンスを作成 {#build-audience}

この **オーディエンスの構築** アクティビティは **ターゲット設定** アクティビティ。 このアクティビティを使用すると、ワークフローに入るオーディエンスを定義できます。 キャンペーンワークフローのコンテキストでメッセージを送信する場合、メッセージオーディエンスは、チャネルアクティビティではなく、 **オーディエンスの構築** アクティビティ。

オーディエンス母集団を定義するには、次の操作を実行します。

* クライアントコンソールでリストとして作成した既存のオーディエンスを選択します。
* Adobe Experience Platformオーディエンスを選択します。
* フィルター条件を定義し組み合わせて、ルールビルダーを使用して新しいオーディエンスを作成します。

>[!NOTE]
>
>このコンテキストでは、オーディエンスをファイルから読み込むことはできません。 この場合、スタンドアロン配信を作成する必要があります。 [詳細情報](../../audience/about-audience.md)

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

## 設定

次の手順に従って、 **オーディエンスの構築** アクティビティ：

1. を追加します。 **オーディエンスの構築** アクティビティ。
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

## 例

次に、2 つの **オーディエンスの構築** アクティビティ。 1 つ目は、ポーカープレーヤーのオーディエンスをターゲットにし、次に E メール配信をターゲットにします。 2 つ目のクエリは、VIPクライアントオーディエンスをターゲットにし、その後に SMS 配信をターゲットにします。

![](../assets/workflow-audience-example.png)