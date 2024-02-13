---
audience: end-user
product: campaign
title: コンテンツテンプレートの操作
description: Adobe Campaign のメールのコンテンツを再利用するためのテンプレートを作成する方法について説明します
feature: Templates
topic: Content Management
role: User
level: Beginner
exl-id: 23818080-d7c6-4829-8117-d6b359bd76dd
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '964'
ht-degree: 50%

---

# コンテンツテンプレートの操作 {#content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_menu"
>title="コンテンツテンプレート"
>abstract="高速で改善されたデザインプロセスを実現するために、スタンドアロンの E メールテンプレートを作成して、Adobe Campaign全体でカスタムコンテンツを簡単に再利用できます。 これらのコンテンツテンプレートは、組み込みまたはカスタムのテンプレートに基づいて、既存のコンテンツから作成したり、コンテンツテンプレートエディターで読み込んで、ゼロからデザインすることができます。"

高速で改善された設計プロセスを実現するために、スタンドアロンテンプレートを作成して、カスタムコンテンツを簡単に再利用できます。 [!DNL Adobe Campaign]. これらのコンテンツテンプレートは、組み込みまたはカスタムのテンプレートに基づいて、既存のコンテンツから作成したり、コンテンツテンプレートエディターで読み込んで、ゼロからデザインすることができます。

この機能により、コンテンツ指向のユーザーがスタンドアロンのテンプレートで操作できるようになり、マーケティングユーザーが独自のメールキャンペーン内でテンプレートを再利用して調整できます。

>[!NOTE]
>
>現在、**メール**&#x200B;コンテンツテンプレートのみがサポートされています。

## コンテンツテンプレートへのアクセス {#access-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_edition"
>title="テンプレートコンテンツの編集"
>abstract="「**コンテンツを編集**」ボタンをクリックして、メールデザイナーでコンテンツを更新します。"

コンテンツテンプレートリストにアクセスするには、 **[!UICONTROL コンテンツ管理]** > **[!UICONTROL コンテンツテンプレート]** メニューをクリックします。

![](assets/content-template-list.png){zoomable=&quot;yes&quot;}

このダッシュボードには、使用可能なすべてのコンテンツテンプレートがリストとして表示されます。 ドロップダウンリストを使用して特定の[フォルダー](../get-started/permissions.md#folders)をフィルタリングしたり、[クエリモデラー](../query/query-modeler-overview.md)を使用してルールを追加したりできます。

![](assets/content-template-list-filters.png){zoomable=&quot;yes&quot;}

リストから、既存のコンテンツテンプレートを編集、複製、削除できます。 コンテンツテンプレートを作成するには、上部のセクションにあるボタンを使用します。


## コンテンツテンプレートの作成 {#create-content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_design"
>title="コンテンツテンプレートのデザイン"
>abstract="コンテンツテンプレートのデザイン"

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_selection"
>title="コンテンツテンプレートの選択"
>abstract="コンテンツテンプレートの選択"

コンテンツテンプレートは、 [既存の電子メールをテンプレートとして保存中](#save-as-template)または電子メールテンプレートのリストから、 **コンテンツテンプレートを作成** ボタン [以下に詳述する](#create-template-from-scratch).

保存すると、このテンプレートを使用して、 [電子メール](../email/create-email.md) 範囲 [!DNL Adobe Campaign]. [詳細情報](use-email-templates.md)

>[!NOTE]
>
>* コンテンツテンプレートに加えた変更は、メールには生成されません。
>
>* 同様に、メールでテンプレートを使用している場合、メールのコンテンツに対して行った編集は、以前に使用したコンテンツテンプレートには影響しません。

### 新しいコンテンツテンプレートを作成します {#create-template-from-scratch}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_properties"
>title="テンプレートプロパティの定義"
>abstract="必要に応じて、取得する E メールコンテンツテンプレートプロパティを簡単に定義します。"

コンテンツテンプレートダッシュボードから新しいコンテンツテンプレートを作成するには、次の手順に従います。

1. 次の場所からコンテンツテンプレートリストを参照します。 **[!UICONTROL コンテンツ管理]** > **[!UICONTROL コンテンツテンプレート]** 左側のレール。

1. 「**[!UICONTROL テンプレートを作成]**」を選択します。

   ![](assets/content-template-create.png){zoomable=&quot;yes&quot;}

1. テンプレートのラベルとプロパティを入力します。 テンプレートを保存するフォルダーを選択できます。デフォルトでは、コンテンツテンプレートは、Adobe Campaign 階層の専用フォルダー（**[!UICONTROL エクスプローラー]**／**[!UICONTROL リソース]**／**[!UICONTROL テンプレート]**／**[!UICONTROL コンテンツテンプレート]**）に保存されます。のフォルダーの詳細を説明します [このページ](../get-started/permissions.md#folders)

   ![](assets/content-template-details.png){zoomable=&quot;yes&quot;}

1. 「**[!UICONTROL 作成]**」をクリックし、次の様々なオプションからテンプレートのデザイン方法を選択します。

   * [コンテンツをゼロから設計する](create-email-content.md) 電子メールデザイナーのインターフェイスを使用する。

   * [Raw HTML をコーディングまたはコピー＆ペースト](code-content.md) - メールデザイナーで直接行います。

   * [既存の HTML コンテンツをインポート](existing-content.md) - ファイルまたは .zip フォルダーから行います。

   * 組み込みまたはカスタムテンプレートのリストから既存のコンテンツを使用します。メールでコンテンツテンプレートを使用する手順については、[この節](use-email-templates.md)を参照してください。

   ![](assets/email_designer-templates.png){zoomable=&quot;yes&quot;}

1. E メールデザイナーが表示されます。 選択したオプションに従って、E メールと同じ方法で、必要に応じてコンテンツを編集します。 電子メールデザイナーの使用方法については、 [この節](get-started-email-designer.md).

   <!--You can test your content if needed. [Learn how](#test-template)-->

1. テンプレートの準備が整ったら、「**[!UICONTROL 保存]**」をクリックします。

   必要に応じて、テンプレート名の横にある矢印をクリックして&#x200B;**[!UICONTROL 詳細]**&#x200B;画面に戻り、テンプレートを編集します。

   ![](assets/content-template-save-back.png){zoomable=&quot;yes&quot;}

このテンプレートは、 **[!UICONTROL コンテンツテンプレート]** リスト。 [詳細情報](#access-templates)

このテンプレートを使用して新しいコンテンツを作成できるようになりました。メールデザイナーの「**[!UICONTROL 保存済みのテンプレート]**」タブで利用できます。[詳細情報](use-email-templates.md)

### メールコンテンツをテンプレートとして保存 {#save-as-template}

[メールをデザイン](create-email-content.md)したら、後で再利用できるように、このコンテンツをテンプレートとして保存できます。保存済みのテンプレートは、Adobe Campaign 環境のすべてのユーザーが使用できます。

メールコンテンツをテンプレートとして保存するには、次の手順に従います。

1. メールデザイナーで、画面の右上にある「**[!UICONTROL その他]**」ボタンをクリックします。

1. ドロップダウンメニューから「**[!UICONTROL コンテンツテンプレートとして保存]**」を選択します。

   ![](assets/email_designer-save-template.png){zoomable=&quot;yes&quot;}

1. このテンプレートの名前を入力して保存します.

   ![](assets/email_designer-template-name.png){zoomable=&quot;yes&quot;}

テンプレートが保存され、 **[!UICONTROL コンテンツテンプレート]** リスト。 このテンプレートは、リスト上の他の項目と同様にアクセス、編集、削除できるスタンドアロンのコンテンツテンプレートになります。[詳細情報](#access-manage-templates)

このテンプレートを使用して新しいコンテンツを作成できるようになりました。メールデザイナーの「**[!UICONTROL 保存済みのテンプレート]**」タブで利用できます。[詳細情報](use-email-templates.md)

![](assets/email_designer-saved-template.png){zoomable=&quot;yes&quot;}


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


## コンテンツテンプレートの変更 {#modify-delete}

既存のコンテンツテンプレートを更新するには、次の手順に従います。

1. コンテンツテンプレートのリストで、変更するテンプレートのラベルをクリックして、編集します。

1. 「**[!UICONTROL コンテンツを編集]**」ボタンをクリックして、[メールデザイナー](get-started-email-designer.md)でコンテンツを更新します。

![](assets/content-template-edition.png){zoomable=&quot;yes&quot;}

>[!NOTE]
>
>コンテンツテンプレートに対して行われた変更は、このコンテンツテンプレートを使用する E メールには反映されません。

## コンテンツテンプレートの削除 {#content-delete}

コンテンツテンプレートを削除する方法は 2 つあります。

* コンテンツテンプレートのリストで、省略記号ボタンをクリックし、「 **削除**

  ![ダッシュボードからのコンテンツテンプレートの削除](assets/content-template-list-delete.png)

* コンテンツテンプレート自体で、 **その他** ボタンをクリックし、 **削除**


>[!NOTE]
>
>コンテンツテンプレートを削除しても、このテンプレートを使用して作成された配信には影響しません。


## コンテンツテンプレートの複製 {#content-duplicate}

コンテンツテンプレートを複製する方法は 2 つあります。

* コンテンツテンプレートのリストで、省略記号ボタンをクリックし、「 **複製**

* コンテンツテンプレート自体で、 **その他** ボタンをクリックし、 **複製**

どちらの場合も、複製を確認して新しいコンテンツテンプレートを作成します。 新しいコンテンツテンプレートのラベルは次のとおりです。 **のコピー`<label of the initial campaign`**. テンプレート設定を参照して、このラベルを更新します。

