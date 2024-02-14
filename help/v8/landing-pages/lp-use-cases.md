---
solution: Journey Optimizer, Campaign, Campaign v8 Web User Interface
product: journey optimizer
title: ランディングページのユースケース
description: Journey Optimizer のランディングページで最も一般的なユースケースについて説明します
feature: Landing Pages, Subscriptions
topic: Content Management
role: User
level: Intermediate
keywords: ランディング, ランディングページ, ユースケース
source-git-commit: 3dcd4631a79ce2752e829f8259e0de1177f21984
workflow-type: tm+mt
source-wordcount: '1307'
ht-degree: 12%

---

# ランディングページの使用方法 {#lp-use-cases}

>[!CONTEXTUALHELP]
>id="acw_landingpages_url"
>title="URL をコピーする際は注意が必要です"
>abstract="ランディングページを完全にテストまたは活用するには、このリンクを Web ブラウザーや配信に直接コピー&amp;ペーストすることはできません。 代わりに、 **コンテンツをシミュレート** 関数を使用してテストし、ドキュメントに記載されている手順に従ってランディングページを適切に使用します。"

ランディングページを適切に使用するには、専用のオプションを使用して、配信でリンクとして参照する必要があります。

>[!CAUTION]
>
>ランディングページを最大限に活用するには、公開された配信ダッシュボードに表示されるリンクを、直接配信または Web ページにコピー&amp;ペーストすることはできません。

Adobe Analytics の [!DNL Adobe Campaign Web] inferface では、標準の 4 つのテンプレートを使用して、様々なユースケースを実装できます。 ただし、主な手順は変わりません。次に詳しく説明します。

1. [ランディングページの作成](create-lp.md#create-landing-page) をクリックし、使用例に従って、目的のテンプレートを選択します。

1. ランディングページのプロパティと設定を定義します。

   ![](assets/lp-uc-properties.png){zoomable=&quot;yes&quot;}

1. お使いの場合に応じて、 **[!UICONTROL 獲得]**, **[!UICONTROL 購読]**, **[!UICONTROL 購読解除]** または **[!UICONTROL ブロックリストに加える]** ページに貼り付けます。

1. ページのコンテンツが表示されます。 ランディングページフォームに対応するパーツを選択します。

   ![](assets/lp-uc-form.png){zoomable=&quot;yes&quot;}

1. 選択したテンプレートに従ってコンテンツを編集します。

   * [獲得](#lp-acquisition)
   * [購読](#lp-subscription)
   * [購読解除](#lp-unsubscription)
   * [ブロックリスト](#lp-denylist)

1. 必要に応じて、残りのコンテンツを変更し、変更を保存して閉じます。

1. を編集します。 **[!UICONTROL 確認]** 必要に応じてページを作成し、 **[!UICONTROL エラー]** および **[!UICONTROL 有効期限]** ページ。 The **[!UICONTROL 確認]** ページは、受信者がフォームを送信すると表示されます。

   ![](assets/lp-uc-confirmation-page.png){zoomable=&quot;yes&quot;}

1. [テスト](create-lp.md#test-landing-page) および [公開](create-lp.md#publish-landing-page) ランディングページを作成します。

1. の作成 [電子メール](../email/create-email.md) ランディングページへのトラフィックを促進する配信

1. メッセージコンテンツに[リンクを挿入](../email/message-tracking.md#insert-links)します。選択 **[!UICONTROL ランディングページ]** として **[!UICONTROL リンクタイプ]** 作成したランディングページを選択します。

   ![](assets/lp-uc-email-link.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >メッセージを送信するには、選択したランディングページがまだ期限切れでないことを確認します。[詳細情報](create-lp.md#create-landing-page)

受信者が電子メールを受け取ったら、ランディングページへのリンクをクリックしてフォームを送信します。

* 確認ページが表示されます。

* ランディングページで定義されたその他のアクションが適用されます。 例えば、ユーザーがお客様のサービスを購読するか、今後お客様からの連絡を受け取らなくなります。

以下に、 [!DNL Adobe Campaign] ランディングページを様々な使用例で使用できます。

## プロファイルの獲得 {#lp-acquisition}

1 つ目のテンプレートでは、Campaign データベースにプロファイルを追加または更新できます。

1. 条件 [ランディングページの作成](create-lp.md#create-landing-page)を選択し、 **[!UICONTROL 獲得]** テンプレート。

1. ランディングページのプロパティで、必ず **[!UICONTROL フォームで参照されるデータを事前入力]** オプションを使用して、プロファイルから既存の情報をプリロードし、重複が作成されないようにします。

1. を選択します。 **[!UICONTROL 獲得]** ページの内容を編集します。

1. 必要に応じて、プロファイルで収集する情報に従って、テキストフィールドを編集します。

1. さらに、顧客がニュースレターサービスを購読するよう促すチェックボックスを追加できます。 [サービスの作成方法を説明します](../audience/manage-services.md)

   ![](assets/lp-uc-acquisition-page.png){zoomable=&quot;yes&quot;}

1. 必要に応じてコンテンツを調整し、変更を保存します。

1. レビューと [公開](create-lp.md#publish-landing-page) ランディングページを作成します。

1. の作成 [電子メール](../email/create-email.md) および [リンクを追加](../email/message-tracking.md#insert-links) をランディングページに追加します。

E メールの受信後、受信者がランディングページへのリンクをクリックしてフォームを送信すると、受信者のプロファイルは Campaign データベースに追加されるか、提供された情報で更新されます。

![](assets/lp-uc-profile-updated.png){zoomable=&quot;yes&quot;}

ニュースレターの受信をオプトインした場合、対応するサービスが購読されます。

![](assets/lp-uc-newsletter-subscriber.png){zoomable=&quot;yes&quot;}

## サービスの購読 {#lp-subscription}

最も一般的なユースケースの 1 つでは、ランディングページを通じて[サービスを購読](../audience/manage-services.md)するよう（ニュースレターやイベントなど）顧客を招待します。以下の手順に従います。

<!--For example, let's say you organize an event next month and you want to launch an event registration campaign. To do this, you're going to send an email including a link to a landing page that will enable your recipients to register for this event. The users who register will be added to the subscription list that you created for this purpose.-->

1. まず、サービスの作成時に簡単に選択できるように、イベントを購読しているユーザー用の確認テンプレートを作成します。 [詳細情報](../audience/manage-services.md#create-confirmation-message)

   ![](assets/lp-uc-confirmation-email.png){zoomable=&quot;yes&quot;}

1. 登録済みユーザーをイベントに保存する購読サービスを作成します。 [サービスの作成方法を説明します](../audience/manage-services.md)

1. ユーザーが購読時に受け取る確認 E メールとして作成したテンプレートを選択します。

   ![](assets/lp-uc-subscription-service.png){zoomable=&quot;yes&quot;}

1. [ランディングページの作成](create-lp.md#create-landing-page) をクリックして、受信者がイベントに登録できるようにします。 を選択します。 **[!UICONTROL 購読]** テンプレート。

1. を選択します。 **[!UICONTROL 購読]** ページの内容を編集します。

1. ページのコンテンツが表示されます。 ランディングページフォームに対応するパーツを選択し、 **[!UICONTROL チェックボックス 1]** 」セクションに入力します。

1. Adobe Analytics の **[!UICONTROL 購読とサービス]** 「 」フィールドで、イベント用に作成したサービスを選択します。 を残します。 **[!UICONTROL オンにした場合は購読]** オプションが有効です。

   ![](assets/lp-uc-subscription-checkbox-1.png){zoomable=&quot;yes&quot;}
<!--
1. You can add an additional checkbox to offer subscription to your newsletter for example.-->

1. 必要に応じてコンテンツを調整し、変更を保存します。

1. レビューと [公開](create-lp.md#publish-landing-page) ランディングページを作成します。

1. の作成 [電子メール](../email/create-email.md) および [リンクを追加](../email/message-tracking.md#insert-links) をクリックして、登録ランディングページにトラフィックを誘導します。

1. イベントの登録が開かれたことを知らせる電子メールをデザインします。

受信者が電子メールを受け取ったら、受信者がランディングページへのリンクをクリックしてフォームを送信すると、確認ページに移動し、購読リストに追加されます。

## 購読解除 {#lp-unsubscription}

顧客がランディングページを使用してサービスを購読解除できるようにします。

1. サービスの作成時に簡単に選択できるように、サービスから購読解除するユーザー用の確認テンプレートを作成したことを確認します。 [詳細情報](../audience/manage-services.md#create-confirmation-message)

1. を [購読サービス](../audience/manage-services.md)「 」で、ユーザーが購読解除時に受け取る確認 E メールとして作成したテンプレートを選択します。

1. [ランディングページの作成](create-lp.md#create-landing-page). を選択します。 **[!UICONTROL 購読解除]** テンプレート。

1. を選択します。 **[!UICONTROL 購読解除]** ページの内容を編集します。

1. ページのコンテンツが表示されます。 ランディングページフォームに対応するパーツを選択します。

1. 次の項目を追加できます： **[!UICONTROL チェックボックス]** セクションで、サービスを選択し、 **[!UICONTROL オンにすると購読解除]** オプション。

   ![](assets/lp-uc-unsubscription-checkbox-1.png){zoomable=&quot;yes&quot;}

1. また、 **[!UICONTROL コールトゥアクション]** 」セクションで、 **[!UICONTROL その他の更新]** オプション。 サービスを選択し、 **[!UICONTROL オプトアウト]** オプション。

   ![](assets/lp-uc-unsubscription-call-to-action.png){zoomable=&quot;yes&quot;}

1. 必要に応じてコンテンツを調整し、変更を保存します。

1. レビューと [公開](create-lp.md#publish-landing-page) ランディングページを作成します。

1. の作成 [電子メール](../email/create-email.md) および [リンクを追加](../email/message-tracking.md#insert-links) をランディングページに追加します。

受信者が E メールを受け取ったら、受信者がランディングページへのリンクをクリックしてフォームを送信すると、購読解除の確認ページに移動し、対応する購読サービスから削除されます。

## ブロックリスト {#lp-denylist}

受信者がブランドからのコミュニケーションを登録解除する機能を提供することは、法的要件で定められています。したがって、常に **配信停止リンク** 受信者に送信されるすべての e メール内。 受信者がこのリンクをクリックすると、オプトアウトを確認するボタンを含むランディングページが表示されます。

次の設定を行うことができます： **[!UICONTROL ブロックリストに加える]** すべての配信のオプトアウトをユーザーに許可するランディングページ。

1. 条件 [ランディングページの作成](create-lp.md#create-landing-page)を選択し、 **[!UICONTROL ブロックリストに加える]** テンプレート。

1. を選択します。 **[!UICONTROL ブロックリストに加える]** ページの内容を編集します。

1. を展開します。 **[!UICONTROL コールトゥアクション]** 」セクションで、 **[!UICONTROL その他の更新]** オプション。

1. 対応するドロップダウンリストで、「 」を選択します。 **[!UICONTROL チャネル（E メール）]** ：受信者が e メール通信のみからオプトアウトできるようにします。 また、 **[!UICONTROL すべてのチャネル別]** すべてのチャネルのすべての通信からすべての通信をオプトする場合。

   ![](assets/lp-uc-denylist.png){zoomable=&quot;yes&quot;}

1. 必要に応じてコンテンツを調整し、変更を保存します。

1. レビューと [公開](create-lp.md#publish-landing-page) ランディングページを作成します。

1. の作成 [電子メール](../email/create-email.md) および [リンクを追加](../email/message-tracking.md#insert-links) をランディングページに追加して、ユーザーが通信の受信をオプトアウトできるようにします。

電子メールを受け取ると、受信者がランディングページへのリンクをクリックしてフォームを送信すると、確認ページに移動ブロックリストに加えるし、提供された情報でプロファイルが更新されます。

対応するプロファイルの選択が更新されたことを確認するには、 **[!UICONTROL プロファイル]** メニューを開き、そのプロファイルを選択します。

例えば、 **[!UICONTROL チャネル（E メール）]** オプションを選択して、 **[!UICONTROL 今後の E メールによる連絡は不要]** オプションがオンになります。

![](assets/lp-uc-denylist-profile.png){zoomable=&quot;yes&quot;}

このプロファイルは、再度購読しない限り、ブランドからの電子メール通信を受け取りません。











