---
title: Campaign web ユーザーインターフェイスワークフローのガードレールと制限
description: Campaign web ユーザーインターフェイスのワークフローを操作する際のガードレールと制限
exl-id: 9c8c67ce-9823-4082-b0bd-5613f3feb6e3
source-git-commit: c156e4105cab5028249a2a3d5a1838205cac7d35
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 100%

---

# ワークフローのガードレールと制限 {#guardrails-limitations}

Campaign クライアントコンソールで作成または変更されたワークフローを Campaign web ユーザーインターフェイスで使用する場合、以下に示すガードレールと制限が適用されます。

このページでは、コンソールと web ユーザーインターフェイスでワークフローを操作する際の主な考慮事項を特定しますが、2 つのインターフェイス間の潜在的な非互換性がすべて含まれているわけではありません。

## ワークフローアクティビティ {#wkf-activities}

>[!CONTEXTUALHELP]
>id="acw_orchestration_query_enrichment_noneditable"
>title="編集不可のアクティビティ"
>abstract="コンソールで追加のデータを使用して「**クエリ**」アクティビティまたは「**エンリッチメント**」アクティビティを設定する際、エンリッチメントデータは Campaign web で考慮され、アウトバウンドトランジションに渡されますが、編集できません。"

Campaign web ユーザーインターフェイスでまだサポートされていない「ワークフロー」アクティビティは読み取り専用で、互換性のないアクティビティとして表示されます。ワークフローの実行、メッセージの送信、ログの確認などは引き続き実行できます。Campaign web ユーザーインターフェイスと Campaign クライアントコンソールの両方で使用できる「ワークフロー」アクティビティは編集可能です。

| コンソール | Web |
| --- | --- |
| ![](assets/limitations-activities-console.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-activities-web.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} |

コンソールで追加のデータを使用して「**クエリ**」アクティビティまたは「**エンリッチメント**」アクティビティを設定する際、エンリッチメントデータは Campaign web で考慮され、アウトバウンドトランジションに渡されますが、編集できません。

| コンソール | Web |
| --- | --- |
| ![](assets/limitations-options-console.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-options-web.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} |

コンソールで、「**エンリッチメント**」アクティビティは、紐付けとエンリッチメントの両方を実行できます。クライアントコンソールで「**エンリッチメント**」アクティビティの紐付け設定を定義した場合、Campaign web ユーザーインターフェイスでは「**紐付け**」アクティビティとして表示されます。

| コンソール | Web |
| --- | --- |
| ![](assets/limitations-enrichment-console.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-enrichment-web.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} |

## ワークフローキャンバス {#wkf-canvas}

Campaign web ユーザーインターフェイスで新しいワークフローを作成する際、キャンバスは 1 つのエントリポイントのみをサポートします。ただし、複数のエントリポイントを持つワークフローをコンソールで作成した場合は、Campaign web ユーザーインターフェイスで開いて編集できます。

| コンソール | Web |
| --- | --- |
| ![](assets/limitations-multiple-console.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-multiple-web.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} |

ノードの配置は、アクティビティが追加または削除されるたびに更新されます。コンソールでワークフローを作成し、Campaign web ユーザーインターフェイスを使用して変更し、コンソールで再度開くと、配置に関する軽微な問題が発生する場合があります。これは、ワークフローのプロセスとタスクには影響しません。

| 最初のワークフロー | 位置の変更 |
| --- | --- |
| ![](assets/limitations-positioning1.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-positioning2.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} |
