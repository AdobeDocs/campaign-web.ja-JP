---
audience: end-user
title: トランザクションメッセージ
description: Adobe Campaign web を使用したトランザクションメッセージについて
exl-id: 90830dca-acff-4aa3-a88b-1005e349cf52
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 100%

---

# トランザクションメッセージについて {#transactional-messaging}

>[!CONTEXTUALHELP]
>id="acw_transacmessages"
>title="トランザクションメッセージ"
>abstract="トランザクションメッセージは、トリガーされたメッセージの処理を目的に設計された Adobe Campaign の特殊なモジュールです。"

<!-- >>[!CONTEXTUALHELP]
>id="acw_transacmessages_exclusionlogs"
>title="Transactional messaging exclusion logs"
>abstract="Transactional messaging exclusion logs" -->

トランザクションメッセージは、トリガーされたメッセージの処理を目的に設計された Adobe Campaign の特殊なモジュールです。これらのメッセージは、情報システムから発生するイベントに応答して自動的に生成されます。このようなイベントの一般的な例としては、ボタンやリンクのクリック、買い物かごの放棄、製品の在庫アラートのリクエスト、アカウントの作成や変更があります。

トランザクションメッセージは、次の送信に使用します。

* 重要な通知（注文確認やパスワードのリセットなど）。
* アカウント作成、購入完了など、顧客のアクションに対するリアルタイムの応答。
* 顧客とのやり取りにとって重要なプロモーション以外のコンテンツ。

トランザクションメッセージのモジュールは、情報システムとシームレスに統合されます。顧客のアクションなどのイベントは Adobe Campaign にプッシュされ、対応するパーソナライズされたメッセージが送信されます。これらのメッセージは、メール、SMS、プッシュ通知などの様々なチャネルを通じて個別に送信することや、一括で送信できます。

**[!UICONTROL トランザクションメッセージ]**&#x200B;のモジュールは、「**[!UICONTROL トリガーされたメッセージ]**」セクションで確認できます。

![トリガーされたメッセージとそのステータスを示すトランザクションメッセージインターフェイス](assets/transactional.png){zoomable="yes"}

**[!UICONTROL トランザクションメッセージ]**&#x200B;ページには、次の 3 つのタブがあります。

* **[!UICONTROL 参照]**：トランザクションメッセージとそのステータスのリストが表示されます。
* **[!UICONTROL テンプレート]**：トランザクションメッセージテンプレートを検索および作成します。
* **[!UICONTROL 履歴]**：実行されたすべてのトランザクションメッセージに関する詳細が表示されます。

このドキュメントでは、次の方法について説明します。

* [トランザクションメッセージの作成](create-transactional.md)：テンプレートを使用し、必要な設定についても説明します。
* [トランザクションメッセージのコンテンツの検証](validate-transactional.md)：パーソナライゼーションのシミュレート方法について説明します。
* [トランザクションメッセージを監視します](monitor-transactional.md)。