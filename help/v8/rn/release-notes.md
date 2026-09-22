---
title: Campaign v8 web ユーザーインターフェイスリリースノート
description: 最新の Campaign web ユーザーインターフェイスリリースで提供される新機能について説明します
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
  - id: c309ee4e-82e4-4f7e-b608-ef345678c34e
    internal-label: Dynamic reporting
  - id: d5ef99fa-df0c-4153-bf94-105ad0724167
    internal-label: Integrations
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
source-git-commit: 7a22b75c81435fa891fa8aa73c5c1acad1931710
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 38%
---
# リリースノート {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="リリースノート"
>abstract="Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。 これにより、Campaign リリースノートは月に数回更新され、最新の機能、改善点、修正が含まれます。 定期的に確認することをお勧めします。"

Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。 したがって、これらのリリースノートは月に数回更新されます。 定期的に確認してください。

## 26年9月リリース {#26-9-release}

_2026年9月22日_

### 新機能 {#26-9-features}

<table>
<thead>
<tr>
<th><strong>LINE チャネル</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Campaignは、人気のあるインスタント メッセージ アプリケーションである<strong>LINE</strong> チャネルをサポートするようになりました。 テキスト、画像、動画コンテンツ、スタンドアロン配信、ワークフローなどを使用して、LINE メッセージを作成、送信できます。 <a href="../line/get-started-line.md">詳細情報</a></p>
</td>
</tr>
</tbody>
</table>

### 改善点 {#26-9-improvements}

* **サイドナビゲーションアクセス**：管理者は、サイドナビゲーションから特定のメニューエントリを非表示にできるようになりました。 [詳細を表示](../administration/schemas-browse-access.md#customize-screen-display-screen-def)
* **追加の承認タイプ**: コンテンツとターゲットの承認に加えて、キャンペーン配信に予算と配信開始の承認を必要とできるようになりました。 [詳細を表示](../campaigns/campaign-approvals.md#configure-approval-settings-configure-approvals)
* **訪問者ベースのSMS ターゲティング**：訪問者ターゲットマッピングをSMS配信で使用できるようになりました。 [詳細を表示](../sms/create-sms.md)
* **ワークフローのキャンセル ボタン**：新しい&#x200B;**キャンセル** ボタンを使用すると、ワークフロー内の保存されていない変更を元に戻すことができます。 [詳細を表示](../workflows/orchestrate-activities.md#save-or-discard-your-changes-save-cancel)
* **複数の値を持つ重複排除**: **値のリストに従う** オプションで、複数の属性がサポートされるようになりました。 [詳細を表示](../workflows/activities/deduplication.md#configure-the-deduplication-activity-deduplication-configuration)
* **モバイルターゲットマッピング**: モバイルアプリケーションターゲットのターゲットマッピングを作成できるようになりました。 [詳細を表示](../administration/target-mappings.md#create-a-target-mapping-create-mapping)
* **外部データベースのエンリッチメント**：外部データベースのデータを&#x200B;**エンリッチメント**&#x200B;または&#x200B;**オーディエンスを構築** アクティビティでエンリッチメントできるようになりました。 [詳細を表示](../workflows/activities/enrichment.md#external-data)
* **ファイルオーディエンスの紐付け**: ファイルからオーディエンスをターゲティングする際に、受信者をデータベースにインポートするかどうかを設定できるようになりました。 [詳細を表示](../audience/file-audience.md#select-and-configure-the-input-file-upload)
* **コレクションで直接結合**：コレクションから直接属性を選択する際に、推奨されるデフォルトオプション、集計関数、または高度な直接結合を使用して、条件の構築方法を選択できるようになりました。 [詳細を表示](../query/build-query.md#custom-conditions-on-linked-tables-1-1-and-1-n-links-links)

