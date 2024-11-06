---
audience: end-user
title: トランザクションメッセージの作成
description: Campaign web ユーザーインターフェイスでトランザクションメッセージを作成する方法について説明します。
source-git-commit: e55b9c875b7700c7ee9d38b8386cc2742ad1f908
workflow-type: ht
source-wordcount: '1189'
ht-degree: 100%

---

# トランザクションメッセージの作成

トランザクションメッセージでは、イベントによってパーソナライズされたメッセージの送信がトリガーされます。
これを有効にするには、イベントタイプごとにメッセージテンプレートを作成する必要があります。これらのテンプレートには、トランザクションメッセージをパーソナライズするのに必要なすべての情報が含まれています。

## トランザクションメッセージテンプレートの作成 {#transactional-template}

Campaign web ユーザーインターフェイスでは、トランザクションメッセージ設定の最初の手順は、テンプレートの作成またはメッセージの直接作成です。これは、[クライアントコンソールでのトランザクションメッセージの設定](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/send/real-time/transactional)とは異なります。

トランザクションメッセージテンプレートを使用すると、プロファイルが受信した配信コンテンツを、最終的なオーディエンスに到達する前にプレビューできます。例えば、管理者はテンプレートを設定し、マーケティングユーザーが使用の準備を整えるようにすることができます。

トランザクションメッセージテンプレートを作成するには、次の手順に従います。

* 「**[!UICONTROL トリガーされたメッセージ]**」セクションで、**[!UICONTROL トランザクションメッセージ]**&#x200B;に移動します。「**[!UICONTROL テンプレート]**」タブでは、トランザクションメッセージの配信テンプレートをすべて確認できます。「**[!UICONTROL トランザクションメッセージテンプレートを作成]**」ボタンをクリックして、テンプレートの作成を開始します。

  ![](assets/transactional-templates.png){zoomable="yes"}

* 表示された新しいページで、テンプレートのチャネルを選択します。この例では、「**[!UICONTROL メール]**」チャネルを選択します。また、別のメッセージテンプレートから作業して、テンプレートリストで選択することもできます。

  ![](assets/transactional-template-channel.png){zoomable="yes"}

  「**[!UICONTROL トランザクションメッセージを作成]**」ボタンをもう一度クリックして、選択したチャネルでのテンプレートの作成を検証します。

* これで、トランザクションメッセージテンプレートの設定にアクセスできます。

  ![](assets/transactional-template-configuration.png){zoomable="yes"}

### トランザクションメッセージのプロパティ {#transactional-properties}

>[!CONTEXTUALHELP]
>id="acw_transacmessages_properties"
>title="トランザクションメッセージのプロパティ"
>abstract="トランザクションメッセージのプロパティを設定するには、このフォームに入力します。"

>[!CONTEXTUALHELP]
>id="acw_transacmessages_email_properties"
>title="トランザクションメッセージングのメールプロパティ"
>abstract="トランザクションメッセージのメールプロパティを設定するには、このフォームに入力します。"

>[!CONTEXTUALHELP]
>id="acw_transacmessages_sms_properties"
>title="トランザクションメッセージの SMS プロパティ"
>abstract="トランザクションメッセージの SMS プロパティを設定するには、このフォームに入力します。"

>[!CONTEXTUALHELP]
>id="acw_transacmessages_push_properties"
>title="トランザクションメッセージのプッシュプロパティ"
>abstract="トランザクションメッセージのプッシュプロパティを設定するには、このフォームに入力します。"

トランザクションメッセージの「**[!UICONTROL プロパティ]**」セクションは、次の設定に役立ちます。

* **[!UICONTROL ラベル]**&#x200B;は、トランザクションメッセージのリストに表示される名前です。調査と今後の使用のために明確にします。
* **[!UICONTROL 内部名]**&#x200B;は、作成された他のメッセージとユーザーのメッセージを区別する一意の名前です。
* **[!UICONTROL フォルダー]**&#x200B;は、トランザクションメッセージテンプレートを作成した場所です。
* **[!UICONTROL 実行フォルダー]**&#x200B;は、実行後にメッセージが保存される場所です。
* **[!UICONTROL 配信コード]**：必要に応じて、レポート用のメッセージを認識するのに役立つコード。
* **[!UICONTROL 説明]**
* **[!UICONTROL 特性]**&#x200B;は、定義済みリストの *deliveryNature* にリストされている配信の特性です。[詳しくは、定義済みリストを参照してください](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/config/configuration/ui-settings#enumerations)。

![](assets/template-properties.png){zoomable="yes"}

### モバイルアプリ {#mobile-app}

>[!CONTEXTUALHELP]
>id="acw_transacmessages_mobileapp"
>title="トランザクションメッセージのモバイルアプリ"
>abstract="このセクションでは、メッセージをプッシュするアプリケーションを選択できます。"

このセクションでは、メッセージをプッシュするアプリケーションを選択できます。

調査アイコンをクリックすると、Adobe Campaign インスタンスにリストされているモバイルアプリケーションにアクセスできます。

![](assets/transactional-mobileapp.png){zoomable="yes"}

### コンテキストサンプル {#context-sample}

>[!CONTEXTUALHELP]
>id="acw_transacmessages_context"
>title="トランザクションメッセージのコンテキスト"
>abstract="コンテキストサンプルを使用すると、プロファイルのパーソナライゼーションで受信したトランザクションメッセージをプレビューするテストイベントを作成できます。"

>[!CONTEXTUALHELP]
>id="acw_transacmessages_addcontext"
>title="トランザクションメッセージのコンテキスト"
>abstract="コンテキストサンプルを使用すると、プロファイルのパーソナライゼーションで受信したトランザクションメッセージをプレビューするテストイベントを作成できます。 "

コンテキストサンプルを使用すると、プロファイルのパーソナライゼーションで受信したトランザクションメッセージをプレビューするテストイベントを作成できます。

この手順はオプションです。コンテキストサンプルなしでテンプレートを使用できますが、パーソナライズされたコンテンツをプレビューできない欠点があります。

パスワードを設定する例では、イベントによってユーザーの名、姓およびパスワードをリセットするパーソナライズしたリンクが送信されます。コンテキストは、次に示すように設定できます。

コンテキストのコンテンツは、必要なパーソナライゼーションによって異なります。

![](assets/transactional-context.png){zoomable="yes"}

### トランザクションメッセージテンプレートのコンテンツ {#transactional-content}

>[!CONTEXTUALHELP]
>id="acw_transacmessages_content"
>title="トランザクションメッセージのコンテンツ"
>abstract="トランザクションメッセージのコンテンツの作成方法について説明します。"

>[!CONTEXTUALHELP]
>id="acw_transacmessages_personalization"
>title="トランザクションメッセージのパーソナライゼーション"
>abstract="トランザクションメッセージのコンテンツのパーソナライズ方法について説明します。"

トランザクションメッセージのコンテンツの操作は、配信のコンテンツ作成に似ています。「**[!UICONTROL E メールデザイナーを開く]**」または「**[!UICONTROL メール本文を編集]**」をクリックし、テンプレートのコンテンツを選択するか、HTML コードをインポートします。

![](assets/template-content.png){zoomable="yes"}

コンテンツにパーソナライゼーションを追加するには、追加するセクションをクリックし、「**[!UICONTROL パーソナライゼーションを追加]**」アイコンを選択します。

![](assets/template-perso.png){zoomable="yes"}

**[!UICONTROL パーソナライゼーションを編集]**ウィンドウにアクセスできます。
トリガーイベントから変数を追加するには、「**[!UICONTROL イベントコンテキスト]**」アイコンをクリックします。テンプレートに対して定義したコンテキスト（[詳しくは、コンテキストを参照](#context-sample)）に移動し、「**[!UICONTROL +]**」ボタンをクリックして必要な変数を挿入できます。

以下の画像で、名のパーソナライゼーションを追加する方法を確認できます。

![](assets/template-firstname.png){zoomable="yes"}

この例では、名、姓の順に追加し、「**[!UICONTROL パスワードをリセット]**」ボタンリンクをパーソナライズします。

![](assets/template-button.png){zoomable="yes"}

### テンプレートのプレビュー

テンプレート作成のこのステージでは、テンプレートのコンテンツをプレビューし、パーソナライゼーションを確認する必要がある場合があります。

これを行うには、[コンテキストサンプル](#context-sample)を入力し、「**[!UICONTROL コンテンツをシミュレート]**」ボタンをクリックします。

![](assets/template-preview.png){zoomable="yes"}

## トランザクションメッセージの作成 {#transactional-message}

トランザクションメッセージは、直接作成することや、トランザクションメッセージテンプレートを使用して作成することができます。[詳しくは、トランザクションメッセージテンプレートの作成方法を参照してください](#transactional-template)。

トランザクションメッセージを作成するには、次の手順に従います。

* 「**[!UICONTROL トリガーされたメッセージ]**」セクションで、**[!UICONTROL トランザクションメッセージ]**&#x200B;に移動します。「**[!UICONTROL 参照]**」タブでは、作成したすべてのトランザクションメッセージを確認できます。「**[!UICONTROL トランザクションメッセージを作成]**」ボタンをクリックして、メッセージの作成を開始します。

  ![](assets/transactional-browse.png){zoomable="yes"}

* 表示された新しいページで、メッセージのチャネルを選択し、操作するテンプレートを選択します。この例では、[ここで作成したテンプレート](#transactional-template)を選択します。

  ![](assets/transactional-channel.png){zoomable="yes"}

  「**[!UICONTROL トランザクションメッセージを作成]**」ボタンをもう一度クリックして、選択したチャネルでのメッセージの作成を検証します。

* これで、トランザクションメッセージの設定にアクセスできます。メッセージは、テンプレートの設定を継承します。このページは、イベントタイプの設定も含まれていることを除いて、トランザクションメッセージテンプレートの設定ページとほとんど同じです。

  ![](assets/transactional-configuration.png){zoomable="yes"}

  テンプレートと同様に次のメッセージの設定を入力します。
   * [トランザクションメッセージのプロパティ](#transactional-properties)
   * [コンテキストサンプル](#context-sample)
   * [メッセージのコンテンツ](#transactional-content)
および次に示すように[イベントタイプを設定](#event-type)します。

* [トランザクションメッセージの検証](validate-transactional.md)後、「**[!UICONTROL レビューして公開]**」ボタンをクリックして、メッセージを作成および公開します。
これで、トリガーによってトランザクションメッセージの送信をプッシュできます。

### イベントタイプについて {#event-type}

>[!CONTEXTUALHELP]
>id="acw_transacmessages_event"
>title="トランザクションメッセージのイベント"
>abstract="イベントタイプの設定により、メッセージがトリガーイベントにリンクされます。"

イベントタイプの設定により、メッセージがトリガーイベントにリンクされます。

Campaign web ユーザーインターフェイスでは、既に作成されているイベントタイプを選択するか、この設定ページでイベントタイプを直接作成することができます。

![](assets/transactional-event-type.png){zoomable="yes"}

>[!CAUTION]
>
>別のトランザクションメッセージで現在使用されているイベントタイプを選択すると、2 つのメッセージがトリガーされます。ベストプラクティスとして、**1 つのイベントタイプを 1 つのトランザクションメッセージにのみリンクすることを強くお勧めします。**

## トランザクションメッセージへのオファーの追加 {#transactional-offers}

トランザクションメッセージにオファーを含めるオプションがあり、メッセージがイベントトリガーされた場合でも、エンドユーザーに関連する提案を提示できます。

この機能は、トランザクションメッセージのコンテンツ編集フェーズ中にアクセスできます。「**[!UICONTROL オファーを設定]**」ボタンをクリックするだけで設定できます。

設定プロセスは、標準配信のオファーを設定する場合と同じです。[詳しくは、メッセージへのオファーの追加方法を参照してください](../msg/offers.md)。

![](assets/transactional-offers.png){zoomable="yes"}
