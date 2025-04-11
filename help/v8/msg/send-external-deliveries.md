---
audience: end-user
title: 外部配信の基本を学ぶ
description: Adobe Campaign Web で外部配信を作成して送信する方法について説明します
exl-id: 08fe9333-aa35-4acf-ba41-4c6895049bbc
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 37%

---

# 外部配信の送信 {#gs-direct-mail}

Adobe Campaignを使用すると、Campaign 以外で作成された配信を管理して、外部システムを通じてパーソナライズされたメール、SMS メッセージまたはプッシュ通知（iOSおよびAndroid）を一括配信できます。

<!--The supported channels are Email, Mobile (SMS), and Push (iOS and Android).-->

外部配信を作成する場合、Adobe Campaignはすべてのターゲットプロファイルと選択したデータを含む抽出ファイルを自動的に生成します。 このファイルは、選択したサーバーに送信されます。サーバーが送信プロセスを処理します。

## 専用の外部アカウントの作成 {#routing-external-account}

外部配信で使用する特定の外部アカウントを設定する必要があります。 **[!UICONTROL ルーティング]**&#x200B;タイプにする必要があります。

>[!NOTE]
>
>ルーティングタイプの外部アカウントを作成する方法について詳しくは、[この節](../administration/external-account.md#routing)を参照してください。

例えば、外部アカウントの&#x200B;**[!UICONTROL モバイル（SMS）]**&#x200B;チャネルを選択します。**[!UICONTROL 配信モード]**&#x200B;として「**[!UICONTROL 外部]**」がデフォルトで選択されます。

![ 外部アカウント配信モードの設定 ](../administration/assets/external-account-delivery-mode.png){zoomable="yes"}

## 外部配信の作成と送信 {#create-external-delivery}

特定の外部アカウントを設定したら、外部配信を作成します。以下の手順に従います。

1. 配信を作成します。[詳細情報](create-deliveries.md)

   次の 3 つのオプションがあります。

   * **ワークフロー内**：外部チャネルアクティビティ（メール、SMS またはプッシュ）をワークフローに追加します。 ワークフローの設定手順について詳しくは、[ このページ ](../workflows/gs-workflow-creation.md) を参照してください。
   * **キャンペーンの場合**：キャンペーンを作成した後に、メール、SMS またはプッシュチャネルの外部配信を作成できます。 キャンペーンの設定について詳しくは、[こちらのページ](../campaigns/gs-campaigns.md)を参照してください。
   * **スタンドアロン配信**：個々の外部配信で顧客を直接、即座にエンゲージします。[詳しくは、配信の作成方法を参照してください](../msg/gs-deliveries.md)

1. 配信または配信テンプレート [ 設定 ](../advanced-settings/delivery-settings.md) で、選択したチャネル用に作成された外部アカウント（この例では SMS チャネル）を選択して保存します。

   ![ 外部配信ルーティング設定 ](assets/external-delivery-routing.png){zoomable="yes"}

   >[!NOTE]
   >
   >配信を作成する場合は、「ルーティング [ タイプの外部アカウントを使用する ](delivery-template.md) 配信テンプレート **[!UICONTROL が選択されていることを確認]** ます。 そうでない場合は、作成した専用アカウントを選択することはできません [ 上記 ](#routing-external-account)。

1. 配信の「**[!UICONTROL コンテンツ]**」セクションで、「**[!UICONTROL コンテンツを編集]**」をクリックします。

   ![ 外部配信のコンテンツの編集 ](assets/external-delivery-edit-content.png){zoomable="yes"}

1. 標準の配信とは異なり、メッセージのコンテンツ自体はデザインしません。 代わりに、外部システムに送信されるファイルのプロパティと列を定義します。

   ![ 外部配信用のファイルプロパティ設定 ](assets/external-delivery-file-properties.png){zoomable="yes"}

   [ダイレクトメール配信](../direct-mail/content-direct-mail.md)で生成される抽出ファイルのコンテンツをデザインする場合と同じ手順に従います。

   * 抽出ファイルのプロパティを定義します。[詳細情報](../direct-mail/content-direct-mail.md#properties)
   * ファイルにエクスポートする情報を含む列を選択します。 [詳細情報](../direct-mail/content-direct-mail.md#content)

1. ファイルをプレビューして配達確認を送信 <!--not in UI right now - to check-->. [詳細情報](../direct-mail/send-direct-mail.md#preview-dm)

   ![ 外部配信をシミュレート ](assets/external-delivery-simulate.png){zoomable="yes"}

1. 配信を送信して、抽出ファイルを生成します。[詳細情報](../direct-mail/send-direct-mail.md#send-dm)

配信が送信されると、抽出ファイルが自動的に生成され、配信テンプレートの設定で選択した [ 外部アカウント ](../administration/external-account.md#create-ext-account) で指定した場所に書き出されます。

配信ページから KPI を追跡し、**[!UICONTROL ログ]** メニューからデータを追跡します。