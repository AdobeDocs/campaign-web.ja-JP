---
title: Campaign でテストプロファイルを作成
description: Adobe Campaign でテストプロファイルを作成および管理する方法を学ぶ
feature: Audiences, Profiles, Seed Address, Proofs
role: User
level: Beginner
exl-id: d372713d-3024-46a1-b62e-f271b8ac829f
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 99%

---

# テストプロファイルの作成と管理 {#create-test-profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_menu"
>title="テストプロファイルを作成"
>abstract="テストプロファイルは、メッセージを送信する前にパーソナライゼーションとレンダリングをプレビューおよびテストできる追加の受信者です。メッセージコンテンツのプレビュー時にテストプロファイルを選択し、本配信前確認をテストプロファイルに送信して、メッセージのコンテンツと設定を制御および検証できます。"

テストプロファイルは、本配信前確認の送信、メッセージのコンテンツと設定の検証に使用されます。これらのプロファイルは、メッセージを送信する前にパーソナライゼーションとレンダリングをプレビューおよびテストできる追加の受信者です。メッセージコンテンツのプレビュー時にテストプロファイルを選択し、本配信前確認をテストプロファイルに送信して、メッセージのコンテンツと設定を制御および検証できます。

➡️ [ビデオでこの機能を確認する](#video)

<!--Learn more about test profiles in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html?lang=ja){target="_blank"}.-->

テストプロファイルに本配信前確認を送信する手順については、[この節](../preview-test/test-deliveries.md#test-profiles)を参照してください。

>[!NOTE]
>
>* テストプロファイルは、クライアントコンソールでシードアドレスとして作成されます。
>
>* テストプロファイルは、**[!UICONTROL クリック数]**、**[!UICONTROL 開封数]**、**[!UICONTROL 購読解除]**&#x200B;の配信統計に関するレポートからは自動的に除外されます。

## テストプロファイルのアクセスと管理 {#access-test-profiles}

テストプロファイルリストにアクセスするには、左側のメニューから&#x200B;**[!UICONTROL 顧客管理]**／**[!UICONTROL プロファイル]**&#x200B;を選択し、「**[!UICONTROL テストプロファイル]**」タブをクリックします。

![テストプロファイルリストビュー](assets/test-profile-list.png){zoomable="yes"}

* ドロップダウンリストを使用して特定の[フォルダー](../get-started/permissions.md#folders)をフィルタリングしたり、[クエリモデラー](../query/query-modeler-overview.md)を使用してルールを追加したりできます。

  ![テストプロファイルリストフィルター](assets/test-profile-list-filters.png){zoomable="yes"}

* 必要に応じて、テストプロファイルを複製し、更新できます。テストプロファイルを編集する手順は、[テストプロファイルを作成](#create-test-profile)する場合と同じです。

* テストプロファイルを削除するには、**[!UICONTROL その他のアクション]**&#x200B;メニューから対応するオプションを選択します。

  ![「テストプロファイルを削除」オプション](assets/test-profile-list-delete.png){zoomable="yes"}

* テストプロファイルを編集するには、リストから目的の項目をクリックします。テストプロファイルを編集する手順は、[テストプロファイルを作成](#create-test-profile)する場合と同じです。

また、**[!UICONTROL エクスプローラー]**&#x200B;ビューの&#x200B;**[!UICONTROL リソース]**／**[!UICONTROL キャンペーン管理]**／**[!UICONTROL シードアドレス]**&#x200B;ノードからテストプロファイルにアクセスすることもできます。

そこから、フォルダーまたはサブフォルダーを参照、作成、管理したり、関連する権限を確認したりできます。[フォルダーの作成方法を学ぶ](../get-started/permissions.md#folders)

![テストプロファイルフォルダービュー](assets/test-profiles-folders.png){zoomable="yes"}

また、**[!UICONTROL エクスプローラー]**&#x200B;ビューから、テストプロファイルをフィルタリング、削除、編集、[作成](#create-test-profile)することもできます。

## テストプロファイルの作成 {#create-test-profile}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_additionaldata"
>title="テストプロファイルの追加データ"
>abstract="データ管理ワークフローで作成された配信に使用され、特定の値を割り当てたいパーソナライズデータを入力します。"

テストプロファイルを作成するには、次の手順に従います。

1. **[!UICONTROL 顧客管理]**／**[!UICONTROL プロファイル]**&#x200B;を参照し、「**[!UICONTROL テストプロファイル]**」タブを選択します。

1. 「**[!UICONTROL テストプロファイルを作成]**」ボタンをクリックします。

   ![「テストプロファイルを作成」ボタン](assets/test-profile-create.png){zoomable="yes"}

1. 必要に応じて、テストプロファイルの詳細を入力します。<!--Most of the fields are the same as when creating profiles. [Learn more]-->

   ![テストプロファイルの詳細フォーム](assets/test-profile-details.png){zoomable="yes"}

   >[!NOTE]
   >
   >「**[!UICONTROL ラベル]**」フィールドには、定義した姓と名が自動的に入力されます。

1. デフォルトでは、テストプロファイルは&#x200B;**[!UICONTROL シードアドレス]**&#x200B;フォルダーに保存されます。目的の場所を参照して変更できます。[詳しくは、フォルダーの操作方法を参照してください](../get-started/permissions.md#folders)

   <!--![](assets/test-profile-folder.png){zoomable="yes"}-->

<!--
You do not need to enter all fields of each tab when creating a seed address. Missing personalization elements are entered randomly during delivery analysis. (Not valid?)
-->

1. 「**[!UICONTROL 連絡先情報]**」セクションに、メールアドレスと他の関連データを入力します。メールアドレスは、テストプロファイルラベルの後の括弧内に表示されます。

   ![「連絡先情報」セクション](assets/test-profile-address.png){zoomable="yes"}

1. 「**[!UICONTROL 今後の連絡は不要（すべてのチャネル）]**」チェックボックスをオンにすると、テストプロファイルはブロックリストに登録されます。このような受信者は、いずれのチャネル（メール、SMS など）でもターゲットに設定されなくなりました。

1. 「**[!UICONTROL 追加データ]**」タブでは、データ管理ワークフローで作成された配信に使用され、特定の値を割り当てたいパーソナライズデータを入力します。[ワークフローの詳細](../workflows/gs-workflows.md)

   ![「追加データ」タブ](assets/test-profile-additional-data.png){zoomable="yes"}

   追加のターゲットデータが、「**[!UICONTROL エンリッチメント]**」ワークフローアクティビティで「@」で始まるエイリアスで定義されていることを確認してください。それ以外の場合は、配信アクティビティでシードアドレスと共に適切に使用できません。[ エンリッチメントアクティビティの詳細情報 ](../workflows/activities/enrichment.md)

1. 「**[!UICONTROL 保存]**」ボタンをクリックします。

作成したテストプロファイルを使用して本配信前確認を送信する準備が整いました。[詳細情報](../preview-test/test-deliveries.md#test-profiles)

<!--Use test profiles in Direct mail? cf v7/v8-->

## チュートリアルビデオ {#video}

Campaign web ユーザーインターフェイスを使用してテストプロファイルを作成および管理する方法について説明します。

>[!VIDEO](https://video.tv.adobe.com/v/3442844?quality=12)