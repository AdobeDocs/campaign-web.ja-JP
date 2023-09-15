---
audience: end-user
title: メールコンテンツの読み込み
description: メールコンテンツの読み込み方法を学ぶ
exl-id: ef9c8e6f-f422-404e-9ebb-a89d1bd45e7f
badge: label="Beta"
source-git-commit: ed12d289c1180fe8705d2c143bd9dce4ed96e313
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 58%

---

# メールコンテンツの読み込み {#existing-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_import_content"
>title="既存のメールコンテンツの使用"
>abstract="メールデザイナーを使用すると、既存の HTML コンテンツをインポートできます。このコンテンツは、スタイルシートが組み込まれた HTML ファイルや、HTML ファイル、スタイルシート（.css）および画像を含んだ .zip フォルダーにすることができます。"

E メールデザイナーで既存のHTMLコンテンツを読み込むことができます。 このコンテンツには次のようなものがあります。

* スタイルシートが組み込まれた **HTML ファイル**
* HTML ファイル、スタイルシート（.css）および画像を含んだ **.zip フォルダー**

  >[!NOTE]
  >
  >.zip ファイル構造に制約はありません。 ただし、.zip フォルダーのツリー構造内に合わせて、相対参照を指定する必要があります。

HTML コンテンツを含んだファイルを読み込むには、次の手順に従います。

1. [メールデザイナー](get-started-email-designer.md)のホームページで、「**[!UICONTROL HTML をインポート]**」を選択します。

   ![](assets/html-import.png)

1. HTML コンテンツを含む HTML または .zip ファイルをドラッグ＆ドロップし、「**[!UICONTROL 読み込み]**」をクリックします。

1. HTMLコンテンツがアップロードされると、コンテンツは **[!UICONTROL 互換性モード]**.

   このモードでは、テキストのパーソナライズ、リンクの追加、コンテンツへのアセットの組み込みのみが可能です。

   ![](assets/html-imported.png)

1. E メールデザイナーのコンテンツコンポーネントを活用するには、 **[!UICONTROL HTML変換器]** タブをクリックし、 **[!UICONTROL 変換]**.

   ![](assets/html-imported-2.png)

   >[!NOTE]
   >
   > の使用 `<table>` タグをHTMLファイルの最初のレイヤーとして使用すると、最上部のレイヤータグの背景や幅の設定など、スタイルが失われる場合があります。

1. これで、E メールデザイナー機能を使用して、必要に応じて読み込んだファイルをパーソナライズできます [詳細情報](content-components.md).

