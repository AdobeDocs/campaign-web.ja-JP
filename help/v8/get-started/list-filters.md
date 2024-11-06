---
audience: end-user
title: リストの参照とフィルタリング
description: Campaign Web v8 のリストを参照およびフィルタリングする方法の確認
exl-id: 46b83e8c-6c8c-40a1-a08b-9d0b438b80cb
source-git-commit: 8a68e1e95f2d030c9386e11ae3e7e07f1496bd84
workflow-type: ht
source-wordcount: '260'
ht-degree: 100%

---

# リストの参照とフィルタリング {#list-screens}

左側のナビゲーションメニューからのリンクのほとんどには、**配信**&#x200B;や&#x200B;**キャンペーン**&#x200B;のリストなど、オブジェクトのリストが表示されます。これらのリスト画面の一部は読み取り専用です。以下で説明するように、リスト表示をカスタマイズし、これらのリストをフィルタリングすることができます。

## リスト画面のカスタマイズ {#custom-lists}

リストは複数の列で表示されます。列の設定を変更すると、追加情報を表示できます。これを行うには、リストの右上隅にある「**カスタムレイアウトの列を設定**」アイコンをクリックします。

![](assets/config-columns.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

**列を設定**&#x200B;画面で、列の追加または削除や表示順序の変更を行うことができます。

リストの順序は、**ドラッグ＆ドロップ**&#x200B;するか、以下に示すように&#x200B;**上下の矢印**&#x200B;を使用して変更できます。

![](assets/list-reorder.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

例えば、次の設定の場合：

![](assets/columns.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

リストには、次の列が表示されます。

![](assets/column-sample.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

## データを並べ替え {#sort-lists}

また、任意の列見出しをクリックすると、リスト内の項目を並べ替えることができます。リストがその列で並べ替えられていることを示す（上または下）矢印が表示されます。

数値列または日付列の場合、**上向き**&#x200B;矢印はリストが昇順、**下向き**&#x200B;矢印は降順で並べ替えられていることを示します。文字列の列または英数字の列の場合、値はアルファベット順に表示されます。

## フィルター {#list-built-in-filters}

項目をすばやく見つけるには、検索バーを使用するか、組み込みフィルターやカスタムフィルターを使用して、コンテキスト条件に基づいてリストを調整します。

![](assets/filter.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

フィルターの使用方法と独自のカスタムフィルターの作成方法について詳しくは、[この節](../query/filter.md)を参照してください。

<!--
## Use advanced attributes {#adv-attributes}

>[!CONTEXTUALHELP]
>id="acw_attributepicker_advancedfields"
>title="Display advanced attributes"
>abstract="Only the most common attributes are displayed by default in the attribute list. Activate the **Display advanced attributes** toggle to see all available attributes for the current list in the left palette of the rule builder, such as nodes, groupings, 1-1 links, 1-N links."

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_advancedfields"
>title="Rule builder advanced fields"
>abstract="Only the most common attributes are displayed by default in the attribute list. Activate the **Display advanced attributes** toggle to see all available attributes for the current list in the left palette of the rule builder, such as nodes, groupings, 1-1 links, 1-N links."

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_properties_advanced"
>title="Rule builder advanced attributes"
>abstract="Only the most common attributes are displayed by default in the attribute list. Activate the **Display advanced attributes** toggle to see all available attributes for the current list in the left palette of the rule builder, such as nodes, groupings, 1-1 links, 1-N links."


Only most common attributes are displayed by default in the attribute list and filter configuration screens. Attributes which were set as `advanced` attributes in the data schema are hidden from the configuration screens. 

Activate the **Display advanced attributes** toggle to see all available attributes for the current list in the left palette of the rule builder, such as nodes, groupings, 1-1 links, 1-N links. The attribute list is updated instantly.


![](assets/adv-toggle.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}
-->