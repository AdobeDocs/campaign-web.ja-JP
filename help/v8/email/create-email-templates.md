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
source-git-commit: 5b42671173e7fd7f024eb7eb03a0836eae7ef622
workflow-type: tm+mt
source-wordcount: '968'
ht-degree: 98%

---

# コンテンツテンプレートの操作 {#content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_menu"
>title="コンテンツテンプレート"
>abstract="設計プロセスを加速し改善するために、スタンドアロンのメールテンプレートを作成すると、Adobe Campaign 全体でカスタムコンテンツを簡単に再利用できます。これらのコンテンツテンプレートは、ビルトインテンプレートまたはカスタムテンプレートに基づいてゼロから設計したり、既存のコンテンツから作成したり、コンテンツテンプレートエディターにインポートしたりできます。"

設計プロセスを加速し改善するために、スタンドアロンのテンプレートを作成すると、[!DNL Adobe Campaign] 全体でカスタムコンテンツを簡単に再利用できます。これらのコンテンツテンプレートは、ビルトインテンプレートまたはカスタムテンプレートに基づいてゼロから設計したり、既存のコンテンツから作成したり、コンテンツテンプレートエディターにインポートしたりできます。

この機能により、コンテンツ指向のユーザーがスタンドアロンのテンプレートで操作できるようになり、マーケティングユーザーが独自のメールキャンペーン内でテンプレートを再利用して調整できます。

>[!NOTE]
>
>現在、**メール**&#x200B;コンテンツテンプレートのみがサポートされています。

## コンテンツテンプレートへのアクセス {#access-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_edition"
>title="テンプレートコンテンツの編集"
>abstract="「**コンテンツを編集**」ボタンをクリックして、メールデザイナーでコンテンツを更新します。"

コンテンツテンプレートリストにアクセスするには、左側のパネルから&#x200B;**[!UICONTROL コンテンツ管理]**／**[!UICONTROL コンテンツテンプレート]**&#x200B;メニューを参照します。

![](assets/content-template-list.png){zoomable=&quot;yes&quot;}

このダッシュボードには、使用可能なすべてのコンテンツテンプレートがリストとして表示されます。ドロップダウンリストを使用して特定の[フォルダー](../get-started/permissions.md#folders)をフィルタリングしたり、[クエリモデラー](../query/query-modeler-overview.md)を使用してルールを追加したりできます。

![](assets/content-template-list-filters.png){zoomable=&quot;yes&quot;}

リストから、既存のコンテンツテンプレートを編集、複製または削除できます。コンテンツテンプレートを作成するには、上部のセクションにあるボタンを使用します。


## コンテンツテンプレートの作成 {#create-content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_design"
>title="コンテンツテンプレートのデザイン"
>abstract="メールコンテンツテンプレートをデザインします。"

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_selection"
>title="コンテンツテンプレートの選択"
>abstract="メールコンテンツテンプレートを選択します。"

コンテンツテンプレートは、[以下の説明に従って](#create-template-from-scratch)、[既存のメールをテンプレートとして保存](#save-as-template)するか、メールテンプレートのリストから「**コンテンツテンプレートを作成**」ボタンを使用して作成できます。

保存すると、[!DNL Adobe Campaign] 内で[メール](../email/create-email.md)を作成する際に、このテンプレートを使用できます。[詳細情報](use-email-templates.md)

>[!NOTE]
>
>* コンテンツテンプレートに加えた変更は、メールには生成されません。
>
>* 同様に、メールでテンプレートを使用している場合、メールのコンテンツに対して行った編集は、以前に使用したコンテンツテンプレートには影響しません。

### 新しいコンテンツテンプレートの作成 {#create-template-from-scratch}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_properties"
>title="テンプレートプロパティの定義"
>abstract="メールコンテンツテンプレートプロパティを定義して、必要に応じて簡単に取得できるようにします。"

コンテンツテンプレートダッシュボードから新しいコンテンツテンプレートを作成するには、次の手順に従います。

1. **[!UICONTROL コンテンツ管理]**／**[!UICONTROL コンテンツテンプレート]**&#x200B;の左側のパネルからコンテンツテンプレートリストを参照します。

1. 「**[!UICONTROL テンプレートを作成]**」を選択します。

   ![](assets/content-template-create.png){zoomable=&quot;yes&quot;}

1. テンプレートのラベルとプロパティを入力します。テンプレートを保存するフォルダーを選択できます。デフォルトでは、コンテンツテンプレートは、Adobe Campaign 階層の専用フォルダー（**[!UICONTROL エクスプローラー]**／**[!UICONTROL リソース]**／**[!UICONTROL テンプレート]**／**[!UICONTROL コンテンツテンプレート]**）に保存されます。フォルダーについて詳しくは、[このページ](../get-started/permissions.md#folders)を参照してください。

   ![](assets/content-template-details.png){zoomable=&quot;yes&quot;}

1. 「**[!UICONTROL 作成]**」をクリックし、次の様々なオプションからテンプレートのデザイン方法を選択します。

   * [コンテンツをゼロからデザイン](create-email-content.md) - E メールデザイナーのインターフェイスを使用します。

   * [Raw HTML をコーディングまたはコピー＆ペースト](code-content.md) - メールデザイナーで直接行います。

   * [既存の HTML コンテンツをインポート](existing-content.md) - ファイルまたは .zip フォルダーから行います。

   * 組み込みまたはカスタムテンプレートのリストから既存のコンテンツを使用します。メールでコンテンツテンプレートを使用する手順については、[この節](use-email-templates.md)を参照してください。

   ![](assets/email_designer-templates.png){zoomable=&quot;yes&quot;}

1. E メールデザイナーが表示されます。選択したオプションに従って、他のメールの場合と同じ方法で、必要に応じてコンテンツを編集します。メールデザイナーの使用方法については、[この節](get-started-email-designer.md)をご覧ください。

   <!--You can test your content if needed. [Learn how](#test-template)-->

1. テンプレートの準備が整ったら、「**[!UICONTROL 保存]**」をクリックします。

   必要に応じて、テンプレート名の横にある矢印をクリックして&#x200B;**[!UICONTROL 詳細]**&#x200B;画面に戻り、テンプレートを編集します。

   ![](assets/content-template-save-back.png){zoomable=&quot;yes&quot;}

このテンプレートは、**[!UICONTROL コンテンツテンプレート]**&#x200B;リストで利用できます。[詳細情報](#access-templates)

このテンプレートを使用して新しいコンテンツを作成できるようになりました。メールデザイナーの「**[!UICONTROL 保存済みのテンプレート]**」タブで利用できます。[詳細情報](use-email-templates.md)

### メールコンテンツをテンプレートとして保存 {#save-as-template}

[メールをデザイン](create-email-content.md)したら、後で再利用できるように、このコンテンツをテンプレートとして保存できます。保存済みのテンプレートは、Adobe Campaign 環境のすべてのユーザーが使用できます。

メールコンテンツをテンプレートとして保存するには、次の手順に従います。

1. メールデザイナーで、画面の右上にある「**[!UICONTROL その他]**」ボタンをクリックします。

1. ドロップダウンメニューから「**[!UICONTROL コンテンツテンプレートとして保存]**」を選択します。

   ![](assets/email_designer-save-template.png){zoomable=&quot;yes&quot;}

1. このテンプレートの名前を入力して保存します.

   ![](assets/email_designer-template-name.png){zoomable=&quot;yes&quot;}

**[!UICONTROL コンテンツテンプレート]**&#x200B;リストにテンプレートが保存され、表示されます。このテンプレートは、リスト上の他の項目と同様にアクセス、編集、削除できるスタンドアロンのコンテンツテンプレートになります。[詳細情報](#access-manage-templates)

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


## コンテンツテンプレートを変更する {#modify-delete}

既存のコンテンツテンプレートを更新するには、次の手順に従います。

1. コンテンツテンプレートのリストで、変更するテンプレートのラベルをクリックして、編集します。

1. 「**[!UICONTROL コンテンツを編集]**」ボタンをクリックして、[メールデザイナー](get-started-email-designer.md)でコンテンツを更新します。

![](assets/content-template-edition.png){zoomable=&quot;yes&quot;}

>[!NOTE]
>
>コンテンツテンプレートに加えた変更は、このコンテンツテンプレートを使用しているメールには反映されません。

## コンテンツテンプレートを削除する {#content-delete}

コンテンツテンプレートを削除するには、次の 2 つがあります。

* コンテンツテンプレートのリストで、省略記号ボタンをクリックし、「**削除**」を選択します。

  ![ダッシュボードからコンテンツテンプレートを削除](assets/content-template-list-delete.png)

* コンテンツテンプレート上で、「**詳細**」ボタンをクリックし、「**削除**」を選択します。


>[!NOTE]
>
>コンテンツテンプレートを削除しても、このテンプレートを使用して作成された配信には影響しません。


## コンテンツテンプレートを複製する {#content-duplicate}

コンテンツテンプレートを複製する方法には、次の 2 つがあります。

* コンテンツテンプレートのリストで、省略記号ボタンをクリックし、「**複製**」を選択します。

* コンテンツテンプレート上で、「**詳細**」ボタンをクリックし、「**複製**」を選択します。

どちらの場合も、複製を確認して新しいコンテンツテンプレートを作成します。新しいコンテンツテンプレートのラベルは、`<label of the initial campaign`**の**&#x200B;コピーです。テンプレートの設定を参照して、このラベルを更新します。

