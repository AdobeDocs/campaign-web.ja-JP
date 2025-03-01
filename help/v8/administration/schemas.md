---
title: スキーマの操作
description: スキーマの操作方法を説明します。
source-git-commit: 1f3f3afb9b21ab37aeea73057d832cea172c00bf
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 2%

---

# スキーマの操作 {#schemas}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn3"
>title="スキーマの操作"
>abstract="リストで名前を選択して、スキーマの詳細にアクセスできるようになりました。 カスタムフィールド編集には、「**カスタム詳細を編集** ボタンからもアクセスできます。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=ja" text="リリースノートを参照してください"



>[!CONTEXTUALHELP]
>id="acw_schema"
>title="スキーマ"
>abstract="**[!DNL Adobe Campaign]** は、XML ベースのスキーマを使用して、アプリケーション内のデータの物理的および論理的構造を定義します。 この画面から、既存のすべてのスキーマを表示し、リストで名前を選択してスキーマの詳細にアクセスできます。 編集可能なスキーマのみを表示するなど、リストを絞り込むのに役立つフィルターを使用できます。"

## スキーマについて {#about}

**[!DNL Adobe Campaign]** は、XML ベースのスキーマを使用して、アプリケーション内のデータの物理的および論理的構造を定義します。 スキーマは、以下を定義するデータベーステーブルにリンクされた XML ドキュメントです。

* SQL テーブル構造（テーブル名、フィールド、関係）。
* XML データ構造（要素、属性、階層、タイプ、デフォルト値、ラベル）。

スキーマは、次の点で重要な役割を果たします。

* アプリケーション データをデータベース テーブルにマッピングします。
* データオブジェクト間の関係の定義。
* 各フィールドの構造とプロパティを指定します。

Adobe Campaignの各エンティティには専用のスキーマがあり、データの一貫性と整理を確保しています。

スキーマについて詳しくは、[Campaign コンソールドキュメント ](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"} を参照してください。

## Web ユーザーインターフェイスのスキーマへのアクセス {#access}

スキーマは、**[!UICONTROL 管理]**/ **[!UICONTROL スキーマ]** メニューからアクセスできます。

![](assets/schemas-list.png)

この画面から、既存のすべてのスキーマを表示できます。 編集可能なスキーマのみを表示するなど、リストを絞り込むのに役立つフィルターを使用できます。

スキーマを開くには、スキーマの名前を選択します。 詳細なスキーマビューが表示されます。

![](assets/schema-details.png)

### スキーマの概要 {#overview}

「**[!UICONTROL 概要]**」タブには、スキーマの一般的なビューが表示されます。

* **[!UICONTROL プロパティ]** セクションには、スキーマ名、名前空間、関連付けられたテーブル名などの主要な情報が表示されます。

* **[!UICONTROL スキーマ定義]** のセクションには、データの紐付けに使用するプライマリキーや他のテーブルとのリンクなどのスキーマ定義の詳細が表示されます。

  「**[!UICONTROL スキーマプレビュー]**」ボタンをクリックして、スキーマを構成する様々なフィールドおよびリンクを表示します。 これにより、スキーマの完全な構造を確認できます。 スキーマがカスタムフィールドを使用して拡張されている場合は、そのすべての拡張を視覚化できます。

* 「**[!UICONTROL コンテンツ]**」セクションには、スキーマの XML コンテンツが表示され、ソース構文と生成された構文を切り替えることができます。

### スキーマデータ {#data}

「**[!UICONTROL データ]**」タブには、スキーマデータに関する情報が表示されます。

![](assets/schemas-data.png)

## カスタムフィールドの編集 {#fields}

カスタムフィールドは、Adobe Campaign コンソールを通じて標準スキーマに追加される追加の属性です。 組織のニーズに合わせて新しい属性を含めることで、スキーマをカスタマイズできます。

カスタムフィールドは、Campaign web インターフェイスのプロファイルの詳細など、様々な画面に表示できます。 表示するフィールドとインターフェイスでの表示方法を制御できます。 これを行うには、**[!UICONTROL スキーマ]** メニューの **[!UICONTROL カスタム詳細を編集]** ボタンをクリックします。

![](assets/schemas-custom.png)

スキーマでカスタムフィールドを編集する方法について詳しくは、この節 [ カスタムフィールドの設定 ](../administration/custom-fields.md) を参照してください。
