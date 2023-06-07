---
title: Campaign でのコンテンツのパーソナライズ
description: Adobe Campaign web UI でのコンテンツのパーソナライズ方法について説明します
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Alpha" type="Positive"
source-git-commit: 573f0bbf396f795029c5e34b436521cb1c7b80a5
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 100%

---


# ビルトインコンテンツブロック {#ootb-content-blocks}

ビルトインコンテンツブロックは次のとおりです。

* **[!UICONTROL Adobe Campaign で有効化]**：「Adobe Campaign で有効化」ロゴを挿入します。
* **[!UICONTROL 固有名詞の書式設定関数]**：JavaScript の **[!UICONTROL toSmartCase]** 関数を生成します。この関数は各単語の最初の文字をすべて大文字に変更します。
* **[!UICONTROL 挨拶]**：受信者の姓名の後にコンマを付けた挨拶文を挿入します。例：「こんにちは、John Doe。」
* **[!UICONTROL ロゴの挿入]**：インスタンス設定で定義されているロゴを挿入します。
* **[!UICONTROL ミラーページへのリンク]**：[ミラーページ](../content/mirror-page.md)へのリンクを挿入します。デフォルトの形式は、「このメッセージが正しく表示されない場合は、ここをクリックしてください」です。
* **[!UICONTROL ミラーページの URL]**：ミラーページの URL を挿入し、配信デザイナーがリンクを確認できるようにします。
* **[!UICONTROL 単一モードのオファー許可 URL]**：オファーを&#x200B;**[!UICONTROL 許可済み]**&#x200B;に設定できる URL を挿入します。（このブロックは、インタラクションモジュールが有効な場合に使用できます）
* **[!UICONTROL 登録の確認]**：購読を確認できるリンクを挿入します。
* **[!UICONTROL 登録リンク]**：購読リンクを挿入します。このリンクは、インスタンス設定で定義されています。デフォルトの内容は「登録するには、ここをクリックしてください。」です。
* **[!UICONTROL 登録リンク（リファラーを含む）]**：購読リンクを挿入し、訪問者と配信を識別できるようにします。このリンクは、インスタンス設定で定義されています。
* **[!UICONTROL 登録ページ URL]**：購読 URL を挿入します。
* **[!UICONTROL コンテンツメールのスタイル]**&#x200B;および&#x200B;**[!UICONTROL 通知スタイル]**：定義済みの HTML スタイルでメールを書式設定するコードを生成します。
* **[!UICONTROL 登録解除リンク]**：すべての配信を購読解除（ブロックリスト登録）できるリンクを挿入します。関連付けられているデフォルトのコンテンツは、「このメッセージが届いたのは、お客様が&#x200B;***組織名***&#x200B;または関連会社と連絡を取ったことがあるからです。***組織名***&#x200B;からメッセージを受け取らないようにするには、ここをクリックしてください。」です。
