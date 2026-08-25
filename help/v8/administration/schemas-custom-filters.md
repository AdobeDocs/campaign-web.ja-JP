---
title: カスタムフィルターを追加
description: カスタムフィルターを、リスト表示のフィルターパネルでクイックアクセスフィールドとして追加する方法について説明します。
exl-id: 2c3d4e5f-6a7b-4c8d-9e0f-1a2b3c4d5e6f
source-git-commit: c2e627d322937b80cb0bc09e86680757d4867dcd
workflow-type: ht
source-wordcount: '320'
ht-degree: 100%

---

# カスタムフィルターを追加 {#custom-filters}

**[!UICONTROL 在庫リスト設定]**／**[!UICONTROL カスタムフィルター]**&#x200B;セクションでは、スキーマのリスト表示の[フィルターパネル](../query/filter.md)（**[!UICONTROL 詳細フィルター]**&#x200B;のルールビルダーの上部）でクイックアクセスフィールドとして表示される属性を選択できます。

画面の定義画面とそのアクセス方法について詳しくは、[画面の定義へのアクセス](schemas-browse-access.md#screen-def)の節を参照してください。

## カスタムフィルターを追加 {#add}

1. **[!UICONTROL スキーマ]**&#x200B;メニューを参照し、フィルターを使用して編集可能なスキーマを見つけます。

1. リストでスキーマ名を選択して開き、スキーマ詳細ビューの「**[!UICONTROL 画面の編集]**」をクリックし、画面の定義にアクセスします。

1. 「**[!UICONTROL 在庫リスト設定]**」セクションに移動し、**[!UICONTROL カスタムフィルター]**&#x200B;テーブルの上にある省略記号アイコンをクリックして、「**[!UICONTROL 属性を選択]**」を選択します。

   ![カスタムフィルターの選択](assets/schemas-custom-filters1.png)

1. 1 つまたは複数の属性を選択して確認します。

   次の項目を選択できます。

   * スキーマの直接的な属性（例：コードやカテゴリ）。
   * リンク属性（例：製品にリンクされたブランド）。この場合、フィルターは、リンクされたスキーマに制限された検索ピッカーを使用します。
   * リンクのサブ属性（例：リンクされたフォルダーの完全な名前やリンクされた受信者のメール）。

   ![直接属性とリンクサブ属性を示す属性ピッカー](assets/schemas-custom-filters2.png)

1. 「**[!UICONTROL 保存]**」をクリックします。上下の矢印を使用するか、ドラッグしてカスタムフィルターを並べ替え、その行のごみ箱アイコンを使用してフィルターを削除できます。

1. このスキーマのレコードのリストを参照し、フィルターパネルを開きます。選択した属性は、**[!UICONTROL 詳細フィルター]**&#x200B;ルールビルダーの上に&#x200B;**[!UICONTROL カスタムフィルター]**&#x200B;として表示されます。

   ![フィルターパネルに表示されているカスタムフィルター](assets/schemas-custom-filters3.png)

   >[!NOTE]
   >
   >日付または日時属性に基づくカスタムフィルターは、日付範囲ピッカーとして表示されます。

1. いずれかのカスタムフィルターに値を入力または選択して、リストを絞り込みます。

<!--
## Configure a custom filter's settings {#settings}

To configure specific settings for a custom filter, click the ellipsis icon on its row and select **[!UICONTROL Edit]**.

![Custom filter settings dialog](assets/schemas-custom-filters5.png)

Available settings are:

* **[!UICONTROL Label (custom)]**: The label to display for this filter. If no label is provided, the attribute's label defined in the schema is used.
* **[!UICONTROL Filter settings]** (for link-type custom filters only): Use the query modeler to specify a condition that restricts the values available in the picker. For example, restrict a delivery filter to deliveries using the email channel.
-->