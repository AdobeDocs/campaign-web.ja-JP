---
title: プロファイルの監視と管理
description: Campaign web でプロファイルを監視および管理する方法について説明します。
badge: label="限定提供（LA）"
exl-id: 0680b726-8f2f-45bf-8aa0-c1d4aa1c2990
source-git-commit: 72899742daf04a0da6e2fb3d802b7841753b8c6c
workflow-type: tm+mt
source-wordcount: '943'
ht-degree: 97%

---

# プロファイルの監視と管理 {#profiles}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="プロファイルの包括的なビュー"
>abstract="新しいプロファイルを作成し、強力なレポートとツールを通じて監視します。プロファイルの属性、インタラクションおよびログにアクセスします。フィルタリングオプションを使用して、プロファイルリストを参照し、プロファイルを編集および更新します。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html?lang=ja" text="リリースノートを参照してください"

<!--TO REMOVE BELOW-->
>[!CONTEXTUALHELP]
>id="acw_homepage_rn4"
>title="プロファイルの包括的なビュー"
>abstract="新しいプロファイルを作成し、強力なレポートとツールを通じて監視します。プロファイルの属性、インタラクションおよびログにアクセスします。フィルタリングオプションを使用して、プロファイルリストを参照し、プロファイルを編集および更新します。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html?lang=ja" text="リリースノートを参照してください"

<!--TO REMOVE ABOVE-->


>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="プロファイル"
>abstract="プロファイルとは、Adobe Campaignから送信されるメッセージの受信をターゲットとしている個人です。 このリストから、権限に基づいてプロファイルの詳細を表示できます。フィルターオプションを使用して、このリストを参照します。プロファイルの属性の一部を編集および更新できます。"

## プロファイルの基本を学ぶ {#gs}

Adobe Campaign web のプロファイルは、データベースに保存される個人で、配信の[オーディエンスを作成](create-audience.md)とコンテンツの[パーソナライゼーションデータを追加](../personalization/personalize.md)するための重要なコンポーネントとして機能します。

**[!UICONTROL テストプロファイル]**&#x200B;など、他のタイプのプロファイルは、データベースに保存されます。これらは、最終的なオーディエンスに送信する前に配信をテストするように設計されています。[詳細情報](test-profiles.md)

プロファイルは、Adobe Campaign クライアントコンソールからのみ作成できます - [詳細情報](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/create-profiles.html?lang=ja){target="_blank"}。ただし、Adobe Campaign web では、左側のナビゲーションパネルの&#x200B;**[!UICONTROL 顧客管理]**／**プロファイル**&#x200B;エントリからアクセスして編集できます。

>[!NOTE]
>
>権限によっては、データベースに保存されているプロファイルの完全なリストへのアクセス権がない場合があります。[詳しくは、権限を参照してください](../get-started/permissions.md)。

* 検索フィールドを使用するか、「**フィルターを表示**」ボタンから使用できるフィルターを使用して、**[!UICONTROL プロファイル]**&#x200B;リストをフィルタリングできます。ドロップダウンリストを使用して結果を特定の[フォルダー](../get-started/permissions.md#folders)に制限したり、[クエリモデラー](../query/query-modeler-overview.md)を使用してルールを追加したりできます。

  ![](assets/profiles-list-filters.png)

* プロファイルを削除するには、**[!UICONTROL その他のアクション]**&#x200B;メニューから対応するオプションを選択します。

* プロファイルを編集するには、リストから目的の項目をクリックします。[詳細情報](#access)

また、**[!UICONTROL プロファイルとターゲット]**／**[!UICONTROL 受信者]**&#x200B;ノードから、**[!UICONTROL エクスプローラー]**&#x200B;ビューを通じてプロファイルにアクセスすることもできます。

そこから、フォルダーまたはサブフォルダーを参照、作成、管理したり、関連する権限を確認したりできます。[フォルダーの作成方法を学ぶ](../get-started/permissions.md#folders)

![](assets/profiles-explorer-folder.png)

また、**[!UICONTROL エクスプローラー]**&#x200B;ビューから、プロファイルのフィルタリング、削除、[編集](#access)を行うこともできます。

## プロファイルの属性へのアクセスと編集 {#access}

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_details"
>title="基本の詳細"
>abstract="この節では、プロファイルの基本の詳細に関するインサイトについて説明します。情報を変更するには、各フィールド内で直接変更を行い、画面の右上隅にある「**保存**」ボタンをクリックします。"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_contactinformation"
>title="連絡先情報"
>abstract="この節では、プロファイルの連絡先情報に関するインサイトについて説明します。情報を変更するには、各フィールド内で直接変更を行い、画面の右上隅にある「**保存**」ボタンをクリックします。"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_address"
>title="住所"
>abstract="この節では、プロファイルの郵送先住所と住所の品質に関するインサイトについて説明します。情報を変更するには、各フィールド内で直接変更を行い、画面の右上隅にある「**保存**」ボタンをクリックします。"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_account"
>title="アカウントの詳細"
>abstract="この節では、プロファイルのアカウント詳細に関するインサイトについて説明します。情報を変更するには、各フィールド内で直接変更を行い、画面の右上隅にある「**保存**」ボタンをクリックします。"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_nolongercontact"
>title="今後の連絡が不要な受信者"
>abstract="この節では、プロファイルの連絡先環境設定に関するインサイトについて説明します。情報を変更するには、各フィールド内で直接変更を行い、画面の右上隅にある「**保存**」ボタンをクリックします。"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_customfields"
>title="カスタムフィールド"
>abstract="カスタムフィールドは、インスタンス用に設定された、ニーズに合わせて調整された特定の属性です。情報を変更するには、各フィールド内で直接変更を行い、画面の右上隅にある「**保存**」ボタンをクリックします。"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_othersfields"
>title="その他"
>abstract="この節では、追加の組み込み属性について説明します。情報を変更するには、各フィールド内で直接変更を行い、画面の右上隅にある「**保存**」ボタンをクリックします。"

>[!CONTEXTUALHELP]
>id="acw_recipients_subscription_list"
>title="受信者の購読リスト"
>abstract="このタブには、プロファイルがサブスクライブしているすべてのサービスがリストされます。"

プロファイルの詳細にアクセスして編集するには、次の手順に従います。

1. **[!UICONTROL 顧客管理]**／**[!UICONTROL プロファイル]**&#x200B;を参照し、**[!UICONTROL プロファイル]**&#x200B;リストから目的の項目をクリックします。

   ![](assets/profiles-list-select.png)

1. プロファイルの詳細情報が表示されます。

   「**[!UICONTROL 詳細]**」タブを使用すると、プロファイルの組み込み属性とカスタム属性を参照できます。属性を編集するには、必要なフィールドに変更を加え、「**[!UICONTROL 保存]**」ボタンをクリックします。

   ![](assets/profile-details.png)

   1. デフォルトでは、プロファイルは&#x200B;**[!UICONTROL 受信者]**&#x200B;フォルダーに保存されます。目的の場所を参照して変更できます。[詳しくは、フォルダーの操作方法を参照してください](../get-started/permissions.md#folders)

      ![](assets/profile-folder.png)

   1. 「**[!UICONTROL 連絡先情報]**」セクションでは、メールアドレスやその他の関連データを更新できます。メールアドレスは、プロファイルラベルの後に括弧で囲まれて表示されます。

      ![](assets/profile-address.png)

   1. 「**[!UICONTROL 今後の連絡は不要]**」オプションをオンにし、必要に応じて更新します。これらのオプションのいずれかを選択すると、プロファイルはブロックリストに登録されます。例えば、受信者がニュースレターの購読解除リンクをクリックした場合、この情報は連絡先データに追加されます。このような受信者は、選択したチャネルのターゲットに設定されなくなりました。[詳細情報](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html?lang=ja){target="_blank"}

      ![](assets/profile-no-longer-contact.png)

   1. **[!UICONTROL カスタムフィールド]**&#x200B;がある場合は、必要に応じて値を更新できます。カスタムフィールドは、Adobe Campaign コンソールを通じて&#x200B;**[!UICONTROL プロファイル]**&#x200B;スキーマに追加される追加属性です。[詳細情報](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema.html?lang=ja){target="_blank"}

      ![](assets/profile-custom-fields.png)

1. 「**[!UICONTROL サブスクリプション]**」タブをクリックして、プロファイルがサブスクライブしているサービスに関する情報にアクセスします。[詳しくは、サブスクリプションサービスを参照してください](manage-services.md)

   ![](assets/profile-subscriptions.png)

1. 画面の右上隅にある「**[!UICONTROL ログ]**」ボタンをクリックすると、送信ログ、除外ログ、トラッキングログを通じてプロファイルのインタラクションの履歴が表示されます。[詳しくは、配信ログを参照してください](../monitor/delivery-logs.md)

   また、「**[!UICONTROL 提案]**」タブで、プロファイルに示されたオファーを確認することもできます。[詳しくは、オファーを参照してください](../msg/offers.md)

   ![](assets/profile-logs.png)
