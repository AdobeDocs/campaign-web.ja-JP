---
audience: end-user
title: メールコンテンツのプレビュー
description: Campaign web UI でメールコンテンツをプレビューする方法を学ぶ
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
badge: label="Alpha" type="Positive"
source-git-commit: 7a58b8323dbecc7cca0ba513d98a5afb213d3bc2
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 28%

---


# メールコンテンツのプレビュー {#preview-content}

以下を使用： [!DNL Campaign] コンテンツシミュレーション機能を使用して、e メールを送信する前に e メールのコンテンツをプレビューできます。 これにより、パーソナライゼーションを制御し、受信者に対するパーソナライゼーションの表示方法を確認できます。

E メールのコンテンツをプレビューするには、次の手順に従います。

1. E メールを参照 [コンテンツを編集](../content/edit-content.md) screen または [メールデザイナー](../content/get-started-email-designer.md).

1. 次をクリック： **[!UICONTROL コンテンツをシミュレート]** 」ボタンをクリックします。

   ![](assets/simulate-button.png)

1. 以下を使用： **[!UICONTROL テストプロファイルを追加]** ボタンを使用して、パーソナライズされたコンテンツのプレビューに使用するプロファイルを選択します。

1. テストプロファイルとプロファイルを組み合わせて、メールをプレビューできます。

   * 「**[!UICONTROL テストプロファイル]**」タブには、データベース内の架空の追加受信者であるすべてのシードアドレスが一覧表示されます。

     >[!NOTE]
     >
     >テストプロファイルは、 [!DNL Campaign] コンソールを **[!UICONTROL リソース]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL シードアドレス]** フォルダー。 詳しくは、 [Campaign v8（コンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/using-seed-addresses/creating-seed-addresses.html){target="_blank"}

   * 「**[!UICONTROL プロファイル]**」タブには、 コンソールから&#x200B;**[!UICONTROL プロファイルとターゲット]**&#x200B;フォルダーに保存されたすべての受信者がリストされます。[!DNL Campaign][詳細情報](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/view-profiles.html){target="_blank"}

   ![](assets/simulate-select-profiles.png)

1. クリック **[!UICONTROL 選択]** をクリックして、両方のタブで選択内容を確認します。

   E メールのプレビューが **[!UICONTROL シミュレート]** 画面 パーソナライズされた要素は、左側のパネルで選択したプロファイルのデータに置き換えられます。

   ![](assets/simulate-preview.png)

1. 複数のプロファイルを追加した場合は、リスト内のプロファイルを切り替えて、対応するメールコンテンツをプレビューできます。また、左側のペインの対応するボタンを使用して、テストプロファイルをさらに追加し、選択を解除することもできます。

1. 次の項目を調整できます。 **[!UICONTROL ズームレベル]** および右上隅の専用アイコンを使用して、デスクトップまたはモバイルデバイスでコンテンツをプレビューします。

1. 次の **[!UICONTROL シミュレート]** 画面では、次のこともできます。
   * 一般的な E メールクライアントで E メールのレンダリングを確認します。 [詳細情報](email-rendering.md)
   * 検証のために特定の受信者にテストメールを送信します — [詳細情報](proofs.md)



