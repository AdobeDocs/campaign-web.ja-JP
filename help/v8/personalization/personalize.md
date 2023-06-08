---
title: Campaign でのコンテンツのパーソナライズ
description: Adobe Campaign web UI でのコンテンツのパーソナライズ方法について説明します
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Positive"
source-git-commit: b8b1cb62c11b66eaade5937fa798d58a9c376127
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 36%

---


# コンテンツのパーソナライズ{#add-personalization}

パーソナライゼーションは、式エディターを使用して、任意の配信に追加できます。

パーソナライゼーションタグは常に次の構文を使用します。 `<%=table.field%>`例えば、受信者テーブルに格納されている受信者の名前を挿入する場合、パーソナライゼーションタグは &lt;%= recipient.lastName %> 構文を使用します。

配信の準備が完了すると、これらのタグはAdobe Campaignで自動的に解釈され、特定の受信者のフィールドの値で置き換えられます。 その後、実際に置き換えられたコンテンツをシミュレートする際に、その内容を確認できます。

配信にパーソナライゼーションタグを追加するには、件名行や SMS 本文など、テキストタイプの編集フィールドからアクセス可能な、パーソナライゼーションダイアログを開くアイコンをクリックします。

![](assets/perso-access.png)

式エディターが表示されます。 パーソナライゼーションフィールドは、画面の左側にある 3 つのメニューに整理されます。 これらのメニューを使用すると、Adobe Campaignデータベースで使用可能なすべてのフィールドにアクセスできます。

| メニュー | 説明 |
|-----|------------|
| ![](assets/do-not-localize/perso-recipients-menu.png) | この **[!UICONTROL 受信者]** メニューには、受信者の名前、年齢、住所など、受信者テーブルに定義されたすべてのフィールドが一覧表示されます。 |
| ![](assets/do-not-localize/perso-message-menu.png) | この **[!UICONTROL メッセージ]** メニューには、配信ログに関連するすべてのフィールドが一覧表示されます。つまり、特定の受信者との最後のイベントの日付など、すべてのチャネルをまたいで受信者やデバイスに送信されたすべてのメッセージが一覧表示されます |
| ![](assets/do-not-localize/perso-delivery-menu.png) | この **[!UICONTROL 配信]** メニューには、配信チャネル、ラベルなど、配信の実行に必要なパラメーターに関連するすべてのフィールドがリストされます。 |

>[!NOTE]
>
>デフォルトでは、リストには選択したテーブル内のすべてのフィールド（受信者、/メッセージ/配信）が表示されます。 選択したテーブルにリンクするテーブルのフィールドを含める場合は、 **[!UICONTROL 詳細属性の表示]** オプションがリストの下に表示されます。

パーソナライゼーションフィールドを追加するには、コンテンツ内の目的の場所にカーソルを置き、「+」ボタンをクリックして挿入します。

![](assets/perso-insert-field.png)

## メールコンテンツのパーソナライズ {#personalize-emails}

メールコンテンツをパーソナライズするには、電子メールデザイナーでメッセージを開き、次の操作を実行します。

1. テキストブロック内をクリックします。
1. コンテキストツールバーで、「**[!UICONTROL パーソナライゼーションを追加]**」を選択します。

   ![](assets/perso-add-to-content.png)

1. パーソナライゼーションエディターに受信者の名前を挿入し、確認します。

   ![](assets/perso-add-name.png)

   パーソナライゼーション属性がメールコンテンツに追加されます。

   コンテンツをシミュレートして、レンダリングを確認できます。[詳細情報](../preview-test/preview-content.md)

   ![](assets/perso-rendering.png)

1. メールにコンテンツブロックを追加するには、同じ手順を適用し、最後のアイコンからコンテンツブロックを選択します。

   ![](assets/perso-insert-block.png)

1. 挿入すると、コンテンツブロックがメールコンテンツに追加されます。配信準備段階で、パーソナライゼーションが生成されると、受信者プロファイルに適合するように自動的に調整されます。

   ![](assets/perso-content-block-in-email.png)


## オファーのパーソナライズ {#personalize-offers}

テキストタイプのコンテンツをオファーの表示域に追加する際に、パーソナライゼーションエディターにアクセスすることもできます。詳しくは、[こちら](../content/offers.md)を参照してください。

