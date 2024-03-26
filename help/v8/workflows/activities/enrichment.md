---
audience: end-user
title: エンリッチメントワークフローアクティビティの使用
description: エンリッチメントワークフローアクティビティの使用方法を説明します
exl-id: 02f30090-231f-4880-8cf7-77d57751e824
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '722'
ht-degree: 100%

---

# エンリッチメント {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment"
>title="エンリッチメントアクティビティ"
>abstract="**エンリッチメント**&#x200B;アクティビティでは、データベースからの追加情報を使用してターゲットデータを強化できます。一般的に、セグメント化アクティビティ後のワークフローで使用されます。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="エンリッチメントアクティビティ"
>abstract="エンリッチメントデータをワークフローに追加すると、エンリッチメントアクティビティ後に追加されたアクティビティで使用して、行動、好み、ニーズに基づいて顧客を個別のグループにセグメント化したり、ターゲットオーディエンスの共感を呼ぶ可能性が高いパーソナライズされたマーケティングメッセージとキャンペーンを作成したりできます。"

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_enrichmentdata"
>title="エンリッチメントデータ"
>abstract="ワークフローの強化に使用するデータを選択します。ターゲットディメンションから単一エンリッチメント属性、またはテーブル間の基数が 1～N を持つリンクの 2 種類のエンリッチメントデータから選択できます。"

**エンリッチメント**&#x200B;アクティビティは、**ターゲティング**&#x200B;アクティビティです。データベースからの追加情報を使用してターゲットデータを強化できます。一般的に、セグメント化アクティビティ後のワークフローで使用されます。

エンリッチメントデータは次のいずれかを実行できます。

* ワークフローのターゲットと&#x200B;**同じ作業用テーブルから**：

  *顧客のグループをターゲットに設定し、「生年月日」フィールドを現在の作業用テーブルに追加*

* **別の作業用テーブルから**：

  *顧客のグループをターゲットにし、「購入」テーブルから取得した「金額」フィールドと「製品のタイプ」フィールドを追加します*。

ワークフローに追加されたエンリッチメントデータは、「**エンリッチメント**」アクティビティ後に追加されたアクティビティで使用して、行動、好み、ニーズに基づいて顧客を個別のグループにセグメント化したり、ターゲットオーディエンスの共感を呼ぶ可能性が高いパーソナライズされたマーケティングメッセージやキャンペーンを作成したりできます。

例えば、顧客の購入に関する情報をワークフローの作業用テーブルに追加し、このデータを使用して、最新の購入または購入金額に応じてメールをパーソナライズできます。

## エンリッチメントアクティビティを設定します。 {#enrichment-configuration}

次の手順に従って、**エンリッチメント**&#x200B;アクティビティを設定します。

1. **オーディエンスを作成**&#x200B;および&#x200B;**結合**&#x200B;アクティビティを追加します。
1. **エンリッチメント**&#x200B;アクティビティを追加します。
1. 「**エンリッチメントデータを追加**」をクリックし、データのエンリッチメントに使用する属性を選択します。

   ターゲットディメンションから[単一エンリッチメント属性](#single-attribute)または[コレクションリンク](#collection-link)の 2 種類のエンリッチメントデータを選択できます。

   >[!NOTE]
   >
   >属性選択画面の「**式を編集**」ボタンを使用すると、属性を選択する高度な式を作成できます。[式エディターの操作方法の詳細を学ぶ](../../query/expression-editor.md)

   ![](../assets/workflow-enrichment1.png)

## 単一エンリッチメント属性 {#single-attribute}

ここでは、生年月日など、単一エンリッチメント属性を追加します。次の手順に従います。

1. 「**属性**」フィールド内をクリックします。
1. ターゲティングディメンションからシンプルなフィールド（この例では生年月日）を選択します。
1. 「**確認**」をクリックします。

![](../assets/workflow-enrichment2.png)

## コレクションリンク {#collection-link}

この、より複雑なユースケースでは、テーブル間で 1-N の基数を持つリンクであるコレクションリンクを選択します。100 ドル未満の、最新 3 回の購入を取得します。そのためには、次を定義する必要があります。

* エンリッチメント属性：「**合計金額**」フィールド
* 取得する行の数：3
* フィルター：100 ドルを超える項目を除外
* 並べ替え：「**注文日付**」フィールドを降順で並び替え。

### 属性を追加 {#add-attribute}

エンリッチメントデータとして使用するコレクションリンクを選択する場所です。

1. 「**属性**」フィールド内をクリックします。
1. 「**詳細属性を表示**」をクリックします。
1. **購入**&#x200B;テーブルから「**合計金額**」フィールドを選択します。

![](../assets/workflow-enrichment3.png)

### コレクション設定の定義{#collection-settings}

次に、データの収集方法と取得するレコード数を定義します。

1. **データの収集方法を選択**&#x200B;ドロップダウンで「**データを収集**」を選択します。
1. 「**取得する行（作成する列）**」フィールドに「3」と入力します。

![](../assets/workflow-enrichment4.png)

例えば、顧客の平均購入額を取得する場合は、代わりに「**集計データ**」を選択し、「**集計関数**」ドロップダウンで「**平均**」を選択します。

![](../assets/workflow-enrichment5.png)

### フィルターの定義{#collection-filters}

ここでは、エンリッチメント属性の最大値を定義します。100 を超える項目は除外します。[詳しくは、クエリモデラーの操作方法を参照してください](../../query/query-modeler-overview.md)

1. 「**フィルターを編集**」をクリックします。
1. **合計金額**&#x200B;が存在し、かつ&#x200B;**合計金額**&#x200B;が 100 未満である、という 2 つのフィルターを追加します。最初のフィルターでは、NULL 値が最大値として表示されるようにフィルタリングします。
1. 「**確認**」をクリックします。

![](../assets/workflow-enrichment6.png)

### 並べ替えを定義{#collection-sorting}

**最新**&#x200B;の 3 つの購入を取得するには、並べ替えを適用する必要があります。

1. 「**並べ替えを有効にする**」オプションをアクティブ化します。
1. 「**属性**」フィールド内をクリックします。
1. 「**オーダー日**」フィールドを選択します。
1. 「**確認**」をクリックします。
1. **並べ替え**&#x200B;ドロップダウンから「**降順**」を選択します。

![](../assets/workflow-enrichment7.png)

<!--

Add other fields
use it in delivery


cardinality between the tables (1-N)
1. select attribute to use as enrichment data

    display advanced fields option
    i button

    note: attributes from the target dimension

1. Select how the data is collected
1. number of records to retrieve if want to retrieve a collection of multiple records
1. Apply filters and build rule

    select an existing filter
    save the filter for reuse
    view results of the filter visually or in code view

1. sort records using an attribute

leverage enrichment data in campaign

where we can use the enrichment data: personalize email, other use cases?

## Example

-->
