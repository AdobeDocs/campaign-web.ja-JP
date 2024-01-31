---
audience: end-user
title: 紐付けワークフローアクティビティの使用
description: 紐付けワークフローアクティビティの使用方法を学ぶ
badge: label="限定提供（LA）"
exl-id: 33f2aa76-1e75-4545-805a-016c95824e09
source-git-commit: 72899742daf04a0da6e2fb3d802b7841753b8c6c
workflow-type: ht
source-wordcount: '828'
ht-degree: 100%

---

# 紐付け {#reconciliation}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation"
>title="紐付けアクティビティ"
>abstract="「**紐付け**」アクティビティは、「**ターゲティング**」アクティビティで、Adobe Campaign データベース内のデータと作業用テーブル内のデータとの間のリンクを定義できます。例えば、非標準のデータをデータベースに読み込むために、「**ファイルを読み込み**」アクティビティの後に「**紐付け**」アクティビティを配置できます。この場合、**紐付け**&#x200B;アクティビティで、Adobe Campaign データベース内のデータと外部テーブル内のデータを結ぶリンクを定義できます。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_field"
>title="紐付け選択フィールド"
>abstract="紐付け選択フィールド"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_condition"
>title="紐付け作成条件"
>abstract="紐付け作成条件"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_complement"
>title="紐付けで補集合を生成"
>abstract="紐付けで補集合を生成"

「**紐付け**」アクティビティは、「**ターゲティング**」アクティビティで、Adobe Campaign データベース内のデータと作業用テーブル内のデータ（外部ファイルから読み込まれたデータなど）との間のリンクを定義できます。

例えば、非標準のデータをデータベースに読み込むために、「**ファイルを読み込み**」アクティビティの後に「**紐付け**」アクティビティを配置できます。この場合、**紐付け**&#x200B;アクティビティで、Adobe Campaign データベース内のデータと作業用テーブル内のデータを結ぶリンクを定義できます。

## ベストプラクティス {#reconciliation-best-practices}

**エンリッチメント**&#x200B;アクティビティでは、ワークフローで処理する追加のデータを定義できますが（**エンリッチメント**&#x200B;アクティビティを使用して、複数のセットからのデータを組み合わせたり、一時リソースへのリンクを作成したりできます）、**紐付け**&#x200B;アクティビティでは、識別されていないデータを既存のリソースにリンクできます。

>[!NOTE]
>紐付け操作は、リンクされたディメンションのデータが既にデータベースに存在することを意味します。例えば、購入された商品、購入時間、商品を購入したクライアントなどを示す購入ファイルを読み込む場合、商品とクライアントはデータベースに既に存在している必要があります。

## 紐付けアクティビティの設定 {#reconciliation-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting"
>title="ターゲティングディメンション"
>abstract="新しいターゲティングディメンションを選択します。ディメンションを使用すると、ターゲット母集団（受信者、アプリのサブスクライバー、オペレーター、サブスクライバーなど）を定義できます。デフォルトでは、現在のターゲティングディメンションが選択されています。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_rules"
>title="紐付けルール"
>abstract="重複排除 - 重複に使用する紐付けフィールドを選択します。1 つまたは複数の紐付け条件を使用できます。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting_selection"
>title="ターゲティングディメンションの選択"
>abstract="紐付けするインバウンドデータのターゲティングディメンションを選択します。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/gs-audiences-recipients.html?lang=ja#targeting-dimensions" text="ターゲティングディメンション"

>[!CONTEXTUALHELP]
>id="acw_orchestration_keep_unreconciled_data"
>title="紐付けられていないデータの保持"
>abstract="デフォルトでは、紐付けされていないデータは、アウトバウンドトランジションに保持され、後で使用するために作業用テーブルで使用できます。紐付けされていないデータを削除するには、「**紐付けされていないデータを保持**」オプションを非アクティブ化します。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_attribute"
>title="紐付け属性"
>abstract="データの紐付けに使用する属性を選択し、「確認」をクリックします。"

**紐付け**&#x200B;アクティビティを設定するには、次の手順に従います。

1. **紐付け**&#x200B;アクティビティをワークフローにドラッグ＆ドロップします。このアクティビティは、Adobe Campaign から直接ターゲティングディメンションを受け取らない母集団を含むトランジションに従って追加する必要があります。

1. 新しいターゲティングディメンションを選択します。ディメンションを使用すると、ターゲット母集団（受信者、アプリのサブスクライバー、オペレーター、サブスクライバーなど）を定義できます。[詳しくは、ターゲティングディメンションを参照してください](../../audience/about-recipients.md#targeting-dimensions)。

1. 紐付けに使用するフィールドを選択します。1 つまたは複数の紐付け条件を使用できます。

   1. 属性を使用してデータを紐付けするには、「**単純な属性**」オプションを選択します。「**ソース**」フィールドには、入力トランジションで使用可能な、紐付けされるフィールドがリストされます。「**宛先**」フィールドは、選択したターゲティングディメンションのフィールドに対応します。データは、ソースと宛先が等しい場合に紐付けされます。例えば、メールアドレスに基づいてプロファイルの重複を排除するには、「**メール**」フィールドを選択します。

      別の紐付け条件を追加するには、「**ルールを追加**」ボタンをクリックします。複数の結合条件が指定される場合、データを相互にリンクさせるには、すべての条件が検証される必要があります。

      ![](../assets/workflow-reconciliation-criteria.png)

   1. 他の属性を使用してデータを紐付けするには、「**高度な紐付け条件**」オプションを選択します。その後、クエリモデラーを使用して独自の紐付け条件を作成できます。クエリモデラーの使用方法については、[この節](../../query/query-modeler-overview.md)を参照してください。

1. 「**フィルターを作成**」ボタンを使用して、データをフィルタリングして紐付けできます。これにより、「[クエリモデラー](../../query/query-modeler-overview.md)」を使用してカスタム条件を作成できます。

デフォルトでは、紐付けされていないデータは、アウトバウンドトランジションに保持され、後で使用するために作業用テーブルで使用できます。紐付けされていないデータを削除するには、「**紐付けされていないデータを保持**」オプションを非アクティブ化します。

## 例 {#reconciliation-example}

次の例は、新しいクライアントを含むインポート済みのファイルから直接プロファイルのオーディエンスを作成するワークフローを示しています。このワークフローは、次のアクティビティで構成されています。

ワークフローは、次のように設計されています。

![](../assets/workflow-reconciliation-sample-1.0.png)


これは、次のアクティビティを使用して作成されます。

* 「[ファイル読み込み](load-file.md)」アクティビティは、外部ツールから抽出されたプロファイルデータが含まれるファイルをアップロードします。

  次に例を示します。

  ```
  lastname;firstname;email;birthdate;
  JACKMAN;Megan;megan.jackman@testmail.com;07/08/1975;
  PHILLIPS;Edward;phillips@testmail.com;09/03/1986;
  WEAVER;Justin;justin_w@testmail.com;11/15/1990;
  MARTIN;Babe;babeth_martin@testmail.net;11/25/1964;
  REESE;Richard;rreese@testmail.com;02/08/1987;
  ```

* 「**紐付け**」アクティビティ：紐付け条件として「**メール**」フィールドと「**生年月日**」フィールドを使用して、受信データをプロファイルとして識別します。

  ![](../assets/workflow-reconciliation-sample-1.1.png)

* 「[オーディエンスを保存](save-audience.md)」アクティビティ：これらの更新に基づいて新しいオーディエンスを作成します。また、特定のオーディエンスを作成または更新する必要がない場合は、「**オーディエンスを保存**」アクティビティを「**終了**」アクティビティに置き換えることもできます。受信者プロファイルは、ワークフローを実行すると常に更新されます。


## 互換性 {#reconciliation-compat}

「**紐付け**」アクティビティは、クライアントコンソールには存在しません。紐付けオプションを有効にしてクライアントコンソールで作成されたすべての「**エンリッチメント**」アクティビティは、Campaign web UI で「**紐付け**」アクティビティとして表示されます。
