---
audience: end-user
title: 重複排除ワークフローアクティビティの使用
description: 重複排除ワークフローアクティビティの使用方法を説明します
badge: label="Beta"
source-git-commit: bbb22de6ff1398dbb1431f51a55350d206b4690a
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 26%

---


# 重複の除外 {#deduplication}

<!--
>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="Fork activity"
>abstract="The Deduplication activity allows you to..."
-->

The **重複排除** アクティビティは **ターゲット設定** アクティビティ。 このアクティビティでは、インバウンドアクティビティの結果から重複を削除できます。 The **重複排除** 「 」アクティビティは、通常、ターゲティングアクティビティの後、およびターゲットデータを使用できるアクティビティの前に使用されます。

## 設定

次の手順に従って、 **スケジューラ** アクティビティ：

1. を追加します。 **重複排除** アクティビティをワークフローに追加します。

   ![](../assets/workflow-deduplication.png)

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
   * **式の使用**：入力した式の値が最小または最大のレコードを保持できます。 ++式++並べ替え
   * **値のリストの使用**：1 つまたは複数のフィールドの優先度の値を定義します。値を定義するには、 **属性** フィールドを選択したり式を作成したりする場合は、該当するテーブルに値を追加します。 新しいフィールドを定義するには、値のリストの上の「新規」ボタンをクリックします。++ 並べ替え

1. 残りの母集団を利用するには、「**補集合を生成**」オプションをチェックします。補集合はすべての重複から構成されます。その後、追加のトランジションがアクティビティに追加されます。

## 例

