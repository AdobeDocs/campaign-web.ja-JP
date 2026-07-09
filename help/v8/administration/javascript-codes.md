---
title: JavaScript コードの操作
description: JavaScript コードの操作方法について説明します。
exl-id: 4f3b7fce-0373-4db1-8239-64b1bda0f14c
TQID: https://experienceleague.adobe.com/MEB6-W3pMbt97vozcG7sKjyFLHzLqTs3D0B9JjU44hw
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: fa12c9e0408d36e41e87ce4caa306671b433d186
workflow-type: tm+mt
source-wordcount: 611
ht-degree: 78%

---

# JavaScript コードの操作 {#javascript-codes}

>[!CONTEXTUALHELP]
>id="acw_javascript_codes_list"
>title="JavaScript コード"
>abstract="JavaScript コードは、ライブラリと同様に、ワークフロー全体で使用できる再利用可能な関数です。 このリストから、JavaScript コードを作成、変更、複製、または削除できます。"

>[!CONTEXTUALHELP]
>id="acw_javascript_codes_create"
>title="JavaScript コードを作成"
>abstract="JavaScript コードの名前空間、名前、ラベルを定義し、条件と日付の書式設定に使用できる事前定義済みの関数を使用してコンテンツを記述します。 作成した名前空間と名前は変更できません。"

>[!CONTEXTUALHELP]
>id="acw_dynamic_javascript_pages_list"
>title="動的な JavaScript ページ"
>abstract="動的JavaScript ページ（JSSP）を使用すると、カスタム API、書き出し、web アプリケーションロジックなどのURLを介してアクセスしたときに動的コンテンツを生成するサーバーサイドページを構築できます。 このリストから、動的なJavaScript ページを作成、変更、複製、または削除できます。"

>[!CONTEXTUALHELP]
>id="acw_dynamic_javascript_pages_create"
>title="ダイナミックJavaScriptページの作成"
>abstract="動的なJavaScript ページの名前空間、名前、ラベルを定義し、JavaScript コードを使用してコンテンツを記述します。 作成した名前空間と名前は変更できません。"

## JavaScript コードについて {#about}

JavaScript コードを使用すると、ライブラリと同様に、ワークフロー全体で利用できる再利用可能な関数を作成できます。 これらの関数は、左側のナビゲーションパネルの&#x200B;**[!UICONTROL 管理]**／**[!UICONTROL JavaScript コード]**&#x200B;メニューに保存されます。

![使用可能なオプションを示す JavaScript コードリストインターフェイス](assets/javascript-list.png)

JavaScript コードリストから、次の操作を実行できます。

* **コードを複製または削除**：省略記号ボタンをクリックし、目的のアクションを選択します。
* **コードを変更**：コードの名前をクリックしてプロパティを開き、変更を行って保存します。
* **新しい JavaScript コードを作成**：「**[!UICONTROL JavaScript コードを作成]**」ボタンをクリックします。

>[!NOTE]
>
>Adobe Campaign コンソールと web ユーザーインターフェイスでは JavaScript コードメニューの場所が異なりますが、リストは同じで、ミラーのように機能します。

## JavaScript コードの作成 {#create}

JavaScript コードを作成するには、次の手順に従います。

1. **[!UICONTROL JavaScript コード]**&#x200B;メニューに移動し、「**[!UICONTROL JavaScript コードを作成]**」ボタンをクリックします。

1. コードのプロパティを定義します。

   * **[!UICONTROL 名前空間]**：カスタムリソースに関連する名前空間を指定します。 デフォルトでは、名前空間は「cus」ですが、実装によって異なる場合があります。
   * **[!UICONTROL 名前]**：コードの参照に使用する一意の ID。
   * **[!UICONTROL ラベル]**：JavaScript コードリストに表示される説明ラベル。

   ![名前空間、名前、ラベルの各フィールドを示すJavaScript コード作成インターフェイス](assets/javascript-create.png)

   >[!NOTE]
   >
   >作成後は、「**[!UICONTROL 名前空間]**」フィールドと「**[!UICONTROL 名前]**」フィールドを変更することはできません。 変更を行うには、必要に応じてコードを複製し、更新します。
   >
   >Campaign コンソールでは、JavaScript コード名は、これら 2 つのフィールドの連結として表示されます。

1. 「**[!UICONTROL コードを作成]**」ボタンをクリックして、JavaScript コードを定義します。 左側のパネルには、条件と日付の書式設定に関連する定義済みの関数を使用できる 2 つのメニューが表示されます。

   ![定義済みの関数を示す JavaScript コードエディターインターフェイス](assets/javascript-code.png)

1. 「**[!UICONTROL 確認]**」をクリックして、コードを保存します。

1. JavaScript コードの準備が整ったら、「**[!UICONTROL 作成]**」をクリックします。 JavaScript コードをワークフロー全体で使用できるようになりました。

## ワークフローからの JavaScript コードの使用 {#workflow}

### JavaScript コードライブラリの読み込み {#library}

ワークフローで JavaScript コードを参照すると、繰り返しタスクのコードを再書き込みする必要がなくなります。 これらのコードを使用するには、ワークフローの初期化スクリプトに対応するライブラリを読み込みます。 これにより、ワークフローで使用する関数を含むすべてのライブラリを一度に読み込むことができます。

ライブラリを読み込むには、次の手順に従います。

1. ワークフローを開き、「**[!UICONTROL 設定]**」ボタンをクリックします。
1. 「**[!UICONTROL 初期化スクリプト]**」セクションに移動し、「**[!UICONTROL コードを作成]**」をクリックします。

   ![コード作成オプションを示すワークフローの初期化スクリプトインターフェイス](assets/javascript-initialization.png)

1. コード内で次の構文を使用して、ライブラリを読み込みます。

   ```
   loadLibrary("/<namespace>/<name>")
   ```

   * `<namespace>` を、JavaScript コードの作成時に指定した名前空間に置き換えます。
   * `<name>` を JavaScript コードの名前に置き換えます。

1. 「**[!UICONTROL 確認]**」をクリックして、設定を保存します。

### ワークフローの関数の参照 {#reference}

JavaScript ライブラリを読み込むと、通常は **[!UICONTROL JavaScript コード]**&#x200B;アクティビティを使用して、ワークフロー内で JavaScript コードに定義された関数を直接参照できます。

![JavaScript 関数の使用状況を示すワークフローインターフェイス](assets/javascript-function.png)