---
audience: end-user
title: 既存オーディエンスの選択
description: オーディエンスの選択方法を学ぶ
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
badge: label="Beta"
source-git-commit: 424caa898ff9d73f3520aa6d682eb1963d992069
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 43%

---


# 既存オーディエンスの選択 {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="既存オーディエンスの選択"
>abstract="リストを参照して、既存のオーディエンスを選択します。「フィルターを表示」アイコンを使用してリストをフィルターするか、特定のフォルダーを選択します。"

この節では、配信のターゲット母集団を定義する際に、既存のオーディエンスを選択する方法について説明します。 配信のメインターゲットを定義する際には、次の操作も実行できます。

* [1 回限りのオーディエンスの構築](one-time-audience.md) ルールビルダーを使用して、
* [外部ファイルからオーディエンスを読み込む](file-audience.md) （e メールの場合のみ）。

配信のターゲットに設定できるオーディエンスには、 **対象ユーザ** 左メニュー。 これらは、クライアントコンソール、Campaign Web オーディエンスワークフロー、Adobe Experience Platformなど、複数のソースから作成されます。 [オーディエンスの監視および管理方法について説明します。](manage-audience.md)

メッセージの既存のオーディエンスを選択するには、次の手順に従います。

1. 次から： **対象ユーザ** 配信作成アシスタントの「 」セクションで、 **[!UICONTROL オーディエンスを選択]** ボタンを選択し、

   ![](assets/create-audience.png)

1. 既存のオーディエンスを使用するには、「**[!UICONTROL オーディエンスを選択]**」を選択します。この画面には、現在のフォルダーの既存のすべてのオーディエンスが表示されます。

   ![](assets/create-audience2.png)

   Adobe Experience Platform からオーディエンスを選択するには、画面のフィルターセクションから `AEP Audiences folder` を参照します。

   ![](assets/select-audience-folder.png)

1. 「フィルター」セクションでは、フィルターオプションにアクセスしてオーディエンスリストを絞り込むことができます。 これをおこなうには、 **ルールを追加** ：ルールビルダーにアクセスします。このビルダーを使用して、オーディエンスのリスト用の詳細フィルターを作成できます。 [ルールビルダーの使用方法を説明します](segment-builder.md)

   ![](assets/create-audience4.png)

1. クリック **確認** オーディエンスを配信のメインターゲットとして追加します。 その後も、 **ルールを編集** 」ボタンをクリックします。

   ![](assets/refine-audience.png)

   また、コントロール母集団を設定して、キャンペーンの影響を測定することもできます。コントロール母集団はメッセージを受信しません。これにより、メッセージを受信した母集団の行動と、受信しなかった連絡先の行動を比較できます。[詳細情報](control-group.md)
