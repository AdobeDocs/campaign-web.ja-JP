---
title: 条件付きコンテンツを作成
description: Adobe Campaign web UI でコンテンツをパーソナライズするための条件を定義する方法について説明します
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Beta"
exl-id: 101ad23b-7ea5-42c7-9249-7c14febe6eb7
source-git-commit: 97e2d37d0a91e50b516f2fa0b6d5559f89b6c096
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 99%

---

# 条件付きコンテンツをビルド{#add-conditions}

>[!CONTEXTUALHELP]
>id="acw_conditional_content"
>title="条件付きコンテンツを追加"
>abstract="条件付きコンテンツフィールドを設定して、受信者のプロファイルデータに基づいて高度な動的パーソナライゼーションを作成します。特定の条件が満たされた場合に、メッセージコンテンツ内のテキストブロック、リンク、件名、画像を置き換えることができます。"

## 条件付きコンテンツの概要 {#gs}

条件付きコンテンツは、受信者のプロファイルに基づいて動的パーソナライゼーションを作成できる強力な機能で、特定の条件が満たされた場合にテキストブロックと画像を自動的に置き換えます。この機能により、キャンペーンを新たな高みに引き上げて、高度にターゲティングされ、パーソナライズされたエクスペリエンスをオーディエンスに提供できます。

条件付きコンテンツフィールドを設定することで、例えば受信者のプロファイルに基づいて高度な動的パーソナライゼーションを作成できます。特定の条件が満たされた場合に、メッセージコンテンツ内のテキストブロック、リンク、件名、画像を置き換えることができます。例えば、Adobe Campaign データベースの「性別」フィールドの値に従って「Mr」または「Mrs」を表示したり、受信者の優先言語に基づいて別のリンクを含めたりできます。

条件付きコンテンツを作成するには、**式エディター**&#x200B;で特定のヘルパー関数を使用して条件を作成する必要があります。この方法は、すべての配信チャネルで、件名、メールリンク、テキスト／ボタンコンテンツコンポーネントなど、式エディターにアクセスできる任意のフィールドで使用できます。[式エディターにアクセスする方法を学ぶ](gs-personalization.md/#access)

<!--In addition to the expression editor, you can leverage a dedicated **conditional content builder** when designing an email that allows you to build conditions using profile attributes only. [Learn how to create conditional content in emails](#condition-condition-builder)-->

## 式エディターでの条件を作成 {#condition-perso-editor}

式エディターを使用して配信の条件付きコンテンツを定義するには、次の手順に従います。この例では、受信者の言語（フランス語または英語）に基づく条件付きコンテンツを作成します。

1. 配信を開き、コンテンツ編集セクションに移動します。

1. 条件付きコンテンツを追加するフィールドを見つけます。例えば、SMS メッセージに条件付きコンテンツを追加できます。

1. フィールドの横にある「**[!UICONTROL パーソナライゼーションダイアログを開く]**」アイコンをクリックして、式エディターを開きます。

   ![](assets/open-perso-editor-sms.png)

1. パーソナライゼーションエディターで、左側にある&#x200B;**[!UICONTROL ヘルパー関数]**&#x200B;メニューを開きます。

1. 条件の作成を開始するには、**If** 関数の横にある「+」アイコンをクリックします。中央の画面に次の行が追加されます：`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } %>`

   * `<FIELD>` を、受信者の言語などのパーソナライゼーションフィールド `recipient.language` に置き換えます。
   * `<VALUE>` を満たす値に置き換えます。例：`'French'`
   * `Ìnsert content here` を、指定した条件を満たすプロファイルに表示するコンテンツに置き換えます。

     ![](assets/condition-sample1.png){width="800" align="center"}

1. 受信者が条件を満たさない場合に表示するコンテンツを指定します。これを行うには、**else** ヘルパー関数を使用します。

   1. 式終了タグ `%>` の前にカーソルを置き、**Else** 関数の横にある `+` をクリックします。

   1. `Ìnsert content here` を、if 関数の条件を満たさないプロファイルに表示するコンテンツに置き換えます。

   ![](assets/condition-sample2.png){width="800" align="center"}

   また、**else if** ヘルパー関数を使用して、複数のコンテンツバリアントを含む条件を作成することもできます。例えば、次の式では、受信者の言語に応じてメッセージの 3 つのバリアントが表示されます。

   ![](assets/condition-sample3.png){width="800" align="center"}

   >[!NOTE]
   >
   >ヘルパー関数を追加するたびに、関数の前後に開始タグ（`<%`）と終了タグ（`%>`）が自動的に追加されます。
   >
   >式内に「Else」ヘルパー関数を追加した後の例を次に示します。
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } <% else { %> Insert content here<% } %>%>`
   >
   >構文エラーを避けるために、これらのタグを削除する必要があります。この例では、**else** 関数タグを削除した後の修正された式を次に示します。
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } else { %> Insert content here<% } %>`

1. 条件の準備が整ったら、コンテンツを保存し、コンテンツをシミュレートしてそのレンダリングを確認できます。

<!--SECTION REMOVED FOR LA > CONDITIONAL CONTENT NOT AVAILABLE ANYMORE FROM THE DEDICATED MENU IN THE EMAIL DESIGNER. ONLY THE EXPRESSION EDITOR IS AVAILABLE FOR NOW

## Create conditional content in emails {#condition-condition-builder}

Conditional content in emails can be created in two ways:
* In the expression editor by building a condition with helper functions,
* In a dedicated conditional content builder that is accessible when designing an email.

Detailed information on how to create conditions using the expression editor is available [here](#condition-perso-editor). The following section provides step-by-step instructions on how to create conditions using the email designer's conditional content capability. In this example, we want to create an email message with multiple variants based on the recipients' language. Follow these steps:

1. Create or open an email delivery, edit its content, and click the **[!UICONTROL Edit email body]** button to open the email designing workspace.

1. Select a content component and click the **[!UICONTROL Enable conditional content]** icon.

    ![](assets/condition-email-enable.png){width="800" align="center"}

1. The **[!UICONTROL Conditional Content]** pane opens on the left-hand side of the screen. In this pane, you can create multiple variants of the selected content component using conditions.

1. Configure your first variant. Hover over **[!UICONTROL Variant - 1]** in the **[!UICONTROL Conditional Content]** pane and click the **[!UICONTROL Add condition]** icon.

1. A query modeler appears. Use profile attributes to create the condition for the first variant of the message and click **[!UICONTROL Confirm]**. In this example, we are creating a rule targeting recipients whose language is 'French'.

    ![](assets/condition-email-rule.png){width="800" align="center"}

1. The rule is now associated to the variant. For better readability, we recommend renaming the variant by clicking the ellipsis menu.

1. Configure how the component should display if the rule is met when sending the message. In this example, we want to display the text in French if it is the recipient's preferred language.

    ![](assets/condition-email-variant1.png){width="800" align="center"}

1. Add as many variants as needed for the content component. You can switch between the variants at any time to check how the content component will display based on their conditional rules.

    >[!NOTE]
    >If none of the rules defined in the variants are met when sending the message, the content component will display the content defined in the **[!UICONTROL Default variant]** from the **[!UICONTROL Conditional Content]** pane.
-->