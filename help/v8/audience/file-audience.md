---
audience: end-user
title: ファイルからの受信者のターゲティング
description: 外部ファイルの受信者を使用して電子メールオーディエンスを作成する方法を説明します
badge: label="Alpha" type="Positive"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: f60f0e34dc5d85808c208223d83d234e22a41c34
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 11%

---

# ファイルから電子メールオーディエンスを読み込む {#audience-from-file}

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

外部ファイルから連絡先をアップロードできます。 プロファイルはデータベースに追加されませんが、入力ファイル内のすべてのフィールドが [パーソナライズ](../personalization/gs-personalization.md). サポートされるファイル形式は次のとおりです。テキスト (TXT) およびコンマ区切り値 (CSV)。

>[!CAUTION]
>
>* この機能は、次の場合にのみ使用できます。 **スタンドアロンの E メール配信**. ワークフローや SMS 配信やプッシュ配信では使用できません。
>
>* 次を使用することはできません： [コントロール母集団](control-group.md) 外部ファイルからターゲット母集団を読み込む際に使用します。



電子メールインターフェイスから直接ローカルファイルからプロファイルをターゲットにするには、次の手順に従います。

1. 既存の E メール配信を開く、または [新しい e メール配信の作成](../email/create-email.md).
1. E メール配信作成ウィンドウで、 **対象ユーザ** セクションで、 **オーディエンスを選択** ボタンをクリックし、 **ファイルから選択** オプション。

   ![](assets/select-from-file.png)

1. アップロードするローカルファイルを選択します。形式は、 [サンプルファイル](#sample-file).
1. 画面の中央のセクションで、データのマッピング方法をプレビューして確認します。
1. 次の中から E メールアドレスを含む列を選択します： **住所フィールド** 」ドロップダウンリストから選択できます。 入力ファイルにこのような情報が含まブロックリストれている場合は、「列を」を選択することもできます。
1. 列の設定を調整し、使用可能なオプションからデータをフォーマットする方法を調整します。
1. 設定が正しければ、「**確認**」をクリックします。

メッセージコンテンツを作成およびパーソナライズする際に、 [パーソナライゼーションエディター](../personalization/gs-personalization.md).

![](assets/select-external-perso.png)


## サンプルファイル {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="サンプルファイル"
>abstract="サポートされているファイル形式：txt、csv。 先頭行を列ヘッダーとして使用します。"

サポートされる形式は TXT および CSV です。 最初の行は列ヘッダーです。

ファイル形式を以下のサンプルファイルに合わせます。

```javascript
{
lastname,firstname,city,birthdate,email,denylist
Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,0
Mars,Daniel,London,17/11/1999,danny.mars@example.com,0
Smith,Clara,Roma,08/02/1979,clara.smith@example.com,0
Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,1
}
```
