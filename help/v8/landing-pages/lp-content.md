---
title: ランディングページ固有のコンテンツを定義する
description: Campaign Web でランディングページ固有のコンテンツをデザインする方法を説明します。
badge: label="限定提供（LA）"
source-git-commit: 2a02015d9d7a7de67f0bcffd328d37080c0f50c4
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 2%

---

# ランディングページ固有のコンテンツを定義する {#lp-content}

>[!CONTEXTUALHELP]
>id="ac_lp_components"
>title="コンテンツコンポーネントの使用"
>abstract="コンテンツコンポーネントは空のコンテンツプレースホルダーで、ランディングページのレイアウトの作成に使用できます。 ユーザーが選択して送信できるようにする特定のコンテンツを定義するには、フォームコンポーネントを使用します。"

ランディングページの任意のページのコンテンツを編集する際には、既に事前入力されています。

プライマリページとは、E メールや Web サイトなど、ランディングページへのリンクをクリックした後、ユーザーに対して直ちに表示されるページです。 プライマリページには、 [ランディングページ固有のフォームコンポーネント](#use-form-component) をクリックして、ユーザーが選択を選択して送信できるようにします。 また、 [ランディングページ固有のスタイル](#lp-form-styles).

ランディングページのコンテンツをさらにデザインするには、E メールと同じコンポーネントを使用できます。 [詳細情報](../email/content-components.md#add-content-components)

<!--
The content of the **[!UICONTROL Confirmation]**, **[!UICONTROL Error]** and **[!UICONTROL Expiration]** pages is also pre-filled. Edit them as needed.

Set the subscription form to the appropriate fields from the database to make sure it will work correctly.

The landing page default fields are already there for the selected template.

>[!NOTE]
>
>You can also create a click-through landing page without a **[!UICONTROL Form]** component. In that case, the landing page will be displayed to users, but they will not be required to submit any form. This can be useful if you only want to showcase a landing page without requiring any action from your recipients such as opt-in or opt out, or want to provide information that doesn't require user input.

Using the landing page content designer, you can also leverage contextual data coming from the primary page in a subpage. [Learn more](#use-primary-page-context)-->

## フォームコンポーネントの使用 {#use-form-component}

>[!CONTEXTUALHELP]
>id="ac_lp_formfield"
>title="フォームコンポーネントフィールドの設定"
>abstract="受信者による選択内容の表示方法と送信方法をランディングページから定義します。"

>[!CONTEXTUALHELP]
>id="acw_landingpages_calltoaction"
>title="「 」ボタンをクリックした場合の動作"
>abstract="ユーザーがランディングページフォームを送信する際の動作を定義します。"

ユーザーが選択して送信できるようにランディングページから特定のコンテンツを定義するには、 **[!UICONTROL フォーム]** コンポーネント。 それには、次の手順に従います。

1. ランディングページ固有 **[!UICONTROL フォーム]** コンポーネントは、選択したテンプレートのキャンバスに既に表示されています。

   >[!NOTE]
   >
   >The **[!UICONTROL フォーム]** コンポーネントは、同じページで 1 回だけ使用できます。

1. 選択します。 The **[!UICONTROL フォームコンテンツ]** タブが右側のパレットに表示され、フォームの各種フィールドを編集できます。

   ![](assets/lp-form-component.png)

   >[!NOTE]
   >
   >次に切り替え： **[!UICONTROL スタイル]** タブを使用して、フォームコンポーネントコンテンツのスタイルをいつでも編集できます。 [詳細情報](#lp-form-styles)

1. 最初のテキストフィールドを展開します。 次から： **[!UICONTROL テキストフィールド 1]** 「 」セクションでは、フィールドタイプ、データベースのフィールド、ラベル、ユーザーがフィールドに入力する前にフィールド内に表示されるテキストを編集できます。

   ![](assets/lp-form-text-field.png)

1. 次を確認します。 **[!UICONTROL フォームフィールドを必須にする]** オプションが必要な場合は選択します。 その場合、ランディングページは、ユーザーがこのフィールドに入力した場合にのみ送信できます。

   >[!NOTE]
   >
   >必須フィールドに値が入力されていない場合は、ユーザーがページを送信する際にエラーメッセージが表示されます。

1. チェックボックスを追加します。 このチェックボックスで、データベースのサービスまたはフィールドを更新するかどうかを選択します。

   ![](assets/lp-form-checkbox.png)

   このチェックボックスでユーザーのオプトイン/オプトアウトをおこなうかどうかを定義します。 次の 2 つのオプションの中から選択します。

   * **[!UICONTROL オンにすると購読]**：ユーザーは、同意するには、チェックボックスをオンにする必要があります（オプトイン）。
   * **[!UICONTROL オンにすると購読解除]**：ユーザーは、「 」チェックボックスをオンにして同意を削除する必要があります（オプトアウト）。

1. 必要に応じて、テキストフィールドやチェックボックスを削除して追加できます。

1. 目的のチェックボックスまたはテキストフィールドをすべて追加したら、 **[!UICONTROL コールトゥアクション]** をクリックして、対応するセクションを展開します。 これにより、 **[!UICONTROL フォーム]** コンポーネント。

   ![](assets/lp-call-to-action.png)

1. 「 」ボタンをクリックした場合の動作を定義します。

   * **[!UICONTROL 確認ページ]**：ユーザーは、 **[!UICONTROL 確認]** 現在のランディングページ用のページセット。

   * **[!UICONTROL リダイレクト URL]**：ユーザーがリダイレクトされるページの URL を入力します。

1. フォームの送信時に追加の更新を行う場合は、 **[!UICONTROL その他の更新]**&#x200B;を選択します。 **[!UICONTROL オプトイン]** または **[!UICONTROL オプトアウト]**&#x200B;をクリックし、使用する E メールアドレスのみ、またはチャネルのサブスクリプションリストを更新するかを定義します。

   ![](assets/lp-form-additionnal-updates.png)

1. コンテンツを保存して、 [ランディングページのプロパティ](create-lp.md).

## ランディングページフォームスタイルの定義 {#lp-form-styles}

1. フォームコンポーネントコンテンツのスタイルを変更するには、いつでも **[!UICONTROL スタイル]** タブをクリックします。

   ![](assets/lp_designer-form-style.png)

1. The **[!UICONTROL フィールド]** 「 」セクションはデフォルトで展開され、ラベルとプレースホルダーのフォント、ラベルの位置、フィールドの背景色、フィールドの境界線など、テキストフィールドの外観を編集できます。

   ![](assets/lp_designer-form-style-fields.png)

1. を展開します。 **[!UICONTROL チェックボックス]** 「 」セクションに追加し、チェックボックスと対応するテキストの外観を定義します。 例えば、フォントファミリやサイズ、チェックボックスの境界線の色を調整できます。

   ![](assets/lp_designer-form-style-checkboxes.png)

1. を展開します。 **[!UICONTROL ボタン]** 「 」セクションを使用して、コンポーネントフォーム内のボタンの外観を変更します。 例えば、フォントの変更、境界線の追加、マウスポインターを置いたときのラベルの色の編集、ボタンの配置の調整を行うことができます。

   ![](assets/lp_designer-form-style-buttons.png)

   ボタンのラベルの色など、設定の一部をプレビューするには、 **[!UICONTROL コンテンツをシミュレート]** 」ボタンをクリックします。 ランディングページのテストの詳細を説明します [ここ](create-lp.md#test-landing-page).

1. を展開します。 **[!UICONTROL フォームレイアウト]** 「 」セクションを使用して、背景色、パディング、余白などのレイアウト設定を編集します。

   ![](assets/lp_designer-form-style-layout.png)

<!--
1. Expand the **[!UICONTROL Form error]** section to adjust the display of the error message that displays in case a problem occurs. Check the corresponding option to preview the error text on the form.

    ![](assets/lp_designer-form-error-preview.png)-->

