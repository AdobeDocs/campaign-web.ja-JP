---
title: Campaign v8 web ユーザーインターフェイスリリースノート
description: 最新の Campaign web ユーザーインターフェイスリリースで提供される新機能について説明します
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2: id: a075b2c1-7748-4328-b7f6-343aa314616aid: c309ee4e-82e4-4f7e-b608-ef345678c34eid: d5ef99fa-df0c-4153-bf94-105ad0724167
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 404a5a4f1d793404a326feb07cd6869aa97af664
workflow-type: tm+mt
source-wordcount: 332
ht-degree: 78%

---

# リリースノート {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="リリースノート"
>abstract="Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。 これにより、Campaign リリースノートは月に数回更新され、最新の機能、改善点、修正が含まれます。 定期的に確認することをお勧めします。"

Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。 したがって、これらのリリースノートは月に数回更新されます。 定期的に確認してください。

## 2026年8月リリース {#26-8-release}

_2026年8月18日（PT）_

### 新機能 {#26-8-features}

<table>
<thead>
<tr>
<th><strong>承認ワークフローアクティビティ</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>以前はクライアントコンソールでのみ使用可能であった<strong>承認</strong>ワークフローアクティビティが、Campaign web ユーザーインターフェイスで使用できるようになりました。 タスクをグループまたは個々のオペレーターに割り当て、通知のタイトルとメッセージをカスタマイズし、考えられる回答（例：はい／いいえ）を出力分岐として定義します。</p>
<p>詳しくは、<a href="../workflows/activities/approval.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

### 改善点 {#26-8-improvements}

* **トラッキングを開く**：Campaign web ユーザーインターフェイスから直接、トラッキングを開いたり、無効にしたりできるようになりました。 これにより、データ保護規制に準拠できます。 [詳細を表示](../advanced-settings/delivery-settings.md#tracking-tab)
* **プログラムリスト表示**：プログラムは、キャンペーン、配信、ワークフローと同様に、専用ビューに一覧表示されるようになりました。 この表示から直接、既存のプログラムを参照したり、新しいプログラムを作成したりできます。 [詳細を表示](../administration/plans-programs.md#create-program)
* **カスタムスキーマ設定**：「**アクションデータ**」セクションで、カスタムスキーマのレコードに対する&#x200B;**複製**&#x200B;アクションを許可できなくなりました。 [詳細を表示](../administration/schemas-action-data.md#action-data)
* **カスタムフィルター**: スキーマエディターで、新しい&#x200B;**リンク設定** ダイアログを使用して、リンクタイプのカスタムフィルターのピッカーで使用できる値を制限できるようになりました。 [詳細を表示](../administration/schemas-custom-filters.md#settings)
* **スキーマ検証**：新しい&#x200B;**チェック** ボタンを使用して、スキーマエディターから直接スキーマの構造を検証できるようになりました。 [詳細を表示](../administration/schemas-create-publish.md#create-new)
* **フォルダーセキュリティ**: フォルダーで使用可能なアクションは、クライアントコンソールの動作と一致して、オペレーターの権限によって一貫して管理されるようになりました。 [詳細情報](../get-started/work-with-folders.md#about-folders)。
  <!--* **Enrichment activity**: You can now enrich data from an external database directly from the **Enrichment** workflow activity. This matches the capability already available in the Client Console.-->
  <!--* **Workflow and delivery templates (only msf???)**: When creating a new workflow or delivery, you must now explicitly select a template. A default template is no longer applied automatically.-->

