---
title: 動的な JavaScript ページの操作
description: 動的な JavaScript ページの操作方法について説明します。
exl-id: b7de9f55-2aef-4ba9-a2a1-e9ca15deacfb
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 2df9759bb21eae0630bcbe9130a1a20b165e8cca
workflow-type: tm+mt
source-wordcount: 392
ht-degree: 100%

---

# 動的な JavaScript ページの操作 {#dynamic-javascript-pages}

>[!CONTEXTUALHELP]
>id="acw_dynamic_javascript_pages_list"
>title="動的な JavaScript ページ"
>abstract="動的な JavaScript ページ（JSSP）を使用すると、カスタム API、エクスポート、web アプリケーションロジックなど、URL を通じてアクセスした際に動的コンテンツを生成するサーバーサイドページを作成できます。 このリストから、動的な JavaScript ページを作成、変更、複製または削除できます。"

>[!CONTEXTUALHELP]
>id="acw_dynamic_javascript_pages_create"
>title="動的な JavaScript ページの作成"
>abstract="動的な JavaScript ページの名前空間、名前、ラベルを定義し、JavaScript コードを使用してコンテンツを記述します。 作成後、名前空間と名前は変更できません。"

## 動的な JavaScript ページについて {#about}

動的な JavaScript ページ（JSSP）を使用すると、カスタム API、エクスポート、web アプリケーションロジックなど、URL を通じてアクセスした際に動的コンテンツを生成するサーバーサイドページを作成できます。 これらのページは、左側のナビゲーションパネルの&#x200B;**[!UICONTROL 管理]**／**[!UICONTROL 動的な JavaScript ページ]**&#x200B;メニューに保存されます。

![使用可能なオプションを示す動的な JavaScript ページリストインターフェイス](assets/dynamic-javascript-pages.png)

動的な JavaScript ページリストから、次の操作を実行できます。

* **ページを複製または削除**：省略記号ボタンをクリックし、目的のアクションを選択します。
* **ページを変更**：ページの名前をクリックしてプロパティを開き、変更を加えて保存します。
* **新しい動的な JavaScript ページを作成**：「**[!UICONTROL 動的な JavaScript ページを作成]**」ボタンをクリックします。

<!--
>[!NOTE]
>
>In the Campaign console, dynamic JavaScript pages are available under **[!UICONTROL Administration]** > **[!UICONTROL Configuration]** > **[!UICONTROL Dynamic JavaScript pages]**. Although the menu location differs from the Web user interface, the list is identical and operates like a mirror.
-->

## 動的な JavaScript ページの作成 {#create}

動的な JavaScript ページを作成するには、次の手順に従います。

1. **[!UICONTROL 動的な JavaScript ページ]**&#x200B;メニューに移動し、「**[!UICONTROL 動的な JavaScript ページを作成]**」ボタンをクリックします。

1. ページのプロパティを定義します。

   * **[!UICONTROL 名前空間]**：カスタムリソースに関連する名前空間を指定します。 デフォルトでは、名前空間は「cus」ですが、実装によって異なる場合があります。
   * **[!UICONTROL 名前]**：ページの参照に使用する一意の ID。
   * **[!UICONTROL ラベル]**：動的な JavaScript ページリストに表示される説明ラベル。

   ![名前空間、名前、ラベルの各フィールドを示す動的な JavaScript ページ作成インターフェイス](assets/dynamic-javascript-pages2.png)

   >[!NOTE]
   >
   >作成後は、「**[!UICONTROL 名前空間]**」フィールドと「**[!UICONTROL 名前]**」フィールドを変更することはできません。 変更を行うには、ページを複製し、必要に応じて更新します。

1. 「**[!UICONTROL コードを作成]**」ボタンをクリックしてページのコンテンツを定義し、`<%@ page %>` ディレクティブと `NL.require()` 呼び出しを使用して JSSP コードを記述してコアライブラリを読み込みます。

   ![動的な JavaScript ページコードエディター](assets/dynamic-javascript-pages4.png)

1. 「**[!UICONTROL 確認]**」をクリックして、コードを保存します。

1. 動的な JavaScript ページの準備が整ったら、「**[!UICONTROL 作成]**」をクリックします。 ページには、名前空間と名前から作成された URL（`https://<your-instance>/<namespace>/<name>` 形式）でアクセスできるようになりました。 例えば、`cus` 名前空間の `recipientAPI.jssp` という名前のページには、`https://<your-instance>/cus/recipientAPI.jssp` からアクセスできます。

再利用可能な JavaScript 関数について詳しくは、[JavaScript コードの操作](javascript-codes.md)を参照してください。
