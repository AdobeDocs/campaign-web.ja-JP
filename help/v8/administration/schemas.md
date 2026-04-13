---
title: スキーマについて
description: スキーマの操作方法について説明します。
exl-id: 1433a441-1673-45a2-9fec-be9550fbba0d
source-git-commit: 9b51dc84a5b6954c973e1560aad877ef770eb8f9
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 39%

---

# スキーマについて {#schemas}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="スキーマのオーサリング"
>abstract="Campaign Web ユーザーインターフェイスから直接スキーマを作成および管理できるようになりました。 新しいテーブルを作成したり、既存のスキーマを拡張したり、カスタムフォームを作成したりできます。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=ja" text="リリースノートを参照してください"

>[!CONTEXTUALHELP]
>id="acw_schema"
>title="スキーマ"
>abstract="Adobe Campaignでは、XML ベースのスキーマを使用して、アプリケーション内のデータの物理構造と論理構造を定義します。 この画面では、Web ユーザーインターフェイスから既存のすべてのスキーマの表示、スキーマの詳細へのアクセス、カスタムフォームの設定、スキーマの作成または拡張を直接行うことができます。"

**[!DNL Adobe Campaign]** は、XML ベースのスキーマを使用して、アプリケーション内のデータの物理的および論理的構造を定義します。スキーマは、次を定義するデータベーステーブルにリンクされた XML ドキュメントです。

* テーブル名、フィールド、関係を含む SQL テーブル構造。
* 要素、属性、階層、タイプ、デフォルト値、ラベルを含む XML データ構造。

スキーマは、次の点で重要な役割を果たします。

* データベーステーブルへのアプリケーションデータのマッピング。
* データオブジェクト間の関係の定義。
* 各フィールドの構造とプロパティの指定。

Adobe Campaign の各エンティティには専用のスキーマがあり、データの一貫性と整理を確保します。

スキーマインターフェイスを使用すると、次のことが可能になります。

* [ スキーマへのアクセスとカスタマイズ ](schemas-browse-access.md) – 使用可能なスキーマを表示し、その詳細を確認して、画面表示をカスタマイズします
* [ リスト列の設定](schemas-list-columns.md) - リストビューにデフォルトで表示される列を設定します。
* [ カスタムフィールドを編集](schemas-custom-fields.md) – 詳細画面に表示するカスタムフィールドを設定し、セクションに整理します。
* [ コレクションリストを追加](schemas-collection-lists.md) - コレクションリストを追加して、プロファイル画面に関連データを表示します。
* [ スキーマの作成と管理](schemas-create-publish.md#create-schemas) – 新しいスキーマの作成と既存のスキーマの拡張
* [ スキーマの公開と同期](schemas-create-publish.md#publish) - スキーマの変更をデータベース構造と同期します。
* [ カスタムフォームの操作](schemas-custom-forms.md) - データ入力フォームを使用して、カスタムスキーマのレコードを作成、編集、管理します。

>[!NOTE]
>
>スキーマを管理するには管理者権限が必要です。

スキーマについて詳しくは、[Campaign コンソールドキュメント](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"}を参照してください。
