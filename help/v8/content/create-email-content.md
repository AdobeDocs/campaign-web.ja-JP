---
audience: end-user
title: 電子メールデザイナーでのメールの設計
description: メールコンテンツをゼロから設計する方法を学ぶ
exl-id: 23e71da3-434d-4619-a48a-334281592d85
badge: label="Alpha" type="Positive"
source-git-commit: 22fdc1713ed893504cba7ad93bb69c7b3f2db7fe
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 61%

---

# メールコンテンツをゼロから開始 {#create-email-content}

>[!CONTEXTUALHELP]
>id="ac_structure_components_email"
>title="構造の追加"
>abstract="構造は、E メールのレイアウトを定義します。 ドラッグ&amp;ドロップ **構造** コンポーネントをキャンバスに追加して、e メールコンテンツのデザインを開始します。"

>[!CONTEXTUALHELP]
>id="ac_structure_components_landing_page"
>title="構造の追加"
>abstract="構造は、ランディングページのレイアウトを定義します。 ドラッグ&amp;ドロップ **構造** コンポーネントをキャンバスに追加して、ランディングページのデザインを開始します。"

>[!CONTEXTUALHELP]
>id="ac_structure_components_fragment"
>title="構造の追加"
>abstract="構造は、フラグメントのレイアウトを定義します。 ドラッグ&amp;ドロップ **構造** コンポーネントをキャンバスに挿入して、フラグメントコンテンツのデザインを開始します。"

>[!CONTEXTUALHELP]
>id="ac_structure_components_template"
>title="構造の追加"
>abstract="構造は、テンプレートのレイアウトを定義します。 ドラッグ&amp;ドロップ **構造** コンポーネントをキャンバスに追加して、テンプレートコンテンツのデザインを開始します。"


>[!CONTEXTUALHELP]
>id="ac_edition_columns_email"
>title="メール列の定義"
>abstract="メールデザイナーを使用すると、列構造を定義することで、メールのレイアウトを簡単に定義できます。"

>[!CONTEXTUALHELP]
>id="ac_edition_columns_landing_page"
>title="ランディングページ列の定義"
>abstract="メールデザイナーを使用すると、列構造を定義することで、ランディングページのレイアウトを簡単に定義できます。"

>[!CONTEXTUALHELP]
>id="ac_edition_columns_fragment"
>title="フラグメント列の定義"
>abstract="メールデザイナーを使用すると、列構造を定義することで、フラグメントのレイアウトを簡単に定義できます。"

>[!CONTEXTUALHELP]
>id="ac_edition_columns_template"
>title="テンプレート列の定義"
>abstract="メールデザイナーを使用すると、列構造を定義することで、テンプレートのレイアウトを簡単に定義できます。"

メールデザイナーを使用すると、メールの構造を簡単に定義できます。簡単なドラッグ＆ドロップ操作で構造要素を追加して移動することで、メールの本文を数秒でデザインできます。

E メールコンテンツの作成を開始するには、次の手順に従います。

1. 次の [メールデザイナー](get-started-email-designer.md#start-authoring) ホームページで、 **[!UICONTROL ゼロからデザイン]** オプション。

   ![](assets/email_designer-from-scratch.png)

1. ドラッグ&amp;ドロップで E メールコンテンツのデザインを開始 **[!UICONTROL 構造]** をキャンバスにドラッグして、e メールのレイアウトを定義します。

   >[!NOTE]
   >
   >列の積み重ねは、すべてのメールプログラムと互換性があるわけではありません。 サポートされていない場合、列は積み重ねられません。

1. 追加する数 **[!UICONTROL 構造]** 必要に応じて、右側の専用パネルで設定を編集します。

   ![](assets/email_designer_structure_components.png)

1. 次の項目を選択できます。 **[!UICONTROL n:n 列]** コンポーネントを使用して、選択する列の数を定義します (3 ～ 10)。 また、各列の下部にある矢印を移動して、各列の幅を定義することもできます。

   >[!NOTE]
   >
   >各列のサイズは、構造コンポーネントの全幅の 10％未満にすることはできません。空でない列は削除できません。

1. 次の **[!UICONTROL コンポーネント]** セクションで、必要な数の要素を 1 つ以上の構造にドラッグ&amp;ドロップします。 [詳しくは、コンテンツコンポーネントを参照してください](content-components.md)

1. 各コンポーネントは、 **[!UICONTROL 設定]** または **[!UICONTROL スタイル]** タブを右にクリックします。 例えば、各コンポーネントのテキストスタイル、パディングまたは余白を変更できます。 [詳しくは、整列とパディングを参照してください](alignment-and-padding.md)

   ![](assets/email_designer-styles.png)

1. パーソナライゼーションフィールドを挿入して、プロファイルデータに基づいて E メールのコンテンツをカスタマイズします。 [詳しくは、コンテンツのパーソナライゼーションを参照してください](../personalization/personalize.md)

1. コンテンツへのリンクを追加します。

   左側のパネルから「**[!UICONTROL リンク]**」タブをクリックすると、追跡するコンテンツのすべての URL が表示されます。必要に応じて、**[!UICONTROL トラッキングタイプ]**&#x200B;または&#x200B;**[!UICONTROL ラベル]**&#x200B;を変更して、**[!UICONTROL カテゴリ]**&#x200B;を追加できます。

[詳しくは、リンクとメッセージトラッキングを参照してください](message-tracking.md)

   ![](assets/email_designer-links.png)

1. 必要に応じて、詳細メニューの「**[!UICONTROL コードエディターに切り替え]**」をクリックして、メールをさらにパーソナライズできます。これにより、例えば、トラッキングタグやカスタム HTML タグを追加するために、メールソースコードを編集できます。[詳しくは、コードエディターを参照してください](code-content.md)

   >[!CAUTION]
   >
   >コードエディターに切り替えた後で、このメールのビジュアルデザイナーに戻すことはできません。

1. コンテンツの準備が整ったら、「**[!UICONTROL コンテンツをシミュレート]**」をクリックして、メールのレンダリングを確認します。デスクトップ表示またはモバイル表示を選択できます。[詳しくは、メールのプレビューを参照してください](../preview-test/preview-test.md)

   ![](assets/email_designer-simulate.png)

1. メールの準備が整ったら、「**[!UICONTROL 保存]**」をクリックします。

