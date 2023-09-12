---
audience: end-user
title: ファイルから受信者をターゲット設定する
description: 外部ファイルの受信者を使用してメールオーディエンスを作成する方法を学ぶ
badge: label="Beta"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: ed9d67c5d84826035785e9543f4ed7655aa094f1
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 75%

---

# ファイルからメールオーディエンスを読み込み {#audience-from-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_select"
>title="ファイル選択"
>abstract="アップロードするローカルファイルを選択します。サポートされる形式は TXT および CSV です。ファイル形式を、以下にリンクしたサンプルファイルに合わせます。"

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_columns"
>title="列の定義"
>abstract="ローカルファイルから挿入する列の形式を確認します。"

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_formatting"
>title="書式設定パラメーター"
>abstract="ファイルの書式設定パラメーターを確認します。"

外部ファイルから連絡先をアップロードできます。プロファイルはデータベースに追加されませんが、入力ファイル内のすべてのフィールドを[パーソナライゼーション](../personalization/gs-personalization.md)に使用できます。サポートされるファイル形式は、テキスト（TXT）とコンマ区切り値（CSV）です。

>[!CAUTION]
>
>* この機能は、**スタンドアロンメール配信**&#x200B;でのみ使用できます。ワークフローや SMS またはプッシュ配信では使用できません。
>
>* 外部ファイルからターゲット母集団を読み込む場合は、[コントロール母集団](control-group.md)を使用できません。

## ファイルをアップロード {#upload}

メールインターフェイスで直接ローカルファイルからプロファイルをターゲットにするには、次の手順に従います。

1. 既存のメール配信を開くか、[新しいメール配信を作成](../email/create-email.md)します。
1. メール配信作成ウィンドウの「**オーディエンス**」セクションで、「**オーディエンスを選択**」ボタンをクリックし、「**ファイルから選択**」オプションを選択します。

   ![](assets/select-from-file.png)

1. アップロードするローカルファイルを選択します。形式は、[サンプルファイル](#sample-file)と一致する必要があります。
1. 画面の中央のセクションで、データがどのようにマッピングされるかをプレビューして確認します。
1. **アドレスフィールド**&#x200B;ドロップダウンからメールアドレスを含む列を選択します。また、入力ファイルにブロックリストの情報がある場合は、ブロックリストの列を選択することもできます。
1. 列設定を調整し、使用可能なオプションからデータをフォーマットする方法を調整します。
1. 設定が正しければ、「**確認**」をクリックします。

メッセージコンテンツを作成およびパーソナライズする際に、[パーソナライゼーションエディター](../personalization/gs-personalization.md)で入力ファイルからフィールドを選択できます。

![](assets/select-external-perso.png)

## メールのプレビューとテスト {#test}

Campaign Web では、ファイルからアップロードされたオーディエンスを使用する際に、テスト用 E メールをプレビューして送信できます。 これを行うには、次の手順に従います。

1. コンテンツをシミュレート
1. プレビューを開きます。 「プロファイルを選択：使用するファイルからプロファイルを選択」をクリックします。
1. テストメールを送信するには、「テスト」をクリックします。
1. テストモード：配達確認のターゲットの定義
1. 2 つ目のファイルからテスト E メールのターゲットをアップロードします（または同じものを使用します）。 ファイルの形式は、アップロードされたファイルと同じです
1. ファイル形式で実行されたチェック
1. 送信をクリック

+ プレビューとテストセクションへのリンク

**質問：**
* 使用できるファイルの代替はありませんか？

## サンプルファイル {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="ファイルからのオーディエンスの読み込み"
>abstract="サポートされるファイル形式は、TXT および CSV です。 先頭行を列ヘッダーとして使用します。ファイル形式を、以下のリンクにあるサンプルファイルに合わせます。"

サポートされる形式は TXT および CSV です。先頭行は列ヘッダーです。

ファイル形式を、以下のサンプルファイルに合わせます。

```javascript
{
lastname,firstname,city,birthdate,email,denylist
Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,0
Mars,Daniel,London,17/11/1999,danny.mars@example.com,0
Smith,Clara,Roma,08/02/1979,clara.smith@example.com,0
Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,1
}
```
