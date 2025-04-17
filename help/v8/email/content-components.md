---
audience: end-user
title: E メールデザイナーのコンテンツコンポーネントの使用
description: メールでコンテンツコンポーネントを使用する方法について説明します
exl-id: a77e7438-4bd3-4f99-a166-b98094a1292b
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '1389'
ht-degree: 49%

---

# コンテンツコンポーネントの使用 {#content-components}

>[!CONTEXTUALHELP]
>id="ac_content_components_email"
>title="コンテンツについて"
>abstract="コンテンツコンポーネントは、メールのレイアウトの作成に使用できる空のコンテンツプレースホルダーです。"

>[!CONTEXTUALHELP]
>id="ac_content_components_landing_page"
>title="コンテンツについて"
>abstract="コンテンツコンポーネントは、ランディングページのレイアウトの作成に使用できる空のコンテンツプレースホルダーです。"

>[!CONTEXTUALHELP]
>id="ac_content_components_fragment"
>title="コンテンツについて"
>abstract="コンテンツコンポーネントは、コンテンツフラグメントのレイアウトの作成に使用できる空のコンテンツプレースホルダーです。"

>[!CONTEXTUALHELP]
>id="ac_content_components_template"
>title="コンテンツについて"
>abstract="コンテンツコンポーネントは、テンプレートのレイアウトの作成に使用できる空のコンテンツプレースホルダーです。"

メールコンテンツを作成する場合は、**[!UICONTROL コンテンツ]** コンポーネントを使用すると、メールに配置して使用できる生の空コンポーネントでメールをパーソナライズできます。

メールのレイアウトを定義する **[!UICONTROL 構造]** 内には、必要な数だけ **[!UICONTROL コンテンツ]** を追加できます。

## コンテンツコンポーネントを追加 {#add-content-components}

メールにコンテンツコンポーネントを追加し、必要に応じて調整するには、次の手順に従います。

1. E メールデザイナーで、[既存のコンテンツ](existing-content.md)を使用するか、**[!UICONTROL 構造]**&#x200B;を空のコンテンツにドラッグ＆ドロップして、メールのレイアウトを定義します。方法については、[こちら](create-email-content.md)を参照してください。

1. 選択した&#x200B;**[!UICONTROL コンテンツ]**&#x200B;を、関係のある構造内にドラッグ＆ドロップします。

   ![ コンテンツコンポーネントをメールDesignerの構造にドラッグ&amp;ドロップする方法を示すスクリーンショット ](assets/email_designer_add_content_components.png){zoomable="yes"}

   >[!NOTE]
   >
   >単一の構造および構造の各列に複数のコンポーネントを追加できます。

1. コンテキストの「**[!UICONTROL 設定]**」タブを使用して、各コンポーネントのオプションを調整します。例えば、デスクトップやモバイルデバイスのみ、またはその両方に表示するように選択します。 また、このタブでリンクオプションを管理することもできます。[ リンク管理の詳細情報 ](message-tracking.md)

1. 「**[!UICONTROL スタイル]**」タブを使用して、各コンポーネントのスタイル属性を調整します。例えば、各コンポーネントのテキストスタイル、パディングまたは余白を変更します。 [詳しくは、整列とパディングを参照してください](alignment-and-padding.md)

   ![ メールDesignerのコンテンツコンポーネント用の「設定」タブを示すスクリーンショット ](assets/email_designer_content_components_settings.png){zoomable="yes"}

1. 右側のパネルにある **[!UICONTROL コンテンツ]** の詳細メニューで、必要に応じてコンテンツコンポーネントを削除または複製します。

## コンテナ {#container}

シンプルなコンテナを追加して、その中に別のコンテンツコンポーネントを追加することができます。これにより、内部で使用されるコンポーネントとは異なる特定のスタイルをコンテナに適用できます。

例えば、**[!UICONTROL コンテナ]**&#x200B;コンポーネントを追加したあと、そのコンテナの内部に[ボタン](#button)コンポーネントを追加します。 コンテナには特定の背景を使用し、ボタンには別の背景を使用します。

![ メールDesignerにコンテナコンポーネントを追加する方法を示すスクリーンショット。](assets/email_designer_container_component.png){zoomable="yes"}

## ボタン {#buttons}

**[!UICONTROL ボタン]**&#x200B;コンポーネントを使用すると、メールに 1 つまたは複数のボタンを挿入し、メールのオーディエンスを別のページにリダイレクトすることができます。

1. **[!UICONTROL コンテンツ]**&#x200B;リストから、**[!UICONTROL ボタン]**&#x200B;コンポーネントを&#x200B;**[!UICONTROL 構造]**&#x200B;コンポーネントにドラッグ＆ドロップします。

   ![ メールDesignerにボタンコンポーネントをドラッグ&amp;ドロップする方法を示すスクリーンショット。](assets/email_designer_13.png){zoomable="yes"}

1. 新しく追加したボタンをクリックして、テキストをパーソナライズし、「**[!UICONTROL 設定]**」タブと **[!UICONTROL スタイル]** タブにアクセスします。

   ![ メールDesignerのボタンコンポーネントの「設定」タブを示すスクリーンショット ](assets/email_designer_14.png){zoomable="yes"}

1. 「**[!UICONTROL 設定]**」タブの「**[!UICONTROL URL]**」フィールドに、ボタンをクリックしたときにリダイレクトする URL を追加します。

1. **[!UICONTROL ターゲット]** ドロップダウンリストを使用して、コンテンツの表示方法を選択します。

   * **[!UICONTROL なし]**：クリックされたのと同じフレームでリンクを開きます（デフォルト）。
   * **[!UICONTROL 空白]**：リンクを新しいウィンドウまたはタブで開きます。
   * **[!UICONTROL セルフ]**：クリックされたのと同じフレームでリンクを開きます。
   * **[!UICONTROL 親]**：親フレームでリンクを開きます。
   * **[!UICONTROL 上]**：ウィンドウの全体でリンクを開きます。

   ![ メールDesignerのボタンコンポーネントのターゲットオプションを示すスクリーンショット ](assets/email_designer_15.png){zoomable="yes"}

1. 「**[!UICONTROL スタイル]**」タブから「**[!UICONTROL 境界線]**」、「**[!UICONTROL サイズ]**」、「**[!UICONTROL 余白]** などのスタイル属性を変更して、ボタンをさらにパーソナライズします。

## テキスト {#text}

**[!UICONTROL テキスト]** コンポーネントを使用してメールにテキストを挿入し、「設定」タブと「**[!UICONTROL スタイル]**」タブを使用してスタイル **[!UICONTROL 境界線、サイズ、パディングなど]** を調整します。

1. **[!UICONTROL コンテンツ]**&#x200B;メニューから、**[!UICONTROL テキスト]**&#x200B;を&#x200B;**[!UICONTROL 構造]**&#x200B;コンポーネントにドラッグ＆ドロップします。

   ![ メールDesignerにテキストコンポーネントをドラッグ&amp;ドロップする方法を示すスクリーンショット ](assets/email_designer_11.png){zoomable="yes"}

1. 新しく追加したコンポーネントをクリックして、テキストをパーソナライズし、「**[!UICONTROL 設定]**」タブと **[!UICONTROL スタイル]** タブにアクセスします。

1. コンテキストツールバーから使用できる次のオプションを使用して、テキストを変更します。

   ![ メールDesignerのテキスト編集ツールバーを示すスクリーンショット。](assets/email_designer_27.png){zoomable="yes"}

   * **[!UICONTROL テキストスタイルの変更]**：テキストに太字、斜体、下線、取り消し線を適用します。
   * **配置の変更**：テキストの行揃えを左揃え、右揃え、中央揃えまたは両端揃えから選択します。
   * **[!UICONTROL リストの作成]**：テキストに箇条書きリストまたは番号リストを追加します。
   * **[!UICONTROL 見出しを設定]**：テキストに最大 6 つの見出しレベルを追加します。
   * **フォントサイズ**：テキストのフォントサイズをピクセル単位で選択します。
   * **[!UICONTROL 画像を編集]**：テキストコンポーネントに画像またはアセットを追加します。
   * **[!UICONTROL ソースコードを表示]**：テキストのソースコードを表示します。これは変更できません。
   * **[!UICONTROL 複製]**：テキストコンポーネントのコピーを追加します。
   * **[!UICONTROL 削除]**：選択したテキストコンポーネントをメールから削除します。
   * **[!UICONTROL パーソナライゼーションを追加]**：パーソナライゼーションフィールドを追加して、プロファイルデータからコンテンツをカスタマイズします。
   * **[!UICONTROL 条件付きコンテンツを有効にする]**：条件付きコンテンツを追加して、コンポーネントのコンテンツをターゲットプロファイルに適応させます。

1. 「**[!UICONTROL スタイル]**」タブから、テキストの色、フォントファミリー、境界線、パディング、余白などの他のスタイル属性を調整します。

   ![ メールDesignerのテキストコンポーネントの「スタイル」タブを示すスクリーンショット ](assets/email_designer_12.png){zoomable="yes"}

## ディバイダー {#divider}

**[!UICONTROL ディバイダー]**&#x200B;コンポーネントを使用すると、分割線を挿入してメールのレイアウトとコンテンツを整理できます。

線の色、スタイル、高さなどのスタイル属性は、「**[!UICONTROL スタイル]**」タブから調整できます。

![ メールDesignerにディバイダーコンポーネントを追加する方法を示すスクリーンショット。](assets/email_designer_16.png){zoomable="yes"}

## HTML {#HTML}

**[!UICONTROL HTML]** コンポーネントを使用して、既存のHTMLの一部をコピーして貼り付けることができます。 これにより、無料のモジュラーHTML コンポーネントを作成して、外部コンテンツを再利用できます。

1. **[!UICONTROL コンポーネント]**&#x200B;から、**[!UICONTROL HTML]** コンポーネントを&#x200B;**[!UICONTROL 構造]**&#x200B;コンポーネントにドラッグ＆ドロップします。

   ![ メールDesignerにHTML コンポーネントをドラッグ&amp;ドロップする方法を示すスクリーンショット。](assets/email_designer_22.png){zoomable="yes"}

1. 新しく追加したコンポーネントをクリックし、コンテキストツールバーから「**[!UICONTROL ソースコードを表示]**」選択して HTML を追加します。

   ![ メールDesignerのHTML コンポーネントのソースコードオプションを示したスクリーンショット。](assets/email_designer_23.png){zoomable="yes"}

>[!NOTE]
>
>外部コンテンツをメールDesignerに準拠させるには、Adobeでは [ ゼロからメッセージを作成し ](create-email-content.md) 既存のメールのコンテンツをコンポーネントにコピーすることをお勧めします。

## 画像 {#image}

>[!IMPORTANT]
>
>Assets メニューへのアクセスは、アクティブな Adobe Experience Manager as a Cloud Service ライセンスを持つユーザーに制限されます。このライセンスを保持していない場合、Assets メニューは使用できません。

**[!UICONTROL 画像]** コンポーネントを使用して、コンピューターからメールに画像ファイルを挿入します。

1. **[!UICONTROL コンテンツ]** メニューから **[!UICONTROL 画像]** を **[!UICONTROL 構造]** コンポーネントにドラッグ&amp;ドロップします。

   ![ メールDesignerに画像コンポーネントをドラッグ&amp;ドロップする方法を示すスクリーンショット ](assets/email_designer_9.png){zoomable="yes"}

1. 「**[!UICONTROL 参照]**」をクリックして、アセットから画像ファイルを選択します。また、「**[!UICONTROL メディアを読み込み]**」を選択することもできます。

   Adobe Experience Managerへのアセットのアップロードと追加について詳しくは、[Adobe Experience Manager as a Cloud Service ドキュメント ](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/manage/add-assets.html?lang=ja) を参照してください。

   ![ メールDesignerの画像コンポーネントの参照オプションを示すスクリーンショット。](assets/email_designer_28.png){zoomable="yes"}

1. フォルダー内を移動して必要な特定のアセットを見つけるか、検索バーを使用して効率的に見つけます。

   検索しているアセットが見つかったら、「**[!UICONTROL 選択]**」をクリックします。

   ![ メールDesignerでのアセット選択プロセスを示すスクリーンショット。](assets/email_designer_29.png){zoomable="yes"}

1. 新しく追加したコンポーネントをクリックし、「**[!UICONTROL 設定]**」タブを使用して画像プロパティを設定します。

   * **[!UICONTROL 画像タイトル]** 画像のタイトルを指定できます。
   * **[!UICONTROL 代替テキスト]**&#x200B;を使用すると、画像にリンクされたキャプションを定義できます。これは、HTML の alt 属性に対応します。

   ![ メールDesignerの画像コンポーネントの「設定」タブを示すスクリーンショット ](assets/email_designer_10.png){zoomable="yes"}

1. オーディエンスを別のコンテンツにリダイレクトするリンクを追加します。 [詳細情報](message-tracking.md)

1. 「**[!UICONTROL スタイル]**」タブを使用して、余白、境界線などの他のスタイル属性を調整します。

## ソーシャル {#social}

**[!UICONTROL ソーシャル]**&#x200B;コンポーネントを使用すると、メールコンテンツにソーシャルメディアページへのリンクを挿入できます。

1. **[!UICONTROL コンテンツ]**&#x200B;コンテンツメニューから、**[!UICONTROL ソーシャル]**&#x200B;コンポーネントを&#x200B;**[!UICONTROL 構造]**&#x200B;コンポーネントにドラッグ＆ドロップします。

1. 新しく追加したコンポーネントをクリックします。

1. 「**[!UICONTROL 設定]**」タブの「**[!UICONTROL ソーシャル]**」フィールドで、追加または削除するソーシャルメディアを選択します。

   ![ メールDesignerのソーシャルコンポーネントの「設定」タブを示すスクリーンショット。](assets/email_designer_20.png){zoomable="yes"}

1. 「**[!UICONTROL 画像のサイズ]**」フィールドでアイコンのサイズを選択します。

1. 各ソーシャルメディアアイコンをクリックして、オーディエンスのリダイレクト先の **[!UICONTROL URL]** を設定します。

   ![ メールDesignerのソーシャルメディアアイコンの URL 設定を示すスクリーンショット。](assets/email_designer_21.png){zoomable="yes"}

1. 必要に応じて、**[!UICONTROL Source]** フィールドで各ソーシャルメディアのアイコンを変更します。

1. 「**[!UICONTROL スタイル]**」タブから、スタイル、余白、境界線などの他のスタイル属性を調整します。