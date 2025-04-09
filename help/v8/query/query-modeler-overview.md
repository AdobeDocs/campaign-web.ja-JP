---
audience: end-user
title: クエリモデラーの操作
description: Adobe Campaign Web クエリモデラーの操作方法について説明します。
exl-id: 56708a66-f654-413a-80ed-1865077b3c0a
source-git-commit: bf7ee45a0702b66af6962453893cf9c50c140d54
workflow-type: tm+mt
source-wordcount: '689'
ht-degree: 91%

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

>[!CONTEXTUALHELP]
>id="acw_deliveries_refine_target"
>title="ターゲットを絞り込む"
>abstract="これらのルールは、デスクトップコンソールでのみ変更できます。"

Adobe Campaign Web ユーザーインターフェイスには、様々な基準に基づいてデータベースをフィルタリングするプロセスを簡素化するクエリモデラーが備わっています。これにより、クライアントコンソールで作成したクエリとの完全な互換性が確保され、web ユーザーインターフェイスへのシームレスなトランジションが簡単になります。

また、クエリモデラーは非常に複雑で長いクエリを効率的に管理できるので、柔軟性と精度が向上します。さらに、条件内で定義済みフィルターをサポートしているので、包括的なオーディエンスのターゲティングとセグメント化戦略に高度な式と演算子を利用しながら、クエリを簡単に絞り込むことができます。

## クエリモデラーへのアクセス

クエリモデラーは、データをフィルタリングするルールを定義する必要があるすべてのコンテキストで使用できます。

| 使用状況 | 例 |
|  ---  |  ---  |
| **オーディエンスの定義**：メッセージやワークフローでターゲットにする母集団を指定し、ニーズに合わせて新しいオーディエンスを簡単に作成します。[詳しくは、オーディエンスの作成方法を参照してください。](../audience/one-time-audience.md) | ![](assets/access-audience.png){zoomable="yes"}{width="200" align="center" zoomable="yes"}{zoomable=&quot;yes&quot;}{width=&quot;200&quot; align=&quot;center&quot; zoomable=&quot;yes&quot;} |
| **ワークフローアクティビティのカスタマイズ**：特定の要件に合わせて、**分割**&#x200B;や&#x200B;**紐付け**&#x200B;などのワークフローアクティビティ内にルールを適用します。[詳しくは、ワークフローアクティビティを参照してください。](../workflows/activities/about-activities.md) | ![](assets/access-workflow.png){zoomable="yes"}{width="200" align="center" zoomable="yes"}{zoomable=&quot;yes&quot;}{width=&quot;200&quot; align=&quot;center&quot; zoomable=&quot;yes&quot;} |
| **定義済みフィルター**：データリストの操作や配信のオーディエンスの形成など、様々なフィルタリング操作中にショートカットとして機能する定義済みフィルターを作成します。[詳しくは、定義済みフィルターの操作方法を参照してください。](../get-started/predefined-filters.md) | ![](assets/access-predefined-filter.png){zoomable="yes"}{width="200" align="center" zoomable="yes"}{zoomable=&quot;yes&quot;}{width=&quot;200&quot; align=&quot;center&quot; zoomable=&quot;yes&quot;} |
| **レポートデータのフィルタリング**：レポートに表示されるデータをフィルタリングするルールを追加します。[詳しくは、レポートの操作方法を参照してください。](../reporting/gs-reports.md) | ![](assets/access-reports.png){zoomable="yes"}{width="200" align="center" zoomable="yes"}{zoomable=&quot;yes&quot;}{width=&quot;200&quot; align=&quot;center&quot; zoomable=&quot;yes&quot;} |
| **リストのカスタマイズ**：受信者、配信リストなどのリストに表示されるデータをフィルタリングするカスタムルールを作成します。[詳しくは、リストをフィルターする方法を参照してください。](../get-started/list-filters.md#list-built-in-filters) | ![](assets/access-lists.png){zoomable="yes"}{width="200" align="center" zoomable="yes"}{zoomable=&quot;yes&quot;}{width=&quot;200&quot; align=&quot;center&quot; zoomable=&quot;yes&quot;} |
| **条件付きコンテンツの作成**：様々な受信者に表示するコンテンツを定義する条件を作成することで、メールコンテンツを動的にします。これにより、パーソナライズされた、関連性の高いメッセージを確実に作成できます。[詳しくは、条件付きコンテンツの作成方法を参照してください。](../personalization/conditions.md) | ![](assets/conditional-content.png){width="200" align="center" zoomable="yes"}{width=&quot;200&quot; align=&quot;center&quot; zoomable=&quot;yes&quot;} |

>[!NOTE]
>
>オーディエンスや定義済みフィルターなどのルールが適用されているクライアントコンソールで作成したオブジェクトにアクセスすると、「**[!UICONTROL ターゲットを絞り込む]**」セクションが表示される場合があります。つまり、ルールのターゲットを絞り込むために追加のパラメーターが設定されています。これらのパラメーターは、コンソールでのみ変更できます。
>
>![](assets/target-warning.png){zoomable="yes"}{zoomable=&quot;yes&quot;}

## クエリモデラーインターフェイス {#interface}

>[!CONTEXTUALHELP]
>id="acw_rule_builder_switch_button"
>title="新しいユーザーエクスペリエンス"
>abstract="Use this toggle to switch between the classic query modeler and the new rule builder experience."

クエリモデラーは、クエリを作成する中央のキャンバスと、クエリに関する情報を示す右側のパネルを提供します。

![](assets/query-interface.png){zoomable="yes"}{zoomable=&quot;yes&quot;}

### 中央のキャンバス {#canvas}

クエリモデラーの中央のキャンバスでは、クエリを作成する様々なコンポーネントを追加して組み合わせます。[クエリの作成方法を学ぶ](build-query.md)

キャンバスの右上隅にあるツールバーには、クエリコンポーネントを簡単に操作し、キャンバス内を移動するオプションが表示されます。

* **複数選択モード**：複数のフィルタリングコンポーネントを選択して、選択した場所にコピー＆ペーストします。
* **回転**：キャンバスを垂直方向に切り替えます。
* **画面に合わせる**：キャンバスのズームレベルを画面に合わせて調整します。
* **ズームアウト**／**ズームイン**：キャンバスをズームアウトまたはズームインします。
* **マップを表示**：現在の位置を示すキャンバスのスナップショットを開きます。

### ルールのプロパティパネル {#rule-properties}

右側にある&#x200B;**[!UICONTROL ルールのプロパティ]**&#x200B;パネルには、クエリに関する情報が表示されます。これにより、様々な操作を実行してクエリを確認し、ニーズに合うことを確認できます。このパネルは、オーディエンスを作成するクエリを作成する際に表示されます。[クエリを確認および検証する方法を学ぶ](build-query.md#check-and-validate-your-query)
