---
audience: end-user
title: オーディエンスの監視と管理
description: Adobe Campaign Web でオーディエンスを監視および管理する方法について説明します
badge: label="Beta"
source-git-commit: f9693c08e1f0a5b5644e8026b7dfe788ee6499c4
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---


# オーディエンスの監視と管理 {#create-audiences}

Campaign Web で使用できるオーディエンスのリストには、 **[!UICONTROL オーディエンス]** メニュー。

![](assets/audiences-list.png)

オーディエンスは複数のソースから作成できます。 The **[!UICONTROL Origin]** 列は、特定のオーディエンスが作成された場所を示します。

* **[!UICONTROL ADOBE EXPERIENCE PLATFORM:]** これらのオーディエンスは、Adobe Experience Platform内で作成され、宛先ソースとAdobeの統合を使用して Campaign Web に統合されます。 でこの統合を設定する方法を説明します。 [Campaign v8（クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html)

* **[!UICONTROL Adobe Campaign]**：これらのオーディエンスは、Campaign の Web オーディエンスワークフローを使用して作成されています。 [オーディエンスの作成方法を説明します](create-audience.md)

*他の起源は？ 習慣なのか？ どこで定義しますか？*

*タイプ列：フィルターでは使用できません。通常 異なるタイプ、グループとは何ですか？ リスト ?*

オーディエンスの詳細を取得するには、リストからオーディエンスを開きます。 オーディエンスのプロパティと、オーディエンスに含まれているプロファイルの数が表示されます。 オーディエンス数は、いつでも **[!UICONTROL 計算]** 」ボタンをクリックします。

The **[!UICONTROL データ]** 「 」タブでは、オーディエンスの一部であるプロファイルを視覚化できます。 列をさらに追加することでこのビューをカスタマイズしたり、詳細フィルターを利用して表示されるデータを絞り込んだりできます。

![](assets/audiences-details.png)

オーディエンスを複製または削除するには、 **[!UICONTROL その他のアクション]** ボタンが表示されます。

*オーディエンスが重複する場合、は (1) などの名前を保持しません。*