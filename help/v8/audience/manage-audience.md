---
audience: end-user
title: オーディエンスの基本を学ぶ
description: Adobe Campaign web でオーディエンスを操作する方法を説明します。
exl-id: ce0785a0-6af5-4ea1-ace7-0ce9d3ff065f
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 66%

---

# オーディエンスの基本を学ぶ {#monitor-manage}

>[!CONTEXTUALHELP]
>id="acw_audiences_properties"
>title="Properties"
>abstract="Here you can find a summary of the audience properties, such as its origin or its storage folder. Click the link in the **Last workflow** section to open the workflow that has been used to create the audience."

>[!CONTEXTUALHELP]
>id="acw_audiences_count"
>title="Audience size"
>abstract="Here you can find the total number of profiles within the audience. Click the **Calculate** button to update and recalculate the audience results."

>[!CONTEXTUALHELP]
>id="acw_audiences_targeting"
>title="Targeting"
>abstract="Targeting"

>[!CONTEXTUALHELP]
>id="acw_audiences_workflow_error_data_execution"
>title="Audience error"
>abstract="Audience data is not available. Please wait for the end of the workflow execution."

オーディエンスは配信のメインターゲット、つまりメッセージを受信するプロファイルです。Campaign Web で使用できるオーディエンスのリストには、**[!UICONTROL オーディエンス]**&#x200B;メニューからアクセスできます。

![Campaign Web で使用可能なオーディエンスのリストを示すスクリーンショット。](assets/audiences-list.png){zoomable="yes"}

オーディエンスは複数のソースから作成できます。**[!UICONTROL 接触チャネル]** 列は、特定のオーディエンスが作成された場所を示します。

* **[!UICONTROL Adobe Campaign]**：これらのオーディエンスは、[Adobe Campaign web ユーザーインターフェイス](create-audience.md)または [Adobe Campaign v8 クライアントコンソール](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html?lang=ja){target="_blank"}で作成されています。

* **[!UICONTROL Adobe Experience Platform：]**&#x200B;これらのオーディエンスは、Adobe Experience Platform 内で作成され、アドビのソースおよび宛先との統合を使用して Campaign web に統合されます。この統合を設定する方法について詳しくは、[Campaign v8（クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html?lang=ja){target="_blank"}を参照してください。

  ➡️ [この機能をビデオで確認](#video)

オーディエンスに関する追加情報を取得するには、リストからオーディエンスを開きます。 オーディエンスプロパティが、オーディエンスに含まれるプロファイルの数と共に表示されます。 「**[!UICONTROL 計算]** ボタンを使用して、いつでもオーディエンス数を更新できます。

「**[!UICONTROL データ]**」タブを使用すると、オーディエンスの一部であるプロファイルを視覚化できます。 列を追加してこのビューをカスタマイズするか、詳細フィルターを使用して表示されるデータを絞り込みます。

![ プロファイルやカスタマイズオプションなど、オーディエンスの詳細を示すスクリーンショット。](assets/audiences-details.png){zoomable="yes"}

オーディエンスを複製または削除するには、オーディエンス名の横またはオーディエンス詳細画面内にあるオーディエンスリストに表示される「**[!UICONTROL その他のアクション]**」ボタンをクリックします。

## チュートリアルビデオ {#video}

Adobe Campaign web ユーザーインターフェイスで Experience Platform オーディエンスを使用する宛先を作成する方法について説明します。

>[!VIDEO](https://video.tv.adobe.com/v/3427635?quality=12)

アドビのソースと宛先の統合を設定する方法について詳しくは、[Campaign v8（クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html?lang=ja){target="_blank"}を参照してください。