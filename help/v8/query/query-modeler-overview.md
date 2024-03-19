---
audience: end-user
title: クエリモデラーの操作
description: Adobe Campaign Web クエリモデラーの操作方法について説明します。
exl-id: 56708a66-f654-413a-80ed-1865077b3c0a
source-git-commit: 717f6f2fb5e07213fb6a16f7ed701f450d1e257e
workflow-type: tm+mt
source-wordcount: '559'
ht-degree: 73%

---

# クエリモデラーの操作 {#segment-builder}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card5"
>title="新しいクエリモデラー"
>abstract="Adobe Campaign Web にはクエリモデラーが備わっています。これにより、データベースをフィルタリングして様々な基準に基づいて特定のターゲットを選択するプロセスが簡素化されます。これには、高度な式と演算子の使用が含まれます。クエリモデラーは、データをフィルタリングするルールを定義する必要があるすべてのコンテキストで使用できます。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_querymessage"
>title="クエリモデラー"
>abstract="データベースから受信者やその他のターゲティングディメンションのフィルタリング条件を定義します。Adobe Experience Platform オーディエンスを活用して、ターゲットオーディエンスをさらに絞り込んで、キャンペーンの効果を最大化します。"

Adobe Campaign Web ユーザーインターフェイスには、様々な基準に基づいてデータベースをフィルタリングするプロセスを簡素化するクエリモデラーが備わっています。これにより、クライアントコンソールで作成したクエリとの完全な互換性が確保され、web ユーザーインターフェイスへのシームレスなトランジションが簡単になります。

また、クエリモデラーは非常に複雑で長いクエリを効率的に管理できるので、柔軟性と精度が向上します。さらに、条件内で定義済みフィルターをサポートしているので、包括的なオーディエンスのターゲティングとセグメント化戦略に高度な式と演算子を利用しながら、クエリを簡単に絞り込むことができます。

## クエリモデラーへのアクセス

クエリモデラーは、データをフィルタリングするルールを定義する必要があるすべてのコンテキストで使用できます。

| 使用状況 | 例 |
|  ---  |  ---  |
| **オーディエンスの定義**：メッセージまたはワークフローのターゲットにする母集団を指定し、必要に応じて容易に新しいオーディエンスを作成します。 [オーディエンスの構築方法を説明します。](../audience/one-time-audience.md) | ![](assets/access-audience.png){zoomable=&quot;yes&quot;}{width="200" align="center" zoomable="yes"} |
| **ワークフローアクティビティのカスタマイズ**：ワークフローアクティビティ内でのルールの適用（例： ） **分割** および **紐づけ**&#x200B;を使用して、特定の要件に合わせます。 [ワークフローアクティビティの詳細を説明します](../workflows/activities/about-activities.md) | ![](assets/access-workflow.png){zoomable=&quot;yes&quot;}{width="200" align="center" zoomable="yes"} |
| **定義済みフィルター**：データリストの操作や配信のオーディエンスの形成など、様々なフィルタリング操作でのショートカットとして機能する定義済みフィルターを作成します。 [定義済みフィルターの操作方法の詳細情報](../get-started/predefined-filters.md) | ![](assets/access-predefined-filter.png){zoomable=&quot;yes&quot;}{width="200" align="center" zoomable="yes"} |
| **レポートデータをフィルタリング**：レポートに表示されるデータをフィルターするルールを追加します。 [レポートの操作方法を説明します。](../reporting/gs-reports.md) | ![](assets/access-reports.png){zoomable=&quot;yes&quot;}{width="200" align="center" zoomable="yes"} |
| **リストのカスタマイズ**：リストに表示されるデータ（受信者、配信リストなど）をフィルターするカスタムルールを作成します。 [リストをフィルターする方法を説明します](../get-started/list-filters.md#list-built-in-filters) | ![](assets/access-lists.png){zoomable=&quot;yes&quot;}{width="200" align="center" zoomable="yes"} |
| **条件付きコンテンツの作成**：様々な受信者に表示するコンテンツを定義する条件を作成することで、E メールコンテンツを動的にします。これにより、パーソナライズされた、関連性の高いメッセージを確実に作成できます。 [条件付きコンテンツの作成方法を説明します](../personalization/conditions.md) | ![](assets/conditional-content.png){width="200" align="center" zoomable="yes"} |

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
