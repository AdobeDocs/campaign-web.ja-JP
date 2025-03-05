---
audience: end-user
title: 外部配信の基本を学ぶ
description: Adobe Campaign Web で外部配信を作成して送信する方法について説明します
exl-id: 08fe9333-aa35-4acf-ba41-4c6895049bbc
source-git-commit: 1f3f3afb9b21ab37aeea73057d832cea172c00bf
workflow-type: ht
source-wordcount: '465'
ht-degree: 100%

---

# 外部配信の送信 {#gs-direct-mail}


Adobe Campaign では、Campaign の外部で作成された配信を処理して、外部システムを通じてパーソナライズされたメール、SMS メッセージまたはプッシュ通知（iOS および Android）を一括配信できます。

<!--The supported channels are Email, Mobile (SMS), and Push (iOs and Android).-->

外部配信を作成する際、Adobe Campaign では、すべてのターゲットプロファイルと選択したデータを含む抽出ファイルを自動的に生成します。このファイルは、選択したサーバーに送信され、そのサーバーで送信プロセスが処理されます。

## 専用の外部アカウントの作成 {#routing-external-account}

まず、外部配信で使用する特定の外部アカウントを設定する必要があります。**[!UICONTROL ルーティング]**&#x200B;タイプにする必要があります。

>[!NOTE]
>
>ルーティングタイプの外部アカウントを作成する方法について詳しくは、[この節](../administration/external-account.md#routing)を参照してください。

例えば、外部アカウントの&#x200B;**[!UICONTROL モバイル（SMS）]**&#x200B;チャネルを選択します。**[!UICONTROL 配信モード]**&#x200B;として「**[!UICONTROL 外部]**」がデフォルトで選択されます。

![](../administration/assets/external-account-delivery-mode.png){zoomable="yes"}

## 外部配信の作成と送信 {#create-external-delivery}

特定の外部アカウントを設定したら、外部配信を作成します。以下の手順に従います。

1. 配信を作成します。[詳細情報](create-deliveries.md)

   次の 3 つのオプションがあります。

   * **ワークフロー内**：外部チャネルアクティビティ（メール、SMS またはプッシュ）をワークフローに追加します。ワークフローの設定方法について詳しくは、[こちらのページ](../workflows/gs-workflow-creation.md)を参照してください。
   * **キャンペーン内**：キャンペーンを作成したら、メール、SMS またはプッシュチャネルの外部配信を作成できます。キャンペーンの設定について詳しくは、[こちらのページ](../campaigns/gs-campaigns.md)を参照してください。
   * **スタンドアロン配信**：個々の外部配信で顧客を直接、即座にエンゲージします。[詳しくは、配信の作成方法を参照してください](../msg/gs-deliveries.md)

1. 配信または配信テンプレートの[設定](../advanced-settings/delivery-settings.md)で、選択したチャネル（この例では、SMS チャネル）用に作成した外部アカウントを選択して、保存します。

   ![](assets/external-delivery-routing.png){zoomable="yes"}

   >[!NOTE]
   >
   >配信を作成する場合は、**[!UICONTROL ルーティング]**&#x200B;タイプの外部アカウントを使用して[配信テンプレート](delivery-template.md)を選択していることを確認します。適切に選択していない場合、[上記](#routing-external-account)で作成した専用アカウントを選択できません。

1. 配信の「**[!UICONTROL コンテンツ]**」セクションで、「**[!UICONTROL コンテンツを編集]**」をクリックします。

   ![](assets/external-delivery-edit-content.png){zoomable="yes"}

1. 標準配信とは異なり、メッセージ自体のコンテンツをデザインするわけではありません。代わりに、外部システムに送信されるファイルのプロパティと列を定義する必要があります。

   ![](assets/external-delivery-file-properties.png){zoomable="yes"}

   [ダイレクトメール配信](../direct-mail/content-direct-mail.md)で生成される抽出ファイルのコンテンツをデザインする場合と同じ手順に従います。

   * 抽出ファイルのプロパティを定義します。[詳細情報](../direct-mail/content-direct-mail.md#properties)
   * そのファイルにエクスポートする情報を含む列を選択します。[詳細情報](../direct-mail/content-direct-mail.md#content)

1. ファイルをプレビューして、配達確認<!--not in UI right now - to check-->を送信できます。[詳細情報](../direct-mail/send-direct-mail.md#preview-dm)

   ![](assets/external-delivery-simulate.png){zoomable="yes"}

1. 配信を送信して、抽出ファイルを生成します。[詳細情報](../direct-mail/send-direct-mail.md#send-dm)

配信を送信すると、抽出ファイルが自動的に生成され、配信テンプレートの設定で選択した[外部アカウント](../administration/external-account.md#create-ext-account)で指定した場所にエクスポートされます。

配信ページから KPI を追跡し、**[!UICONTROL ログ]**&#x200B;メニューからデータを追跡できます。
