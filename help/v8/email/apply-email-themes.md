---
audience: end-user
title: メール作成体験の向上
description: 再利用可能なテーマやモジュールを活用して、メール作成を合理化し、キャンペーン全体のデザイン一貫性と効率性を確保する方法を説明します。
badge: label="限定提供（LA）" type="Informative"
feature: Email Design
topic: Content Management
role: User
level: Beginner, Intermediate
keywords: メールのテーマ、モジュール、再利用性、ブランドの一貫性、メールデザイン、カスタム CSS、モバイル最適化
exl-id: c9e02bca-032d-4771-ad53-5bbebabc4c5d
source-git-commit: 65031741dc7c667ef74469d75b8ea60a5fc20aaf
workflow-type: ht
source-wordcount: '2077'
ht-degree: 100%

---

# メールコンテンツへのテーマの追加 {#apply-email-themes}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="E メールデザイナー（LA）のテーマ"
>abstract="再利用可能なテーマスタイルと変数を適用すると、メールコンテンツのブランドとの一貫性を維持できます。 この機能は、一連の組織でのみ使用できます（限定提供）。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=ja" text="リリースノートを参照してください"

>[!CONTEXTUALHELP]
>id="acw_email_apply_theme"
>title="メールへのテーマの適用"
>abstract="メールのテーマを選択して、ブランドやデザインに合った特定のスタイル設定をすばやく適用します。"

>[!AVAILABILITY]
>
>この機能は限定提供（LA）中です。ご利用になるには、Adobe 担当者にお問い合わせください。

テーマを使用すると、技術に詳しくないユーザーでも、標準テンプレート <!-- to achieve brand specific results--> の上にカスタムスタイルを追加することで、特定のブランドやデザイン言語に合った再利用可能なコンテンツを作成できるようになります。

この機能により、マーケターはブランドに即した魅力的なメールを、より迅速かつ容易に活用できるようになります。また、独自のデザインニーズに合わせて高度なカスタマイズオプションを利用できます。

## ガードレールと制限 {#themes-guardrails}

* メールをゼロから作成する際に、テーマを使ってコンテンツの作成を開始し、ブランドやデザインに合った特定のスタイルをすばやく適用することができます。

  手動スタイルモードを選択した場合、メールをリセットしない限り、テーマを適用することはできません。

* [フラグメント](../content/fragments.md)は、テーマを使用モードと手動スタイル設定モード間で互換性がありません。

   * テーマを使用せずに作成されたメールコンテンツでは、テーマ別のフラグメントは使用できません。

   * テーマ別コンテンツで[フラグメント](../content/fragments.md)を活用するには、このフラグメントがテーマを使用して作成されている必要があります。[詳細情報](#leverage-themes-fragment)

   * メールコンテンツでフラグメントを使用する場合は、このフラグメント用に定義したテーマを適用していることを確認してください。これを行わない場合、特に Outlook 2021 以前のバージョンで、表示の問題が発生する可能性があります。[詳細情報](#leverage-themes-fragment)

* HTML で作成されたコンテンツを使用している場合、[互換モード](existing-content.md)になり、このコンテンツにテーマを直接適用することはできません。

   * テーマを適用するには、最初に読み込んだコンテンツを[新しいテンプレート](../content/create-email-templates.md#save-as-template)として保存してから、このテンプレートをテーマ互換コンテンツに変換する必要があります。次に、このテンプレートを使用してメールコンテンツを作成します。[このセクション](#theme-convertor)では、手動スタイル設定で作成したテンプレートを変換する方法を説明します。

   * また、読み込んだ HTML コンテンツを変換することもできます。[詳細情報](existing-content.md)

  <!--To fully leverage all the capabilities of the Email Designer, including themes, you must either create a new content in Use Themes mode, or convert your imported HTML content. [Learn more](existing-content.md)-->

* テーマでカスタム web フォント（Google フォントを含む）を使用する場合は、多くのメールクライアントが対応していないことに注意してください。あらゆるメールクライアントで読みやすさを確保するために、テーマには必ず適切なフォールバックフォントを定義してください。

   * Gmail と Yahoo!HTML/CSS で指定したフォントファミリーに関係なく、外部の web フォントを読み込まず、システムフォントにフォールバックします。
   * Gmail でサポートされている Google フォントは、Roboto と Google Sans のみです。
   * Web フォントを&#x200B;*サポート*&#x200B;しているメールクライアントには、Apple Mail、iOS Mail、Android Mail、Thunderbird、Outlook for macOS などがあります。

<!--If you apply a theme to a content using a [fragment](../content/fragments.md) created with Manual Styling mode, the rendering may not be optimal.-->

## テーマを作成 {#create-and-edit-themes}

今後のメールコンテンツで活用できるテーマを定義するには、次の手順に従います。

1. 開始するには、新しい[コンテンツテンプレート](../content/create-email-templates.md)を作成します。

1. 「**[!UICONTROL テーマを作成または編集]**」オプションを選択します。

   ![「テーマを作成または編集」オプションを表示するコンテンツテンプレートエディター](assets/theme-create.png)

1. アドビのテーマを選択します。この例では、「**[!UICONTROL デフォルトのテーマ]**」を選択し、「**[!UICONTROL 作成]**」をクリックします。

   ![デフォルトのテーマが選択されたテーマピッカーと作成ボタン](assets/theme-select.png)

1. 「**[!UICONTROL マイテーマ]**」タブからカスタムテンプレートを選択し、「**[!UICONTROL 編集]**」をクリックして更新することもできます。

   ![編集がハイライト表示されたカスタムテーマを一覧表示する「マイテーマ」タブ](assets/theme-edit.png)

1. 「**[!UICONTROL 一般設定]**」タブで、ブランドに適した具体的な名前を付けてテーマの定義を開始しましょう。メールのデフォルトのビューポート幅を調整できます<!--and also export the current theme for reuse-->。

   <!--![General settings tab for theme name, viewport width, and export](assets/theme-general-settings.png)-->

1. 右側のパネルを使用して、様々なタブを移動し、デザイン設定を更新します。

   ![色、テキスト、間隔、その他のデザイン設定のタブが表示されている、テーマエディターの右パネル](assets/theme-right-pane.png)

1. 「**[!UICONTROL カラー]**」タブから：

   * 「**[!UICONTROL 編集]**」ボタンを使用して、ブランドのデフォルトカラーで&#x200B;**[!UICONTROL カラーパレット]**&#x200B;を設定します。「**[!UICONTROL プリセット]**」を選択して、すばやくカラースキームを作成するか、テーマの各色を個別に調整します。両方を組み合わせて使用することもできます。

     ![プリセットとカスタムカラーを使用してテーマカラーパレットを編集しているアニメーション](assets/theme-colors.gif)

   * 「**[!UICONTROL バリアントを追加]**」をクリックして、ライトモードやダークモードなど、テーマの各バリアントに独自のカラーパレットとニュアンスのコントロールがある複数のカラーバリアントを作成します。

     ![追加パレット用の「バリアントを追加」が表示された、テーマエディターのカラーバリアント](assets/theme-colors-variant.png)

   * バリアントごとに、**[!UICONTROL 編集]** アイコンをクリックして、個々の要素を編集します。作成したデフォルトのパレットまたは任意のカスタムカラーを使用できます。

     ![テーマカラーバリアント内での個別のカラーを編集しているアニメーション](assets/theme-colors-edit-variant.gif)

1. 「**[!UICONTROL テキスト設定]**」では、テーマ全体で使用するグローバルフォントを設定できます。さらに細かくコントロールするには、各見出しと段落タイプを編集して、フォント、サイズ、スタイルなどを調整することもできます。

   ![テーマ内のグローバルフォントおよび見出し、または段落スタイルの「テキスト設定」タブ](assets/theme-text.png)

   >[!NOTE]
   >
   >カスタム web フォントを選択する場合、Gmail や Yahoo! などの多くのメールクライアントでは、外部 web フォントはサポートしておらず、システムフォントにフォールバックします。あらゆるメールクライアントでコンテンツが正しく表示されるように、フォールバックフォントを含めることを検討してください。[詳細情報](#themes-guardrails)

1. 「**[!UICONTROL 間隔]**」タブで、リストから個々の要素を選択して、異なるコンポーネント間で適切に間隔を空けます。

   <!--![Spacing tab listing structure elements to adjust spacing between components](assets/theme-spacing.png)-->

1. 右側の他のタブを使用すると、このテーマの各ボタン要素、ディバイダー、追加の画像書式設定、グリッドレイアウト間隔を個別に管理できます。

   ![テーマエディターの右側のパネルのボタンのスタイル設定コントロール](assets/theme-buttons.png)

1. 「**[!UICONTROL 保存]**」をクリックして、今後の使用のためにこのテーマを保存します。「**[!UICONTROL マイテーマ]**」タブに表示されるようになりました。

<!--A little strange upon hitting Save, because once the theme is created, you need to hit Close to go back to Design your template screen, then click Cancel if you don't want to proceed with template creation.-->

## メールコンテンツへのテーマの追加 {#apply-themes-email}

コンテンツテンプレートまたはメールにデフォルトまたはカスタムのスタイル設定テーマを適用するには、次の手順に従います。

1. [!DNL Adobe Campaign] では、[メール配信を作成](create-email.md)するか、既存の配信から作業するか、メール[コンテンツテンプレート](../content/create-email-templates.md#create-template-from-scratch)を作成し、[メールコンテンツを編集](get-started-email-designer.md#start-authoring)します。

1. 次のいずれかのアクションを選択できます。

   * ビルトインの[メールテンプレート](../content/use-email-templates.md)を選択して、E メールデザイナーを開きます。各テンプレートに固有のデフォルトテーマが自動的に適用されます。

   * [新しいコンテンツをゼロからデザイン](create-email-content.md)し、**[!UICONTROL テーマを使用]**&#x200B;を選択して、定義済みのスタイル設定テーマの使用を開始します。

     ![「テーマの使用」と「手動スタイル設定」オプションを使用した E メールデザイナーの開始画面](assets/theme-from-scratch.png)

     >[!CAUTION]
     >
     >手動スタイル設定モードを選択した場合、デザインをリセットしない限り、テーマを適用することはできません。
     >
     >テーマ別コンテンツで[フラグメント](../content/fragments.md)を活用するには、このフラグメントがテーマを使用して作成されている必要があります。[詳細情報](#leverage-themes-fragment)

1. E メールデザイナーを開いたら、右側のパネルの「**[!UICONTROL テーマ]**」ボタンをクリックします。デフォルトのテーマまたはテンプレートのテーマが表示されます。このテーマでは、2 つのカラーバリアントを切り替えることができます。

   ![アクティブなテーマとカラーのババリアントを表示するテーマパネルが開いた、E メールデザイナーのキャンバス](assets/theme-default-hero.png)

1. 現在使用しているテーマの横にある矢印をクリックします。使用可能なカスタムテーマと Adobe テーマのリストが表示されます。

   ![テーマのドロップダウンが展開され、Adobe テーマとマイテーマが表示されている](assets/theme-hero-change.png)

1. 「**[!UICONTROL マイテーマ]**」をクリックし、作成したテーマを選択します。

   ![ユーザーが作成したテーマがテーマピッカーで選択されている、マイテーマリスト](assets/theme-select-custom.png)

1. ドロップダウンリストの外側をクリックします。新しく選択したカスタムテーマは、すべてのメールコンポーネントにそのスタイルを自動的に適用します。カラーバリアントがある場合は、切り替えることができます。

1. コンテンツテンプレートでテーマを選択した場合、「**[!UICONTROL テーマを編集]**」ボタンをクリックして更新できます。[詳細情報](#create-and-edit-themes)

   ![テーマパネルの「テーマを編集」ボタンを使用した、E メールデザイナーのコンテンツテンプレート](assets/theme-edit-in-template.png){width="40%"}

   >[!NOTE]
   >
   >このオプションは、メールコンテンツでテーマを使用する場合は使用できません。

1. 複数のカラーバリアントを使用してテーマを活用する場合は、指定した構造コンポーネントに対して特定のバリアントを選択できます。これにより、コンテンツ全体に対してカラーバリアントを定義し、ある特定の構造に対してのみ異なるバリアントを使用することができます。

   >[!NOTE]
   >
   >コンテンツコンポーネントに対してこのアクションを実行することはできません。

   これを行うには、構造コンポーネントを選択し、右側の「**[!UICONTROL スタイル]**」タブから「**[!UICONTROL 特定のテーマのバリアントを使用]**」オプションをクリックして、目的のバリアントをその構造に適用します。

   ![「スタイル」タブの「特定のテーマのバリアントを使用」オプションで選択された構造](assets/theme-structure-variant.png)

   この例では、現在のテーマの最初のカラーバリアントはメールコンテンツ全体に適用されますが、3 番目のカラーバリアントは選択した構造に適用されます。特定の構造の本文とビューポートの背景色が、他のコンテンツとは異なることがわかります。

テーマはいつでも切り替えることができます。メールコンテンツは変更されませんが、新しいテーマを反映するようにスタイルが更新されます。

### スタイルのロック解除 {#unlocking-styles}

コンポーネントの選択時、「**[!UICONTROL スタイル]**」タブの専用アイコンを使用して、そのスタイルのロックを解除できます。

![スタイルのロック解除アイコンが表示されている、選択したコンポーネントの「スタイル」タブ](assets/theme-unlock-style.png){width="90%"}

選択したテーマは、引き続きそのコンポーネントに適用されますが、そのスタイル設定要素を上書きすることができます。テーマを変更すると、新しいテーマは、上書きされなかったスタイル設定要素にのみ適用されます。<!--can you revert this action?-->

例えば、テキストコンポーネントのロックを解除すると、フォントカラーを<!--the font size from 11 to 14 and -->黒から赤に変更できます。

![白い背景にカスタムの赤いテキストカラーが使用されている、ロック解除されたテキストコンポーネント](assets/theme-unlock-style-ex-white.png){width="80%" align="center" zoomable="yes"}

テーマを変更した場合、<!--the font size is still 14 and -->そのコンポーネントのフォントカラーは引き続き赤になりますが、このコンポーネントの背景色は新しいテーマに変更されます。

![赤い色を保持した同じロック解除テキストと、新しいテーマで更新された背景](assets/theme-unlock-style-ex-colored.png){width="80%"}

## フラグメント内のテーマの活用 {#leverage-themes-fragment}

[テーマが適用された](#apply-themes-email)テンプレートまたはメール内のフラグメントを活用するには、このフラグメント自体がテーマを使用して作成されている必要があります。そうでない場合、テーマ付きのコンテンツでこのフラグメントを使用することはできません。

テーマと互換性のあるフラグメントを作成するには、次の手順に従います。

1. [!DNL Adobe Campaign] で、ビジュアルフラグメントを作成し、「**[!UICONTROL 作成]**」をクリックして、フラグメントのコンテンツをデザインします。[詳細情報](../content/create-fragment.md#create-from-scratch)

1. 「**[!UICONTROL テーマを使用]**」を選択して、定義済みのスタイル設定テーマで開始します。

   ![「テーマを使用」が選択されている、フラグメント E メールデザイナーのスタートオプション](assets/fragment-use-themes.png){width="100%"}

   >[!CAUTION]
   >
   >手動スタイル設定モードを選択した場合、フラグメントデザインをリセットしない限り、テーマを適用することはできません。

1. E メールデザイナーで、フラグメントの作成を開始できます。

1. 右側のパネルの「**[!UICONTROL テーマ]**」ボタンをクリックします。デフォルトのテーマが表示されます。このテーマの異なるカラーバリアントを切り替えることができます。

   ![テーマパネルにデフォルトのテーマが表示されている、E メールデザイナーのフラグメントコンテンツ](assets/fragment-default-theme.png){width="100%" align="center" zoomable="yes"}

1. 他のテーマを選択して、フラグメントコンテンツをプレビューできます。これを行うには、デフォルトのテーマの横にある矢印を選択し、「**[!UICONTROL テーマを選択]**」をクリックします。

   ![矢印の付いたテーマヘッダーとフラグメントプレビュー用の「テーマを選択」コントロール](assets/fragment-select-themes.png){width="40%"}

1. **[!UICONTROL Adobe テーマ]**&#x200B;と&#x200B;**[!UICONTROL マイテーマ]**&#x200B;の間を移動し、フラグメントと互換性のあるテーマを（両方のタブから）最大 5 つ選択できます。

   ![Adobe テーマとマイテーマのタブが表示された、互換性のあるテーマを選択するダイアログ](assets/fragment-select-compatible-themes.png){width=70%}

   >[!CAUTION]
   >
   >メールコンテンツでフラグメントを使用する場合は、このフラグメントに定義した[テーマを適用](#apply-themes-email)してください。これを行わない場合、特に Outlook 2021 以前のバージョンで、表示の問題が発生する可能性があります。

1. 「**[!UICONTROL 閉じる]**」をクリックします。

1. 「**[!UICONTROL デフォルトテーマ]**」の横にある矢印をもう一度選択します。選択したさまざまなテーマを切り替えて、各スタイルレンダリングをプレビューできるようになりました。

   ![テーマパネルでプレビュー用に複数のテーマを選択しているフラグメントキャンバス](assets/fragment-selected-themes.png){width=90%}

1. 「**[!UICONTROL テーマを選択]**」をもう一度クリックして、さらにテーマを追加するか、選択範囲を変更します。

## テーマと互換性のあるテンプレートにする {#theme-convertor}

[!DNL Adobe Campaign] を使用すると、手動スタイル設定を使用して作成されたテンプレートを、テーマ互換コンテンツに変換できます。これは、テーマが [!DNL Adobe Campaign] に導入される前にコンテンツテンプレートを作成した場合や、外部コンテンツを読み込む場合に特に便利です。

>[!NOTE]
>
> テーマと互換性を持つよう変換できるのは、**メールテンプレート**&#x200B;のみです。個々のメールは変換できません。まず、コンテンツをテンプレートとして保存する必要があります。

1. メール[コンテンツテンプレート](../content/create-email-templates.md)を開くか、E メールデザイナーを使用してコンテンツを編集します。

1. 右側のパネルで **[!UICONTROL テーマ]** アイコンを選択し、「**[!UICONTROL コンテンツからテーマを生成]**」ボタンをクリックします。

   ![「コンテンツからテーマを生成」ボタンがハイライト表示されたテーマパネル](assets/generate-theme.png){width=100%}

1. **[!UICONTROL テーマを作成]**&#x200B;ウィンドウが開きます。[!DNL Adobe Campaign]は、スタイル設定要素を自動的に検出し、新しいテーマに統合します。

   ![テンプレートコンテンツから検出されたスタイルを要約した、テーマを作成ダイアログ](assets/generate-theme-create-window.png){width=90%}

1. テーマに名前を付けます。

1. カラーバリアントの追加やフォントの編集など、ゼロからテーマを作成する場合と同じように、必要に応じて独自の調整を行います。[詳細情報](#create-and-edit-themes)

   ![カラーパレットとバリアントコントロールを表示している、エディターで生成されたテーマ](assets/generate-theme-colors.png){width=90%}

1. 「**[!UICONTROL 保存]**」をクリックして、この新しいテーマを再利用できるよう保存します。これで、このテーマを、他のテーマなどのコンテンツに適用できるようになりました。[詳細情報](#apply-themes-email)
