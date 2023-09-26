---
audience: end-user
title: オーディエンスの監視と管理
description: Adobe Campaign Web でオーディエンスを監視および管理する方法について説明します
badge: label="Beta"
source-git-commit: 21436695f6f4bc9e99bb7983e4705cbbe40f07eb
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 14%

---


# オーディエンスの監視と管理 {#monitor}

>[!CONTEXTUALHELP]
>id="acw_audiences_workflow_error_data_execution"
>title="オーディエンスエラー"
>abstract="オーディエンスデータを使用できません。 ワークフローの実行が終了するまでお待ちください。"

Campaign Web で使用できるオーディエンスのリストには、 **[!UICONTROL オーディエンス]** メニュー。

![](assets/audiences-list.png)

オーディエンスは複数のソースから作成できます。 The **[!UICONTROL Origin]** 列は、特定のオーディエンスが作成された場所を示します。

* **[!UICONTROL Adobe Campaign]**：これらのオーディエンスはAdobe Campaign V8 コンソールで作成されます。 詳しくは、[Campaign v8（クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html?lang=ja){target="_blank"}を参照してください。

* **[!UICONTROL ADOBE EXPERIENCE PLATFORM:]** これらのオーディエンスは、Adobe Experience Platform内で作成され、宛先ソースとAdobeの統合を使用して Campaign Web に統合されます。 でこの統合を設定する方法を説明します。 [Campaign v8（クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

>[!NOTE]
>
>Campaign で Adobe Experience Platform オーディエンスを使用するには、アドビのソースおよび宛先との統合を設定する必要があります。[Campaign v8（クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}を参照してください。

* **[!UICONTROL Adobe Campaign WebUI]**：これらのオーディエンスは、Campaign の Web オーディエンスワークフローを使用して作成されます。 [オーディエンスの作成方法を説明します](create-audience.md)

オーディエンスの詳細を取得するには、リストからオーディエンスを開きます。 オーディエンスのプロパティと、オーディエンスに含まれているプロファイルの数が表示されます。 オーディエンス数は、いつでも **[!UICONTROL 計算]** 」ボタンをクリックします。

The **[!UICONTROL データ]** 「 」タブでは、オーディエンスの一部であるプロファイルを視覚化できます。 列をさらに追加することでこのビューをカスタマイズしたり、詳細フィルターを利用して表示されるデータを絞り込んだりできます。

![](assets/audiences-details.png)

オーディエンスを複製または削除するには、 **[!UICONTROL その他のアクション]** ボタンが表示されます。