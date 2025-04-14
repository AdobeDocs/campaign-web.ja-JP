---
title: ターゲティングディメンション
description: Adobe Campaign Web でのターゲティングディメンションについて説明します
exl-id: b910649a-7300-4f99-8f40-3a8965572ee9
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 25%

---

# ターゲティングディメンション {#targeting-dimensions}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_dimension"
>title="Select the targeting dimension"
>abstract="The targeting dimension lets you define the population targeted by the operation: recipients, contract beneficiaries, operator, subscribers, and more. By default, for emails and SMS, the target is selected from the Recipients built-in table. For Push notifications, the default target dimension is Subscriber applications."

## ワークフローのターゲティングディメンション {#workflow}

ワークフローのターゲティングディメンションは、最初の **[!UICONTROL オーディエンスを作成]** アクティビティによって定義され、ワークフローが終了するまで、後続のすべてのアクティビティで使用されます。 例えば、データベースからプロファイルに対してクエリを実行する場合、アウトバウンドトランジションには「受信者」タイプのデータが含まれ、これが次のアクティビティに送信されます。

[ ディメンションを変更アクティビティ ](../workflows/activities/change-dimension.md) を使用して、ワークフローのターゲティングディメンションを切り替えます。 これにより、購入や購読などの特定のテーブルに対してデータベースにクエリを実行し、ターゲティングディメンションを「受信者」に変更して、対応するプロファイルに配信を送信できます。

（ワークフロー設定または **オーディエンスを作成**、**紐付け**、**ディメンションを変更** などのアクティビティで）ターゲティングディメンションを選択すると、一般的に使用されるスキーマのリストがデフォルトで表示されます。 使用可能なすべてのスキーマを表示するには、「**[!UICONTROL すべてのスキーマを表示]** ボタンを切り替えます。 オプションの選択は、各ユーザーに対して保存されます。

![ 「すべてのスキーマを表示」ボタンが有効になっているターゲティングディメンションインターフェイスを示すスクリーンショット。](assets/targeting-dimension-show-all.png){zoomable="yes"}

## ターゲティングディメンション {#list}

デフォルトでは、メールと SMS 配信テンプレートは、プロファイルをターゲットにしています。ターゲットディメンションには、**nms:recipient** テーブルのフィールドが使用されます。 プッシュ通知の場合、デフォルトのターゲットマッピングは&#x200B;**サブスクライバーのアプリケーション（nms:appSubscriptionRcp）**&#x200B;であり、受信者のテーブルにリンクされています。

次に示すように、ワークフローと配信では、その他の組み込みのターゲットマッピングを使用します。

| 名前 | を使用してに配信します | スキーマ |
|-----------------------|-------------------------------------------------------|-------------------------|
| 受信者 | プロファイル/受信者（組み込みの受信者テーブル） | nms:recipient |
| 訪問者 | リファラルを使用してプロファイルが収集された訪問者（バイラルマーケティングなど） | mns:visitor |
| 購読 | ニュースレターなどの情報サービスを購読しているプロファイル | nms:subscription |
| 訪問者の購読 | 情報サービスを購読した訪問者 | nms:visitorSub |
| オペレーター | Adobe Campaign演算子 | nms:operator |
| 外部ファイル | 必要な情報がすべて含まれているファイルを介した配信 | リンクされるスキーマなし、入力されるターゲットなし |
| サブスクライバーのアプリケーション | アプリケーションを購読しているプロファイル | nms:appSubscriptionRcp |

さらに、特定のニーズに基づいて新しいターゲットマッピングを作成します。 この操作は、クライアントコンソールからのみ実行します。 詳しくは、[Campaign v8（クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=ja#new-mapping){target="_blank"}を参照してください。