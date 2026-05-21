---
audience: end-user
title: ミラーページへのリンクの追加
description: ミラーページへのリンクを追加および管理する方法を学ぶ
exl-id: 0c22357f-0465-4fdc-833e-5fda5805fe42
TQID: https://experienceleague.adobe.com/iigr3vwibRH-qRbWaTXszxTuJqgdFJG6QEC1T9Z487s
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: beb7a3c1-66ab-4786-b879-7621375b3c40
  - id: cc72dcf1-72e1-48cc-b434-e7c27d62d67c
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 5a231f1dc49379d1be5d36e1732660111f851649
workflow-type: tm+mt
source-wordcount: 397
ht-degree: 100%

---

# ミラーページ {#mirror-page}

ミラーページは、メールのオンラインバージョンです。 メールマーケティングでは、ミラーページへのリンクを追加することをお勧めします。 例えば、インボックスでメールを表示する際にレンダリングの問題や壊れた画像が発生した場合に、ユーザーはメールのミラーページにアクセスできます。 アクセシビリティ上の理由から、またはソーシャル共有を促進するために、オンラインバージョンを提供することもお勧めします。

Adobe Campaign で生成されるミラーページには、すべてのパーソナライゼーションデータが含まれています。

![メール内のミラーリンクの例](assets/mirror-page-link.png){width="600" align="left"}

## ミラーページへのリンクの追加 {#link-to-mirror-page}

Adobe Campaign では、専用の&#x200B;**パーソナライゼーションブロック**&#x200B;を使用して、メールのコンテンツにミラーページへのリンクを挿入します。 ビルトインの「**ミラーページへのリンク**」パーソナライゼーションブロックでは、`<%@ include view='MirrorPage' %>` コードをメールのコンテンツに挿入します。

メールにミラーページへのリンクを追加するには、次の手順に従います。

1. 要素（テキストまたは画像）を選択し、コンテキストツールバーから「**[!UICONTROL リンクを挿入]**」をクリックします。

   ![「リンクを挿入」オプションを示すコンテキストツールバー](assets/message-tracking-mirror-page.png){zoomable="yes"}

1. 「**[!UICONTROL パーソナライゼーションを追加]**」アイコンを選択して、パーソナライゼーションメニューにアクセスします。

   ![Adobe Campaign のパーソナライゼーションメニュー](assets/message-tracking-mirror-page_2.png){zoomable="yes"}

1. **[!UICONTROL フラグメント]**&#x200B;メニューから、「**[!UICONTROL ミラーページ URL]**」を選択し、「**[!UICONTROL 追加]**」をクリックします。 [詳しくは、式フラグメントの使用方法を参照してください](../content/use-expression-fragments.md)

   ![フラグメントメニューのミラーページ URL オプション](assets/message-tracking-mirror-page_3.png){zoomable="yes"}

ミラーページが自動的に作成されます。

メールを送信すると、ミラーページのリンクをクリックした受信者には、メールのコンテンツがデフォルトの web ブラウザーに表示されます。

デフォルトでは、ミラーページの保持期間は **60 日**&#x200B;です。 この期間を過ぎると、ミラーページは使用できなくなります。

>[!CAUTION]
>
>* ミラーページのリンクは自動生成され、編集できません。 これらには、元のメールのレンダリングに必要な、暗号化およびパーソナライズされたデータがすべて含まれています。 値が大きいパーソナライズ属性を使用すると、長いミラーページの URL が生成される可能性があり、URL の長さが最大長の web ブラウザーでリンクが機能しなくなる可能性があります。
>
>* テストプロファイルに送信される本配信前確認では、ミラーページへのリンクはアクティブになっていません。 最終的なメッセージでのみアクティブになります。

## ミラーページの生成 {#mirror-page-generation}

デフォルトでは、メールコンテンツが空でなく、ミラーページへのリンク（ミラーリンクとも呼ばれる）が含まれている場合、Adobe Campaign は自動的にミラーページを生成します。

配信プロパティで使用可能なオプションを通じて、メールのミラーページの生成モードを制御します。 [詳細情報](../advanced-settings/delivery-settings.md#mirror)