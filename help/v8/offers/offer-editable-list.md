---
audience: end-user
title: 編集可能リストをオファースキーマに追加
description: カスタムコレクションリンクを、編集可能なリストとしてオファーの詳細画面に直接表示する方法について説明します。
feature: Offers
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 043cc60da1938800404964aa7e698f959ef908fd
workflow-type: ht
source-wordcount: 449
ht-degree: 100%

---

# 編集可能リストをオファースキーマに追加 {#offer-editable-list}

オファーにリンクされた一連のセグメントなど、カスタムコレクションリンクを使用して [ [!DNL nms:offer]  スキーマ](../administration/schemas.md)を拡張すると、オファーの「**[!UICONTROL カスタムオプション]**」セクションで編集可能なリストとして直接表示できます。別の画面で関連レコードを管理する代わりに、コレクションがオファーの詳細にリストとして表示され、専用のダイアログを通じてインラインで新しい関連レコードを作成できます。

>[!NOTE]
>
>この機能は現在、オファースキーマでのみ使用できます。

## コレクションリンクフィールドを追加 {#add-field}

1. カスタムコレクションを使用して [!DNL nms:offer] スキーマを拡張し、**[!UICONTROL スキーマ]**&#x200B;メニューに移動して、**[!UICONTROL マーケティングオファー]**&#x200B;スキーマを開き、「**[!UICONTROL 画面編集]**」をクリックします。[詳細情報](../administration/schemas-browse-access.md#screen-def)。

   ![画面の定義ボタンを示すスクリーンショット。](assets/offers-editable-list.png){zoomable="yes"}

1. 「**[!UICONTROL 詳細画面の設定]**」セクションで、**[!UICONTROL カスタムフィールドのリスト]**&#x200B;テーブルの上にある省略記号アイコンをクリックし、「**[!UICONTROL 属性を選択]**」を選択します。[詳細情報](../administration/schemas-custom-fields.md)。

   ![画面の定義ボタンを示すスクリーンショット。](assets/offers-editable-list-0.png){zoomable="yes"}

1. 属性を参照し、コレクションアイコンで識別される、カスタムコレクションのリンクを選択します。

   ![コレクションリンク属性を持つ属性ピッカーを示すスクリーンショット。](assets/offers-editable-list-1.png){zoomable="yes"}

   >[!NOTE]
   >
   >コレクションリンクフィールドは必須にすることはできず、サブ属性をサポートしていません。デフォルトでは、フォーム内で 2 列にまたがっています。

1. 選択内容を確認します。コレクションリンクが&#x200B;**[!UICONTROL カスタムフィールドのリスト]**&#x200B;テーブルに追加され、タイプは&#x200B;**[!UICONTROL コレクション]**&#x200B;になります。

   ![追加された属性を示すスクリーンショット。](assets/offers-editable-list-2.png){zoomable="yes"}

## コレクションの編集可能なリストの設定 {#configure-list}

1. コレクションフィールドの行にある省略記号アイコンをクリックし、「**[!UICONTROL 編集]**」を選択して、**[!UICONTROL コレクションリンク設定]**&#x200B;ダイアログを開きます。

   ![編集ボタンを示すスクリーンショット。](assets/offers-editable-list-3.png){zoomable="yes"}

1. 「**[!UICONTROL 一般]**」タブから、オプションで「**[!UICONTROL 次の場合に表示]**」条件を設定するか、「**[!UICONTROL 読み取り専用]**」を有効にします。

   ![編集画面を示すスクリーンショット。](assets/offers-editable-list-4.png){zoomable="yes"}

1. 「**[!UICONTROL 画面設定]**」タブで「**[!UICONTROL 属性を選択]**」をクリックし、新しい要素をリストに追加する際に使用する属性（例：セグメント名やカスタムフィールド）を選択します。

   ![コレクションリンク設定ダイアログの「画面設定」タブを示すスクリーンショット。](assets/offers-editable-list-5.png){zoomable="yes"}

1. 「**[!UICONTROL レイアウト]**」タブで、**[!UICONTROL 2 列にまたがる]**&#x200B;を有効または無効にします。

1. 「**[!UICONTROL 確認]**」をクリックしてから、画面定義を&#x200B;**[!UICONTROL 保存]**&#x200B;します。

## 編集可能なリストをオファーで使用 {#use-list}

1. 左側のメニューから「**オファー**」をクリックして、オファーを開きます。[詳細情報](create-offer.md#create)

   ![オファー画面を示すスクリーンショット。](assets/offers-editable-list-7.png){zoomable="yes"}

1. オファープロパティにアクセスします。コレクションは、「**カスタムオプション**」セクションにリストとして表示されます。

   ![オファーの詳細画面に表示される編集可能なリストを示すスクリーンショット。](assets/offers-editable-list-6.png){zoomable="yes"}

1. 「**[!UICONTROL 追加]**」をクリックして、設定した属性を表示し、入力して、「**[!UICONTROL 確認]**」をクリックします。新しい要素がリストに追加されます。

   同じリストに複数の要素を追加でき、オファーの詳細には複数の編集可能なリストを含めることができます。

1. 「**[!UICONTROL 保存]**」をクリックします。

<!--
Each element added through the editable list creates a new related record. For instance, adding a segment to an offer generates the following payload:

```xml
<offer ...>
  <offerSegment segmentName="..." _operation="insert"/>
</offer>
```
-->