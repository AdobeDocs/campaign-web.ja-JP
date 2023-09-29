---
audience: end-user
title: 分岐ワークフローアクティビティの使用
description: 分岐ワークフローアクティビティの使用方法を学ぶ
badge: label="Beta"
source-git-commit: dfd3c62a8eeb6be3e5e63e7a1fdf352c280adbd0
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 100%

---


# 分岐 {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork"
>title="分岐アクティビティ"
>abstract="**分岐**&#x200B;アクティビティを使用すると、アウトバウンドトランジションを作成して、複数のアクティビティを同時に開始できます。"


>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="分岐アクティビティのトランジション"
>abstract="デフォルトでは、**分岐**&#x200B;アクティビティで 2 つのトランジションが作成されます。「**トランジションを追加**」ボタンをクリックして追加のアウトバウンドトランジションを定義し、そのラベルを入力します。"

**分岐**&#x200B;アクティビティは&#x200B;**フロー制御**&#x200B;アクティビティです。アウトバウンドトランジションを作成して、複数のアクティビティを同時に開始できます。

## 分岐アクティビティの設定{#fork-configuration}

次の手順に従って、**分岐**&#x200B;アクティビティを設定します。

![](../assets/workflow-fork.png)

1. **分岐**&#x200B;アクティビティをワークフローに追加します。
1. **トランジションを追加**&#x200B;をクリックし、新しいアウトバウンドトランジションを追加します。デフォルトでは、2 つのトランジションが定義されています。
1. 各トランジションにラベルを追加します。

## 例{#fork-example}

次の例では、2 つの&#x200B;**分岐**&#x200B;アクティビティを使用しています。

* 2 つのクエリの前にある 1 つのクエリは、同時に実行されます。
* 積集合の後の 1 つは、ターゲット母集団にメールと SMS を同時に送信します。

![](../assets/workflow-fork-example.png)

