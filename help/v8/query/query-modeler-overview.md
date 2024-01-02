---
audience: end-user
title: クエリモデラーを操作
description: Adobe Campaign web クエリモデラーの操作方法について説明します。
source-git-commit: 9992ae7007b5af80e927dd96b6fff25840d8c3e1
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 96%

---

# クエリモデラーを操作 {#segment-builder}


>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="新しいクエリモデラー"
>abstract="Adobe Campaign web には、データベースをフィルタリングして様々な基準に基づいて特定のターゲットを選択するプロセスを簡素化するクエリモデラーが備わっています。これには、高度な式や演算子の使用も含まれます。 クエリモデラーは、データをフィルタリングするルールを定義する必要があるすべてのコンテキストで使用できます。"

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

クエリモデラーは、クエリを作成する様々なコンポーネントを追加して組み合わせることができる中央のキャンバスを提供します。

右側にあるルールのプロパティパネルには、クエリに関する情報が表示されます。これにより、様々な操作を実行してクエリを確認し、ニーズに合うことを確認できます。詳しくは、クエリを確認および検証する方法を参照してください

![](assets/query-interface.png)
