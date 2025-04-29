---
audience: end-user
title: オーディエンスの基本を学ぶ
description: Adobe Campaign web でオーディエンスを操作する方法を説明します。
exl-id: ce0785a0-6af5-4ea1-ace7-0ce9d3ff065f
source-git-commit: b330230a031a366b674ebac37681274ee89ec6c8
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 49%

---

# オーディエンスの基本を学ぶ {#monitor-manage}

>[!CONTEXTUALHELP]
>id="acw_audiences_properties"
>title="プロパティ"
>abstract="ここでは、オリジンやストレージフォルダーなど、オーディエンスプロパティの概要を確認できます。 「**前回のワークフロー**」セクションのリンクをクリックして、オーディエンスの作成に使用したワークフローを開きます。"

>[!CONTEXTUALHELP]
>id="acw_audiences_count"
>title="オーディエンスサイズ"
>abstract="ここでは、オーディエンス内のプロファイルの合計数を確認できます。「**計算**」ボタンをクリックして、オーディエンスの結果を更新および再計算します。"

>[!CONTEXTUALHELP]
>id="acw_audiences_targeting"
>title="ターゲティング"
>abstract="ターゲティング"

>[!CONTEXTUALHELP]
>id="acw_audiences_workflow_error_data_execution"
>title="オーディエンスエラー"
>abstract="オーディエンスデータは利用できません。ワークフローの実行が終了するまでお待ちください。"

オーディエンスは配信のメインターゲット、つまりメッセージを受信するプロファイルです。Campaign Web で使用できるオーディエンスのリストには、**[!UICONTROL オーディエンス]**&#x200B;メニューからアクセスできます。

![Campaign Web で使用可能なオーディエンスのリストを示すスクリーンショット。](assets/audiences-list.png){zoomable="yes"}

オーディエンスは複数のソースから作成できます。**[!UICONTROL 接触チャネル]** 列は、特定のオーディエンスが作成された場所を示します。

* **[!UICONTROL Adobe Campaign]**：これらのオーディエンスは、[Adobe Campaign web ユーザーインターフェイス ](create-audience.md) または [Adobe Campaign v8 クライアントコンソール ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html?lang=ja){target="_blank"} で作成されています。

* **[!UICONTROL Adobe Experience Platform：]**&#x200B;これらのオーディエンスは、Adobe Experience Platform 内で作成され、アドビのソースおよび宛先との統合を使用して Campaign web に統合されます。この統合の設定方法については、[Campaign v8 （クライアントコンソール）ドキュメント ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html?lang=ja){target="_blank"} を参照してください。

  ➡️ [この機能をビデオで確認](#video)

オーディエンスに関する追加情報を取得するには、リストからオーディエンスを開きます。 オーディエンスプロパティが、オーディエンスに含まれるプロファイルの数と共に表示されます。 「**[!UICONTROL 計算]** ボタンを使用して、いつでもオーディエンス数を更新できます。

オーディエンスの一時スキーマをプレビューするには、「プロパティ」セクションの **[!UICONTROL スキーマプレビュー]** ボタンをクリックします。

「**[!UICONTROL データ]**」タブを使用すると、オーディエンスの一部であるプロファイルを視覚化できます。 列を追加してこのビューをカスタマイズするか、詳細フィルターを使用して表示されるデータを絞り込みます。

![ プロファイルやカスタマイズオプションなど、オーディエンスの詳細を示すスクリーンショット。](assets/audiences-details.png){zoomable="yes"}

オーディエンスを複製または削除するには、オーディエンス名の横またはオーディエンス詳細画面内にあるオーディエンスリストに表示される「**[!UICONTROL その他のアクション]**」ボタンをクリックします。

## チュートリアルビデオ {#video}

Adobe Campaign web ユーザーインターフェイスで Experience Platform オーディエンスを使用する宛先を作成する方法について説明します。

>[!VIDEO](https://video.tv.adobe.com/v/3427635?quality=12)

Adobeのソースと宛先の統合を設定する方法について詳しくは、[Campaign v8 （クライアントコンソール）ドキュメント ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html?lang=ja){target="_blank"} を参照してください。