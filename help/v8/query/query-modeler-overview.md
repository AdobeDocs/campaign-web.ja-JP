---
audience: end-user
title: クエリモデラーを操作
description: Adobe Campaign web クエリモデラーの操作方法について説明します。
badge: label="限定提供（LA）"
source-git-commit: 9c72d73b5279a01492ea3ccd295e513e91f0c050
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 60%

---

# クエリモデラーを操作 {#segment-builder}


>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card5"
>title="新しいクエリモデラー"
>abstract="Adobe Campaign web には、データベースをフィルタリングして様々な基準に基づいて特定のターゲットを選択するプロセスを簡素化するクエリモデラーが備わっています。これには、高度な式や演算子の使用も含まれます。 クエリモデラーは、データをフィルタリングするルールを定義する必要があるすべてのコンテキストで使用できます。"

<!--TO REMOVE BELOW-->
>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="新しいクエリモデラー"
>abstract="Adobe Campaign web には、データベースをフィルタリングして様々な基準に基づいて特定のターゲットを選択するプロセスを簡素化するクエリモデラーが備わっています。これには、高度な式や演算子の使用も含まれます。 クエリモデラーは、データをフィルタリングするルールを定義する必要があるすべてのコンテキストで使用できます。"

<!--TO REMOVE ABOVE-->


>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_querymessage"
>title="クエリモデラー"
>abstract="データベースから受信者やその他のターゲティングディメンションのフィルタリング条件を定義します。Adobe Experience Platform オーディエンスを活用して、ターゲットオーディエンスをさらに絞り込んで、キャンペーンの効果を最大化します。"

Adobe Campaign web には、データベースをフィルタリングして様々な基準に基づいて特定のターゲットを選択するプロセスを簡素化するクエリモデラーが備わっています。これには、高度な式と演算子の使用が含まれます。

## クエリモデラーへのアクセス

クエリモデラーは、データをフィルタリングするルールを定義する必要があるすべてのコンテキストで使用できます。

| 使用状況 | 例 |
|  ---  |  ---  |
| **オーディエンスの定義**：メッセージやワークフローでターゲットにする母集団を指定し、ニーズに合わせて新しいオーディエンスを簡単に作成します。 | ![](assets/access-audience.png){width="200" align="center" zoomable="yes"} |
| **ワークフローアクティビティのカスタマイズ**：特定の要件に合わせて、分割や紐付けなどのワークフローアクティビティ内にルールを適用します。 | ![](assets/access-workflow.png){width="200" align="center" zoomable="yes"} |
| **定義済みフィルター**：データリストの操作や配信のオーディエンスの形成など、様々なフィルタリング操作中にショートカットとして機能する定義済みフィルターを作成します。 | ![](assets/access-predefined-filter.png){width="200" align="center" zoomable="yes"} |
| **レポートデータのフィルタリング**：レポートに表示されるデータをフィルタリングするルールを追加します。 | ![](assets/access-reports.png){width="200" align="center" zoomable="yes"} |
| **リストのカスタマイズ**：受信者、配信リストなどのリストに表示されるデータをフィルタリングするカスタムルールを作成します。 | ![](assets/access-lists.png){width="200" align="center" zoomable="yes"} |

<!--**Dynamize content**: make your content dynamic by creating conditions that define which content should be displayed to different recipients, ensuring personalized and relevant messaging.

+++Example

![](assets/access-audience.png)

 +++
-->

## クエリモデラーインターフェイス {#interface}

クエリモデラーは、クエリを作成する中央キャンバスと、クエリに関する情報を提供する右側のウィンドウを提供します。

![](assets/query-interface.png)

### 中央のキャンバス {#canvas}

クエリモデラーの中央キャンバスでは、クエリを作成する様々なコンポーネントを追加および組み合わせることができます。 [クエリの作成方法を説明します](build-query.md)

キャンバスの右上隅にあるツールバーには、クエリコンポーネントを簡単に操作し、キャンバス内を移動するためのオプションが用意されています。

* **複数選択モード**：複数のフィルターコンポーネントを選択して、コピーし、選択した場所に貼り付けます。
* **回転**：キャンバスを垂直方向に切り替えます。
* **画面に合わせる**：キャンバスのズームレベルを画面に合わせます。
* **ズームアウト** / **ズームイン**：ズームアウトするか、キャンバスでズームします。
* **マップを表示**：現在の位置を示すキャンバスのスナップショットを開きます。

### [ ルールのプロパティ ] ウィンドウ {#rule-properties}

右側には、 **[!UICONTROL ルールのプロパティ]** ウィンドウには、クエリに関する情報が表示されます。 様々な操作を実行して、クエリを確認し、ニーズに合っていることを確認できます。 [クエリを確認および検証する方法を説明します](build-query.md#check-and-validate-your-query)
