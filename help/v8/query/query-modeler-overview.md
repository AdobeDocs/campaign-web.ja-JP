---
audience: end-user
title: クエリモデラーの操作
description: Adobe Campaign web クエリモデラーの操作方法について説明します。
exl-id: 56708a66-f654-413a-80ed-1865077b3c0a
source-git-commit: 32bffad5ea6641a723887ca9fa3e58b8cc428c00
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 82%

---

# クエリモデラーの操作 {#segment-builder}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card5"
>title="新しいクエリモデラー"
>abstract="Adobe Campaign web にはクエリモデラーが備わっています。これにより、データベースをフィルタリングして様々な基準に基づいて特定のターゲットを選択するプロセスが簡素化されます。これには、高度な式と演算子の使用が含まれます。クエリモデラーは、データをフィルタリングするルールを定義する必要があるすべてのコンテキストで使用できます。"

<!--TO REMOVE BELOW-->
>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="新しいクエリモデラー"
>abstract="Adobe Campaign web にはクエリモデラーが備わっています。これにより、データベースをフィルタリングして様々な基準に基づいて特定のターゲットを選択するプロセスが簡素化されます。これには、高度な式と演算子の使用が含まれます。クエリモデラーは、データをフィルタリングするルールを定義する必要があるすべてのコンテキストで使用できます。"

<!--TO REMOVE ABOVE-->


>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_querymessage"
>title="クエリモデラー"
>abstract="データベースから受信者やその他のターゲティングディメンションのフィルタリング条件を定義します。Adobe Experience Platform オーディエンスを活用して、ターゲットオーディエンスをさらに絞り込んで、キャンペーンの効果を最大化します。"

Adobe Campaign Web ユーザーインターフェイスには、クエリモデラーが備わっており、様々な条件に基づいてデータベースをフィルタリングするプロセスが簡単になります。 これにより、クライアントコンソールで作成されたクエリとの完全な互換性が確保され、Web ユーザーインターフェイスへのシームレスな切り替えが容易になります。

さらに、クエリモデラーは、非常に複雑で長いクエリを効率的に管理でき、柔軟性と精度が向上しました。 さらに、条件内で定義済みフィルターをサポートし、高度な式や演算子を利用して包括的なオーディエンスのターゲティングとセグメント化戦略に利用しながら、簡単にクエリを絞り込むことができます。

## クエリモデラーへのアクセス

クエリモデラーは、データをフィルタリングするルールを定義する必要があるすべてのコンテキストで使用できます。

| 使用状況 | 例 |
|  ---  |  ---  |
| **オーディエンスの定義**：メッセージやワークフローでターゲットにする母集団を指定し、ニーズに合わせて新しいオーディエンスを簡単に作成します。 | ![](assets/access-audience.png){zoomable=&quot;yes&quot;}{width="200" align="center" zoomable="yes"} |
| **ワークフローアクティビティのカスタマイズ**：特定の要件に合わせて、分割や紐付けなどのワークフローアクティビティ内にルールを適用します。 | ![](assets/access-workflow.png){zoomable=&quot;yes&quot;}{width="200" align="center" zoomable="yes"} |
| **定義済みフィルター**：データリストの操作や配信のオーディエンスの形成など、様々なフィルタリング操作中にショートカットとして機能する定義済みフィルターを作成します。 | ![](assets/access-predefined-filter.png){zoomable=&quot;yes&quot;}{width="200" align="center" zoomable="yes"} |
| **レポートデータのフィルタリング**：レポートに表示されるデータをフィルタリングするルールを追加します。 | ![](assets/access-reports.png){zoomable=&quot;yes&quot;}{width="200" align="center" zoomable="yes"} |
| **リストのカスタマイズ**：受信者、配信リストなどのリストに表示されるデータをフィルタリングするカスタムルールを作成します。 | ![](assets/access-lists.png){zoomable=&quot;yes&quot;}{width="200" align="center" zoomable="yes"} |

<!--**Dynamize content**: make your content dynamic by creating conditions that define which content should be displayed to different recipients, ensuring personalized and relevant messaging.

+++Example

![](assets/access-audience.png){zoomable="yes"}

 +++
-->

## クエリモデラーインターフェイス {#interface}

クエリモデラーは、クエリを作成する中央のキャンバスと、クエリに関する情報を示す右側のパネルを提供します。

![](assets/query-interface.png){zoomable=&quot;yes&quot;}

### 中央のキャンバス {#canvas}

クエリモデラーの中央のキャンバスでは、クエリを作成する様々なコンポーネントを追加して組み合わせます。[クエリの作成方法を学ぶ](build-query.md)

キャンバスの右上隅にあるツールバーには、クエリコンポーネントを簡単に操作し、キャンバス内を移動するオプションが表示されます。

* **複数選択モード**：複数のフィルタリングコンポーネントを選択して、選択した場所にコピー＆ペーストします。
* **回転**：キャンバスを垂直方向に切り替えます。
* **画面に合わせる**：キャンバスのズームレベルを画面に合わせて調整します。
* **ズームアウト**／**ズームイン**：キャンバスをズームアウトまたはズームインします。
* **マップを表示**：現在の位置を示すキャンバスのスナップショットを開きます。

### ルールのプロパティパネル {#rule-properties}

右側にある&#x200B;**[!UICONTROL ルールのプロパティ]**&#x200B;パネルには、クエリに関する情報が表示されます。これにより、様々な操作を実行してクエリを確認し、ニーズに合うことを確認できます。[クエリを確認および検証する方法を学ぶ](build-query.md#check-and-validate-your-query)
