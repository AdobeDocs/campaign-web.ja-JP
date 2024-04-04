---
audience: end-user
title: ファイルからメールオーディエンスを読み込み
description: 外部ファイルからプロファイルを読み込んでメールオーディエンスを作成する方法を学ぶ
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: b166d06215e06d6426ab9ce9a757fcc041810df9
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

Adobe Campaign Web ユーザーインターフェイスを使用すると、外部ファイルに保存されたプロファイルをターゲットに設定できます。 プロファイルが読み込まれると、入力ファイルのすべてのフィールドを使用して配信をパーソナライズできます [コンテンツをパーソナライズする方法を説明します。](../personalization/personalize.md).

入力ファイルのプロファイルは、データベースに追加されません。 これらは読み込まれ、この特定のスタンドアロン E メール配信でのみ使用できます。

>[!NOTE]
>
>このページでは、スタンドアロンの E メール配信を作成する際に、ファイルから外部プロファイルを読み込む方法について説明します。 ワークフローのコンテキストでファイルからデータを読み込むには、 [このページ](../workflows/activities/load-file.md).

## 必読 {#must-read}

* この機能は、で使用できます。 **電子メール配信** のみ。
* サポートされるファイル形式は、テキスト（TXT）とコンマ区切り値（CSV）です。
* 外部ファイルからターゲット母集団を読み込む場合は、[コントロール母集団](control-group.md)を使用できません。

## 入力ファイルを選択して設定 {#upload}

E メール内のファイルからプロファイルをターゲットにするには、次の手順に従います。

1. 既存のメール配信を開くか、[新しいメール配信を作成](../email/create-email.md)します。
1. Adobe Analytics の **対象ユーザ** セクションで、 **オーディエンスを選択** ボタンを選択し、 **ファイルから選択**.

   ![](assets/select-from-file.png){zoomable=&quot;yes&quot;}

1. 読み込むローカルファイルを選択します。 ファイル形式は、 [サンプルファイル](#sample-file).
1. 画面の中央のセクションで、データがどのようにマッピングされるかをプレビューして確認します。

   ![](assets/select-from-file-map.png)

1. からの電子メールアドレスを格納する列を指定します。 **住所フィールド** 」ドロップダウンリストから選択できます。 また、入力ファイルにブロックリストの情報がある場合は、ブロックリストの列を選択することもできます。
1. 列の設定を調整し、使用可能なオプションからデータをフォーマットする方法を調整します。
1. 設定が正しければ、「**確認**」をクリックします。

メッセージコンテンツを作成する際に、入力ファイルのフィールドを活用してパーソナライゼーションを追加できます。 [コンテンツをパーソナライズする方法を学ぶ](../personalization/personalize.md)

![](assets/select-external-perso.png){zoomable=&quot;yes&quot;}

## サンプルファイル {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="ファイルからオーディエンスを読み込み"
>abstract="サポートされるファイル形式は TXT および CSV です。先頭行を列ヘッダーとして使用します。ファイル形式を、以下のリンクにあるサンプルファイルに合わせます。"

配信内のプロファイルをターゲットにする外部ファイルを読み込む際に、入力ファイルが以下の推奨事項と一致していることを確認します。

* サポートされる形式は TXT および CSV です。
* ファイルの最初の行は、列ヘッダーです。
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

   ![](assets/file-upload-preview.png){zoomable=&quot;yes&quot;}

1. 本配信前確認を送信するには、「**[!UICONTROL 本配信前確認を送信]**」ボタンをクリックします。

1. 「**[!UICONTROL 配達確認プロファイルをアップロード]**」ボタンをクリックし、プルーフの受信者を含む .txt ファイルまたは .csv ファイルを選択します。 

   >[!CAUTION]
   >
   >ファイル形式がオーディエンスのアップロードに使用した形式と一致していることを確認してください。形式エラーがあると警告が表示されます。

1. 本配信前確認プロファイルを追加し、本配信前確認を送信する準備が整ったら、「**[!UICONTROL 本配信前確認を送信]**」ボタンをクリックし、送信を確定します。

   ![](assets/file-upload-test.png){zoomable=&quot;yes&quot;}

1. 「**[!UICONTROL 本配信前確認を表示]**」ボタンを使用して、いつでも本配信前確認の送信を監視できます。[詳しくは、本配信前確認の監視を参照してください](../preview-test/test-deliveries.md#access-test-deliveries)
