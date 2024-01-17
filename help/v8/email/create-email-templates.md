---
audience: end-user
product: campaign
title: コンテンツテンプレートの操作
description: Adobe Campaign E メールでコンテンツを再利用するためのテンプレートの作成方法を説明します
feature: Templates
topic: Content Management
role: User
level: Beginner
badge: label="限定提供（LA）"
source-git-commit: 0d9d61e8561d21bca00cb5c274884624119eaa53
workflow-type: tm+mt
source-wordcount: '802'
ht-degree: 12%

---

# コンテンツテンプレートの操作 {#content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_menu"
>title="独自のコンテンツを定義する"
>abstract="複数の E メールでコンテンツを再利用可能にするために、スタンドアロンのカスタムテンプレートをゼロから作成します。"

高速で改善された設計プロセスを実現するために、スタンドアロンテンプレートを作成して、カスタムコンテンツを簡単に再利用できます。 [!DNL Adobe Campaign].

この機能を使用すると、コンテンツ指向のユーザーがスタンドアロンテンプレートで作業できるので、マーケティングユーザーは、自分の E メールキャンペーン内で再利用および調整できます。

>[!NOTE]
>
>現在のみ **電子メール** コンテンツテンプレートがサポートされています。

## テンプレートへのアクセスと管理 {#access-manage-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_edition"
>title="テンプレートコンテンツを編集"
>abstract="次をクリック： **コンテンツを編集** ボタンをクリックして、E メールデザイナーでコンテンツを更新します。"

コンテンツテンプレートリストにアクセスするには、 **[!UICONTROL コンテンツ管理]** > **[!UICONTROL コンテンツテンプレート]** を選択します。

![](assets/content-template-list.png)

作成されたすべてのテンプレート。 [テンプレートとして保存](#save-as-template) オプション ( **[!UICONTROL コンテンツテンプレート]** メニュー — が表示されます。

<!--You can sort content templates by creation or modification date. You can also choose to display only the items that you created or modified.-->

特定の [フォルダー](../get-started/permissions.md#folders) ドロップダウンリストを使用するか、 [クエリモデラー](../query/query-modeler-overview.md).

![](assets/content-template-list-filters.png)

テンプレートコンテンツを編集するには、リストから目的の項目をクリックします。 以下を行うことができます。

* プロパティを編集します。

* 次をクリック： **[!UICONTROL コンテンツを編集]** ボタンを使用して、コンテンツを更新します。 [E メールデザイナー](get-started-email-designer.md).

![](assets/content-template-edition.png)

テンプレートを削除するには、 **[!UICONTROL その他のアクション]** メニュー。

![](assets/content-template-list-delete.png)

>[!NOTE]
>
>テンプレートを削除しても、このテンプレートを使用して作成された配信は影響を受けません。

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

* 左側のレールを使用して、最初からコンテンツテンプレートを作成する **[!UICONTROL コンテンツテンプレート]** メニュー。 [詳細情報](#create-template-from-scratch)

* E メールをデザインする際に、E メールの内容をテンプレートとして保存します。 [詳細情報](#save-as-template)

一度保存すると、新規に作成した場合も、以前の E メールから作成した場合も、このテンプレートを使用して、 [電子メール](../email/create-email.md) 範囲 [!DNL Adobe Campaign]. [詳細情報](use-email-templates.md)

>[!NOTE]
>
>* コンテンツテンプレートに対しておこなった変更は E メールには反映されません。
>
>* 同様に、テンプレートを E メールで使用する場合、E メールコンテンツに対して行った編集は、以前に使用したコンテンツテンプレートには影響しません。

### 最初からテンプレートを作成 {#create-template-from-scratch}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_properties"
>title="テンプレートプロパティを定義する"
>abstract="テンプレートを最初から作成する場合は、必要に応じてプロパティを定義し、取得しやすくします。"

コンテンツテンプレートを最初から作成するには、次の手順に従います。

1. でコンテンツテンプレートリストにアクセスする **[!UICONTROL コンテンツ管理]** > **[!UICONTROL コンテンツテンプレート]** 左メニュー。

1. 選択 **[!UICONTROL テンプレートを作成]**.

   ![](assets/content-template-create.png)

1. テンプレートの詳細を入力します。 テンプレートを保存するフォルダーを選択できます。 デフォルトでは、コンテンツテンプレートはAdobe Campaign階層の専用フォルダーに保存されます。 **[!UICONTROL エクスプローラ]** > **[!UICONTROL リソース]** > **[!UICONTROL テンプレート]** > **[!UICONTROL コンテンツテンプレート]**. [フォルダーの作成方法を説明します](../get-started/permissions.md#folders)

   ![](assets/content-template-details.png)

   >[!NOTE]
   >
   >現在、 **電子メール** チャネルと **HTML** タイプがサポートされています。

1. クリック **[!UICONTROL 作成]** を選択し、様々なオプションからテンプレートのデザイン方法を選択します。

   * [メールをゼロからデザイン](create-email-content.md) 電子メールデザイナーのインターフェイスを使用する。

   * [コードまたはコピー&amp;ペーストの生のHTML](code-content.md) を直接 E メールデザイナーに追加します。

   * [既存のHTMLコンテンツの読み込み](existing-content.md) ファイルまたは.zip フォルダーから。

   * 組み込みテンプレートまたはカスタムテンプレートのリストの既存のコンテンツを使用します。 E メールでコンテンツテンプレートを使用する手順については、 [この節](use-email-templates.md).

   ![](assets/email_designer-templates.png)

1. The [E メールデザイナー](get-started-email-designer.md) が表示されます。 選択したオプションに従って、E メールと同じ方法で、必要に応じてコンテンツを編集します。

   <!--You can test your content if needed. [Learn how](#test-template)-->

1. テンプレートの準備が整ったら、「 **[!UICONTROL 保存]**.

   必要に応じて、テンプレート名の横にある矢印をクリックし、 **[!UICONTROL 詳細]** 画面を開いて、テンプレートを編集します。

   ![](assets/content-template-save-back.png)

このテンプレートは、Adobe Campaign階層のデフォルトのフォルダー (**[!UICONTROL エクスプローラ]** > **[!UICONTROL リソース]** > **[!UICONTROL テンプレート]** > **[!UICONTROL コンテンツテンプレート]**) をクリックします。 [フォルダーの詳細を表示](../get-started/permissions.md#folders)

また、 **[!UICONTROL コンテンツテンプレート]** リスト。 [詳細情報](#access-manage-templates)

これで、このテンプレートを使用して新しいコンテンツを作成できます。コンテンツは、 **[!UICONTROL 保存済みのテンプレート]** E メールデザイナーのタブ。 [詳細情報](use-email-templates.md)

### メールコンテンツをテンプレートとして保存 {#save-as-template}

[メールをデザイン](create-email-content.md)したら、後で再利用できるように、このコンテンツをテンプレートとして保存できます。保存済みのテンプレートは、Adobe Campaign 環境のすべてのユーザーが使用できます。

メールコンテンツをテンプレートとして保存するには、次の手順に従います。

1. E メールデザイナーで、 **[!UICONTROL その他]** ボタンを使用して、画面の右上に表示されます。

1. ドロップダウンメニューから「**[!UICONTROL コンテンツテンプレートとして保存]**」を選択します。

   ![](assets/email_designer-save-template.png)

1. このテンプレートの名前を入力して保存します.

   ![](assets/email_designer-template-name.png)

このテンプレートは、Adobe Campaign階層のデフォルトのフォルダー (**[!UICONTROL エクスプローラ]** > **[!UICONTROL リソース]** > **[!UICONTROL テンプレート]** > **[!UICONTROL コンテンツテンプレート]**) をクリックします。 [フォルダーの詳細を表示](../get-started/permissions.md#folders)

また、 **[!UICONTROL コンテンツテンプレート]** リスト。 これは、そのリスト上の他の項目としてアクセス、編集、削除が可能なスタンドアロンコンテンツテンプレートになります。 [詳細情報](#access-manage-templates)

これで、このテンプレートを使用して新しいコンテンツを作成できます。コンテンツは、 **[!UICONTROL 保存済みのテンプレート]** E メールデザイナーのタブ。 [詳細情報](use-email-templates.md)

![](assets/email_designer-saved-template.png)

>[!NOTE]
>
>その新しいテンプレートに対する変更は、元の電子メールには反映されません。 同様に、元のコンテンツがその E メール内で編集された場合、新しいテンプレートは変更されません。

<!--

Test your content template {#test-template}

You can test the rendering of any email content template, whether created from scratch or from an email. To do so, follow the steps below.

1. Access the content template list.

1. Click **[!UICONTROL Edit content]** from the **[!UICONTROL Template properties]**.

1. Click **[!UICONTROL Simulate Content]** and select a test profile to check your email rendering. You can choose the desktop or mobile view.

1. You can send a proof to test your content and have it approved by some internal users before using it. To do so, click the **[!UICONTROL Send proof]** button and follow the steps described in .

-->



