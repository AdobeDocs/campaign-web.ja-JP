---
title: プロファイルディメンションの作成
description: プロファイルデータに基づいてプロファイルディメンションを作成する方法を説明します。
audience: reporting
content-type: reference
level: Intermediate
exl-id: a12dc772-13c7-45ff-9fbf-3dfdd3801eae
source-git-commit: fb5bcde9c087f73bfe5724463fe280c1e494ef1f
workflow-type: ht
source-wordcount: '478'
ht-degree: 100%

---

# プロファイルディメンションの作成{#creating-a-custom-profile-dimension}

レポートは、受信者スキーマの拡張時に作成されたプロファイルデータに基づいて作成および管理することもできます。

* [手順 1：受信者スキーマを拡張する](##extend-schema)
* [手順 2：新しいカスタムフィールドをリンクする](#link-custom)
* [手順 3：プロファイルディメンションを使用して、受信者をフィルタリングする動的レポートを作成する](#create-report)

## 手順 1：受信者スキーマを拡張する {#extend-schema}

新しいプロファイルフィールドを追加するには、スキーマを拡張する必要があります。次の手順に従ってください。

1. エクスプローラーの&#x200B;**[!UICONTROL 管理]**／**[!UICONTROL 設定]**／**[!UICONTROL データスキーマ]**&#x200B;フォルダーに移動します。

   ![](assets/custom_field_1.png)

1. カスタム受信者スキーマを特定し、選択します。ビルトイン nms:recipient スキーマをまだ拡張していない場合は、[この手順](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema)を参照してください。

1. カスタムフィールドをスキーマエディターに追加します。

   例えば、受信者スキーマにロイヤルティのカスタムフィールドを追加するには、次のようにします。

   ```
   <attribute label="Loyalty" name="loyalty" type="string"/>
   ```

   ![](assets/custom_field_2.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

1. 次に、カスタム broadLogRcp スキーマを特定して選択します。ビルトイン配信ログスキーマをまだ拡張していない場合は、[この手順](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema)を参照してください。

1. 受信者スキーマと同じカスタムフィールドをスキーマエディターに追加します。

   ![](assets/custom_field_3.png)

1. 「**[!UICONTROL 保存]**」をクリックします。

1. スキーマに加えた変更を適用するには、**[!UICONTROL ツール]**／**[!UICONTROL 詳細]**／**[!UICONTROL データベース構造を更新]**&#x200B;からデータベース更新ウィザードを起動して、「データベース構造を更新」を実行します。[詳細情報](https://experienceleague.adobe.com/ja/docs/campaign/campaign-v8/developer/shemas-forms/update-database-structure)

   ![](assets/custom_field_4.png)

これで、受信者が新しいプロファイルフィールドを使用して選択する準備が整いました。

## 手順 2：新しいカスタムフィールドをリンクする {#link-custom}

>[!NOTE]
>
> 動的レポートに追加できるカスタムフィールドは、最大 20 個までです。

プロファイルフィールドを作成したら、対応する動的レポートのディメンションにこのフィールドをリンクする必要があります。

プロファイルフィールドを使用してログを拡張する前に、PII データを動的レポートに送信できるように PII ウィンドウが許可されていることを確認します。詳しくは、この[ページ](pii-agreement.md)を参照してください。

1. エクスプローラーの&#x200B;**[!UICONTROL 管理]**／**[!UICONTROL 設定]**／**[!UICONTROL データスキーマ]**／**[!UICONTROL 追加のレポートフィールド]**&#x200B;フォルダーに移動します。

   ![](assets/custom_field_5.png)

1. 「**[!UICONTROL 新規]**」をクリックして、対応する動的レポートのディメンションを作成します。

1. 「**[!UICONTROL 式を編集]**」を選択し、受信者スキーマを参照して、以前に作成したプロファイルフィールドを見つけます。

   ![](assets/custom_field_6.png)

1. 「**[!UICONTROL 終了]**」をクリックします。

1. 動的レポートに表示されるディメンション&#x200B;**[!UICONTROL ラベル]**&#x200B;を入力し、「**[!UICONTROL 保存]**」をクリックします。

   ![](assets/custom_field_7.png)

レポートで、プロファイルフィールドをプロファイルディメンションとして使用できるようになりました。プロファイルディメンションを削除するには、ディメンションを選択して&#x200B;**[!UICONTROL 削除]**&#x200B;アイコンをクリックします。

このプロファイルフィールドを使用して受信者スキーマを拡張し、カスタムディメンションを作成したので、配信で受信者のターゲティングを開始できます。

## 手順 3：プロファイルディメンションを使用して、受信者をフィルタリングする動的レポートを作成する {#create-report}

配信を送信したら、プロファイルディメンションを使用してレポートを分類できます。

1. 「**[!UICONTROL レポート]**」タブから、標準レポートを選択するか、「**[!UICONTROL 作成]**」ボタンをクリックして一から作成します。

   ![](assets/custom_field_8.png)

1. 「**[!UICONTROL ディメンション]**」カテゴリで、「**[!UICONTROL プロファイル]**」をクリックし、フリーフォームテーブルにプロファイルディメンションをドラッグ＆ドロップします。

   ![](assets/custom_field_9.png)

1. 指標をドラッグ＆ドロップして、データのフィルタリングを開始します。

1. 必要に応じて、ワークスペースにビジュアライゼーションをドラッグ＆ドロップします。

