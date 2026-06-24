---
title: スキーマについて
description: スキーマの操作方法について説明します。
exl-id: 1433a441-1673-45a2-9fec-be9550fbba0d
TQID: https://experienceleague.adobe.com/D7gEyOdvyADCac9T3By3KKnx7kpN8LuE2-rnRBJDyMA
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2: id: b82389f8-9b5e-4083-8e3b-3cef299fb8b9
subfeature_v2: id: cfc95e9b-b035-4403-a6a9-b27a8a053a37
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 5a231f1dc49379d1be5d36e1732660111f851649
workflow-type: ht
source-wordcount: 319
ht-degree: 100%

---

# スキーマについて {#schemas}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="スキーマのオーサリング"
>abstract="Campaign web ユーザーインターフェイスから直接スキーマを作成および管理できるようになりました。 新しいテーブルの作成、既存のスキーマの拡張、カスタムフォームの作成ができます。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=ja" text="リリースノートを参照してください"

>[!CONTEXTUALHELP]
>id="acw_schema"
>title="スキーマ"
>abstract="Adobe Campaign は、XML ベースのスキーマを使用して、アプリケーション内のデータの物理構造と論理構造を定義します。 この画面から、既存のすべてのスキーマを表示し、スキーマの詳細にアクセスし、カスタムフォームを設定して、web ユーザーインターフェイスから直接スキーマを作成または拡張できます。"

**[!DNL Adobe Campaign]** は、XML ベースのスキーマを使用して、アプリケーション内のデータの物理的および論理的構造を定義します。 スキーマは、次を定義するデータベーステーブルにリンクされた XML ドキュメントです。

* テーブル名、フィールド、関係を含む SQL テーブル構造。
* 要素、属性、階層、タイプ、デフォルト値、ラベルを含む XML データ構造。

スキーマは、次の点で重要な役割を果たします。

* データベーステーブルへのアプリケーションデータのマッピング。
* データオブジェクト間の関係の定義。
* 各フィールドの構造とプロパティの指定。

Adobe Campaign の各エンティティには専用のスキーマがあり、データの一貫性と整理を確保します。

スキーマインターフェイスを使用すると、次のことが可能になります。

* [スキーマへのアクセスとカスタマイズ](schemas-browse-access.md) – 使用可能なスキーマを表示し、その詳細を確認して、画面表示をカスタマイズします
* [リスト列の設定](schemas-list-columns.md) - リスト表示にデフォルトで表示される列を設定します。
* [カスタムフィールドを編集](schemas-custom-fields.md) – 詳細画面に表示するカスタムフィールドを設定し、セクションに整理します。
* [コレクションリストを追加](schemas-collection-lists.md) - コレクションリストを追加して、プロファイル画面に関連データを表示します。
* [スキーマの作成と管理](schemas-create-publish.md#create-schemas) – 新しいスキーマを作成して、既存のスキーマを拡張します
* [スキーマの公開と同期](schemas-create-publish.md#publish) - スキーマの変更をデータベース構造と同期します。
* [カスタムフォームの操作](schemas-custom-forms.md) - データ入力フォームを使用して、カスタムスキーマのレコードを作成、編集、管理します。

>[!NOTE]
>
>スキーマを管理するには、管理者権限が必要です。

スキーマについて詳しくは、[Campaign コンソールドキュメント](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"}を参照してください。
