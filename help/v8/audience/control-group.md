---
audience: end-user
title: コントロール母集団の設定
description: Campaign web ユーザーインターフェイスでメッセージのコントロール母集団を設定する方法について説明します
exl-id: 02f3adec-681a-4cec-a895-41c80eb345db
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '799'
ht-degree: 41%

---

# コントロール母集団の設定 {#control-group}

コントロール母集団は、配信から除外されるサブ母集団です。コントロール母集団を定義すると、オーディエンスの一部にメッセージを送信しないようにし、配信後の動作をメインターゲットと比較できます。 このオプションは、キャンペーンの影響を測定するのに役立ちます。

➡️ [この機能をビデオで確認](create-audience.md#video)

## コントロール母集団を有効にする {#add-a-control-group}

コントロール母集団を追加するには、配信のオーディエンスを定義する際にオプションを有効にします。 コントロール母集団は、メインターゲットからランダムに抽出することも、特定の母集団から選択することもできます。 したがって、コントロール母集団を定義する主な方法は 2 つあります。

* メインターゲットから複数のプロファイルを抽出します。
* リストから、またはクエリで定義された条件に基づいて、一部のプロファイルを除外します。

コントロール母集団を定義する際は、両方の方法を組み合わせることができます。

配信準備段階でコントロール母集団に含まれているすべてのプロファイルが、メインターゲットから削除されます。 これらのプロファイルは、メッセージを受信しません。

>[!CAUTION]
>
>ターゲット母集団の読み込み時には、[外部ファイルから](file-audience.md)コントロール母集団を使用できません。

配信にコントロール母集団を追加するには、配信作成画面の **[!UICONTROL オーディエンス]** セクションにある **コントロールグループを有効にする** 切替スイッチを有効にします。

![ 配信作成画面の「コントロールグループを有効にする」オプションを切り替えます ](assets/control-group1.png)

## ターゲットから抽出 {#extract-target}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_target"
>title="抽出モード"
>abstract="コントロール母集団は、配信から除外される一連のプロファイルです。コントロール母集団を定義するには、ターゲット母集団から無作為に、または並べ替えに基づいて、一定の割合または一定数のプロファイルを抽出できます。"

### コントロール母集団を作成 {#build-extract-target}

コントロール母集団を定義するには、ターゲット母集団から一定の割合または一定数のプロファイルを、無作為または並べ替えに基づいて抽出します。 追加の母集団を追加する場合は、「**抽出なし**」オプションを選択し、追加の母集団 [ 詳しくはこちらを参照 ](#extra-population) を選択します。

まず、ターゲットからプロファイルを抽出する方法（ランダムまたは並べ替えに基づく）を定義します。

「**コントロール母集団**」セクションで、**抽出モード**&#x200B;を選択します。

* Adobe Campaign **ランダム**：配信を準備すると、サイズ制限として設定された割合または最大数に応じてプロファイルがランダムに抽出されます。
* **属性ごとにランク付け**：このオプションでは、特定の並べ替え順で特定の属性に基づいて一連のプロファイルを除外します。

次に、「**サイズ制限**」セクションを使用して、メインターゲットから抽出するプロファイルの数を設定します。 生の数値（除外する 50 個のプロファイルなど）または初期オーディエンスの割合（メインターゲットの 5% など）を指定できます。

### コントロール母集団の例 {#control-group-sample}

例えば、100 人の最年少プロファイルを持つコントロール母集団を作成するには、次の手順に従います。

1. 「**年齢**」フィールドを並べ替え条件として選択します。**昇順**&#x200B;並べ替えオプションはそのままにしておきます。
1. 「**作成日**」フィールドを追加します。**降順**&#x200B;並べ替えオプションに変更します。
1. 「**サイズ制限**」セクションでしきい値に 100 を定義します。

   ![ 最年少プロファイルのコントロール母集団設定 ](assets/control-group2.png){zoomable="yes"}

この 100 個の最年少プロファイルがメインターゲットから除外されます。

### コントロール母集団を確認 {#check-control-group}

ログを表示して、除外されたプロファイルを確認および特定します。 例えば、5 つのプロファイルをランダムに除外するとします。

![ ログ内の除外されたプロファイルの例 ](assets/control-group4.png){zoomable="yes"}

配信準備が完了したら、除外がどのように適用されたかを確認します。

* 配信ダッシュボードで、送信前に **除外対象** KPI を確認します。

  ![ 「除外対象」 KPI を示す配信ダッシュボード ](assets/control-group5.png){zoomable="yes"}

* 配信ログの「ログ」タブには、除外手順が表示されます。

  ![ 除外ステップを表示する配信ログ ](assets/control-group-sample-logs.png){zoomable="yes"}

<!--

 * The **Exclusion logs** tab displays each profile and the related exclusion **Reason**.

    ![](assets/control-group6.png){zoomable="yes"}

-->

* **除外の原因** タブには、タイポロジルールごとに除外されたプロファイルの数が表示されます。

  ![ タイポロジルールの除外を表示する除外の原因タブ ](assets/control-group7.png){zoomable="yes"}

配信ログについて詳しくは、[こちら](../monitor/delivery-logs.md)を参照してください。

## 追加の母集団を追加 {#extra-population}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_extra"
>title="追加の母集団"
>abstract="コントロール母集団は、配信から除外される一連のプロファイルです。既存のオーディエンスを選択するか、クエリを定義すると、配信オーディエンスから特定の母集団を除外できます。"

コントロール母集団を定義するもう 1 つの方法は、既存のオーディエンス内の特定の母集団を選択するか、クエリを定義することです。

**コントロール母集団**&#x200B;の定義画面で、「**追加の母集団**」セクションの「**[!UICONTROL オーディエンスを選択]**」ボタンをクリックします。

![ 追加母集団選択画面 ](assets/control-group3.png){zoomable="yes"}

* 既存のオーディエンスを使用するには、「**オーディエンスを選択**」をクリックします。詳しくは、[こちら](add-audience.md)を参照してください。
* 新しいクエリを定義するには、「**独自に作成**」を選択し、クエリモデラ―を使用して除外条件を定義します。詳しくは、[こちら](../query/query-modeler-overview.md)を参照してください。

オーディエンスに含まれるプロファイル、またはクエリの結果と一致するプロファイルは、配信ターゲットから **除外** されます。 メッセージは届きません。

## 結果を比較 {#control-group-results}

配信が送信されたら、送信ログを抽出して、通信を受信しなかったプロファイルと有効なターゲット間の動作を比較します。 配信ログを使用して新しいターゲティングを作成します。

ターゲットから削除されたプロファイルを確認するには、**配信ログ**&#x200B;を確認します。詳しくは、[この節](#check-control-group)を参照してください。