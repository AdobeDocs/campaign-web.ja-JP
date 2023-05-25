---
audience: end-user
title: ファイルからの受信者のターゲティング
description: 外部ファイルの受信者を使用して電子メールオーディエンスを作成する方法を説明します
badge: label="Alpha" type="Positive"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: fd9a5724aa9b97bffc6d143853742e0107bd3483
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 20%

---

# ファイルから受信者を読み込む {#audience-from-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_select"
>title="ファイル選択"
>abstract="アップロードするローカルファイルを選択します。サポートされる形式は TXT および CSV です。 ファイル形式を、以下にリンクしたサンプルファイルに合わせます。"

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_columns"
>title="列の定義"
>abstract="ローカルファイルから挿入する列の形式を確認します。"

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_formatting"
>title="書式設定パラメーター"
>abstract="ファイルの形式設定パラメーターを確認します。"

外部ファイルから連絡先をアップロードできます。 この機能は、E メール配信でのみ使用できます。 サポートされるファイル形式は次のとおりです。テキスト (TXT) およびコンマ区切り値 (CSV)。 プロファイルはデータベースに追加されませんが、入力ファイル内のすべてのフィールドをパーソナライゼーションに使用できます。

>[!NOTE]
>
>インポートワークフローを作成して、データベース内の複数のプロファイルを追加または更新できます。 詳細情報


インターフェイスから直接ローカルファイルからプロファイルをターゲットにするには、次の手順に従います。

1. E メール配信作成ウィンドウで、 **対象ユーザ** セクションで、 **オーディエンスを選択** ボタンをクリックし、 **ファイルから選択** オプション。

   ![](assets/select-from-file.png)

1. アップロードするローカルファイルを選択します。
1. 画面の中央のセクションで、データのマッピング方法をプレビューして確認します。
1. 次の中から E メールアドレスを含む列を選択します： **住所フィールド** 」ドロップダウンリストから選択できます。 入力ファイルにこのような情報が含まブロックリストれている場合は、「列を」を選択することもできます。
1. 列の設定を調整し、使用可能なオプションからデータをフォーマットする方法を調整します。
1. 設定が正しければ、「**確認**」をクリックします。

メッセージコンテンツを作成およびパーソナライズする際に、パーソナライゼーションエディターで入力ファイルからフィールドを選択できます。

![](assets/select-external-perso.png)

>[!CAUTION]
>
>次を使用することはできません： [コントロール母集団](control-group.md) 外部ファイルからターゲット母集団を読み込む際に使用します。

## サンプルファイル {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="サンプルファイル"
>abstract="サポートされているファイル形式：txt、csv。 先頭行を列ヘッダーとして使用します。"


```json
{
lastname,firstname,city,birthdate,email,denylist
Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,0
Mars,Daniel,London,17/11/1999,dannymars@example.com,0
Smith,Clara,Roma,08/02/1979,clara.smith@example.com,0
Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,1
}
```
