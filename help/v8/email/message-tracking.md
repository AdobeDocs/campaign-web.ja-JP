---
audience: end-user
title: メッセージの追跡
description: リンクを追加し、送信済みメッセージを追跡する方法を学ぶ
exl-id: ea0d4214-5f14-470c-8791-e8b179ca3a42
source-git-commit: a95a70aa56061106a920584a3501cd4b1434ec8a
workflow-type: tm+mt
source-wordcount: '535'
ht-degree: 100%

---

# リンクの追加とメッセージのトラッキング {#tracking}

E メールデザイナーを使用してコンテンツにリンクを追加し、受信者の行動を監視するために送信されたメッセージを追跡します。

## リンクを挿入 {#insert-links}

メッセージをデザインする際に、コンテンツにリンクを追加できます。

>[!NOTE]
>
>トラッキングが有効になっている場合、メッセージコンテンツに含まれるすべてのリンクが追跡されます。

メールコンテンツにリンクを挿入するには、次の手順に従います。

1. 要素を選択し、コンテキストツールバーから「**[!UICONTROL リンクを挿入]**」をクリックします。

1. 作成するリンクのタイプを選択します。

   ![](assets/message-tracking-insert-link.png){zoomable="yes"}

   * **[!UICONTROL 外部リンク]**：外部 URL へのリンクを挿入します。

     >[!AVAILABILITY]
     >
     >次の機能（**[!UICONTROL ランディングページ]**、**[!UICONTROL 購読リンク]**&#x200B;および&#x200B;**[!UICONTROL 購読解除リンク]**）は限定提供（LA）中です。これらは、**Adobe Campaign Standard から Adobe Campaign v8** に移行する顧客に限定されており、他の環境にデプロイすることはできません。

   * **[!UICONTROL ランディングページ]**：ランディングページへのリンクを挿入します。動的ランディングページを選択した場合（**[!UICONTROL URL からのサービス]**&#x200B;オプションが選択されている場合）、リストから任意のサービスを選択できます。[詳細情報](../landing-pages/create-lp.md#define-actions-on-form-submission)

     ![](assets/email-link-to-landing-page.png){zoomable="yes"}

   * **[!UICONTROL 購読リンク]**：購読サービスへのリンクを挿入します。ユーザーがリンクをクリックすると、選択したサービスで参照される購読ランディングページに移動します。[詳細情報](../audience/manage-services.md#create-service)

     ![](assets/service-create-default-lp-link.png){zoomable="yes"}

   * **[!UICONTROL 購読解除リンク]**：購読解除サービスへのリンクを挿入します。サブスクライバーがリンクをクリックすると、選択したサービスで参照される購読解除ランディングページに移動します。[詳細情報](../audience/manage-services.md#create-service)

   <!--* **[!UICONTROL Mirror page]**: Add a link to display the email content in a web browser. [Learn more]-->

1. 対応するフィールドに目的の URL を入力するか、ランディングページまたはサービスを選択して、リンクの設定とスタイルを定義します。

1. **[!UICONTROL ラベル]**&#x200B;と&#x200B;**[!UICONTROL リンク]**&#x200B;を追加します。

1. 変更内容を保存します。

1. リンクを作成したら、「**[!UICONTROL 設定]**」タブから変更できます。

   * リンクを編集して、**[!UICONTROL ターゲット]**&#x200B;を変更できます。
   * リンクに下線を引くかどうかは、対応するオプションをオンにすることで選択できます。

   ![](assets/message-tracking-link-settings.png){zoomable="yes"}

>[!NOTE]
>
>マーケティングタイプのメールメッセージには、オプトアウトリンクを含める必要があります。これはトランザクションメッセージには必要ありません。メッセージカテゴリ（**[!UICONTROL マーケティング]**&#x200B;または&#x200B;**[!UICONTROL トランザクション]**）はチャネルサーフェスレベルでメッセージの作成時に定義されます。

すべてのメールメッセージに、ミラーページへの特定のリンクを追加する必要があります。ミラーページについて詳しくは、[この節](mirror-page.md)を参照してください。

## トラッキングの管理 {#manage-tracking}

[E メールデザイナー](create-email-content.md)を使用すると、各リンクのトラッキングタイプを編集するなど、追跡する URL を管理できます。

1. 左側のパネルで 「**[!UICONTROL リンク]**」アイコンをクリックすると、追跡するコンテンツのすべての URL のリストが表示されます。

   このリストを使用すると、一元表示が可能になり、メールコンテンツ内の各 URL を特定できます。

1. リンクを編集するには、対応する鉛筆アイコンをクリックします。

   ![](assets/message-tracking-edit-links.png){zoomable="yes"}

1. 必要に応じて、**[!UICONTROL トラッキングタイプ]**&#x200B;を変更できます。

   ![](assets/message-tracking-edit-a-link.png){zoomable="yes"}

   追跡する URL ごとに、トラッキングモードを次のいずれかの値に設定できます。

   * **[!UICONTROL トラッキング対象]**：この URL のトラッキングをアクティブ化します。
   * **[!UICONTROL オプトアウト]**：この URL をオプトアウトまたは購読解除 URL とみなします。
   * **[!UICONTROL ミラーページ]**：この URL をミラーページの URL とみなします。
   * **[!UICONTROL なし]**：この URL のトラッキングをアクティブ化しません。<!--This information is saved: if the URL appears again in a future message, its tracking is automatically deactivated.-->

1. 「**[!UICONTROL カテゴリ]**」をリンクに追加して、トラッキングされたリンクをグループ化し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/message-tracking-edit-a-link_2.png){zoomable="yes"}

1. 配信を送信したら、配信レポートにアクセスします。 **[!UICONTROL トラッキング]**&#x200B;メニューの下の **[!UICONTROL URL とクリックストリーム]**&#x200B;レポートには、配信で最も訪問回数の多い URL が表示されます。 [詳細情報](../reporting/gs-reports.md)
