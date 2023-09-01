---
audience: end-user
title: Adobe Campaign Web でのワークフローの作成
description: Adobe Campaign Web を使用してワークフローを作成する方法
badge: label="ベータ版"
exl-id: 26e7360e-cce7-4240-bb29-1dc8613f55ca
source-git-commit: 9fb4a5057ec05877ffbadc85d1198ab24faf8972
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 100%

---


# ワークフローの作成 {#create-first-workflow}

>[!CONTEXTUALHELP]
>id="acw_workflow_creation_properties"
>title="ワークフローのプロパティ"
>abstract="この画面で、ワークフローの作成に使用するテンプレートを選択し、ラベルを指定します。 「その他のオプション」セクションを展開して、ワークフロー保存フォルダーやタイムゾーンなどの特定の設定を指定します。"

Campaign v8 Web でワークフローを作成する最初の手順は、ワークフローをスタンドアロンワークフローとして作成するか、キャンペーン内で直接作成し、その一般的なプロパティを定義することです。それには、次の手順に従います。

1. まず、スタンドアロンワークフローを作成するか、キャンペーン内に直接統合するかを決定します。

   * **スタンドアロンワークフロー**：ワークフローメニューに移動し、右上隅の「ワークフローを作成」ボタンをクリックします。
   * **キャンペーンワークフロー：**&#x200B;キャンペーンメニューに移動し、新しいワークフローを作成するキャンペーンを開きます。 「ワークフロー」タブの右上隅にある「ワークフローを作成」ボタンをクリックします。

   ワークフローのプロパティダイアログボックスが表示されます。

   ![](assets/workflow-create.png)

1. ワークフローの作成に使用するテンプレートを選択し、ワークフローのラベルを指定します。

   ワークフローテンプレートには、新しいワークフローの作成に再利用できる、事前に設定されたアクティビティと全体的なプロパティ設定が含まれています。これらはクライアントコンソールから作成されます。[テンプレートの使用方法を学ぶ](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/build-a-workflow.html?lang=ja#workflow-templates)

1. 「**[!UICONTROL その他のオプション]**」のセクションを展開して、保存フォルダーやタイムゾーンなど、ワークフローの特定の設定を指定します。[ワークフローのプロパティを設定する方法を学ぶ](workflow-settings.md)

1. 「**[!UICONTROL ワークフローを作成]**」ボタンをクリックして、ワークフローの作成を確定します。

ワークフローを作成したら、専用の視覚的なキャンバスで実行される様々なタスクの調整を開始できます。[ワークフローアクティビティの調整方法については、こちらを参照してください](orchestrate-activities.md)
