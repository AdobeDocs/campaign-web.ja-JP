---
audience: end-user
title: 自動配信ワークフローアクティビティ
description: 自動配信ワークフローアクティビティの使用方法について説明します
exl-id: a9c485f1-0369-414d-9e43-bedb0390a2f5
source-git-commit: 65031741dc7c667ef74469d75b8ea60a5fc20aaf
workflow-type: ht
source-wordcount: '643'
ht-degree: 100%

---

# 自動配信 {#automated-delivery}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="自動配信アクティビティ"
>abstract="自動配信ワークフローアクティビティがワークフローパレットで使用できるようになりました。 配信アクションの作成または実行（準備、配達確認の送信、準備と開始など）に使用できます。 ワークフローに直接組み込むことができます。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=ja" text="リリースノートを参照してください"

>[!CONTEXTUALHELP]
>id="acw_orchestration_automated-delivery"
>title="自動配信アクティビティ"
>abstract="**自動配信**&#x200B;アクティビティは自動処理に使用されます。ワークフロー内で配信を作成または再利用し、実行するアクション（準備、準備と開始、配達確認の送信など）を選択します。 ワークフローの外部で作成された既存の明示的な配信を選択するか、アクティビティが実行されるたびにテンプレートから新しい配信を作成できます。"

**自動配信**&#x200B;アクティビティを使用すると、ワークフロー内で直接、配信アクションを作成、設定、実行できます。定義済みの配信をスケジュール上または自動フローの一部として実行する場合や、アクティビティが実行されるたびにテンプレートから新しい配信を生成する場合に使用します。

<!--
**[Continuous delivery](continuous-delivery.md)** always uses a template. The first run creates one delivery; later runs send to new recipients through that same delivery. **Automated delivery** is different: you either reuse one existing delivery every run, or you create a new delivery from a template each time—so each run can be its own delivery if you want. 
-->

このアクティビティを設定するには、次の手順に従います。

1. 配信設定を定義します。[詳細情報](#delivery-settings)
1. 実行するアクションを選択します。[詳細情報](#action-to-execute)
1. トランジションを設定します。[詳細情報](#transition-to-execute)
1. 変更スクリプトを定義します。[詳細情報](#script)

## 配信設定の定義 {#delivery-settings}

アクティビティを設定する際は、配信の送信元を選択します。この節では、次の 2 つのオプションを使用できます。

![自動配信を示すスクリーンショット](../assets/automated-delivery.png){zoomable="yes"}

* 既存の配信（例：スタンドアロン配信やキャンペーンから作成された配信）に対して操作を実行する際は、「**明示的な配信**」を選択します。「**配信を選択**」ボタンを使用して配信を選択します。ワークフローが実行され、このアクティビティに到達するたびに、**同じ**&#x200B;配信に対して操作が実行されます。 実行ごとに新しい配信は作成されません。アクティビティは、同じ配信を再利用します。これは、スケジュール上や承認手順の後など、単一の配信を繰り返し準備または送信する際に役立ちます。

<!-- by default, the list shows unfinished deliveries in the Deliveries folder. You can browse other folders to select a delivery from another campaign. You choose the action to perform (prepare, prepare and start, send a proof, and so on).-->

* アクティビティが実行されるたびに&#x200B;**新しい**&#x200B;配信を作成する際は、「**新規（テンプレートから作成）**」を選択します。「**テンプレートを選択**」ボタンを使用して、配信テンプレートを選択します。各実行では、そのテンプレートに基づいて新しい配信が生成されます。各ワークフロー実行で個別の配信が必要な場合（例えば、実行ごとに 1 通のメール）に使用します。

<!-- Unlike the Continuous delivery activity, there is no “append” to a previous execution—each run produces a separate delivery. -->

>[!NOTE]
>
>高度なユースケースに使用される「**トランジションで指定**」および「**スクリプトで計算**」オプションは、クライアントコンソールでのみ設定できます。[Campaign v8 ドキュメント](https://experienceleague.adobe.com/ja/docs/campaign/automation/workflows/wf-activities/action-activities/delivery){target="_blank"}を参照してください。

## 実行するアクションの選択 {#action-to-execute}

この節では、アクティビティで配信に対して行う処理を選択します。次のオプションを使用できます。

![自動配信で実行するアクションを示すスクリーンショット](../assets/automated-delivery2.png){zoomable="yes"}

* **保存**：分析または送信せずに配信を作成および保存します。
* **ターゲットを推定**：配信ターゲットを計算し、可能性を評価します（最初の分析フェーズ）。
* **準備**：完全な分析（ターゲットの計算とコンテンツの準備）を実行します。 配信は送信されません。
* **配達確認を送信**：配信の配達確認を送信します。
* **準備と開始**：完全な分析プロセス（ターゲットの計算とコンテンツの準備）を実行し、配信を送信します。

## トランジションの設定 {#transition-to-execute}

この節では、アクティビティの後にトランジションを生成するかどうかを選択できます。次のオプションを使用できます。

![自動配信のトランジションを示すスクリーンショット](../assets/automated-delivery3.png){zoomable="yes"}

* **アウトバウンドトランジションを生成**：アクティビティが終了すると、アウトバウンドトランジションが生成されます。
* **トランジションラベル**：キャンバスのトランジションに表示されるラベルをカスタマイズできます。
* **エラーを処理**：エラー処理のトランジションを追加します。

## 変更スクリプトの定義 {#script}

スクリプトを使用すると、アクティビティの動作（例：アクティビティラベルなどの配信パラメーター）を変更できます。このアクティビティに対してカスタムロジックが必要な場合に使用します。

「**スクリプトを作成**」をクリックし、エディターで変更ロジックを書き込みます。

## 関連トピック {#related}

* [ワークフローアクティビティについて](about-activities.md)
* [連続配信](continuous-delivery.md)
* [メール, SMS, プッシュ, ダイレクトメールアクティビティ](channels.md)
* [配信テンプレート](../../msg/delivery-template.md)
