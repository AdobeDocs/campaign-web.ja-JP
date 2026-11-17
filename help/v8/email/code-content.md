---
audience: end-user
title: 独自のメールコンテンツをコーディング
description: 独自のメールコンテンツのコーディング方法を説明します
exl-id: a387bff6-3dc8-421c-9efd-043c16694ef0
TQID: 'https://experienceleague.adobe.com/PPrenfLb4utuqvAsrSitbtZzDHcCehzrOMK4R7L2EMw'
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
source-git-commit: 7bbc2d4c383886788afc1ef83cdd27e7ec4b24ae
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 77%
---
# 独自のメールコンテンツをコーディング {#code-content}

**[!UICONTROL 独自にコーディング]**&#x200B;モードを使用して、Raw HTML をインポートしたり、メールコンテンツをコーディングしたりします。

>[!CAUTION]
>
>この方法には、HTML の知識が必要です。

>[!IMPORTANT]
>
>電子メールコンテンツでHTML `<base>` タグを使用しないでください。 セキュリティ上の理由から、このタグはサポートされておらず、コンテンツエディターでのコンテンツの読み込みを妨げる可能性があります。 代わりに、リンクと外部リソースに絶対URLを使用してください。

1. [E メールデザイナー](get-started-email-designer.md)のホームページで、「**[!UICONTROL 独自にコーディング]**」を選択します。

   ![E メールデザイナーのホームページで「独自にコーディング」オプションを示すスクリーンショット](assets/code-your-own.png){zoomable="yes"}

1. メインキャンバスに生の HTML コードを入力するかペーストします。

1. 左側のパネルを使用してパーソナライゼーション機能にアクセスします。 [詳細情報](../personalization/gs-personalization.md)

   ![左側のパネルに、パーソナライゼーションオプションを含むコードエディターを示すスクリーンショット](assets/code-editor-personalization.png){zoomable="yes"}

1. 「**[!UICONTROL コンテンツをシミュレート]**」ボタンをクリックして、テストプロファイルを使用してメッセージデザインとパーソナライゼーションをプレビューします。 [詳細情報](../preview-test/preview-test.md)

1. コードが完成したら、「**[!UICONTROL 保存して閉じる]**」をクリックし、メッセージ作成画面に戻り、メッセージを最終決定します。