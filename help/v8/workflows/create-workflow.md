---
audience: end-user
title: Adobe Campaign Web でのワークフローの作成
description: Adobe Campaign Web を使用してワークフローを作成する方法
badge: label="Alpha" type="Positive"
exl-id: 26e7360e-cce7-4240-bb29-1dc8613f55ca
source-git-commit: 5c3e76ae3c28908144a219d77d82a1b868cdbbdc
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 14%

---


# ワークフローの作成 {#create-first-workflow}

>[!CONTEXTUALHELP]
>id="acw_workflow_creation_properties"
>title="ワークフローのプロパティ"
>abstract="未定"

Campaign v8 Web でワークフローを作成する最初の手順は、ワークフローをスタンドアロンワークフローとして、またはキャンペーン内で直接作成し、その一般的なプロパティを定義することです。 それには、次の手順に従います。

1. まず、スタンドアロンワークフローを作成するか、キャンペーン内に直接統合するかを決定します。

   * **スタンドアロンワークフロー**:ワークフローメニューに移動し、右上隅の「ワークフローを作成」ボタンをクリックします。
   * **キャンペーンワークフロー：** キャンペーンメニューに移動し、新しいワークフローを作成するキャンペーンを開きます。 「ワークフロー」タブの右上隅にある「ワークフローを作成」ボタンをクリックします。

   ワークフローのプロパティダイアログボックスが表示されます。

   ![](assets/workflow-create.png)

1. ワークフローの作成に使用するテンプレートを選択し、ワークフローのラベルを指定します。

   ワークフローテンプレートには、事前に設定されたアクティビティと、新しいワークフローの作成に再利用できる全体的なプロパティ設定が含まれています。 クライアントコンソールから作成されます。 [テンプレートの使用方法を説明します。](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/build-a-workflow.html#workflow-templates)

1. 保存フォルダーやタイムゾーンなど、ワークフローに固有の設定を行う場合は、「追加オプション」セクションを展開します。 [ワークフローのプロパティを設定する方法を説明します](workflow-settings.md)

1. 「ワークフローを作成」ボタンをクリックして、ワークフローの作成を確定します。

ワークフローを作成したら、専用のビジュアルキャンバスを使用して、実行する様々なタスクのオーケストレーションを開始できます。 [ワークフローアクティビティの調整方法については、こちらを参照してください](orchestrate-activities.md)
