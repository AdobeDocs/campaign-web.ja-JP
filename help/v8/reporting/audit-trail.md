---
product: campaign
title: 監査記録
description: Campaign 監査記録を使用してインスタンスを監視する方法について説明します
feature: Audit Trail, Monitoring, Workflows
exl-id: f4b4a33f-8250-4f4e-b2dc-129c56f9ea0f
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 33%

---

# 監査記録 {#audit-trail}

Adobe Campaign web ユーザーインターフェイスの **[!UICONTROL 監査記録]** 機能を使用すると、インスタンス内の重要なエンティティ（通常はインスタンスのスムーズな操作に大きな影響を与えるエンティティ）に加えられたすべての変更を完全に可視化できます。

>[!IMPORTANT]
>
>* Adobe Campaign web ユーザーインターフェイスは、ユーザー権限、テンプレート、パーソナライゼーションまたはキャンペーン内で行われた変更を監査しません。
>* 監査記録を管理できるのは、インスタンスの管理者のみです。

**[!UICONTROL 監査記録]** 機能は、Adobe Campaign インスタンス内で発生するアクションとイベントの詳細なログを常にリアルタイムで記録します。 データの時系列の記録にアクセスする便利な方法を提供し、ワークフローのステータス、変更する最新の個人、インスタンス内のユーザーが実行したアクティビティなどのクエリに対処します。

+++ 使用可能な監査記録エンティティの詳細を説明します

* **Source スキーマ監査証跡** を使用すると、Campaign v8 クライアントコンソール内のスキーマに対するアクティビティと最近の変更を監視できます。

  スキーマについて詳しくは、[Campaign v8 のドキュメント](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/developer/shemas-forms/schemas)を参照してください。

* **ワークフロー監査記録**&#x200B;を使用すると、アクティビティとワークフローに対して行った最近の変更とを追跡できます。その例として、次のような現在の状態があります。

   * 開始
   * 一時停止
   * 停止
   * 再度開始
   * クリーンアップ：履歴のパージと同じ
   * シミュレーション （アクション「シミュレーションモードで開始」と同じ）
   * ウェイクアップ （アクション「保留中のタスクを今すぐ実行」）
   * 無条件停止

  ワークフローについて詳しくは、この[ページ](../workflows/gs-workflows.md)を参照してください。

* **オプション監査記録** を使用すると、Campaign v8 のオプションに対するアクティビティと最近の変更を監視できます。

  オプションについて詳しくは、この[ページ](https://experienceleague.adobe.com/ja/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options)を参照してください。

* **配信監査記録**&#x200B;では、アクティビティと、配信に最後に行った変更を確認できます。

  配信について詳しくは、この[ページ](../msg/gs-deliveries.md)を参照してください。

* **外部アカウント** を使用すると、Campaign v8 で外部アカウントに加えられた変更を確認でき、テクニカルワークフローやキャンペーンワークフローなどのテクニカルプロセスで使用されます。

  外部アカウントについて詳しくは、この [ ページ ](../administration/external-account.md) を参照してください。

* **配信マッピング** を使用すると、Campaign v8 の配信マッピングに対するアクティビティと最近の変更を監視できます。

  配信マッピングについて詳しくは、この[ページ](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/audience/add-profiles/target-mappings)を参照してください。

* **Web アプリケーション** を使用すると、Campaign v8 で web フォームに加えられた変更を確認したり、入力フィールドと選択フィールドを含むページを作成したり、データベースのデータを含めたりすることができます。

  Web アプリケーションについて詳しくは、この [ ページ ](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/content/webapps) を参照してください。

* **オファー**&#x200B;では、アクティビティと、オファーに最後に行った変更を確認できます。

  オファーについて詳しくは、この[ページ](../msg/offers.md)を参照してください。

* **オペレーター** を使用すると、Campaign v8 でオペレーターに加えられたアクティビティと最近の変更を監視できます。

  オペレーターについて詳しくは、この[ページ](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/offers/interaction-settings/interaction-operators)を参照してください。

+++

## 監査記録へのアクセス {#accessing-audit-trail}

インスタンスの&#x200B;**[!UICONTROL 監査記録]**&#x200B;にアクセスするには：

1. **[!UICONTROL 管理]**&#x200B;メニューで、「**[!UICONTROL 監査記録]**」を選択します。

   ![ 「監査記録」オプションが選択された管理メニューを示すスクリーンショット ](assets/audit-trail-1.png)

1. **[!UICONTROL 監査記録]**&#x200B;ウィンドウが開き、エンティティのリストが表示されます。Adobe Campaign web ユーザーインターフェイスは、ワークフロー、オプション、配信およびスキーマの作成、編集および削除アクションを監査します。

   最後の変更の詳細を確認するには、いずれかのエンティティを選択します。

1. **[!UICONTROL エンティティを監査]** ウィンドウには、選択したエンティティに関する次のような詳細情報が表示されます。

   * **[!UICONTROL タイプ]**：ワークフロー、オプション、配信またはスキーマ。
   * **[!UICONTROL エンティティ]**：アクティビティの内部名。
   * **[!UICONTROL 変更者]**：このエンティティを最後に変更したユーザー名。
   * **[!UICONTROL アクション]**：このエンティティで最後に実行されたアクション（作成済み、変更済み、または削除済み）。
   * **[!UICONTROL 変更日]**：このエンティティで最後に実行されたアクションの日付。

   コードブロックは、エンティティで正確に変更された内容に関する詳細情報を提供します。

   ![ 変更に関する詳細情報を含むエンティティを監査ウィンドウを示すスクリーンショット ](assets/audit-trail-2.png)