---
audience: end-user
title: データ更新ワークフローアクティビティの使用
description: データ更新ワークフローアクティビティの使用方法について学ぶ
exl-id: db978482-43f6-48a7-8d8d-4b921eb610b2
source-git-commit: 93ac61808049da6f0d800a19f2baf97946d8612c
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 100%

---

# データの更新 {#update-data}

**データ更新**&#x200B;アクティビティは、**データ管理**&#x200B;アクティビティのひとつで、データベース内のフィールドに対して一括更新を実行できます。データ更新は、いくつかのオプションを使用してパーソナライズすることができます。

<!--
The **Operation type** field lets you choose the process to be carried out on the data in the database. Select the first option to add data or update (it if it has already been added). You can also only add data, only update data, or delete data. Select the **Update and merge collections** to select a primary record to link duplicates to, and delete those duplicates safely

Specify how to identify the records in the database: if data relate to an existing targeting dimension, select the **Using the targeting dimension** option and select the targeting dimension and fields to update. Otherwise, specify one or more custom links to identify the data in the database, or direct use of reconciliation keys.

Select the fields to update and reconciliation settings. You can use the **Auto-mapping** option to automatically identify the fields to be updated.

The **Advanced options** section let you specify additional settings to manage data and duplicates.

Toggle the **Generate an outbound transition** option to add an outbound transition that will be activated at the end of the execution of the **Update data** activity. The update generally marks the end of a targeting workflow and therefore the option is not activated by default.

Toggle the **Generate an outbound transition for rejects** option to add an outbound transition containing records that have not been correctly processed after the update (for example if there is a duplicate). The update generally marks the end of a targeting workflow and therefore the option is not activated by default.
-->

## データ更新アクティビティの設定{#update-data-configuration}

**データ更新**&#x200B;アクティビティをを設定するには、まずアクティビティをワークフローに追加してラベルを定義します。

![](../assets/workflow-update-data.png)

### 操作のタイプ

「**操作のタイプ**」フィールドで、データベース内のデータに実行する処理を選択します。

* **挿入または更新**：データを挿入するか、データベースに既にレコードが存在する場合は更新します。
* **挿入**：データのみ挿入します。既に存在するレコードは更新されません。紐付け条件が定義されている場合は、紐付けされていないレコードのみ追加されます。
* **更新**：データベースに既に存在するレコードのみを更新します。
* **削除**：データを削除する場合。

「**バッチサイズ**」フィールドで、更新するインバウンドトランジション要素の数を選択できます。例えば 500 を選択すると、処理される最初の 500 レコードが更新されます。

### レコード識別

このセクションでは、データベース内のレコードを識別する方法を指定できます。

* データエントリが既存のターゲティングディメンションに関係する場合は、「**ターゲティングディメンションを使用**」オプションを選択し、「**更新するターゲティングディメンション**」フィールドで、そのターゲティングディメンションを選択します。
* また、「**カスタムリンクの使用**」を選択し、データベース内のデータを識別できる 1 つ以上のリンクを指定することもできます。
* 選択した操作タイプに更新が必要な場合は、「**紐付けルールの使用**」オプションを使用する必要があります。

### 更新するフィールド

「**更新するフィールド**」セクションで、更新を適用するフィールドを追加し、必要に応じて条件を追加して、更新を実行します。そのためには、「**次の場合に考慮**」フィールドを使用します。条件はリスト順に順番に適用されます。更新の順序を変更するには、右側の矢印を使用します。同じ宛先フィールドを何度も使用できます。

「**自動マッピング**」ボタンを使用すると、フィールドを自動的にリンクできます。自動リンクでは、同じ名前のフィールドが検出されます。

操作タイプの&#x200B;**挿入または更新**&#x200B;中に、各フィールドに適用する操作を個別に選択できます。それには、「**操作タイプ**」フィールドで目的の値を選択します。

### 詳細オプション

「**詳細オプション**」で、データを更新し、重複データを管理するための追加オプションを指定できます。

<!--
* **Disable automatic key management**
* **Disable audit**
* **Empty the destination value if the source value is empty**
* **Update all columns with matching names**
* **Ignore records which concern the same target**: only the first in the list of expressions will be considered
-->

次に示す最後の 2 つのオプションを使用すると、特定のアクションを実行できます。

* **アウトバウンドトランジションを生成**：実行の終了時にアクティブ化されるアウトバウンドトランジションを作成します。通常は、更新によってターゲティングワークフローの終了が示されるので、このオプションはデフォルトでは有効化されません。

* **却下に対するアウトバウンドトランジションを生成**：更新後に（例えば、重複レコードが存在するなどで）正しく処理されなかったレコードを含むアウトバウンドトランジションを作成します。通常は、更新によってターゲティングワークフローの終了が示されるので、このオプションはデフォルトではアクティブ化されません。
