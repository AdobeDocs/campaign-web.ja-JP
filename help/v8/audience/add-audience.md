---
audience: end-user
title: 既存オーディエンスの選択
description: オーディエンスの選択方法を学ぶ
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
source-git-commit: a0da65d8facedb3730947eb969e362a367e4d317
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 93%

---


# 既存オーディエンスの選択 {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="既存オーディエンスの選択"
>abstract="リストを参照して、既存のオーディエンスを選択します。「フィルターを表示」アイコンを使用してリストをフィルターするか、特定のフォルダーを選択します。"

この節では、配信のターゲット母集団を定義する際に、既存のオーディエンスを選択する方法について説明します。配信のメインターゲットを定義する際には、次の操作も可能です。
* クエリモデラーを使用して、[1 回限りのオーディエンスを作成します](one-time-audience.md)。
* [外部ファイルのオーディエンスを読み込みます](file-audience.md)（メールの場合のみ）。

配信のターゲットに設定できるオーディエンスには、**オーディエンス**&#x200B;の左メニューからアクセスできます。オーディエンスは、クライアントコンソール、Campaign Web オーディエンスワークフロー、Adobe Experience Platformなど、複数のソースから選びます。[オーディエンスの詳細情報](manage-audience.md)

メッセージの既存のオーディエンスを選択するには、次の手順に従います。

1. から **対象読者** 「配信作成アシスタント」セクションで、 **[!UICONTROL オーディエンスを選択]** ボタンをクリックしてから、を選択 **[!UICONTROL オーディエンスを選択]**.

   ![](assets/create-audience.png){zoomable=&quot;yes&quot;}

1. この画面には、現在のフォルダーの既存のすべてのオーディエンスが表示されます。

   ![](assets/create-audience2.png){zoomable=&quot;yes&quot;}

   Adobe Experience Platform からオーディエンスを選ぶには、画面のフィルターセクションから `AEP Audiences folder` を参照します。[詳しくは、Adobe Experience Platform オーディエンスを参照してください](manage-audience.md#monitor)

   ![](assets/select-audience-folder.png){zoomable=&quot;yes&quot;}

1. 「フィルター」セクションでは、フィルターオプションにアクセスしてオーディエンスリストを絞り込むことができます。これを行うには、「**ルールを追加**」をクリックして、クエリモデラーにアクセスし、オーディエンスのリスト用の詳細フィルターを作成します。[クエリモデラーの使用方法を説明します](../query/query-modeler-overview.md)

   例えば、次のように、オーディエンスの接触チャネルに基づいてフィルタリングするルールを定義できます。

   ![](assets/filter-on-aep-audience.png){zoomable=&quot;yes&quot;}

1. 「**確認**」をクリックして、オーディエンスを配信のメインターゲットとして追加します。その後も、「**ルールを編集**」ボタンをクリックすれば、クエリモデラーを使用して、オーディエンスを絞り込むことができます。

   ![](assets/refine-audience.png){zoomable=&quot;yes&quot;}

   また、コントロール母集団を設定して、キャンペーンの影響を測定することもできます。コントロール母集団はメッセージを受信しません。これにより、メッセージを受信した母集団の行動と、受信しなかった連絡先の行動を比較できます。[詳細情報](control-group.md)
