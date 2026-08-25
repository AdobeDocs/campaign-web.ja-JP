---
audience: end-user
title: オファースペースの作成と管理
description: Campaign Web でオファースペースを作成、設定、デプロイ、プレビューする方法について説明します。
feature: Offers
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 58c94bacd8eaf86f9f90a4c641f42bd04a442fab
workflow-type: ht
source-wordcount: 921
ht-degree: 100%

---

# オファースペースの作成と管理 {#offer-space}

**オファースペース**&#x200B;は、使用するチャネル（メール、ダイレクトメール、SMS、インバウンド web など）、オファーで使用できるコンテンツフィールド、最終的な表示域を作成する方法など、オファーで連絡先に表示される場所と方法を定義します。1 つの環境に複数のオファースペースを含めることができ、各表示ポイントに対して 1 つのスペースが割り当てられます。

オファースペースは、それ自体がチャネルではありません。オファーがチャネル上に表示される特定の場所を表します。同じ web ページ上の 2 つのバナーは、通常、2 つの異なるオファースペースに対応します。完全な概念的モデルについて詳しくは、[Campaign v8 ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html?lang=ja){target="_blank"}を参照してください。

## オファースペースの作成または変更{#create-offer-space}

オファースペースは、オファー環境フォルダーの下に保存されます。プラットフォームで使用可能なオファースペースを参照するには、**[!UICONTROL エクスプローラー]**&#x200B;を開き、オファー環境に移動して、それらを含むサブフォルダーを選択します。

![オファースペースリストを示すスクリーンショット。](assets/offers-space.png){zoomable="yes"}

そこから、既存のオファースペースを開くか、「**[!UICONTROL オファースペースを作成]**」をクリックして新しいスペースを作成できます。

![オファースペース画面を示すスクリーンショット。](assets/offers-space-1.png){zoomable="yes"}

### プロパティを定義 {#properties}

このセクションでは、次の操作を実行できます。

* オファースペースの&#x200B;**[!UICONTROL ラベル]**&#x200B;を入力する。
* 表示ポイント（メール、ダイレクトメール、SMS、web など）に一致する&#x200B;**[!UICONTROL チャネル]**&#x200B;を選択する。
* 一括配信の呼び出しに加え、オファーエンジンへの単一（リアルタイム、単一オファー）の呼び出しもサポートする必要がある場合は、「**[!UICONTROL 単一モードを有効にする]**」を選択する。

### コンテンツフィールドを定義 {#content-fields}

コンテンツフィールドには、オファーレベルで編集でき、レンダリング関数で再利用できる属性が一覧表示されます。オファースペースにフィールドを追加する順序により、オファーの「**[!UICONTROL コンテンツ]**」セクションに表示される順序が決定されます。

デフォルトでは、すべてのオファーに、**[!UICONTROL タイトル]**、**[!UICONTROL 宛先 URL]**、**[!UICONTROL 画像 URL]**、**[!UICONTROL HTML コンテンツ]**、**[!UICONTROL テキストコンテンツ]**&#x200B;など、標準のコンテンツフィールドが用意されています。このリストは、レンダリングに必要な任意のカスタムフィールド（例：**短いコンテンツ**、**追跡対象の URL**、スキーマ拡張を通じて追加された任意の属性）で拡張できます。

「**[!UICONTROL コンテンツフィールドを追加]**」をクリックし、オファースキーマから表示する属性を選択するか、「**[!UICONTROL 式を編集]**」をクリックして、代わりにカスタム式を定義します。

>[!IMPORTANT]
>
>オファーの「**[!UICONTROL コンテンツ]**」セクションからカスタム属性を編集可能にするには、[!DNL nms:offer] スキーマの「**[!UICONTROL オファーコンテンツ]**」セクションでも属性を宣言する必要があります。詳しくは、[スキーマの操作](../administration/schemas.md)を参照してください。

### レンダリング関数を設定 {#rendering}

レンダリング関数は、コンテンツフィールドから最終的なオファー表示域を作成します。コンテンツをそのままシンプルに出力するデフォルトのレンダリングか、フィールドを HTML、XML またはテキストと組み合わせるカスタム関数を選択できます。

「**[!UICONTROL HTML レンダリング]**」タブ、「**[!UICONTROL XML レンダリング]**」タブまたは「**[!UICONTROL テキストレンダリング]**」タブを選択し、「**[!UICONTROL レンダリング関数をオーバーロード]**」を有効にしてアクティブ化します。

式エディターを使用して、レンダリング関数を書き込みます。スペースで定義されたコンテンツフィールド、オファー属性および任意の関数を[式エディター](../query/expression-editor.md)から参照できます。

>[!NOTE]
>
>レンダリング関数が定義されていない場合、オファーコンテンツは、標準属性を使用して、そのまま返されます。XML レンダリング関数は、オファースペースで「**[!UICONTROL 単一モードを有効にする]**」が選択されている場合にのみ使用できます。

### ストレージと提案のステータスを設定 {#storage}

このセクションでは、このスペースを通じて生成された提案を保持する方法や、そのライフサイクル全体を通じてステータスの推移を制御できます。

* **[!UICONTROL 提案の挿入を無効にする]** - このオファースペースを通じて生成された提案が、提案ストレージテーブルに挿入されるのを防ぎます。

* 提案の&#x200B;**[!UICONTROL ステータス]** - オファーエンジンが提案を返す瞬間に提案に適用されるステータス（通常、アウトバウンド配信の場合は&#x200B;**[!UICONTROL 提示済み]**）。

* 承認の&#x200B;**[!UICONTROL ステータス]** - 受信者がオファーを操作した際に適用されるステータス（通常は&#x200B;**[!UICONTROL 承認済み]**）。

使用可能なステータスの値は、クライアントコンソールで使用されるリストと一致します。詳しくは、コンソールドキュメントの [Campaign v8 ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html?lang=ja#offer-proposition-statuses){target="_blank"}を参照してください。

<!--
>[!NOTE]
>
>Status updates run asynchronously through the tracking workflow. For an outbound delivery containing a tracked link, the status of the proposition is automatically switched to **[!UICONTROL Presented]** when the delivery reaches the **[!UICONTROL Sent]** state. To trigger the **[!UICONTROL Interested]** status from a click, add the `_urlType="11"` attribute to the link. The full **inbound interaction** URL syntax (for example to apply the **[!UICONTROL Rejected]** status from a web app) must be configured in the client console — see [Inbound interaction status update](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html#configuring-the-status-when-the-proposition-is-accepted){target="_blank"}.
-->

### 詳細設定を指定 {#advanced}

このセクションでは、**[!UICONTROL ターゲット ID]** を定義できます。「**[!UICONTROL 追加]**」をクリックして 1 つまたは複数の&#x200B;**[!UICONTROL 受信者]**&#x200B;属性を選択するか、「**[!UICONTROL 式を編集]**」をクリックして、代わりにカスタム式を定義します。この設定は、基本的なオファースペースではオプションです。完全な参照と動作について詳しくは、[Campaign v8 ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer-spaces.html?lang=ja){target="_blank"}を参照してください。

**インバウンド web チャネル**&#x200B;で作成されたオファースペースでは、オファーを表示し、オファーエンジンを呼び出すように web サイトを設定する必要もあります。この統合はクライアントコンソールで実行されます。Campaign v8 ドキュメントの[リアルタイムでのオファーの表示](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-present-offers.html?lang=ja){target="_blank"}および[オファーエンジン統合の設定](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-integration.html?lang=ja){target="_blank"}を参照してください。

## オファースペースをデプロイ {#deploy}

配信でオファースペースを使用する前に、オファースペースをデプロイする必要があります。オファースペースを保存し、「**デプロイ**」をクリックします。デプロイメントのステータスは、オファースペースに反映されます。

![オファーのデプロイを示すスクリーンショット。](assets/offers-space-2.png){zoomable="yes"}

## オファースペースをプレビュー {#preview}

プレビューを使用すると、特定のターゲットに対してオファーがどのように選択され、レンダリングされるかをシミュレートできます。

1. オファースペースから、**[!UICONTROL 概要]**&#x200B;の横にある「**[!UICONTROL プレビュー]**」タブを選択します。

   ![オファーのプレビューを示すスクリーンショット。](assets/offers-space-3.png){zoomable="yes"}

1. ターゲットプロファイルを選択し、プレビューを実行します。一致するオファーは、レンダリング関数によって生成された表示域と共に返されます。

>[!NOTE]
>
>提案が返されない場合は、オファーの実施要件ルールとスペースの設定を確認してください。

次に、カタログで[オファーを作成](create-offer.md)し、このスペースに割り当てます。
