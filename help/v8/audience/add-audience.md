---
audience: end-user
title: 既存オーディエンスの選択
description: オーディエンスの選択方法を学ぶ
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
badge: label="Alpha" type="Positive"
source-git-commit: d4645689ebaa5439a01b2f558f398cbeb79089a7
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 95%

---


# 既存オーディエンスの選択 {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="既存オーディエンスの選択"
>abstract="オーディエンスは、Adobe Campaign v8 コンソールで定義されます。Adobe Experience Platform 統合を使用できる場合は、Platform で定義されたオーディエンスも表示されます。"

この節では、メール配信のターゲット母集団を定義する際に、既存のオーディエンスを選択する方法について説明します。

また、次のこともできます。

* 新しいオーディエンスを構築します。 [詳細情報](segment-builder.md)
* 外部ファイルからオーディエンスを読み込みます。 [詳細情報](file-audience.md)
* Adobe Experience Platform オーディエンスの使用。[詳細情報](aep-audience.md)


メッセージの既存のオーディエンスを選択するには、次の手順に従います。

1. 配信作成アシスタントの「**オーディエンス**」セクションで、「**[!UICONTROL オーディエンスを選択]**」ボタンをクリックします。

   ![](assets/create-audience.png)

1. 既存のオーディエンスを使用するには、「**[!UICONTROL オーディエンスを選択]**」を選択します。このメールで使用する新しいオーディエンスを作成するには、「**独自に作成**」を選択します。[こちら](segment-builder.md)を参照してください。

   この画面には、Adobe Campaign コンソールまたは Adobe Experience Platform で定義されたすべての既存オーディエンスが表示されます。

   ![](assets/create-audience2.png)

   >[!NOTE]
   >
   >Adobe Experience Platform オーディエンスを活用するには、宛先との統合を設定する必要があります。 [宛先に関するドキュメント](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=ja){target="_blank"}を参照してください。

1. オーディエンスを選択し、「**選択**」をクリックします。

1. オーディエンスを絞り込む必要がある場合は、「**ルールを編集**」をクリックします。

   ![](assets/create-audience3.png)

1. ルールビルダーでは、追加のフィルターを使用したり、様々なオーディエンスを組み合わせたりして、オーディエンスをエンリッチメントできます。[こちら](segment-builder.md)を参照してください。

   ![](assets/create-audience4.png)

1. 「**保存**」をクリックします。

また、コントロール母集団を設定して、キャンペーンの影響を測定することもできます。コントロール母集団はメッセージを受信しません。これにより、メッセージを受信した母集団の行動と、受信しなかった連絡先の行動を比較できます。[こちら](control-group.md)を参照してください。