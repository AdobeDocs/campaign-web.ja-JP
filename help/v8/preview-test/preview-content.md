---
audience: end-user
title: 配信コンテンツのプレビュー
description: Campaign web UI で配信コンテンツをプレビューする方法を学ぶ
exl-id: 663a8395-c5b7-4427-bfdd-055230f9bc05
badge: label="限定提供（LA）"
source-git-commit: 7b42927b689bfc762c61fa52e4af23e8c283f486
workflow-type: ht
source-wordcount: '384'
ht-degree: 100%

---


# メッセージコンテンツのプレビュー {#preview-content}

[!DNL Campaign] コンテンツシミュレーション機能を使用して、メッセージを送信する前にコンテンツをプレビューします。これにより、パーソナライゼーションを制御し、受信者に対するパーソナライゼーションの表示方法を確認できます。

配信のコンテンツをプレビューするには、次の手順に従います。

1. 配信のコンテンツを編集画面または[メールデザイナー](../email/get-started-email-designer.md)を参照します。

1. 「**[!UICONTROL コンテンツをシミュレート]**」ボタンをクリックします。

   ![](assets/simulate-button.png)

1. パーソナライズされたコンテンツのプレビューに使用するプロファイルを選択するには、次を使用します。

   * **[!UICONTROL テストプロファイルを追加]**：メールと SMS 配信のプレビュー用

   * **[!UICONTROL サブスクライバーを追加]**：プッシュ通知のプレビュー用

1. テストプロファイルとプロファイルを組み合わせて、メールまたは SMS メッセージをプレビューできます。

   * 「**[!UICONTROL テストプロファイル]**」タブには、データベース内の架空の追加受信者であるすべてのシードアドレスが一覧表示されます。

     ![](assets/simulate-select-profiles.png)

     >[!NOTE]
     >
     >テストプロファイルは、**[!UICONTROL 顧客管理]**／**[!UICONTROL プロファイル]**&#x200B;メニューから作成できます。[詳細情報](../audience/test-profiles.md#create-test-profiles)

   * 「**[!UICONTROL プロファイル]**」タブには、コンソールから&#x200B;**[!UICONTROL プロファイルとターゲット]**&#x200B;フォルダーに保存されたすべての受信者がリストされます。[!DNL Campaign]詳しくは、[Campaign v8（クライアントコンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/view-profiles.html?lang=ja){target="_blank"}を参照してください。

     >[!NOTE]
     >
     >また、Campaign web UI の対応するタブから、プロファイルを表示および管理することもできます。[詳細情報](../audience/about-recipients.md)

1. テストプロファイルリストまたはプロファイルリストを参照する際に、フィルターを使用して検索を絞り込むことができます。

   ![](assets/simulate-test-profile-filter.png)

   例えば、**[!UICONTROL 見込み客]**&#x200B;ステータスとなっている、すべてのテストプロファイルを検索するルールを定義できます。ルールの追加方法については、[クエリモデラー](../query/query-modeler-overview.md)を参照してください。

1. 「**[!UICONTROL 選択]**」をクリックして選択内容を確定します。

   配信コンテンツのプレビューが、**[!UICONTROL シミュレート]**&#x200B;画面の右側のパネルに表示されます。パーソナライズされた要素は、左側のパネルで選択したプロファイルのデータに置き換えられます。

   ![](assets/simulate-preview.png)

1. 複数のプロファイルを追加した場合は、リスト内のプロファイルを切り替えて、対応する配信コンテンツをプレビューできます。また、左側のパネルの対応するボタンを使用して、さらにテストプロファイルを追加したり、選択をクリアしたりすることもできます。

1. メール配信の場合、右上隅の専用アイコンを使用して、**[!UICONTROL ズームレベル]**&#x200B;を調整し、デスクトップまたはモバイルデバイスでコンテンツをプレビューできます。

1. **[!UICONTROL シミュレート]**&#x200B;画面では、次の操作も実行できます。
   * 検証用の特定の受信者へのテスト配信の送信 - [詳細情報](test-deliveries.md)
   * 送信済みテスト配信のログへのアクセス - [詳細情報](test-deliveries.md#access-test-deliveries)
   * メールのみの場合、一般的なメールクライアントでのメッセージコンテンツのレンダリングの確認 - [詳細情報](email-rendering.md)



