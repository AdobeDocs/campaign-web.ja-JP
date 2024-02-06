---
title: ランディングページの作成
description: Campaign Web でランディングページを設定して公開する方法を説明します
badge: label="限定提供（LA）"
source-git-commit: 7635ab284900c8a4cd5ceca5675e57dbedb39f3a
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 8%

---

# ランディングページの作成と公開 {#create-lp}

>[!CONTEXTUALHELP]
>id="acw_landingpages_menu"
>title="ランディングページの作成と管理"
>abstract="Adobe Campaignでは、ランディングページを作成、デザインおよび共有して、組み込みのテンプレートに基づいて、獲得、購読/購読解除およびブロックリストの使用例を管理できる、オンライン Web ページにユーザーを誘導できます。"

Adobe Campaignでは、ランディングページを作成、デザインおよび共有して、組み込みのテンプレートに基づいて、獲得、購読/購読解除およびブロックリストの使用例を管理できる、オンライン Web ページにユーザーを誘導できます。

## ランディングページへのアクセス {#access-landing-pages}

ランディングページのリストにアクセスするには、「 **[!UICONTROL キャンペーン管理]** > **[!UICONTROL ランディングページ]** を選択します。

![](assets/lp-inventory.png)

The **[!UICONTROL ランディングページ]** 在庫には、作成されたすべての品目が表示されます。 フィルタリングするには、 **フィルターを表示** 」ボタンをクリックします。 ドロップダウンリストを使用して結果を特定の[フォルダー](../get-started/permissions.md#folders)に制限したり、[クエリモデラー](../query/query-modeler-overview.md)を使用してルールを追加したりできます。

![](assets/lp-inventory-filter.png)

<!--From this list, you can access the [landing page Live report](../reports/lp-report-live.md) or [landing page Global report](../reports/lp-report-global.md) for published items.-->

>[!CAUTION]
>
>Campaign Web のクライアントコンソールから作成したランディングページは、表示または編集できません。 詳しくは、 [Campaign コンソールのドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/content/webapps.html){target="_blank"}.

<!--If you unpublish a landing page which is referenced in a message, the link to the landing page will be broken and an error page will be displayed. You cannot delete a published landing page. To delete it, you must first unpublish it.-->

ランディングページは複製または削除できます。 ランディングページの横にある 3 つのドットをクリックし、目的のアクションを選択します。

## ランディングページの作成 {#create-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_properties"
>title="ランディングページのプロパティを定義する"
>abstract="ラベルなどのプロパティフィールドに入力し、必要に応じてスキーマを変更します。 また、内部名の編集、ランディングページの保存先フォルダーの変更、説明の入力をおこなうこともできます。"

>[!CONTEXTUALHELP]
>id="acw_landingpages_pages_list"
>title="ページのコンテンツを定義"
>abstract="このランディングページの一部である各ページのコンテンツを編集します。"

>[!CONTEXTUALHELP]
>id="acw_landingpages_schedule"
>title="ランディングページのスケジュール設定"
>abstract="ランディングページの開始日と終了日を定義できます。 ページが期限切れの場合、 **有効期限** ページが表示されます。"


>[!CONTEXTUALHELP]
>id="acw_landingpages_primarypage"
>title="プライマリページの設定を定義する"
>abstract="プライマリページは、E メールや Web サイトなど、ランディングページへのリンクをクリックした後、ユーザーに対して直ちに表示されます。"

>[!CONTEXTUALHELP]
>id="acw_landingpages_subscription"
>title="サブスクリプションランディングページを設定"
>abstract="購読ページを使用すると、顧客はサービスを購読できます。"

<!--The main steps to create landing pages are as follows:

![](assets/lp-creation-process.png)-->

1. 次から： **[!UICONTROL ランディングページ]** 在庫、クリック **[!UICONTROL ランディングページを作成]**.

   ![](assets/lp-create-button.png)

1. テンプレートを選択：
   * **[!UICONTROL 獲得]**：ランディングページのデフォルトテンプレートで、プロファイルデータを取得および更新できます。
   * **[!UICONTROL 購読]**：サービスのサブスクリプションをオファーするには、このテンプレートを使用します。
   * **[!UICONTROL 購読解除]**：サービスの購読登録者に送信された E メールからリンクできるテンプレートで、これを使用して登録者がこのサービスから購読解除できます。
   * **[!UICONTROL ブロックリストに加える]**：プロファイルが Campaign からの連絡を受けたくない場合に使用するテンプレートです。 管理の詳細をブロックリストに加える説明します

   ![](assets/lp-templates.png)

1. 「**[!UICONTROL 作成]**」をクリックします。

1. ラベルなどのプロパティフィールドに入力します。 デフォルトでは、ランディングページは **[!UICONTROL Web アプリケーション]** フォルダー。 変更するには、 **[!UICONTROL その他のオプション]**. [詳しくは、フォルダーの操作方法を参照してください](../get-started/permissions.md#folders)

   ![](assets/lp-properties.png)

1. Adobe Analytics の **[!UICONTROL データのプリロード]** 「 」セクションでは、次の 2 つのオプションがデフォルトで選択されています。

   * The **[!UICONTROL フォームで参照されるデータを事前入力]** 「 」オプションを使用すると、フォームの入力および結合フィールドに一致するデータを自動的にプリロードします。

   * プロファイルを更新しない場合、「**[!UICONTROL ID がない場合にプリロードをスキップ]**」オプションを選択する必要があります。この場合、入力した各プロファイルは、フォームの承認後にデータベースに追加されます。例えば、フォームが Web サイトに投稿される際に、このオプションが使用されます。

1. Adobe Analytics の **[!UICONTROL ページ]** セクションで、 **[!UICONTROL コンテンツを編集]** ボタンをクリックします。 各ページのコンテンツは既に入力済みです。 必要に応じて編集します。 [詳細情報](lp-content.md)

   ![](assets/lp-pages.png)

1. The **[!UICONTROL プリロードされたレコードを更新]** オプションはデフォルトで選択されています。 ランディングページを使用してデータベースに格納されたプロファイルを更新する場合、プリロードボックスを使用できます。 プリロードボックスを使用すると、データベース内で更新されるレコードの検索方法を指定できます。 また、ランディングページの現在のコンテキストのフィールドから選択し、データベースで対応するプロファイルを見つけるために使用するフィールドも選択できます。

   ![](assets/lp-storage-schedule.png)

1. ランディングページの開始日と終了日を定義できます。 選択 **[!UICONTROL スケジュールを有効にする]** 日付を設定します。 ページが期限切れの場合、 **[!UICONTROL 有効期限]** ページが表示されます。

1. クリック **[!UICONTROL レビューと公開]**.

すべてのページを設定およびデザインしたら、次の操作を実行できます。 [テスト](#test-landing-page) および [公開](#publish-landing-page) ランディングページを作成します。

## ランディングページのテスト {#test-landing-page}

>[!CONTEXTUALHELP]
>id="acw_landingpages_simulate"
>title="ランディングページをシミュレート"
>abstract="ランディングページのプレビューは、Campaign Web ユーザーインターフェイスで表示するか、新しい Web ブラウザータブで開くことができます。"

>[!CONTEXTUALHELP]
>id="ac_preview_lp_profiles"
>title="ランディングページのプレビューとテスト"
>abstract="ランディングページの設定とコンテンツを定義したら、テストプロファイルを使用してプレビューできます。"

ランディングページの設定とコンテンツを定義したら、テストプロファイルを使用してプレビューできます。 以下を挿入した場合、 [パーソナライズされたコンテンツ](../personalization/gs-personalization.md)を使用すると、テストプロファイルデータを使用して、このコンテンツがランディングページにどのように表示されるかを確認できます。

>[!CAUTION]
>
>メッセージをプレビューし、配達確認を送信するには、使用可能なテストプロファイルが必要です。 方法を学ぶ [テストプロファイルを作成](../audience/test-profiles.md).

1. ランディングページのインターフェイスで、 **[!UICONTROL コンテンツをシミュレート]** ボタンをクリックして、テストプロファイルの選択にアクセスします。

   ![](assets/lp-simulate-content.png)

1. 次から： **[!UICONTROL シミュレート]** 画面で、1 つ以上のテストプロファイルを選択します。

   テストプロファイルを選択する手順は、メッセージをテストする場合と同じです。 詳しくは、 [プレビューとテスト](../preview-test/preview-test.md) 」セクションに入力します。

1. 選択 **[!UICONTROL プレビューを開く]** をクリックして、ランディングページをテストします。

   ![](assets/lp-open-preview.png)

1. ランディングページのプレビューが新しいタブで開きます。 パーソナライズされた要素は、選択したテストプロファイルデータに置き換えられます。

   ![](assets/lp-preview.png)

1. 他のテストプロファイルを選択して、ランディングページの各バリアントのレンダリングをプレビューします。

<!--Can you preview Confirmation/Error/Expiration pages?-->

## ランディングページの公開 {#publish-landing-page}

ランディングページの準備が整ったら、公開して、メッセージで使用できるようにします。

ランディングページが公開されると、ランディングページは **[!UICONTROL 公開済み]** ステータス。 これで、ライブ状態になり、使用できる状態になりました。

![](assets/lp-published.png)

公開後、 **[!UICONTROL ランディングページの URL]** Web ブラウザー内で、ページの上部に表示される。

ランディングページの影響は、ログや特定のレポートを通じて監視できます。
