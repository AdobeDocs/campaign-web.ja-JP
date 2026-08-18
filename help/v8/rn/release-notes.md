---
title: Campaign v8 web ユーザーインターフェイスリリースノート
description: 最新の Campaign web ユーザーインターフェイスリリースで提供される新機能について説明します
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
  - id: c309ee4e-82e4-4f7e-b608-ef345678c34e
  - id: d5ef99fa-df0c-4153-bf94-105ad0724167
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: d6b9b9c9905d840e65ac0aa267a665997c6e6b16
workflow-type: tm+mt
source-wordcount: 330
ht-degree: 33%

---

# リリースノート {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="リリースノート"
>abstract="Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。 これにより、Campaign リリースノートは月に数回更新され、最新の機能、改善点、修正が含まれます。 定期的に確認することをお勧めします。"

Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。 したがって、これらのリリースノートは月に数回更新されます。 定期的に確認してください。

>[!NOTE]
>
>以下の機能と改善点に関する詳細なドキュメントは、今後数日間にわたって段階的に追加されます。

## 26年8月リリース {#26-8-release}

_2026年8月18日_

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
<p>以前はクライアントコンソールでのみ使用していた<strong>承認</strong> ワークフローアクティビティが、Campaign Web ユーザーインターフェイスで使用できるようになりました。 タスクをグループまたは個々のオペレーターに割り当て、通知タイトルとメッセージをカスタマイズし、可能な回答（Yes/Noなど）を出力ブランチとして定義します。</p>
</td>
</tr>
</tbody>
</table>

### 改善点 {#26-8-improvements}

* **トラッキングを開く**: Campaign Web ユーザーインターフェイスから直接トラッキングを開いたり、無効にしたりできるようになりました。 これにより、データ保護規制に準拠することができます。
* **プログラムリストビュー**：プログラムは、キャンペーン、配信、ワークフローと同様に、専用ビューに一覧表示されるようになりました。 このビューから既存のプログラムを参照し、新しいプログラムを直接作成できます。
* **カスタムスキーマ設定**: **アクションデータ** セクションで、カスタムスキーマのレコードに対する&#x200B;**重複** アクションを許可できなくなるようになりました。
  <!--* **Workflow and delivery templates (only msf???)**: When creating a new workflow or delivery, you must now explicitly select a template. A default template is no longer applied automatically.-->
* **カスタムフィルター**: スキーマエディターで、カスタムフィルターでダイレクトリンクのフィルター条件がサポートされるようになりました。新しい&#x200B;**カスタムフィルター設定**&#x200B;を使用して、任意の属性のデフォルトラベルを上書きできます。
* **スキーマ検証**：新しい「**検証**」ボタンを使用して、スキーマエディターから直接スキーマの構造を検証できるようになりました。
* **フォルダーセキュリティ**: ユーザーが&#x200B;**挿入**&#x200B;または&#x200B;**編集** アクセス権を持っている場合に、**名前を変更** オプションをフォルダーで使用できるようになりました。
  <!--* **Enrichment activity**: You can now enrich data from an external database directly from the **Enrichment** workflow activity. This matches the capability already available in the Client Console.-->
