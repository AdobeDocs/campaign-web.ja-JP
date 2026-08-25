---
audience: end-user
title: オファー管理の基本を学ぶ
description: Adobe Campaign web でのオファーの管理方法について学ぶ
feature: Offers
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 58c94bacd8eaf86f9f90a4c641f42bd04a442fab
workflow-type: ht
source-wordcount: 763
ht-degree: 100%

---

# オファー管理の基本を学ぶ {#gs-offer-management}

この機能では、パーソナライズされたオファーを配信に追加し、特定のコンテキストで各プロファイルに最も関連性の高いオファーを表示できます。オファーは、シンプルなコミュニケーションメッセージである場合や、1 つまたは複数の製品に関するプロモーションである場合があります。オファーエンジンは、実施要件ルールと優先度の重み付けに基づいて、表示する最適な提案を選択します。

Campaign Web ユーザーインターフェイスを使用すると、オファーをエンドツーエンドで管理できます。オファー環境の作成と設定、オファースペースの設計、オファーカタログの作成、実施要件ルールの設定、オファーコンテンツの編集、オファーの公開を行うことができます。

その後、**実施要件ルール**&#x200B;と&#x200B;**優先度の重み付け**&#x200B;に基づき、配信を通じて、受信者にオファーが表示されるので、特定のコンテキストで各プロファイルに対して最適なオファーが選択されます。

>[!NOTE]
>
>Campaign Web ユーザーインターフェイスは、最も一般的なオファー管理の使用状況に焦点を当てています。詳細設定は、Campaign クライアントコンソールで引き続き使用できます。[Campaign v8 ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=ja){target="_blank"}を参照してください

<!--
and check the [Campaign Web and client console capability matrix](../get-started/capability-matrix.md#offer-capabilities) for the current scope.
-->

## 主な概念 {#concepts}

オファーの操作を開始する前に、関連する主なオブジェクトについて理解しておきます。

* **オファー環境** - オファーカタログと関連するオファースペースを保持するコンテナ。オファーの作成や設定を行う&#x200B;**デザイン**&#x200B;環境と、読み取り専用の&#x200B;**[!UICONTROL ライブ]**&#x200B;環境（配信に使用できる、承認済みオブジェクトとデプロイ済みのオブジェクトが含まれる）の 2 つのタイプがあります。[詳細情報](offer-environment.md)

* **オファースペース** - オファーの公開場所と公開方法（メール、ダイレクトメール、SMS、インバウンド web など）を定義します。このスペースには、オファーで使用できるコンテンツフィールド、オファー表示域を作成するレンダリング関数、提案ステータスを推進するストレージ設定が一覧表示されます。[詳細情報](offer-space.md)

* **オファーカタログとカテゴリ** - オファーは、**カテゴリ**&#x200B;とサブカテゴリの階層型カタログに整理されます。各カテゴリでは、実施要件ルール、有効期限、**アプリケーションのテーマ**&#x200B;を共有できます。デザイン環境には、すべてのオファーを受信するデフォルトのカテゴリが用意されています。

<!--
To configure categories in depth — including sub-categories, fallback categories, and theme management — refer to the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-catalog/interaction-offer-catalog.html){target="_blank"}.
-->

* **オファー** - 独自の実施期間、ターゲットフィルター、重み付けおよびコンテンツを持つ、個別のオファー。オファーは、受信者に表示される前に承認およびデプロイされます。[詳細情報](create-offer.md)

* **オファーの提案** - 特定のオファースペース（web サイトのバナー、メール、SMS など）で連絡先にオファーを表示する結果。配信あたりの提案の数は、[配信でオファーを設定](../msg/offers.md)する際に指定されます。

* **裁定** - オファーエンジンが、表示するオファーを選択するために、実施要件を満たすオファーを優先度でランク付けする原則。裁定では、カテゴリ、オファーおよびコンテキストオファーで定義された条件を使用します。

## オファー管理フロー {#workflow}

Campaign Web UI での一般的なエンドツーエンドのフローは次のとおりです。

1. **オファー環境設定を確認** - デザイン／ライブマッピング、実施要件および重み付け管理設定を確認します。[詳細情報](offer-environment.md)

1. **オファースペースを作成** - コンテンツフィールド、レンダリング関数およびチャネルに一致する高度なパラメーターを定義します。[詳細情報](offer-space.md)

1. **カタログ内のオファーを作成** - 各オファーの実施期間、ターゲットフィルター、重み付け、コンテンツを設定します。[詳細情報](create-offer.md)

1. **承認してデプロイ** - 承認のためにオファーを送信し、そのコンテンツと実施要件を承認してから、デプロイメントプロセスでライブ環境に公開します。[詳細情報](create-offer.md#approve-deploy)

1. **配信にオファーを追加** - メール、SMS、プッシュまたはダイレクトメールの配信で、オファースペースと提案を参照します。[詳細情報](../msg/offers.md)

## Web UI でのオファーへのアクセス {#access}

オファーは、左側のメニューにある&#x200B;**[!UICONTROL オファー]**&#x200B;から使用できます。そこから、カタログを参照し、編集用のオファーを開き、その承認とデプロイメントのステータスを監視できます。

![オファーメニューを示すスクリーンショット。](assets/offers-gs.png){zoomable="yes"}

オファー環境とオファースペースには、対応するフォルダーに移動して、**[!UICONTROL エクスプローラー]**&#x200B;を通じてアクセスします。


## コンソール専用の補完機能 {#console-complements}

一部のオファー機能は、web ユーザーインターフェイスにまだ公開されておらず、引き続きクライアントコンソールから設定する必要があります。

* **オファーのシミュレーション** - オファーの配分を送信前にテストできる&#x200B;**シミュレーション**&#x200B;モジュール。[オファーのシミュレーション](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer.html?lang=ja#offer-simulation){target="_blank"}を参照してください。

* **定義済みフィルター**&#x200B;の管理 - 任意のオファーから参照できる再利用可能なフィルタールール。[定義済みフィルターの管理](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-predefined-filters.html?lang=ja){target="_blank"}を参照してください。

* **オファーのトラッキング** - 提案の履歴をフィードするオファー提案のトラッキングの設定。[オファー提案の追跡](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-tracking.html?lang=ja){target="_blank"}を参照してください。

* **オペレーターの役割** - オファーマネージャー／配信マネージャーの権限の割り当て。[インタラクションモジュールのオペレーター](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-operators.html?lang=ja){target="_blank"}を参照してください。

* **インタラクションのベストプラクティスと裁定ルール**。[Campaign のインタラクションのベストプラクティス](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-best-practices.html?lang=ja){target="_blank"}を参照してください。

* **レポート** - 専用のオファーおよび提案レポートは、web ユーザーインターフェイスではまだ使用できません。