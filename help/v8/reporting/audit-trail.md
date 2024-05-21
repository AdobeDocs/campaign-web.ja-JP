---
product: campaign
title: 監査記録
description: Campaign 監査記録を使用してインスタンスを監視する方法について説明します
feature: Audit Trail, Monitoring, Workflows
source-git-commit: 4f7dd30f02f83624a00b3d0e6ac7ba74c1c242e0
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 41%

---

# 監査記録{#audit-trail}

>[!IMPORTANT]
>
>Adobe Campaign web ユーザーインターフェイスは、ユーザー権限、テンプレート、パーソナライゼーションまたはキャンペーン内で行われた変更を監査しません。\
>監査記録は、インスタンスの管理者のみが管理できます。

Adobe Campaign Web ユーザーインターフェイスで、 **[!UICONTROL 監査記録]** この機能により、インスタンス内の重要なエンティティ（通常、インスタンスのスムーズな操作に大きな影響を与えるエンティティ）に加えられたすべての変更を完全に可視化できます。

**[!UICONTROL 監査記録]** この機能は、Adobe Campaign インスタンス内で発生するアクションとイベントの詳細なログを常にリアルタイムで記録します。 データの時系列の記録にアクセスする便利な方法を提供し、ワークフローのステータス、変更する最新の個人、インスタンス内のユーザーが実行したアクティビティなどのクエリに対処します。

+++ 監査記録が使用可能なエンティティについて説明します

* **ソーススキーマ監査証跡** を使用すると、Campaign V8 クライアントコンソール内のスキーマに加えられたアクティビティと最近の変更を監視できます。

  スキーマについて詳しくは、次を参照してください： [Campaign v8 ドキュメント](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas).

* **ワークフロー監査記録** を使用すると、ワークフローのアクティビティと最近の変更を、現在の状態を含めて追跡できます。例えば、次のようなものがあります。

   * 開始
   * 一時停止
   * 停止
   * 再度開始
   * クリーンアップ（「履歴をパージ」アクションと同じ）
   * シミュレーション（「シミュレーションモードで開始」アクションと同じ）
   * ウェイクアップ（「保留中のタスクを今すぐ実行」アクションと同じ）
   * 無条件停止

  ワークフローについて詳しくは、この[ページ](../workflows/gs-workflows.md)を参照してください。

* **オプション監査証跡** を使用すると、Campaign V8 でオプションに加えられたアクティビティと最近の変更を監視できます。

  オプションについて詳しくは、この[ページ](https://experienceleague.adobe.com/ja/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options)を参照してください。

* **配信監査記録**&#x200B;では、アクティビティと、配信に最後に行った変更を確認できます。

  配信について詳しくは、この[ページ](../msg/gs-deliveries.md)を参照してください。

* **外部アカウント** Campaign V8 で外部アカウントに加えられ、テクニカルワークフローやキャンペーンワークフローなどのテクニカルプロセスで使用された変更を確認できます。

  外部アカウントについて詳しくは、この[ページ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/external-accounts)を参照してください。

* **配信マッピング** を使用すると、Campaign V8 の配信マッピングに対するアクティビティと最近の変更を監視できます。

  配信マッピングについて詳しくは、この[ページ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/audience/add-profiles/target-mappings)を参照してください。

* **Web アプリケーション**&#x200B;では、入力フィールドと選択フィールドを含むページの作成に使用される Campaign V8 の web フォームに行った変更を確認できます。これには、データベースのデータが含まれている場合があります。

  Web アプリケーションについて詳しくは、この[ページ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/content/webapps)を参照してください。

* **オファー**&#x200B;では、アクティビティと、オファーに最後に行った変更を確認できます。

  オファーについて詳しくは、こちらを参照してください。 [ページ](../msg/offers.md).

* **演算子** を使用すると、Campaign V8 でオペレーターに加えられたアクティビティと最近の変更を監視できます。

  オペレーターについて詳しくは、この[ページ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/offers/interaction-settings/interaction-operators)を参照してください。

+++

## 監査記録へのアクセス {#accessing-audit-trail}

インスタンスの&#x200B;**[!UICONTROL 監査記録]**&#x200B;にアクセスするには：

1. の下 **[!UICONTROL 管理]** メニュー、選択 **[!UICONTROL 監査記録]** .

   ![](assets/audit-trail-1.png)

1. **[!UICONTROL 監査記録]**&#x200B;ウィンドウが開き、エンティティのリストが表示されます。Adobe Campaignの web ユーザーインターフェイスは、ワークフロー、オプション、配信およびスキーマの作成、編集および削除アクションを監査します。

   最後の変更の詳細を確認するには、いずれかのエンティティを選択します。

1. **[!UICONTROL エンティティを監査]**&#x200B;ウィンドウには、選択したエンティティに関する次のような詳細情報が表示されます。

   * **[!UICONTROL タイプ]** ：ワークフロー、オプション、配信、スキーマ。
   * **[!UICONTROL Entity]** ：アクティビティの内部名。
   * **[!UICONTROL 変更者]** ：このエンティティを最後に変更したユーザー名。
   * **[!UICONTROL アクション]** ：このエンティティで最後に実行されたアクション（作成済み、変更済み、削除済み）。
   * **[!UICONTROL 変更日]** ：このエンティティで最後に実行されたアクションの日付。

   コードブロックには、エンティティ内で正確に変更された内容に関する詳細情報が表示されます。

   ![](assets/audit-trail-2.png)

