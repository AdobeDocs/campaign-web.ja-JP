---
audience: end-user
title: ワークフロー作成の主な原則
description: Adobe Campaign Web でのワークフローの主な原則について説明します
exl-id: ac6e63fb-34f2-474f-b364-d2af44f649b1
source-git-commit: c156e4105cab5028249a2a3d5a1838205cac7d35
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 100%

---


# ワークフロー作成の主な原則 {#gs-workflow-creation}

Adobe Campaign Web を使用すると、ワークフローを視覚的なキャンバスに作成して、セグメント化、キャンペーン実行、ファイル処理などのクロスチャネルプロセスを設計できます。

## ワークフローの内部とは {#gs-workflow-inside}

ワークフローダイアグラムは、実行される処理を表したものです。これは、実行される様々なタスクと、タスク同士の関係を示すものです。

![](assets/workflow-example.png){zoomable=&quot;yes&quot;} {zoomable=&quot;yes&quot;}

各ワークフローには次が含まれます。

* **アクティビティ**：アクティビティとは、実行されるタスクです。各種アクティビティは、ダイアグラム内にアイコンで示されます。各アクティビティには、特定のプロパティと、すべてのアクティビティに共通のその他のプロパティがあります。

  ワークフローのダイアグラムでは、指定されたアクティビティが、特にループまたは繰り返しアクションがある場合に複数のタスクを生成できます。

* **トランジション**：トランジションは、ソースアクティビティを宛先アクティビティにリンクし、そのシーケンスを定義します。

* **作業用テーブル**：作業用テーブルには、トランジションによって実行されるすべての情報が含まれます。各ワークフローは、複数のワークテーブルを使用します。これらのテーブルで伝達されたデータは、ワークフローのライフサイクルを通じて使用できます。

## ワークフローを作成するための主な手順 {#gs-workflow-steps}


キャンペーンでは、2 つの方法でワークフローを作成できます。

1. ワークフローは、**ワークフロー**&#x200B;メニューからスタンドアロンワークフローとして作成できます。

   ![](assets/create-a-standalone-wf.png){zoomable=&quot;yes&quot;}

1. ワークフローは、キャンペーンの「**ワークフロー**」タブからキャンペーン内で直接作成できます。キャンペーンに含めると、ワークフローは他のすべてのキャンペーンのワークフローと共に実行され、レポート指標はすべてキャンペーンレベルでグループ化されます。

   ![](assets/create-a-wf-from-a-campaign.png){zoomable=&quot;yes&quot;}

ワークフローを作成する主な手順は次のとおりです。

![](assets/workflow-creation-process.png){zoomable=&quot;yes&quot;}

以下の手順については、次の節で詳しく説明します。

1. [ワークフローを作成し、そのプロパティを定義](create-workflow.md)
1. [アクティビティを調整および設定](orchestrate-activities.md)
1. [ワークフローの詳細設定を指定](workflow-settings.md)
1. [ワークフローを開始し、その実行を監視](start-monitor-workflows.md)
