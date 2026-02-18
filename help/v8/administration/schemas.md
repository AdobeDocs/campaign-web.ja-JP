---
title: スキーマについて
description: スキーマの操作方法について説明します。
exl-id: 1433a441-1673-45a2-9fec-be9550fbba0d
source-git-commit: 28f7bcf5f65671136be25c79b414f149532b749f
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 42%

---

# スキーマについて {#schemas}

>[!CONTEXTUALHELP]
>id="acw_schema"
>title="スキーマ"
>abstract="Adobe Campaignでは、XML ベースのスキーマを使用して、アプリケーション内のデータの物理的および論理的構造を定義します。 この画面では、既存のすべてのスキーマを表示したり、スキーマの詳細にアクセスしたり、カスタムフォームを設定したり、web ユーザーインターフェイスから直接スキーマを作成または拡張したりできます。"

**[!DNL Adobe Campaign]** は、XML ベースのスキーマを使用して、アプリケーション内のデータの物理的および論理的構造を定義します。スキーマは、次を定義するデータベーステーブルにリンクされた XML ドキュメントです。

* テーブル名、フィールド、関係を含む SQL テーブル構造。
* 要素、属性、階層、タイプ、デフォルト値、ラベルを含む XML データ構造。

スキーマは、次の点で重要な役割を果たします。

* データベーステーブルへのアプリケーションデータのマッピング。
* データオブジェクト間の関係の定義。
* 各フィールドの構造とプロパティの指定。

Adobe Campaign の各エンティティには専用のスキーマがあり、データの一貫性と整理を確保します。

スキーマインターフェイスを使用すると、次のことができます。

* [ スキーマへのアクセスとカスタマイズ ](schemas-browse-access.md) – 使用可能なスキーマを表示し、その詳細を参照して、画面表示をカスタマイズします
* [ リスト列を設定 ](schemas-list-columns.md) - リスト表示にデフォルトで表示される列を設定します。
* [ カスタムフィールドの編集 ](schemas-custom-fields.md) – 詳細画面に表示するカスタムフィールドを設定し、セクションに整理します。
* [ コレクションリストの追加 ](schemas-collection-lists.md) - コレクションリストを追加して、プロファイル画面に関連データを表示します。
* [ スキーマの作成と管理 ](schemas-create-publish.md#create-schemas) – 新しいスキーマを作成し、既存のスキーマを拡張します
* [ スキーマの公開と同期 ](schemas-create-publish.md#publish) - スキーマの変更をデータベース構造と同期します。
* [ カスタムフォームの操作 ](schemas-custom-forms.md) - データ入力フォームを使用して、カスタムスキーマのレコードを作成、編集、管理します。

>[!NOTE]
>
>スキーマを管理するには、管理者権限が必要です。

スキーマについて詳しくは、[Campaign コンソールドキュメント](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"}を参照してください。
