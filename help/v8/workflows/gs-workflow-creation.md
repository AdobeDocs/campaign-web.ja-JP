---
audience: end-user
title: Adobe Campaign Web でのワークフローの作成
description: Adobe Campaign Web を使用してワークフローを作成する方法
badge: label="Alpha" type="Positive"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: 748fef18a91a61f5ed956f65762a979e7dacabf3
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 73%

---


# ワークフロー作成の主な原則 {#gs-workflow-creation}

Campaign v8 Web を使用すると、ワークフローを視覚的なキャンバスに作成して、セグメント化、キャンペーン実行、ファイル処理などのクロスチャネルプロセスを設計できます。

ワークフローは、スタンドアロンのワークフロー、ワークフローメニューから、またはキャンペーン内から直接作成できます。その場合、ワークフローはキャンペーンにリンクされ、他のすべてのキャンペーンのワークフローと共に実行されます。

## ワークフローの内部とは

ワークフローダイアグラムは、実行される処理を表したものです。これは、実行される様々なタスクと、タスク同士の関係を示すものです。

![](assets/workflow-example.png)

各ワークフローには次が含まれます。

* **アクティビティ**：アクティビティとは、実行されるタスクです。各種アクティビティは、ダイアグラム内にアイコンで示されます。各アクティビティには、特定のプロパティと、すべてのアクティビティに共通のその他のプロパティがあります。

   ワークフローのダイアグラムでは、指定されたアクティビティが、特にループまたは繰り返しアクションがある場合に複数のタスクを生成できます。

* **トランジション**：トランジションは、ソースアクティビティを宛先アクティビティにリンクし、そのシーケンスを定義します。

* **作業用テーブル**：作業用テーブルには、トランジションによって実行されるすべての情報が含まれます。各ワークフローは、複数のワークテーブルを使用します。これらのテーブルで伝達されたデータは、ワークフローのライフサイクルを通じて使用できます。

## ワークフローを作成するための主な手順

ワークフローを作成する主な手順は次のとおりです。

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="create-workflow.md#create">
<img alt="リード" src="assets/do-not-localize/workflow-process-1 .jpeg">
</a>
<div><a href="create-workflow.md#create"><strong>ワークフローの作成</strong>
</div>
<p>
</td>
<td>
<a href="create-workflow.md#build">
<img alt="低頻度" src="assets/do-not-localize/workflow-process-2.jpeg">
</a>
<div>
<a href="create-workflow.md#build"><strong>アクティビティの調整</strong></a>
</div>
<p></td>
<td>
<a href="workflow-settings.md">
<img alt="検証" src="assets/do-not-localize/workflow-process-3.jpeg">
</a>
<div>
<a href="workflow-settings.md"><strong>詳細設定（オプション）</strong></a>
</div>
<p>
</td>
<td>
<a href="start-monitor-workflows.md">
<img alt="ワークフローの開始と監視" src="assets/do-not-localize/workflow-process-4.jpeg">
</a>
<div>
<a href="start-monitor-workflows.md"><strong>ワークフローの実行を開始および監視</strong></a>
</div>
<p>
</td>
</tr></table>