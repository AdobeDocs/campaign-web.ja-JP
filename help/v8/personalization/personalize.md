---
title: Campaign でのコンテンツのパーソナライズ
description: Adobe Campaign Web UI でコンテンツをパーソナライズする方法を説明します
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
source-git-commit: 2d23b04b81ab625de0936fdf058f6ac8bd1017c3
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 7%

---

# コンテンツのパーソナライズ{#add-personalization}

![](../assets/do-not-localize/badge.png)

メッセージの内容は、次の方法でパーソナライズできます。

* 動的な挿入 **パーソナライゼーションフィールド**

   パーソナライゼーションフィールドは、メッセージの第 1 レベルのパーソナライゼーションに使用されます。 パーソナライゼーションエディターから、データベースで使用可能な任意のフィールドを選択できます。 配信の場合は、受信者、メッセージまたは配信に関連する任意のフィールドを選択できます。 これらのパーソナライゼーション属性は、メッセージの件名行または本文に挿入できます。

   ![](assets/perso-subject-line.png)

   上記の構文は、受信者の市区町村をコンテンツに挿入します。&lt;%= recipient.location.city %> です。

* 事前定義済みの挿入 **コンテンツブロック**

   Campaign には、配信に挿入できる特定のレンダリングを含む、一連のパーソナライゼーションブロックが付属しています。 例えば、メッセージのミラーページにロゴ、挨拶メッセージまたはリンクを追加できます。 コンテンツブロックは、パーソナライゼーションエディターの専用のエントリから使用できます。

   ![](assets/perso-content-blocks.png)
<!--
* Create **conditional content**

    Configure conditional content to add dynamic personalization based on the recipient’s profile for example. Text blocks and/or images are inserted when a particular condition is true.
-->

## E メールの件名行をパーソナライズ {#personalize-subject-line}

パーソナライゼーションを **[!UICONTROL 件名]** メッセージの「 」フィールドで、次の手順に従います。

1. 次をクリック： **パーソナライゼーションダイアログを開く** アイコン **件名** フィールドに入力します。
1. 件名行のコンテンツを入力し、追加するパーソナライゼーション属性を選択します。
1. 「確認」をクリックして確定します。 パーソナライゼーション属性が件名行に追加されます。

![](assets/perso-subject.png)

## E メールコンテンツをパーソナライズ {#personalize-emails}

E メールの内容をパーソナライズするには、E メールデザイナーでメッセージを開き、次の操作を実行します。

1. テキストブロック内をクリックします。
1. コンテキストツールバーで、「 」を選択します。 **パーソナライゼーションを追加**.

   ![](assets/perso-add-to-content.png)

1. パーソナライゼーションエディターで受信者の名前を挿入し、確定します。

   ![](assets/perso-add-name.png)

   パーソナライゼーション属性が E メールコンテンツに追加されます。

   コンテンツをシミュレートして、レンダリングを確認できます。 [詳細情報](../preview-test/preview-content.md)

   ![](assets/perso-rendering.png)


## メール内のリンクをパーソナライズ {#personalize-links}

をパーソナライズするには **リンク**:

1. テキストブロックまたは画像を選択します。
1. コンテキストツールバーで、「 」を選択します。 **パーソナライゼーションを追加**.

   ![](assets/perso-link.png)

1. パーソナライゼーションエディターを使用して、リンクを定義およびパーソナライズします。

## オファーをパーソナライズする {#personalize-offers}

テキストタイプのコンテンツをオファーの表示域に追加する際に、パーソナライゼーションエディターにアクセスすることもできます。
