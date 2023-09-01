---
audience: end-user
title: 既存オーディエンスの選択
description: オーディエンスの選択方法を学ぶ
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
badge: label="ベータ版"
source-git-commit: 334014d3d89c878617b8e43ea73c9ff4e957f6d7
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 58%

---


# 既存オーディエンスの選択 {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="既存オーディエンスの選択"
>abstract="リストを参照して、既存のオーディエンスを選択します。 「フィルターを表示」アイコンを使用してリストをフィルターするか、特定のフォルダーを選択します。"

この節では、メール配信のターゲット母集団を定義する際に、既存のオーディエンスを選択する方法について説明します。

また、次のこともできます。

* 新しいオーディエンスを作成します。[詳細情報](segment-builder.md)
* 外部ファイルからオーディエンスを読み込みます（E メールの場合のみ）。 [詳細情報](file-audience.md)
* Adobe Experience Platform オーディエンスの使用。[詳細情報](aep-audience.md)


メッセージの既存のオーディエンスを選択するには、次の手順に従います。

1. 配信作成アシスタントの「**オーディエンス**」セクションで、「**[!UICONTROL オーディエンスを選択]**」ボタンをクリックします。

   ![](assets/create-audience.png)

1. 既存のオーディエンスを使用するには、「**[!UICONTROL オーディエンスを選択]**」を選択します。このメールで使用する新しいオーディエンスを作成するには、「**独自に作成**」を選択します。[こちら](segment-builder.md)を参照してください。

   この画面には、現在のフォルダーの既存のすべてのオーディエンスが表示されます。

   ![](assets/create-audience2.png)

   オーディエンスは **対象ユーザ** 左メニュー。 クライアントコンソールでも作成できます。

   Adobe Experience Platformオーディエンスを使用するには、宛先との統合を設定する必要があります。 詳しくは、 [Adobe Experience Platform Destinations ドキュメント](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=ja){target="_blank"}.

1. オーディエンスを選択し、「**選択**」をクリックします。
1. 以下を使用します。 **フィルターを表示** アイコンをクリックしてフィルターオプションを表示します。 クリック **ルールを追加** ルールビルダーにアクセスするには：ルールビルダーを使用して、オーディエンスのリストに対する詳細フィルターを作成できます。 このルールビルダーの使用方法を説明します [セクション](segment-builder.md).

   ![](assets/create-audience4.png)

1. 「**保存**」をクリックします。

また、コントロール母集団を設定して、キャンペーンの影響を測定することもできます。コントロール母集団はメッセージを受信しません。これにより、メッセージを受信した母集団の行動と、受信しなかった連絡先の行動を比較できます。詳しくは、[こちら](control-group.md)を参照してください。