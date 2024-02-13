---
audience: end-user
title: 「ファイルを読み込み」ワークフローアクティビティの使用
description: 「ファイルを読み込み」ワークフローアクティビティの使用方法について説明します
exl-id: 230177e2-1926-451a-8a66-0db962ada514
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 100%

---

# ファイルを読み込み {#load-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile"
>title="ファイルを読み込みアクティビティ"
>abstract="「**ファイルを読み込み**」アクティビティは、「**データ管理**」アクティビティです。このアクティビティを使用して、外部ファイルに保存されるデータを操作します。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_samplefile"
>title="サンプルファイル"
>abstract="サンプルファイル"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_nameofthefile"
>title="ファイルの名前"
>abstract="ファイルの名前"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetdb"
>title="ターゲットデータベース"
>abstract="ターゲットデータベース"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_rejectmgt"
>title="「ファイルを読み込み」アクティビティの管理を却下"
>abstract="「ファイルを読み込み」アクティビティの管理を却下"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition"
>title="管理のアウトバウンドトランジションを却下"
>abstract="管理のアウトバウンドトランジションを却下"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition_reject"
>title="却下に対する管理のアウトバウンドトランジションを却下"
>abstract="却下に対する管理のアウトバウンドトランジションを却下"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_formatting"
>title="「ファイルを読み込み」アクティビティの書式設定"
>abstract="「ファイルを読み込み」アクティビティの書式設定"

「**ファイルを読み込み**」アクティビティは、「**データ管理**」アクティビティです。このアクティビティを使用して、外部ファイルに保存されるプロファイルとデータを操作します。プロファイルとデータはデータベースに追加されませんが、入力ファイル内のすべてのフィールドを[パーソナライゼーション](../../personalization/gs-personalization.md)や、プロファイルまたは他のテーブルの更新に使用できます。

>[!NOTE]
>サポートされるファイル形式は、テキスト（TXT）とコンマ区切り値（CSV）です。

このアクティビティを「[紐付け](reconciliation.md)」アクティビティと使用すると、識別されていないデータを既存のリソースにリンクできます。例えば、非標準のデータをデータベースにインポートする場合は、「**紐付け**」アクティビティの前に「**ファイルを読み込み**」アクティビティを配置できます。

## 「ファイルを読み込み」アクティビティの設定 {#load-configuration}

「**ファイルを読み込み**」アクティビティを設定するには、次の手順に従います。

1. ワークフローに「**ファイルを読み込み**」アクティビティをドラッグ＆ドロップします。「**ファイルから選択**」ボタンをクリックします。

1. 使用するローカルファイルを選択します。形式は、[サンプルファイル](../../audience/file-audience.md#sample-file)と一致させる必要があります。

1. 画面の中央のセクションで、データがどのようにマッピングされるかをプレビューして確認します。

   ![](../assets/load-file.png)

1. 左パネルの「**列**」セクションを使用して、各列のデータタイプと幅を調整します。

1. 列設定の下にある「**書式設定**」セクションで、データが正しくインポートされるように外部ファイルを書式設定する方法を指定します。

1. 設定が正しければ、「**確認**」をクリックします。

## 例{#load-example}

「**紐付け**」アクティビティで使用する外部ファイルの読み込みのサンプルについては、[このセクション](reconciliation.md#reconciliation-example)を参照してください。
