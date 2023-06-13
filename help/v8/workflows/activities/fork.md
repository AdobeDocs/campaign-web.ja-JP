---
audience: end-user
title: 分岐ワークフローアクティビティの使用
description: 分岐ワークフローアクティビティの使用方法を説明します
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 19%

---


# 分岐 {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="分岐 アクティビティ"
>abstract="「分岐」アクティビティを使用すると、アウトバウンドトランジションを作成して、複数のアクティビティを同時に開始できます。"

## 設定

次の手順に従って、 **分岐** アクティビティ：

1. を追加します。 **分岐** アクティビティをワークフローに追加します。
1. クリック **トランジションを追加** 新しいアウトバウンドトランジションを追加する場合。 デフォルトでは、2 つのトランジションが定義されています。
1. 各トランジションにラベルを追加します。

## 例

次の例では、2 つの **分岐** アクティビティ：

* 2 つのクエリの 1 つ前に、同時に実行します。
* 積集合の後 1 つ。ターゲット母集団に E メールと SMS を同時に送信します。

![](../assets/workflow-fork-example.png)

