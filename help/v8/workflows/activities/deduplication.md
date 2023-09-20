---
audience: end-user
title: 重複排除ワークフローアクティビティの使用
description: 重複排除ワークフローアクティビティの使用方法を説明します
badge: label="Beta"
source-git-commit: d79828c19803b21e8414b8251388f694c465fd80
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 15%

---


# 重複の除外 {#deduplication}

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="重複を識別するためのフィールド"
>abstract="Adobe Analytics の **重複を識別するためのフィールド** セクションで、 **属性を追加** ボタンを使用して、E メールアドレス、名、姓など、同一の値を使用して重複を識別できるフィールドを指定します。 フィールドの順序を使用すると、最初に処理するフィールドを指定できます。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication"
>title="重複排除 — 重複アクティビティ"
>abstract="The **重複排除** 「 」アクティビティでは、インバウンドアクティビティの結果から重複を削除できます。 主に、ターゲティングアクティビティの後、およびターゲットデータを使用できるアクティビティの前に使用されます。"


>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="補集合を生成"
>abstract="残りの母集団が重複として除外された、追加のアウトバウンドトランジションを生成できます。 これをおこなうには、 **補集合を生成** オプション"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="重複排除設定"
>abstract="受信データ内の重複を削除するには、以下のフィールドで重複排除方法を定義します。 デフォルトでは、1 つのレコードのみが保持されます。 また、式または属性に基づいて重複排除モードを選択する必要があります。 デフォルトでは、重複から除外するレコードはランダムに選択されます。"

The **重複排除** アクティビティは **ターゲット設定** アクティビティ。 このアクティビティでは、受信者リストに重複したプロファイルなど、インバウンドアクティビティの結果から重複を削除できます。 The **重複排除** 「 」アクティビティは、通常、ターゲティングアクティビティの後、およびターゲットデータを使用できるアクティビティの前に使用されます。

## 重複排除 — 重複アクティビティの設定{#deduplication-configuration}

次の手順に従って、 **重複排除** アクティビティ：

![](../assets/workflow-deduplication.png)

1. を追加します。 **重複排除** アクティビティをワークフローに追加します。

1. Adobe Analytics の **重複を識別するためのフィールド** セクションで、 **属性を追加** ボタンを使用して、E メールアドレス、名、姓など、同一の値を使用して重複を識別できるフィールドを指定します。 フィールドの順序を使用すると、最初に処理するフィールドを指定できます。

1. 一意の数を選択 **保持する重複**. このフィールドのデフォルト値は 1 です。値 0 を指定すると、すべての重複を保持できます。

<!--
    For example, if records A and B are considered duplicates of record Y, and a record C is considered as a duplicate of record Z:

    * If the value of the field is 1: only the Y and Z records are kept.
    * If the value of the field is 0: all the records are kept.
    * If the value of the field is 2: records C and Z are kept and two records from A, B, and Y are kept, by chance or depending on the deduplication method selected thereafter.

-->

1. を選択します。 **重複排除メソッド** 次を使用します。

   * **ランダム選択**：重複に含めないレコードがランダムに選択されます。
   * **式の使用**：入力した式の値が最小または最大のレコードを保持できます。
   * **値のリストの使用**：1 つまたは複数のフィールドの優先度の値を定義します。値を定義するには、 **属性** フィールドを選択したり式を作成したりする場合は、該当するテーブルに値を追加します。 新しいフィールドを定義するには、値のリストの上の「新規」ボタンをクリックします。

1. 残りの母集団を利用するには、「**補集合を生成**」オプションをチェックします。補集合はすべての重複から構成されます。その後、追加のトランジションがアクティビティに追加されます。

## 例{#deduplication-example}

次の例では、配信を送信する前に、重複排除 — 重複アクティビティを使用して、ターゲットから重複を除外します。 識別された重複した受信者は、必要に応じて再利用できる専用オーディエンスに追加されます。 を選択します。 **電子メール** 重複を特定するアドレス。 1 つのエントリを保持し、 **ランダム** 重複排除メソッド。

![](../assets/workflow-deduplication-example.png)
