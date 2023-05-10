---
audience: end-user
title: ファイルからの受信者のインポート
description: 外部ファイルから受信者をインポートする方法
badge: label="Alpha" type="Positive"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: ef8418294540ee0462725cdaf6824ba7ee4d9b59
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 97%

---

# ファイルからの受信者のインポート {#audience-from-file}

テキストファイル（TXT）またはコンマ区切り値ファイル（CSV）をアップロードして、配信インターフェイスから連絡先を追加または更新できます。それにより、プロファイルはデータベースに追加されます。

>[!NOTE]
>
>また、インポートワークフローを作成して、複数のプロファイルを追加または更新することもできます。


インターフェイスで直接ローカルファイルからプロファイルを追加するには、次の手順に従います。

1. 配信作成ウィンドウで、「**オーディエンスを選択**」ボタンをクリックし、「**ファイルから選択**」オプションを選択します。
1. アップロードするローカルファイルを選択します。
1. 列設定とデータのフォーマット方法を定義します。列をスキップするには、「**列を無視**」切替スイッチを使用します。
1. 画面の中央のセクションで、データがどのようにマッピングされるかをプレビューします。
1. 設定が正しければ、「**確認**」をクリックします。

メッセージコンテンツを作成およびパーソナライズする際に、パーソナライゼーションエディターで入力ファイルからフィールドを選択できます。

## サンプルファイル {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="サンプルファイル"
>abstract="サポートされているファイル形式：txt、csv。 先頭行を列ヘッダーとして使用します。"


```json
{
lastname,firstname,birthdate,email,crmID
Smith,Hayden,23/05/1989,hayden.smith@example.com,124365
Mars,Daniel,17/11/1987,dannymars@example.com,123545
Smith,Clara,08/02/1989,clara.smith@example.com,124567
Durance,Allison,15/12/1978,allison.durance@example.com,120987
}
```
