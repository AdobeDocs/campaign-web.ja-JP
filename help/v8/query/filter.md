---
audience: end-user
title: フィルターリスト
description: 組み込みフィルターとカスタムフィルターを使用して、Adobe Campaign Web リストをフィルタリングする方法について説明します。
exl-id: 41c3c4c3-5991-4223-ad02-e2531d76fdda
source-git-commit: 485d8b4b715192cc5edb6442df0fa958e29d15ff
workflow-type: ht
source-wordcount: '413'
ht-degree: 100%

---

# フィルターリスト {#filter-lists}

Adobe Campaign Web では、オブジェクトの各リスト内にフィルターを提供し、特定のコンテキスト条件に基づいて情報をフィルタリングできます。例えば、ステータス、チャネル、連絡日またはフォルダーに基づいて配信をフィルタリングできます。また、配達確認を非表示にすることもできます。

>[!IMPORTANT]
>
>クエリモデラーで新しいインターフェイスを使用できます。新しいルールビルダーでは、簡素化されたインターフェースにより、クエリをより簡単に作成できます。このエクスペリエンスに切り替えるには、右上隅の切替スイッチボタンを押します。切替スイッチボタンを押して新しいインターフェイスを無効にするだけで、いつでも従来のクエリモデラーに戻ることができます。この新しいインターフェイスでは、クエリモデラーと同じ原則を適用できます。
>![新しいルールビルダーインターフェイスの切替スイッチを示す画像](assets/query-modeler-toggle.png){zoomable="yes"}

## フィルターの適用 {#apply}

リストにフィルターを適用するには、リストの左上隅の検索バーの横にある「**[!UICONTROL フィルターを表示]**」ボタンをクリックします。

フィルターパネルが開き、選択したリストで使用可能なフィルターが表示されます。例えば、キャンペーンをステータス、開始日と終了日またはストレージフォルダーに基づいてフィルタリングでき、サブスクリプションサービスのリストをチャネルとストレージフォルダーに基づいてフィルタリングできます。

![リストで使用可能なフィルターを示すフィルターパネル](assets/filters-pane.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

独自の条件に基づいてリストをフィルタリングするには、カスタムフィルターを作成します。これを行うには、フィルターパネルの下部を参照し、「**ルールを追加**」ボタンをクリックします。[詳しくは、カスタムフィルターの作成方法を参照してください](#custom)。

リストに適用すると、検索バーの下にフィルターが表示されます。個別のフィルターはいつでも削除できます。また、「**すべてクリア**」ボタンをクリックしてすべてのフィルターを削除することもできます。

## カスタムフィルターの作成 {#custom}

カスタムフィルターを使用すると、独自の条件に基づいてリストを絞り込むことができます。これらは、Campaign クエリモデラーを使用して設計されています。カスタムフィルターを作成するには、次の手順に従います。

1. フィルターパネルを開き、パネルの下部にある「**ルールを追加**」ボタンをクリックします。

1. クエリモデラーが開きます。ニーズに応じて、フィルター条件を定義して組み合わせます。クエリモデラーの使用方法について詳しくは、[この節](../query/query-modeler-overview.md)を参照してください。

   次の例は、ランニング部門またはヨガ部門のオペレーターによって実行された SMS キャンペーンを、キャンペーンリストに表示するように設計されたカスタムフィルターを示しています。

   ![部門別にフィルタリングされた SMS キャンペーンを示すカスタムフィルターの例](assets/filters-sample.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

1. カスタムフィルターを設定したら、「**[!UICONTROL 確認]**」をクリックしてリストに適用します。