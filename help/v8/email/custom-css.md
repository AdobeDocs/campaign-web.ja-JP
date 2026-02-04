---
title: メールコンテンツへのカスタム CSS の追加
description: Adobe Campaign の E メールデザイナー内でメールコンテンツにカスタム CSS を直接追加する方法について説明します
feature: Email Design
topic: Content Management
role: User
level: Intermediate
keywords: CSS, エディター, 概要, メール
exl-id: 7969b656-8130-49cf-9c85-d80bd74b285a
source-git-commit: 8f8c1645952c6a7f73c083573e18d2b04e9d9ac7
workflow-type: ht
source-wordcount: '692'
ht-degree: 100%

---

# メールコンテンツへのカスタム CSS の追加 {#email-metadata}

>[!CONTEXTUALHELP]
>id="ac_edition_css"
>title="独自の CSS を入力"
>abstract="コンテンツの外観に対する柔軟性と制御を高めるために、E メールデザイナー内で直接カスタム CSS を追加して、高度で特定のスタイルを適用できます。"

メールをデザインする際に、[E メールデザイナー](get-started-email-designer.md)内で独自のカスタム CSS を直接追加できます。この機能により、コンテンツの外観に対する柔軟性と制御を高めるのに、高度で特定のスタイルを適用できます。

## カスタム CSS の定義 {#define-custom-css}

メールコンテンツにカスタム CSS を追加するには、次の手順に従います。

1. 1 つ以上の[コンポーネント](content-components.md)を追加して、E メールデザイナーにコンテンツが定義されていることを確認します。

1. 左側の&#x200B;**[!UICONTROL ナビゲーションツリー]**&#x200B;または右側のパネルの上部にある「**[!UICONTROL 本文]**」を選択します。「**[!UICONTROL CSS スタイル]**」セクションが右側に表示されます。

   ![「カスタム CSS を追加」ボタンを選択](assets/email-body-css-styles.png){width="85%"}

   >[!NOTE]
   >
   >「**[!UICONTROL CSS スタイル]**」セクションは、コンテンツが既にエディターに存在する場合にのみ使用できます。

1. 「**[!UICONTROL カスタム CSS を追加]**」ボタンをクリックします。

   >[!NOTE]
   >
   >「**[!UICONTROL カスタム CSS を追加]**」ボタンは、「**[!UICONTROL 本文]**」を選択した場合にのみ使用できます。ただし、コンテンツ内のすべてのコンポーネントにカスタム CSS スタイルを適用できます。

1. ポップアップされる専用のテキスト領域に CSS コードを入力します。カスタム CSS が有効で、適切な構文に従っていることを確認します。[詳細情報](#use-valid-css)

   ![専用のテキスト領域にカスタム CSS を入力](assets/email-body-custom-css.png){width="65%"}

1. カスタム CSS を保存し、カスタム CSS がコンテンツに正しく適用されていることを確認します。該当しない場合は、[トラブルシューティング](#troubleshooting)の節を確認してください。

   ![「カスタム CSS を追加」ボタンを選択](assets/email-body-custom-css-applied.png){width="85%"}

1. すべてのコンテンツを削除すると、セクションが非表示になり、以前に定義したカスタム CSS は適用されなくなります。

1. コンテンツをエディターに追加し直すと、「**[!UICONTROL CSS スタイル]**」セクションが再表示されます。カスタム CSS が再度適用されます。

## 有効な CSS の使用の確認 {#use-valid-css}

**[!UICONTROL カスタム CSS を追加]**&#x200B;テキスト領域に有効な CSS 文字列を入力できます。適切な形式の CSS がコンテンツにすぐに適用されます。

>[!CAUTION]
>
>ユーザーは、カスタム CSS のセキュリティに対して責任があります。CSS によって脆弱性が発生したり、既存のコンテンツと競合したりしないことを確認します。
>
>意図せずコンテンツのレイアウトや機能を損なう可能性がある CSS の使用は回避します。

+++ CSS のサンプル

有効な CSS の例を以下に示します。

```css
.acr-component[data-component-id="form"] {
  display: flex;
  justify-content: center;
  background: none;
}

.acr-Form {
  width: 100%;
  padding: 20px 100px;
  border-spacing: 0px 8px;
  box-sizing: border-box;
  margin: 0;
}

.acr-Form .spectrum-FieldLabel {
  width: 20%;
}

.acr-Form.spectrum-Form--labelsAbove .spectrum-FieldLabel,
.acr-Form [data-form-item="checkbox"] .spectrum-FieldLabel {
  width: auto;
}

.acr-Form .spectrum-Textfield {
  width: 100%;
}

#acr-form-error,
#acr-form-confirmation {
  width: 100%;
  padding: var(--spectrum-global-dimension-static-size-500);
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: center;
  gap: var(--spectrum-global-dimension-static-size-200);
}

.spectrum-Form-item.is-required .spectrum-FieldLabel:after{
  content: '*';
  font-size: 1.25rem;
  margin-left: 5px;
  position: absolute;
}

/* Error field placeholder */
.spectrum-HelpText {
  display: none !important;
}

.spectrum-HelpText.is-invalid,
.is-invalid ~ .spectrum-HelpText {
  display: flex !important;
}
```

```css
@media only screen and (min-width: 600px) {
  .acr-paragraph-1 {
    width: 100% !important;
  }
}
```

+++

無効な CSS を入力すると、CSS を保存できないことを示すエラーメッセージが表示されます。無効な CSS の例を以下に示します。

+++ 無効な CSS のサンプル

`<style>` タグの使用は許可されていません。

```html
<style type="text/css">
  .acr-Form {
    width: 100%;
    padding: 20px 100px;
    border-spacing: 0px 8px;
    box-sizing: border-box;
    margin: 0;
  }
</style>
```

中括弧の欠落などの無効な構文は許可されていません。

```css
body {
  background: red;
```

+++

## 技術的実装 {#implementation}

次の例に示すように、カスタム CSS は、`data-name="global-custom"` 属性を持つ `<style>` タグの一部として `<head>` セクションの末尾に追加されます。これにより、カスタムスタイルがコンテンツにグローバルに適用されます。

+++ 詳しくは、サンプルを参照してください 

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="content-version" content="3.3.31">
    <meta name="x-apple-disable-message-reformatting">
    <meta name="viewport" content="width=device-width,initial-scale=1.0">
    <style data-name="default" type="text/css">
      td { padding: 0; }
      th { font-weight: normal; }
    </style>
    <style data-name="grid" type="text/css">
      .acr-grid-table { width: 100%; }
    </style>
    <style data-name="acr-theme" type="text/css" data-theme="default" data-variant="0">
      body { margin: 0; font-family: Arial; }
    </style>
    <style data-name="media-default-max-width-500px" type="text/css">
      @media screen and (max-width: 500px) {
        body { width: 100% !important; }
      }
    </style>
    <style data-name="global-custom" type="text/css">
      /* Add you custom CSS here */
    </style>
  </head>
  <body>
    <!-- Minimal content -->
  </body>
</html>
```

+++

カスタム CSS は、E メールデザイナーの&#x200B;**[!UICONTROL 設定]**&#x200B;パネルでは解釈または検証されません。これは完全に独立しており、「**[!UICONTROL カスタム CSS を追加]**」オプションを通じてのみ変更できます。

<!--
If the `global-custom` style tag has the attribute `data-disabled` set to `true`, the custom CSS will not be applied. 

+++ See sample

For example:

```html
<style data-name="global-custom" type="text/css" data-disabled="true"> body: { color: red; } </style>
```

+++
-->

## ガードレール - インポートしたコンテンツ

E メールデザイナーにインポートしたコンテンツでカスタム CSS を使用する場合は、次の点を考慮します。

* CSS を含む外部 HTML コンテンツをインポートする場合、そのコンテンツを変換しない限り、**[!UICONTROL 互換性モード]**&#x200B;になり、「**[!UICONTROL CSS スタイル]**」セクションは使用できません。[既存のコンテンツのインポートの詳細情報](existing-content.md)

* 「**[!UICONTROL カスタム CSS を追加]**」オプションを通じて適用された CSS を含む、E メールデザイナーで作成したコンテンツをインポートする場合、以前に適用された CSS は同じオプションから表示および編集できます。

<!--
* If importing content created with the Email Designer with CSS applied externally, the CSS code previously applied cannot be accessed within the **[!UICONTROL Add custom CSS]** pop-up window, but you can still override it with new custom CSS.-->

## トラブルシューティング {#troubleshooting}

カスタム CSS が適用されない場合は、以下のオプションを考慮します。

* CSS が有効で、構文エラー（中括弧の欠落、プロパティ名の誤りなど）がないことを確認します。[詳細情報](#use-valid-css)

* CSS が `data-name="global-custom"` 属性を持つ `<style>` タグに追加されていることを確認します。

* `global-custom` スタイルのタグに属性 `data-disabled` が `true` に設定されているかどうかを確認します。該当する場合、カスタム CSS は適用されません。

  +++例：

  ```html
  <style data-name="global-custom" type="text/css" data-disabled="true"> body: { color: red; } </style>
  ```

  +++

* CSS が他の CSS ルールによって上書きされていないことを確認します。

   * ブラウザーの開発者ツールを使用して、コンテンツを調べ、CSS が正しいセレクターをターゲットにしていることを確認します。

   * 優先されるようにするには、宣言に `!important` を追加することを考慮します。

     +++ 例：

     ```css
     .acr-Form {
       background: red !important;
     }
     ```

     +++
