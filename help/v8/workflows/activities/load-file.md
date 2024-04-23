---
audience: end-user
title: 「ファイルを読み込み」ワークフローアクティビティの使用
description: 「ファイルを読み込み」ワークフローアクティビティの使用方法について説明します
exl-id: 230177e2-1926-451a-8a66-0db962ada514
source-git-commit: 935fba929c26d6d7b3057ee7c24148215a04e45e
workflow-type: ht
source-wordcount: '392'
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

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetfile"
>title="「ファイルを読み込み」アクティビティのターゲットファイル"
>abstract="「ファイルを読み込み」アクティビティのターゲットファイル"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_valueremapping"
>title="「ファイルを読み込み」アクティビティの値の再マッピング"
>abstract="「ファイルを読み込み」アクティビティの値の再マッピング"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_command"
>title="「ファイルを読み込み」コマンド"
>abstract="前処理に任意のコマンドを許可するとセキュリティ上の問題があるので、セキュリティオプション XtkSecurity_Disable_Preproc を無効にして、コマンドの定義済みリストの使用を適用します。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_delete"
>title="読み込み後にファイルを削除"
>abstract="「**読み込み後にファイルを削除**」を切り替えて、ファイルの読み込み後に元のファイルをサーバーから削除します。"

「**ファイルを読み込み**」アクティビティは、「**データ管理**」アクティビティです。このアクティビティを使用して、外部ファイルに保存されるプロファイルとデータを操作します。プロファイルとデータはデータベースに追加されませんが、入力ファイル内のすべてのフィールドを[パーソナライゼーション](../../personalization/gs-personalization.md)や、プロファイルまたは他のテーブルの更新に使用できます。

>[!NOTE]
>サポートされるファイル形式は、テキスト（TXT）とコンマ区切り値（CSV）です。

このアクティビティを「[紐付け](reconciliation.md)」アクティビティと使用すると、識別されていないデータを既存のリソースにリンクできます。例えば、非標準のデータをデータベースにインポートする場合は、「**紐付け**」アクティビティの前に「**ファイルを読み込み**」アクティビティを配置できます。

## 「ファイルを読み込み」アクティビティの設定 {#load-configuration}

「**ファイルを読み込み**」アクティビティを設定するには、次の手順に従います。

1. 「**ファイルを読み込み**」アクティビティをワークフローに追加します。「**ファイルから選択**」ボタンをクリックします。

1. 使用するローカルファイルを選択します。形式は、[サンプルファイル](../../audience/file-audience.md#sample-file)と一致させる必要があります。

1. 画面の中央のセクションで、データがどのようにマッピングされるかをプレビューして確認します。

   ![](../assets/load-file.png)

1. 左パネルの「**列**」セクションを使用して、各列のデータタイプと幅を調整します。

1. 列設定の下にある「**書式設定**」セクションで、データが正しくインポートされるように外部ファイルを書式設定する方法を指定します。

1. 設定が正しければ、「**確認**」をクリックします。

## 例{#load-example}

「**紐付け**」アクティビティで使用する外部ファイルの読み込みのサンプルについては、[このセクション](reconciliation.md#reconciliation-example)を参照してください。
