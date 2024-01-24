---
audience: end-user
product: campaign
title: コンテンツテンプレートの操作
description: Adobe Campaign のメールのコンテンツを再利用するためのテンプレートを作成する方法について説明します
feature: Templates
topic: Content Management
role: User
level: Beginner
badge: label="限定提供（LA）"
exl-id: 23818080-d7c6-4829-8117-d6b359bd76dd
source-git-commit: 72899742daf04a0da6e2fb3d802b7841753b8c6c
workflow-type: tm+mt
source-wordcount: '802'
ht-degree: 89%

---

# コンテンツテンプレートの操作 {#content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_menu"
>title="独自のコンテンツの定義"
>abstract="スタンドアロンのカスタムテンプレートをゼロから作成して、複数のメール全体でコンテンツを再利用できるようにします。"

設計プロセスを加速し改善するために、スタンドアロンのテンプレートを作成すると、[!DNL Adobe Campaign] 全体でカスタムコンテンツを簡単に再利用できます。

この機能により、コンテンツ指向のユーザーがスタンドアロンのテンプレートで操作できるようになり、マーケティングユーザーが独自のメールキャンペーン内でテンプレートを再利用して調整できます。

>[!NOTE]
>
>現在、**メール**&#x200B;コンテンツテンプレートのみがサポートされています。

## テンプレートへのアクセスと管理 {#access-manage-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_edition"
>title="テンプレートコンテンツの編集"
>abstract="「**コンテンツを編集**」ボタンをクリックして、メールデザイナーでコンテンツを更新します。"

コンテンツテンプレートリストにアクセスするには、左側のメニューから&#x200B;**[!UICONTROL コンテンツ管理]**／**[!UICONTROL コンテンツテンプレート]**&#x200B;を選択します。

![](assets/content-template-list.png)

「[テンプレートとして保存](#save-as-template)」オプションを使用したメールから作成した、または、**[!UICONTROL コンテンツテンプレート]**&#x200B;メニューから作成したすべてのテンプレートが表示されます。

<!--You can sort content templates by creation or modification date. You can also choose to display only the items that you created or modified.-->

ドロップダウンリストを使用して特定の[フォルダー](../get-started/permissions.md#folders)をフィルタリングしたり、[クエリモデラー](../query/query-modeler-overview.md)を使用してルールを追加したりできます。

![](assets/content-template-list-filters.png)

テンプレートコンテンツを編集するには、リストから目的の項目をクリックします。以下を行うことができます。

* プロパティを編集します。

* 「**[!UICONTROL コンテンツを編集]**」ボタンをクリックして、[メールデザイナー](get-started-email-designer.md)でコンテンツを更新します。

![](assets/content-template-edition.png)

テンプレートを削除するには、**[!UICONTROL その他のアクション]**&#x200B;メニューから対応するオプションを選択します。

![](assets/content-template-list-delete.png)

>[!NOTE]
>
>テンプレートを削除しても、このテンプレートを使用して作成した配信は影響を受けません。

## コンテンツテンプレートの作成 {#create-content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_design"
>title="コンテンツテンプレートのデザイン"
>abstract="コンテンツテンプレートのデザイン"

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_selection"
>title="コンテンツテンプレートの選択"
>abstract="コンテンツテンプレートの選択"

コンテンツテンプレートを作成する方法は 2 つあります。

* 左側のパネルの&#x200B;**[!UICONTROL コンテンツテンプレート]**&#x200B;メニューを使用して、コンテンツテンプレートをゼロから作成します。[詳細情報](#create-template-from-scratch)

* メールをデザインする際は、メールのコンテンツをテンプレートとして保存します。[詳細情報](#save-as-template)

保存すると、ゼロから作成した場合でも、以前のメールから作成した場合でも、[!DNL Adobe Campaign] 内で[メール](../email/create-email.md)を作成する際にこのテンプレートを使用できるようになります。[詳細情報](use-email-templates.md)

>[!NOTE]
>
>* コンテンツテンプレートに加えた変更は、メールには生成されません。
>
>* 同様に、メールでテンプレートを使用している場合、メールのコンテンツに対して行った編集は、以前に使用したコンテンツテンプレートには影響しません。

### ゼロからのテンプレートの作成 {#create-template-from-scratch}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_properties"
>title="テンプレートプロパティの定義"
>abstract="テンプレートをゼロから作成する際は、必要に応じて簡単に取得できるようにそのプロパティを定義します。"

コンテンツテンプレートをゼロから作成するには、次の手順に従います。

1. **[!UICONTROL コンテンツ管理]**／**[!UICONTROL コンテンツテンプレート]**&#x200B;の左側のメニューからコンテンツテンプレートリストにアクセスします。

1. 「**[!UICONTROL テンプレートを作成]**」を選択します。

   ![](assets/content-template-create.png)

1. テンプレートの詳細を入力します。テンプレートを保存するフォルダーを選択できます。デフォルトでは、コンテンツテンプレートはAdobe Campaign階層の専用フォルダーに保存されます。 **[!UICONTROL エクスプローラ]** > **[!UICONTROL リソース]** > **[!UICONTROL テンプレート]** > **[!UICONTROL コンテンツテンプレート]**. [詳しくは、フォルダーの作成方法を参照してください](../get-started/permissions.md#folders)

   ![](assets/content-template-details.png)

   >[!NOTE]
   >
   >現在、**メール**&#x200B;チャネルと **HTML** タイプのみがサポートされています。

1. 「**[!UICONTROL 作成]**」をクリックし、次の様々なオプションからテンプレートのデザイン方法を選択します。

   * [メールをゼロからデザイン](create-email-content.md) - メールデザイナーのインターフェイスを使用します。

   * [Raw HTML をコーディングまたはコピー＆ペースト](code-content.md) - メールデザイナーで直接行います。

   * [既存の HTML コンテンツをインポート](existing-content.md) - ファイルまたは .zip フォルダーから行います。

   * 組み込みまたはカスタムテンプレートのリストから既存のコンテンツを使用します。メールでコンテンツテンプレートを使用する手順については、[この節](use-email-templates.md)を参照してください。

   ![](assets/email_designer-templates.png)

1. [メールデザイナー](get-started-email-designer.md)が表示されます。選択したオプションに従って、他のメールの場合と同じ方法で、必要に応じてコンテンツを編集します。

   <!--You can test your content if needed. [Learn how](#test-template)-->

1. テンプレートの準備が整ったら、「**[!UICONTROL 保存]**」をクリックします。

   必要に応じて、テンプレート名の横にある矢印をクリックして&#x200B;**[!UICONTROL 詳細]**&#x200B;画面に戻り、テンプレートを編集します。

   ![](assets/content-template-save-back.png)

このテンプレートは、Adobe Campaign階層のデフォルトのフォルダー (**[!UICONTROL エクスプローラ]** > **[!UICONTROL リソース]** > **[!UICONTROL テンプレート]** > **[!UICONTROL コンテンツテンプレート]**) をクリックします。 [フォルダーの詳細を表示](../get-started/permissions.md#folders)

また、 **[!UICONTROL コンテンツテンプレート]** リスト。 [詳細情報](#access-manage-templates)

このテンプレートを使用して新しいコンテンツを作成できるようになりました。メールデザイナーの「**[!UICONTROL 保存済みのテンプレート]**」タブで利用できます。[詳細情報](use-email-templates.md)

### メールコンテンツをテンプレートとして保存 {#save-as-template}

[メールをデザイン](create-email-content.md)したら、後で再利用できるように、このコンテンツをテンプレートとして保存できます。保存済みのテンプレートは、Adobe Campaign 環境のすべてのユーザーが使用できます。

メールコンテンツをテンプレートとして保存するには、次の手順に従います。

1. メールデザイナーで、画面の右上にある「**[!UICONTROL その他]**」ボタンをクリックします。

1. ドロップダウンメニューから「**[!UICONTROL コンテンツテンプレートとして保存]**」を選択します。

   ![](assets/email_designer-save-template.png)

1. このテンプレートの名前を入力して保存します.

   ![](assets/email_designer-template-name.png)

このテンプレートは、Adobe Campaign階層のデフォルトのフォルダー (**[!UICONTROL エクスプローラ]** > **[!UICONTROL リソース]** > **[!UICONTROL テンプレート]** > **[!UICONTROL コンテンツテンプレート]**) をクリックします。 [フォルダーの詳細を表示](../get-started/permissions.md#folders)

また、 **[!UICONTROL コンテンツテンプレート]** リスト。 このテンプレートは、リスト上の他の項目と同様にアクセス、編集、削除できるスタンドアロンのコンテンツテンプレートになります。[詳細情報](#access-manage-templates)

このテンプレートを使用して新しいコンテンツを作成できるようになりました。メールデザイナーの「**[!UICONTROL 保存済みのテンプレート]**」タブで利用できます。[詳細情報](use-email-templates.md)

![](assets/email_designer-saved-template.png)

>[!NOTE]
>
>その新しいテンプレートに対する変更は、送信元のメールには生成されません。同様に、そのメール内の元のコンテンツを編集しても、新しいテンプレートは変更されません。

<!--

Test your content template {#test-template}

You can test the rendering of any email content template, whether created from scratch or from an email. To do so, follow the steps below.

1. Access the content template list.

1. Click **[!UICONTROL Edit content]** from the **[!UICONTROL Template properties]**.

1. Click **[!UICONTROL Simulate Content]** and select a test profile to check your email rendering. You can choose the desktop or mobile view.

1. You can send a proof to test your content and have it approved by some internal users before using it. To do so, click the **[!UICONTROL Send proof]** button and follow the steps described in .

-->
