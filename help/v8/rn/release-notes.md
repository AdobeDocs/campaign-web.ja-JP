---
title: Campaign v8 web ユーザーインターフェイスリリースノート
description: 最新の Campaign web ユーザーインターフェイスリリースで提供される新機能について説明します
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2: id: a075b2c1-7748-4328-b7f6-343aa314616aid: c309ee4e-82e4-4f7e-b608-ef345678c34eid: d5ef99fa-df0c-4153-bf94-105ad0724167
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: cbecd07b053d0ceb4e9114aa3c6d37752392febc
workflow-type: ht
source-wordcount: 243
ht-degree: 100%

---

# リリースノート {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="リリースノート"
>abstract="Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。 これにより、Campaign リリースノートは月に数回更新され、最新の機能、改善点、修正が含まれます。 定期的に確認することをお勧めします。"

Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。 したがって、これらのリリースノートは月に数回更新されます。 定期的に確認してください。

## 2026年6月リリース {#26-6-release}

_2026年6月16日（PT）_

### 改善点 {#26-6-improvements}

<!--
* Technical administrators can now create and configure brands directly from the Campaign Web User Interface, without using the Client Console. All brand settings, including identity, subdmain and protocols, email header parameters and URL tracking parameters, are now available in the Web UI. <!-- [Learn more](../administration/branding/branding-configure.md)
-->

* トラッキングログを含む任意のリスト画面からデータをエクスポートできるようになりました。リストを見つけて、エクスポートボタンをクリックするだけです。エクスポートでは、現在読み込まれている行が含まれ、画面に表示されている列やアクティブな検索またはフィルターが考慮されます。[詳細情報](../get-started/list-filters.md)

* **重複排除 - 重複**&#x200B;および&#x200B;**終了**&#x200B;ワークフローアクティビティで、複数のインバウンドトランジションがサポートされるようになりました複数のインバウンドトランジションが使用可能な場合は、アクティビティプロパティの「**結合の設定**」セクションを使用して、
接続するトランジションを選択します。詳しくは、[重複排除 - 重複](../workflows/activities/deduplication.md)、[終了](../workflows/activities/end.md)の各ページを参照してください。

* **オーディエンスを作成**（クエリタイプ）および&#x200B;**エンリッチメント**&#x200B;ワークフローアクティビティの「**エンリッチメントデータ**」セクションで、詳細設定パラメーターが公開されるようになりました。これらのパラメーターを使用すると、グループ化、重複排除 - 重複、プライマリキーの処理、インバウンドイベントデータなど、エンリッチメントデータの作成方法を微調整できます。[詳細情報](../workflows/activities/enrichment.md)

<!--
* Delivery templates now allow you to define a time zone in the Schedule settings.
-->
