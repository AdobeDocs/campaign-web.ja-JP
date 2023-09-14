---
audience: end-user
title: オーディエンスの監視と管理
description: Adobe Campaign Web でオーディエンスを監視および管理する方法について説明します
badge: label="Beta"
source-git-commit: 4924653e67f77a2108574e743c9016c6fc95a7e6
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 9%

---


# オーディエンスの監視と管理 {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_read_only"
>title="このオーディエンスは読み取り専用です"
>abstract="このオーディエンスを編集する権限がありません。 必要に応じて、管理者に連絡し、アクセス権の付与を依頼してください。"

Campaign Web で使用できるオーディエンスのリストには、 **[!UICONTROL オーディエンス]** メニュー。

![](assets/audiences-list.png)

オーディエンスは複数のソースから作成できます。 The **[!UICONTROL Origin]** 列は、特定のオーディエンスが作成された場所を示します。

* **[!UICONTROL Adobe Campaign]**：これらのオーディエンスはAdobe Campaign V8 コンソールで作成されます。 詳しくは、[Campaign v8（クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html?lang=ja){target="_blank"}を参照してください。

* **[!UICONTROL ADOBE EXPERIENCE PLATFORM:]** これらのオーディエンスは、Adobe Experience Platform内で作成され、宛先ソースとAdobeの統合を使用して Campaign Web に統合されます。 でこの統合を設定する方法を説明します。 [Campaign v8（クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html)

* **[!UICONTROL Adobe Campaign WebUI]**：これらのオーディエンスは、Campaign の Web オーディエンスワークフローを使用して作成されます。 [オーディエンスの作成方法を説明します](create-audience.md)

オーディエンスの詳細を取得するには、リストからオーディエンスを開きます。 オーディエンスのプロパティと、オーディエンスに含まれているプロファイルの数が表示されます。 オーディエンス数は、いつでも **[!UICONTROL 計算]** 」ボタンをクリックします。

The **[!UICONTROL データ]** 「 」タブでは、オーディエンスの一部であるプロファイルを視覚化できます。 列をさらに追加することでこのビューをカスタマイズしたり、詳細フィルターを利用して表示されるデータを絞り込んだりできます。

![](assets/audiences-details.png)

オーディエンスを複製または削除するには、 **[!UICONTROL その他のアクション]** ボタンが表示されます。
