---
audience: end-user
title: ファイル読み込みワークフローアクティビティの使用
description: ファイル読み込みワークフローアクティビティの使用方法を説明します
badge: label="限定提供（LA）"
source-git-commit: 88daf84e617595a80c5cd3fd536969618f0fdcf5
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 39%

---

# ファイルを読み込み {#load-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile"
>title="ファイルを読み込みアクティビティ"
>abstract="The **ファイルを読み込み** アクティビティは **データ管理** アクティビティ。 このアクティビティを使用して、外部ファイルに保存されたデータを操作します。"

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


The **ファイルを読み込み** アクティビティは **データ管理** アクティビティ。 このアクティビティを使用して、外部ファイルに保存されたプロファイルとデータを操作します。 プロファイルとデータはデータベースに追加されませんが、入力ファイル内のすべてのフィールドは [パーソナライゼーション](../../personalization/gs-personalization.md)またはを使用して、プロファイルやその他のテーブルを更新します。


>[!NOTE]
>サポートされるファイル形式は、テキスト（TXT）とコンマ区切り値（CSV）です。


このアクティビティは、 [紐づけ](reconciliation.md) 「 」アクティビティを使用して、識別されていないデータを既存のリソースにリンクします。 例えば、 **ファイルを読み込み** アクティビティは、 **紐づけ** アクティビティを設定します。


## 「ファイル読み込み」アクティビティの設定 {#load-configuration}

次の手順に従って、 **ファイルを読み込み** アクティビティ：


1. 次をドラッグ&amp;ドロップ： **ファイルを読み込み** アクティビティをワークフローに追加します。 次をクリック： **ファイルから選択** 」ボタンをクリックします。
1. 使用するローカルファイルを選択します。形式は、次のように整列する必要があります。 [サンプルファイル](../../audience/file-audience.md#sample-file).
1. 画面の中央のセクションで、データがどのようにマッピングされるかをプレビューして確認します。
1. 列設定を調整し、使用可能なオプションからデータをフォーマットする方法を調整します。
1. 設定が正しければ、「**確認**」をクリックします。

## 例{#load-example}

外部ファイルの読み込み例は、 **紐づけ** アクティビティ [この節](reconciliation.md#example).