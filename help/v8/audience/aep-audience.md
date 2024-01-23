---
audience: end-user
title: Adobe Experience Platform オーディエンスの使用
description: Adobe Experience Platform のオーディエンスの使用方法
badge: label="限定提供（LA）"
exl-id: beb73107-3d27-40ac-afef-ac2b66ae8d34
source-git-commit: 703196ad2bb504eb1d50008af110f952d8045eaa
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 85%

---

# Adobe Experience Platform オーディエンスの使用{#aep-audience}

Adobe Campaign Managed Cloud Service の宛先とソースコネクタを使用すると、Adobe Campaign と Adobe Experience Platform をシームレスに統合できます。

Adobe Experience Platform オーディエンスを作成し、クライアントコンソールで使用できるようになったら、ユーザーは Campaign オーディエンスと同じようにこれを使用し、メッセージをパーソナライズして送信できます。

>[!NOTE]
>
>Campaign で Adobe Experience Platform オーディエンスを使用するには、アドビのソースおよび宛先との統合を設定する必要があります。[Campaign v8（クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html?lang=ja){target="_blank"}を参照してください。

配信のオーディエンスを選択するには、次の手順で実行することもできます。

* 新しいオーディエンスを作成します。[詳細情報](../query/query-modeler-overview.md)
* 外部ファイルのオーディエンスを読み込みます。[詳細情報](file-audience.md)
* 既存のオーディエンスを使用します。[詳細情報](add-audience.md)

配信用の Adobe Experience Platform オーディエンスを選択するには、次の手順に従います。

1. 配信作成アシスタントの「**オーディエンス**」セクションで、「**[!UICONTROL オーディエンスを選択]**」ボタンをクリックします。

   ![](assets/create-audience.png)

1. 既存のオーディエンスを使用するには、「**[!UICONTROL オーディエンスを選択]**」を選択します。このメールで使用する新しいオーディエンスを作成するには、「**独自に作成**」を選択します。[こちら](../query/query-modeler-overview.md)を参照してください。

   この画面には、現在のフォルダーに対して、Adobe Campaign クライアントコンソールで定義されたすべての既存のオーディエンスが表示されます。Adobe Experience Platform からオーディエンスを選択するには、画面のフィルターセクションから `AEP Audiences folder` を参照します。

   ![](assets/select-audience-folder.png)

   次のように、オーディエンスの接触チャネルに基づいてフィルタリングするルールを定義することもできます。

   「フィルター」セクションでは、フィルターオプションにアクセスしてオーディエンスリストを絞り込むことができます。これをおこなうには、 **ルールを追加** ：クエリモデラーにアクセスします。このモデラーを使用して、オーディエンスのリストの詳細フィルターを作成できます。 [クエリモデラーの使用方法を説明します](../query/query-modeler-overview.md)

   ![](assets/filter-on-aep-audience.png)

1. オーディエンスを選択し、「**選択**」をクリックします。

1. オーディエンスを絞り込む必要がある場合は、「**ルールを編集**」をクリックします。

   ![](assets/refine-audience.png)

1. クエリモデラーを使用すると、追加のフィルターでオーディエンスをエンリッチメントしたり、異なるオーディエンスを組み合わせたりできます。 [こちら](../query/query-modeler-overview.md)を参照してください。

1. 「**保存**」をクリックします。
