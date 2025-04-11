---
audience: end-user
title: E メールデザイナーでのメールの設計
description: メールコンテンツをゼロから設計する方法を学ぶ
exl-id: 23e71da3-434d-4619-a48a-334281592d85
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 62%

---

# メールコンテンツをゼロから開始 {#create-email-content}

>[!CONTEXTUALHELP]
>id="ac_structure_components_email"
>title="構造を追加"
>abstract="構造は、メールのレイアウトを定義します。**構造**&#x200B;コンポーネントをキャンバスにドラッグ＆ドロップして、メールコンテンツのデザインを開始します。"

>[!CONTEXTUALHELP]
>id="ac_structure_components_landing_page"
>title="構造を追加"
>abstract="構造は、ランディングページのレイアウトを定義します。**構造**&#x200B;コンポーネントをキャンバスにドラッグ＆ドロップして、ランディングページのデザインを開始します。"

>[!CONTEXTUALHELP]
>id="ac_structure_components_fragment"
>title="構造を追加"
>abstract="構造は、コンテンツフラグメントのレイアウトを定義します。**構造**&#x200B;コンポーネントをキャンバスにドラッグ＆ドロップして、フラグメントコンテンツのデザインを開始します。"

>[!CONTEXTUALHELP]
>id="ac_structure_components_template"
>title="構造を追加"
>abstract="構造は、テンプレートのレイアウトを定義します。**構造**&#x200B;コンポーネントをキャンバスにドラッグ＆ドロップして、テンプレートコンテンツのデザインを開始します。"

>[!CONTEXTUALHELP]
>id="ac_edition_columns_email"
>title="メール列の定義"
>abstract="E メールデザイナーを使用すると、列構造を定義することで、メールのレイアウトを簡単に定義できます。"

>[!CONTEXTUALHELP]
>id="ac_edition_columns_landing_page"
>title="ランディングページ列の定義"
>abstract="E メールデザイナーを使用すると、列構造を定義することで、ランディングページのレイアウトを簡単に定義できます。"

>[!CONTEXTUALHELP]
>id="ac_edition_columns_fragment"
>title="コンテンツフラグメント列の定義"
>abstract="メールデザイナーを使用すると、列構造を定義することで、コンテンツフラグメントのレイアウトを簡単に定義できます。"

>[!CONTEXTUALHELP]
>id="ac_edition_columns_template"
>title="テンプレート列の定義"
>abstract="E メールデザイナーを使用すると、列構造を定義することで、テンプレートのレイアウトを簡単に定義できます。"

E メールデザイナーを使用すると、メールの構造を簡単に定義できます。簡単なドラッグ&amp;ドロップ操作で構造要素を追加して移動することで、メールの本文を数秒でデザインできます。

➡️ [この機能をビデオで確認](#video)

メールコンテンツの作成を開始するには、次の手順に従います。

1. [E メールデザイナー](get-started-email-designer.md#start-authoring)のホームページで、「**[!UICONTROL ゼロからデザイン]**」オプションを選択します。

   ![ 「ゼロからデザイン」オプションがハイライト表示されたメールDesignerのホームページを示すスクリーンショット。](assets/email_designer-from-scratch.png){zoomable="yes"}

1. **[!UICONTROL 構造]** をキャンバスにドラッグ&amp;ドロップしてメールコンテンツのデザインを開始し、メールのレイアウトを定義します。

   >[!NOTE]
   >
   >列の積み重ねは、すべてのメールプログラムと互換性があるわけではありません。サポートされていない場合、列は積み重ねられません。

1. 必要に応じて **[!UICONTROL 構造]** を追加し、右側の専用パネルで設定を編集します。

   ![ メールDesignerの構造コンポーネントパネルを示すスクリーンショット。](assets/email_designer_structure_components.png){zoomable="yes"}

1. **[!UICONTROL n:n 列]**&#x200B;コンポーネントを選択して、選択する列の数（3 ～ 10）を定義します。各列の下部にある矢印を移動して、各列の幅を定義します。

   >[!NOTE]
   >
   >各列のサイズは、構造コンポーネントの全幅の 10％未満にすることはできません。空でない列は削除できません。

1. 「**[!UICONTROL コンポーネント]**」セクションから、必要な数の要素を 1 つ以上の構造にドラッグ&amp;ドロップします。 [詳しくは、コンテンツコンポーネントを参照してください](content-components.md)

1. 右側の **[!UICONTROL 設定]** タブまたは **[!UICONTROL スタイル]** タブを使用して、各コンポーネントをカスタマイズします。 例えば、各コンポーネントのテキストスタイル、パディングまたは余白を変更します。 [詳しくは、整列とパディングを参照してください](alignment-and-padding.md)

   ![ メールDesignerのスタイルのカスタマイズオプションを示すスクリーンショット。](assets/email_designer-styles.png){zoomable="yes"}

1. パーソナライゼーションフィールドを挿入して、プロファイルデータに基づいてメールコンテンツをカスタマイズします。 [詳しくは、コンテンツのパーソナライゼーションを参照してください](../personalization/personalize.md)

1. コンテンツへのリンクを追加します。

   左側のパネルから「**[!UICONTROL リンク]**」タブをクリックすると、追跡するコンテンツのすべての URL が表示されます。**[!UICONTROL トラッキングタイプ]** または **[!UICONTROL ラベル]** を変更し、必要に応じて **[!UICONTROL カテゴリ]** を追加します。

[詳しくは、リンクとメッセージトラッキングを参照してください](message-tracking.md)

   ![ メールDesignerの「リンク」タブを示すスクリーンショット。](assets/email_designer-links.png){zoomable="yes"}

1. 必要に応じて、詳細メニューの「**[!UICONTROL コードエディターに切り替え]**」をクリックしてコードエディターに切り替え、メールをさらにパーソナライズします。 これにより、例えばトラッキングタグやカスタム HTML タグを追加するために、メールソースコードを編集できます。 [詳しくは、コードエディターを参照してください](code-content.md)

   >[!CAUTION]
   >
   >コードエディターに切り替えた後で、このメールのビジュアルデザイナーに戻すことはできません。

1. コンテンツの準備が整ったら、「**[!UICONTROL コンテンツをシミュレート]**」をクリックして、メールのレンダリングを確認します。デスクトップ表示またはモバイル表示を選択します。 [詳しくは、メールのプレビューを参照してください](../preview-test/preview-test.md)

   ![ メールDesignerのシミュレーションオプションを示すスクリーンショット。](assets/email_designer-simulate.png){zoomable="yes"}

1. メールの準備が整ったら、「**[!UICONTROL 保存]**」をクリックします。

## チュートリアルビデオ {#video}

E メールデザイナーの操作方法について説明します。メールをゼロから構築およびデザインし、パーソナライズし、テストする方法を説明します。

>[!VIDEO](https://video.tv.adobe.com/v/3425867/?quality=12)