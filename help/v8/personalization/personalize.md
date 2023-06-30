---
title: Campaign でのコンテンツのパーソナライズ
description: Adobe Campaign web UI でのコンテンツのパーソナライズ方法について説明します
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: ht
source-wordcount: '431'
ht-degree: 100%

---


# コンテンツのパーソナライズ {#add-personalization}

式エディターを使用して、任意の配信をパーソナライズできます。式エディターには、「**[!UICONTROL パーソナライゼーションダイアログを開く]**」アイコンのある各フィールド（件名行、メールリンク、テキスト/ボタンのコンテンツコンポーネントなど）からアクセスできます。[式エディターにアクセスする方法を学ぶ](gs-personalization.md/#access)

## パーソナライゼーション構文 {#syntax}

パーソナライゼーションタグは、次の特定の構文 `<%= table.field %>` に従います。例えば、受信者テーブルから受信者の姓を挿入するには、`<%= recipient.lastName %>` 構文を使用します。

配信準備プロセス中に、Adobe Campaign はこれらのタグを自動的に解釈し、各受信者の対応するフィールド値に置き換えます。コンテンツをシミュレートすると、実際の置き換えを確認できます。

スタンドアロンのメール配信用に外部ファイルから連絡先をアップロードする場合、入力ファイル内のすべてのフィールドをパーソナライズに使用できます。構文は次のようになります。`<%= dataSource.field %>`

## パーソナライゼーションタグを追加 {#add}

配信にパーソナライゼーションタグを追加するには、次の手順に従います。

1. 式エディターを開くには、テキストタイプの編集フィールド（件名行や SMS 本文など）からアクセスできる「**[!UICONTROL パーソナライゼーションダイアログを開く]**」アイコンを使用します。[式エディターにアクセスする方法を学ぶ](gs-personalization.md/#access)

   ![](assets/perso-access.png){width="800" align="center"}

1. 式エディターが開きます。画面の左側にあるいくつかのメニューに、Adobe Campaign データベースで使用可能なパーソナライゼーションフィールドが整理されています。

   ![](assets/perso-insert-field.png){width="800" align="center"}

   | メニュー | 説明 |
   |-----|------------|
   | ![](assets/do-not-localize/perso-subscribers-menu.png) | **[!UICONTROL サブスクライバーのアプリケーション]**&#x200B;メニューには、使用するターミナルやオペレーティングシステムなど、アプリケーションのサブスクライバーに関連するフィールドが一覧表示されます。*このメニューは、プッシュ通知でのみ使用できます* |
   | ![](assets/do-not-localize/perso-recipients-menu.png) | **[!UICONTROL 受信者]**&#x200B;メニューには、受信者の名前、年齢、アドレスなど、受信者テーブルで定義されたフィールドが一覧表示されます。スタンドアロンのメール配信用に[外部ファイルからの連絡先をアップロード](../audience/file-audience.md)すると、このメニューに入力ファイルで使用できるすべてのフィールドが一覧表示されます。 |
   | ![](assets/do-not-localize/perso-message-menu.png) | **[!UICONTROL メッセージ]**&#x200B;メニューには、配信ログに関連するフィールドが一覧表示されます。特定の受信者との最後のイベントの日付など、すべてのチャネルにわたって受信者またはデバイスに送信されたすべてのメッセージが含まれます |
   | ![](assets/do-not-localize/perso-delivery-menu.png) | **[!UICONTROL 配信]**&#x200B;メニューには、配信チャネルやラベルなど、配信の実行に必要なパラメーターに関連するフィールドが一覧表示されます。 |

   >[!NOTE]
   >
   >デフォルトでは、各メニューには、選択したテーブル内のすべてのフィールド（受信者、メッセージ、配信）が一覧表示されます。選択したテーブルにリンクするテーブルのフィールドを含める場合は、リストの下にある「**[!UICONTROL 詳細属性を表示]**」オプションを有効にします。

1. パーソナライゼーションフィールドを追加するには、コンテンツ内の目的の場所にカーソルを置き、「`+`」ボタンをクリックして挿入します。

1. コンテンツの準備が整ったら、コンテンツを保存し、シミュレーションを実行して、パーソナライゼーションのレンダリングをテストできます。次の例は、受信者の名を使用した SMS メッセージのパーソナライズを示しています。

   ![](assets/perso-preview1.png){width="800" align="center"}

   ![](assets/perso-preview2.png){width="800" align="center"}
