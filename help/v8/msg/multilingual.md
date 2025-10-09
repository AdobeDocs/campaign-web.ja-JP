---
audience: end-user
title: 多言語配信の設定
description: 多言語配信の設定方法を学ぶ
source-git-commit: 0457e4d0150fe445ae5313377eb299cde40a51b9
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 18%

---

# 多言語配信の設定 {#multilingual-delivery}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_multilingual"
>title="言語を追加"
>abstract="このタブには、配信を送信する言語のリストがあります。「言語を追加」ボタンをクリックするか、このタブから別の言語を複製して、さらに言語を追加できます。"

Campaign web UI では、配信を多言語として設定し、プロファイルの優先言語に基づいてメッセージを送信できます。 環境設定を定義していない場合、メッセージはデフォルトの言語で送信されます。

多言語配信では、言語管理はバリアントに基づいています。各バリアントは 1 つの言語を表します。 配信の作成時には、メッセージに必要な言語の数に一致する複数の言語のバリアントを追加できます。 また、これらのバリアントを追加した後、いつでもデフォルト言語を変更できます。

現在、多言語機能は、メール、プッシュ通知、トランザクションメッセージで使用できます。

>[!AVAILABILITY]
>
>多言語プッシュ通知、トランザクションメッセージ、SMS は、一連の組織（使用制限あり）でのみ使用でき、今後のリリースでグローバルにロールアウトされます。 サーバーは 8.8.2 以降にアップグレードする必要があります。

多言語配信を設定するには、次の主な手順に従います。

1. 言語バリアントを追加します [&#x200B; 詳細を表示 &#x200B;](#add-variant)
1. 各バリアントのコンテンツを定義します [&#x200B; 詳細を表示 &#x200B;](#define-content)
1. 言語バリアントの管理 [&#x200B; 詳細を表示 &#x200B;](#manage-variant)

## 言語バリアントの追加{#add-variant}

言語バリアントを作成するには、次の手順に従います。

1. 配信ダッシュボードで、鉛筆アイコンをクリックして配信コンテンツ編集画面にアクセスし、「**[!UICONTROL 言語を追加]**」をクリックします。

   >[!IMPORTANT]
   >
   >「**[!UICONTROL 言語を追加]**」ボタンは、ターゲットディメンションに **言語** スキーマが含まれている場合にのみ使用できます。 スキーマとターゲットディメンションについて詳しくは、[&#x200B; 詳細ドキュメント &#x200B;](../audience/targeting-dimensions.md) を参照してください。

   ![](assets/edit-content_2.png){zoomable="yes"}

1. **言語を追加** ドロップダウンから、追加する言語を選択し、確認します。

   最初に追加した言語が自動的にデフォルトに設定され、既存のコンテンツがデフォルトバージョンになります。 言語を追加すると、その内容は最初デフォルト言語からコピーされます。

   ![](assets/edit-content_3.png){zoomable="yes"}

   >[!NOTE]
   >
   >このリストから使用できる言語は、**Language** 属性で定義された値（system、user、dbenum などの値）によって異なります。 列挙の管理について詳しくは、この [&#x200B; 節 &#x200B;](../administration/enumerations.md) を参照してください。

1. 他の言語を追加するには、この操作を繰り返します。 **[!UICONTROL 言語]** パネルの左側には、選択した言語のリスト、言語数およびデフォルト言語が表示されます。

   例えば、英語、フランス語、スウェーデン語を選択した場合、これら 3 つの言語は以下のように表示されます。

   ![](assets/edit-content_9.png){zoomable="yes"}

   言語のバリアントの管理方法については、この [&#x200B; 節 &#x200B;](#manage-variant) を参照してください。

## 各バリアントのコンテンツを定義します{#define-content}

言語を設定したら、言語ごとに配信のコンテンツを定義します。

1. 配信コンテンツ編集画面で、左側の **[!UICONTROL 言語]** パネルから言語を選択します。

   ![](assets/edit-content_11.png){zoomable="yes"}

1. この言語用にメッセージのコンテンツを定義します。 詳しくは、[この節](../msg/create-deliveries.md)を参照してください。

1. 各言語に対してこの操作を繰り返します。

<!--
>[!BEGINTABS]

>[!TAB Email delivery]

1. From the delivery content edition screen, choose a language and click the **[!UICONTROL Edit email body]** button. You can also hover over the email preview and select **[!UICONTROL Open email designer]**.

    ![](assets/edit-content_11.png){zoomable="yes"}

1. Define the content of your email for this language. [Read more](../email/get-started-email-designer.md#start-authoring)

1. Repeat this operation for each language.

>[!TAB SMS delivery]

1. From the delivery content edition screen, choose a language.

1. Edit the content of the SMS message for this language. [Read more](../sms/create-sms.md)

    ![](assets/edit-content_11-sms.png){zoomable="yes"}

1. Repeat this operation for each language.

>[!ENDTABS]

-->

配信をプレビューするには、「**[!UICONTROL コンテンツをシミュレート]**」ボタンをクリックし、プロファイルを選択します。 プロファイルごとに適切なコンテンツが表示されていることを確認します。

![](assets/edit-content_5.png){zoomable="yes"}

## 言語バリアントの管理{#manage-variant}

左側のパネルには、すべての言語バリアント情報が表示されます。 すべての言語を削除するには、「展開」ボタンをクリックし、「**[!UICONTROL すべてのバリアントを削除]**」をクリックします。

![](assets/edit-content_13.png){zoomable="yes"}

言語のバリアントのリストで、次のアクションを実行できます。

* **編集**：関連コンテンツを保持したまま、言語を変更します。
* **デフォルトとして設定**：言語をデフォルトとして設定します。 プロファイルに言語が定義されていない場合、メッセージはデフォルトの言語で送信されます。
* **複製**：この言語用に定義したコンテンツを複製し、別のバリアントを選択します。
* **削除**：バリアントと、関連するコンテンツを削除します。

![](assets/edit-content_13-sms.png){zoomable="yes"}

