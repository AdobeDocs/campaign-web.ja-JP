---
audience: end-user
title: ファイルからメールオーディエンスを読み込み
description: 外部ファイルからプロファイルを読み込んでメールオーディエンスを作成する方法を学ぶ
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: a0da65d8facedb3730947eb969e362a367e4d317
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# ファイルからメールオーディエンスを読み込み {#audience-from-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_select"
>title="ファイル選択"
>abstract="アップロードするローカルファイルを選択します。サポートされる形式は TXT および CSV です。ファイル形式を、以下にリンクしたサンプルファイルに合わせます。"

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_columns"
>title="列の定義"
>abstract="外部ファイルの列の形式を確認します。"

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_formatting"
>title="書式設定パラメーター"
>abstract="データが正しくインポートされるように外部ファイルの書式設定を指定します。"

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_preview"
>title="ファイルをプレビュー"
>abstract="外部ファイルの列のプレビューを確認します。この画面には、最大 30 個のレコードのみが表示されます。"

Adobe Campaign web ユーザーインターフェイスを使用すると、外部ファイルに保存されているプロファイルをターゲットにすることができます。プロファイルを読み込むと、入力ファイルのすべてのフィールドを配信のパーソナライズに使用できます（[詳しくは、コンテンツのパーソナライズ方法を参照してください](../personalization/personalize.md)）。

入力ファイルのプロファイルは、データベースに追加されません。これらは読み込まれ、この特定のスタンドアロンメール配信にのみ使用できます。

>[!NOTE]
>
>このページでは、スタンドアロンのメール配信を作成する際にファイルから外部プロファイルを読み込む方法について説明します。ワークフローのコンテキスト内のファイルからデータを読み込むには、[このページ](../workflows/activities/load-file.md)を参照してください。

## 必読 {#must-read}

* この機能は、**メール配信**&#x200B;でのみ使用できます。
* サポートされるファイル形式は、テキスト（TXT）とコンマ区切り値（CSV）です。
* 外部ファイルからターゲット母集団を読み込む場合は、[コントロール母集団](control-group.md)を使用できません。

## 入力ファイルを選択して設定 {#upload}

メール内のファイルからプロファイルをターゲットにするには、次の手順に従います。

1. 既存のメール配信を開くか、[新しいメール配信を作成](../email/create-email.md)します。
1. 「**オーディエンス**」セクションで、「**オーディエンスを選択**」ボタンをクリックし、「**ファイルから選択**」を選択します。

   ![](assets/select-from-file.png){zoomable="yes"}

1. 読み込むローカルファイルを選択します。ファイル形式は、[サンプルファイル](#sample-file)と一致する必要があります。
1. 画面の中央のセクションで、データがどのようにマッピングされるかをプレビューして確認します。

   ![](assets/select-from-file-map.png)

1. **アドレスフィールド**&#x200B;ドロップダウンリストからメールアドレスを含む列を指定します。また、入力ファイルにブロックリストの情報がある場合は、ブロックリストの列を選択することもできます。
1. 列設定を調整し、使用可能なオプションからデータをフォーマットする方法を調整します。
1. 設定が正しければ、「**確認**」をクリックします。

メッセージコンテンツを作成する際に、入力ファイルのフィールドを活用してパーソナライゼーションを追加できます。[コンテンツをパーソナライズする方法について説明します。](../personalization/personalize.md)

![](assets/select-external-perso.png){zoomable="yes"}

## サンプルファイル {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="ファイルからオーディエンスを読み込み"
>abstract="サポートされるファイル形式は TXT および CSV です。先頭行を列ヘッダーとして使用します。ファイル形式を、以下のリンクにあるサンプルファイルに合わせます。"

外部ファイルを配信のターゲットプロファイルに読み込む際は、入力ファイルが以下の推奨事項と一致していることを確認します。

* サポートされる形式は TXT および CSV です。
* ファイルの先頭行は、列ヘッダーです。
* ファイル形式を、以下のサンプルファイルに合わせます。

  ```javascript
  {
  lastname,firstname,city,birthdate,email,denylist
  Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,0
  Mars,Daniel,London,17/11/1999,danny.mars@example.com,0
  Smith,Clara,Roma,08/02/1979,clara.smith@example.com,0
  Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,1
  }
  ```

## メールのプレビューとテスト {#test}

Campaign web では、ファイルからアップロードされたオーディエンスを使用する際に、本配信前確認をプレビューして送信できます。これを行うには、次の手順に従います。

1. 配信コンテンツ編集画面で「**[!UICONTROL コンテンツをシミュレートボタン]**」をクリックし、「**[!UICONTROL テストプロファイルを追加]**」ボタンをクリックします。

1. アップロードされたファイルに含まれるプロファイルが表示されます。コンテンツのプレビューに使用するプロファイルを選択し、「**[!UICONTROL 選択]**」をクリックします。

1. 配信コンテンツのプレビューが、画面の右側のパネルに表示されます。パーソナライズされた要素は、左側のパネルで選択したプロファイルのデータに置き換えられます。[配信コンテンツのプレビューの詳細情報](../preview-test/preview-content.md)

   ![](assets/file-upload-preview.png){zoomable="yes"}

1. 本配信前確認を送信するには、「**[!UICONTROL 本配信前確認を送信]**」ボタンをクリックします。

1. 「**[!UICONTROL 配達確認プロファイルをアップロード]**」ボタンをクリックし、プルーフの受信者を含む .txt ファイルまたは .csv ファイルを選択します。 

   >[!CAUTION]
   >
   >ファイル形式がオーディエンスのアップロードに使用した形式と一致していることを確認してください。形式エラーがあると警告が表示されます。

1. 本配信前確認プロファイルを追加し、本配信前確認を送信する準備が整ったら、「**[!UICONTROL 本配信前確認を送信]**」ボタンをクリックし、送信を確定します。

   ![](assets/file-upload-test.png){zoomable="yes"}

1. 「**[!UICONTROL 本配信前確認を表示]**」ボタンを使用して、いつでも本配信前確認の送信を監視できます。[詳しくは、本配信前確認の監視を参照してください](../preview-test/test-deliveries.md#access-test-deliveries)
