---
title: Campaign でのコンテンツのパーソナライズ
description: Adobe Campaign web UI でのコンテンツのパーソナライズ方法について説明します
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Positive"
source-git-commit: 218f433eb72a0ed928732c96ebee64294daee852
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 79%

---


# コンテンツのパーソナライズ{#add-personalization}

## メッセージの件名行をパーソナライズ {#personalize-subject-line}

メッセージの「**[!UICONTROL 件名]**」フィールドにパーソナライゼーションを追加するには、次の手順に従います。

1. 配信を開き、 **[!UICONTROL コンテンツを編集]**.
1. 次をクリック： **[!UICONTROL パーソナライゼーションダイアログを開く]** アイコン **[!UICONTROL 件名]** 電子メールのフィールド、または **[!UICONTROL タイトル]** プッシュ/SMS 配信用のフィールド。

   ![](assets/perso-subject.png){width="600"}

1. 件名行またはタイトルを入力し、追加するパーソナライゼーション属性を選択します。

1. 「**[!UICONTROL 確認]**」をクリックして確定します。パーソナライゼーション属性がコンテンツに追加されます。

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

## メール内のリンクのパーソナライズ {#personalize-links}

**リンク**&#x200B;をパーソナライズするには：

1. テキストブロックまたは画像を選択します。
1. コンテキストツールバーで、「**リンクを挿入**」を選択します。

   ![](assets/perso-link.png)

1. リンクラベルを入力し、「**リンクを挿入**」ボタンを使用して、リンクをパーソナライズします。

   ![](assets/perso-link-insert-icon.png)

1. パーソナライゼーションエディターを使用して、リンクを定義およびパーソナライズし、確定します。

   ![](assets/perso-link-edit.png)


## オファーのパーソナライズ {#personalize-offers}

テキストタイプのコンテンツをオファーの表示域に追加する際に、パーソナライゼーションエディターにアクセスすることもできます。詳しくは、[こちら](../content/offers.md)を参照してください。

