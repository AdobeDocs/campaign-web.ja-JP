---
title: プロファイルの基本を学ぶ
description: Campaign web でプロファイルを監視および管理する方法について説明します。
badge: label="限定提供（LA）"
source-git-commit: 22b183a739dd92d7c4245fb4694034a247511d75
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 68%

---

# プロファイルの基本を学ぶ {#profiles}

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

## プロファイルとは {#what}

Adobe Campaign web のプロファイルは、データベースに保存される個人で、配信の[オーディエンスを作成](create-audience.md)とコンテンツの[パーソナライゼーションデータを追加](../personalization/personalize.md)するための重要なコンポーネントとして機能します。

Adobe Campaignでは、インターフェイスから直接プロファイルを作成および監視できます。 ここから、プロファイルを作成し、プロファイルの詳細なビューにアクセスして、編集できます。

**[!UICONTROL テストプロファイル]**&#x200B;など、他のタイプのプロファイルは、データベースに保存されます。これらは、最終的なオーディエンスに送信する前に配信をテストするように設計されています。[テストプロファイルの操作方法を説明します。](test-profiles.md)

## プロファイルのリストへのアクセス {#access}

プロファイルは、Web ページ上の **[!UICONTROL 顧客管理]** > **プロファイル** エントリをクリックします。

また、 **[!UICONTROL エクスプローラ]** ビュー、 **[!UICONTROL プロファイルとターゲット]** > **[!UICONTROL 受信者]** ノード。 そこから、フォルダーまたはサブフォルダーを参照、作成、管理したり、関連する権限を確認したりできます。[フォルダーの作成方法を学ぶ](../get-started/permissions.md#folders)

>[!NOTE]
>
>権限によっては、データベースに保存されているプロファイルの完全なリストへのアクセス権がない場合があります。[詳しくは、権限を参照してください](../get-started/permissions.md)。

検索フィールドを使用するか、「**フィルターを表示**」ボタンから使用できるフィルターを使用して、**[!UICONTROL プロファイル]**&#x200B;リストをフィルタリングできます。ドロップダウンリストを使用して結果を特定の[フォルダー](../get-started/permissions.md#folders)に制限したり、[クエリモデラー](../query/query-modeler-overview.md)を使用してルールを追加したりできます。

![](assets/profiles-list-filters.png)

プロファイルの詳細にアクセスするには、リストからプロファイルの名前をクリックします。 プロファイルの詳細ビューが開き、属性と購読したサービスを確認できます。 [プロファイルの詳細を参照する方法を説明します](create-profile.md)

プロファイルを削除するには、**[!UICONTROL その他のアクション]**&#x200B;メニューから対応するオプションを選択します。
