---
audience: end-user
title: オーディエンスの保存ワークフローアクティビティを使用する
description: 分岐ワークフローアクティビティの使用方法を学ぶ
badge: label="Beta"
source-git-commit: b2cd72ce06e1b18689be4c40c80f3abde85f922e
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 14%

---


# オーディエンスを保存 {#save-audience}

>[!CONTEXTUALHELP]
>id="???"
>title="オーディエンスアクティビティを保存"
>abstract="「オーディエンスを保存」アクティビティを使用すると、次の操作を実行できます。"

モードオーディエンスラベルAdobe Campaignは、このラベルを既存のオーディエンスと照合します。 一致が見つかった場合は、そのオーディエンスが更新されます。一致しなかった場合は、新しいオーディエンスが作成されます。
更新メソッド

オーディエンスを新しいデータに置換

新しいデータフォルダーリスト (/Profiles and Targets/Lists/) でオーディエンスを完了

アウトバウンドトランジションを生成


The **オーディエンスを保存** アクティビティは **ターゲット設定** アクティビティ。 このアクティビティを使用すると、既存のオーディエンスを更新したり、ワークフローの上流で計算された母集団から新しいオーディエンスを作成したりできます。 作成したオーディエンスは、アプリケーションオーディエンスのリストに追加され、 **オーディエンス** メニュー。

このアクティビティは、基本的に、同じワークフローで計算された母集団グループを再利用可能なオーディエンスに変換することで、そのグループを維持するために使用されます。 他のターゲティングアクティビティ（など）に接続します。 **オーディエンスの構築** または **結合** アクティビティ。

## 設定

次の手順に従って、 **オーディエンスを保存** アクティビティ：

1. を追加します。 **オーディエンスを保存** アクティビティをワークフローに追加します。

   <!--![](../assets/workflow-save-audience.png)-->

1. Adobe Analytics の **モード** ドロップダウンで、実行するアクションを選択します。

   * **既存のオーディエンスを作成または更新**：定義 **オーディエンスラベル**. オーディエンスが既に存在する場合は更新されます。存在しない場合は新しいオーディエンスが作成されます。

   * **既存のオーディエンスの更新**：を選択します。 **対象ユーザ** 既存のオーディエンスのリストの中で更新する場合。

1. を選択します。 **モードを更新** 既存のオーディエンスに適用される条件：

   * **オーディエンスコンテンツを新しいデータで置き換える**：すべてのオーディエンスコンテンツを置き換えます。 古いデータは失われます。「オーディエンスの保存」アクティビティのインバウンドトランジションからのデータのみが保持されます。このオプションを選択すると、オーディエンスのタイプと、更新されたオーディエンスのターゲティングディメンションが消去されます。

   * **新しいデータでオーディエンスを完了**：古いオーディエンスコンテンツは保持され、「オーディエンスの保存」アクティビティのインバウンドトランジションのデータが追加されます。

1. 残りの母集団を利用するには、「**補集合を生成**」オプションをチェックします。その後、追加のトランジションがアクティビティに追加されます。

保存したオーディエンスの内容は、そのオーディエンスの詳細表示で利用できます。詳細表示には、 **オーディエンス** メニュー。 この表示で使用できる列は、ワークフローの **SAve オーディエンス** アクティビティ。


## 例


