---
audience: end-user
title: フォルダーの操作
description: Adobe Campaign でフォルダーを管理する方法について説明します
exl-id: a4518a21-03cd-46ac-9c40-d181692e1b9b
source-git-commit: 5f9cc8915f2897ebc14d571357773fef057cf9c1
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 100%

---

# フォルダーの操作 {#folders}

>[!CONTEXTUALHELP]
>id="acw_folder_properties"
>title="フォルダーのプロパティ"
>abstract="フォルダーのプロパティ"

>[!CONTEXTUALHELP]
>id="acw_folder_security"
>title="フォルダーのセキュリティ"
>abstract="フォルダーのセキュリティ"

>[!CONTEXTUALHELP]
>id="acw_folder_restrictions"
>title="フォルダーの制限"
>abstract="フォルダーの制限"

>[!CONTEXTUALHELP]
>id="acw_folder_schedule"
>title="フォルダーのスケジュール"
>abstract="フォルダーのスケジュール"

>[!CONTEXTUALHELP]
>id="acw_folder_favorites"
>title="お気に入り"
>abstract="お気に入り"

## フォルダーについて {#about-folders}

フォルダーは、コンポーネントとデータを整理できる Adobe Campaign のオブジェクトです。

ナビゲーションツリーで、フォルダーの作成、名前変更、並べ替え、移動を行うことができます。また、権限に基づいて削除することもできます。

![フォルダー組織を示すフォルダーインターフェイス](assets/folders.png){zoomable="yes"}

フォルダータイプを設定できます。例：配信のフォルダー。フォルダーのアイコンは、タイプに応じて変わります。

## 新しいフォルダーの作成 {#create-a-folder}

Adobe Campaign web UI で新しいフォルダーを作成するには、次の手順に従います。

1. **[!UICONTROL エクスプローラー]**&#x200B;で、新しいフォルダーを作成するフォルダーに移動します。**[!UICONTROL …]** メニューの下で、「**[!UICONTROL 新しいフォルダーを作成]**」を選択します。

![エクスプローラーメニューの「新しいフォルダーを作成」オプション](assets/folder_create.png){zoomable="yes"}

新しいフォルダーを作成すると、フォルダータイプはデフォルトで親フォルダーのタイプになります。この例では、**[!UICONTROL 配信]**&#x200B;フォルダーにフォルダーを作成します。

![配信フォルダーで作成した新しいフォルダー](assets/folder_new.png){zoomable="yes"}

1. 必要に応じてフォルダータイプアイコンをクリックしてフォルダータイプを変更し、以下に示すように、表示されるリストから目的のタイプを選択します。

![フォルダータイプ選択インターフェイス](assets/folder_type.png){zoomable="yes"}

「**[!UICONTROL 確認]**」ボタンをクリックして、フォルダータイプを設定します。

特定のタイプのないフォルダーを作成する場合は、「**[!UICONTROL 汎用フォルダー]**」タイプを選択します。

また、[Adobe Campaign コンソールでフォルダーを作成および管理](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/config/configuration/folders-and-views)することもできます。

## フォルダーを並べ替え {#reorder-folders}

必要に応じて、フォルダーを並べ替えることができます。これを行うには、次に示すように、「**[!UICONTROL フォルダーを並べ替え]**」をクリックします。

この例では、**配信**&#x200B;フォルダーに 4 つのサブフォルダーが含まれています。

![フォルダー階層を示すフォルダーを並べ替えインターフェイス](assets/folder-reorder.png){zoomable="yes"}

フォルダーの順序は、**ドラッグ＆ドロップ**&#x200B;または&#x200B;**上下の矢印**&#x200B;を使用して変更できます。

![フォルダーの並べ替えのドラッグ＆ドロップ機能](assets/folder-draganddrop.png){zoomable="yes"}

## フォルダーの削除 {#delete-a-folder}

>[!CAUTION]
>
>フォルダーを削除すると、そのフォルダーに保存されているすべてのデータも削除されます。

フォルダーを削除するには、**[!UICONTROL エクスプローラー]**&#x200B;ツリーでそのフォルダーを選択し、**[!UICONTROL ...]** メニューをクリックします。「**[!UICONTROL フォルダーを削除]**」を選択します。

![エクスプローラーメニューの「フォルダーを削除」オプション](assets/folder_delete.png){zoomable="yes"}

## フォルダー内の値の配分 {#distribution-values-folder}

値の配分は、テーブル内の列の値の割合を把握するのに役立ちます。

フォルダー内の値の配分を把握するには、次の手順に従います。

例えば、配信間で、**チャネル**&#x200B;列の値の配分を把握するとします。

この情報を取得するには、**[!UICONTROL 配信]**&#x200B;フォルダーに移動し、**[!UICONTROL 列を設定]**&#x200B;アイコンをクリックします。

**[!UICONTROL 列を設定]**&#x200B;ウィンドウで、分析する列に関する&#x200B;**[!UICONTROL 情報]**&#x200B;アイコンをクリックします。次に、「**[!UICONTROL 値の配分]**」ボタンをクリックします。

![配信用の値の配分インターフェイス](assets/values_deliveries.png){zoomable="yes"}

**[!UICONTROL チャネル]**&#x200B;列の値の割合が表示されます。

![チャネル列の値の割合配分](assets/values_percentage.png){zoomable="yes"}

>[!NOTE]
>
>多くの値を持つ列の場合、最初の 20 個の値のみが表示されます。**[!UICONTROL 部分読み込み]**&#x200B;という警告通知が表示されます。

また、リンクの値の配分を表示することもできます。

属性リストで、以下に示すように、目的のリンクの横にある「**+**」ボタンをクリックします。これにより、リンクが&#x200B;**[!UICONTROL 出力列]**&#x200B;に追加されます。**[!UICONTROL 情報]**&#x200B;アイコンにアクセスして、値の配分を表示できるようになりました。**[!UICONTROL 出力列]**&#x200B;にリンクを保持しない場合は、「**[!UICONTROL キャンセル]**」ボタンをクリックします。

![出力列のリンクの値の配分](assets/values_link.png){zoomable="yes"}

クエリモデラーで値の配分を表示することもできます。[詳しくは、こちらを参照してください](../query/build-query.md#distribution-of-values-in-a-query)。

### 値のフィルタリング {#filter-values}

値の配分ウィンドウの&#x200B;**[!UICONTROL 詳細フィルター]**&#x200B;を使用すると、指定した条件に基づいて結果をフィルタリングできます。

チャネルごとの配分を示す上記の配信リストの例では、フィルタリングして、ステータスが&#x200B;**完了**&#x200B;の配信のみを表示できます。

![値の配分に適用される詳細フィルター](assets/values_filter.png){zoomable="yes"}