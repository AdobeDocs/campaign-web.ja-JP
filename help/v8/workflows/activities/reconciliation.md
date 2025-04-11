---
audience: end-user
title: 紐付けワークフローアクティビティの使用
description: 紐付けワークフローアクティビティの使用方法を学ぶ
exl-id: 33f2aa76-1e75-4545-805a-016c95824e09
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '824'
ht-degree: 41%

---

# 紐付け {#reconciliation}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation"
>title="紐付けアクティビティ"
>abstract="**紐付け** アクティビティは、Adobe Campaign データベースのデータとワークテーブルのデータ間のリンクを定義する **ターゲティング** アクティビティです。 例えば、非標準のデータをデータベースに読み込むために、「**ファイルを読み込み**」アクティビティの後に「**紐付け**」アクティビティを配置できます。この場合、**紐付け** アクティビティは、Adobe Campaign データベース内のデータと外部テーブル内のデータ間のリンクを定義します。"

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

**紐付け** アクティビティは、Adobe Campaign データベース内のデータと作業表内のデータ（外部ファイルから読み込まれたデータなど）間のリンクを定義する **ターゲティング** アクティビティです。

例えば、非標準のデータをデータベースに読み込むために、「**ファイルを読み込み**」アクティビティの後に「**紐付け**」アクティビティを配置できます。この場合、「紐付け **アクティビティは** Adobe Campaign データベース内のデータとワークテーブル内のデータ間のリンクを定義します。

## ベストプラクティス {#reconciliation-best-practices}

**エンリッチメント** アクティビティは、ワークフローで処理する追加データを定義しますが（複数のセットからのデータの結合や一時的なリソースへのリンクの作成など）、**紐付け** アクティビティは、識別されていないデータを既存のリソースにリンクします。

>[!NOTE]
>紐付け操作を行うには、リンクされたディメンションのデータがデータベースに既に存在する必要があります。 例えば、購入された製品、時刻、クライアントを示す購入ファイルをインポートする場合、製品とクライアントがデータベース内に既に存在している必要があります。

## 紐付けアクティビティの設定 {#reconciliation-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting"
>title="ターゲティングディメンション"
>abstract="新しいターゲティングディメンションを選択します。ディメンションは、ターゲット母集団（受信者、アプリの購読者、オペレーター、購読者など）を定義します。 デフォルトでは、現在のターゲティングディメンションが選択されています。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_rules"
>title="紐付けルール"
>abstract="重複排除の紐付けルールを選択します。 属性を使用するには、「**単純な属性**」オプションを選択し、ソースフィールドと宛先フィールドを選択します。クエリモデラーを使用して独自の紐付け条件を作成するには、「**高度な紐付け条件**」オプションを選択します。"
>additional-url="https://experienceleague.adobe.com/ja/docs/campaign-web/v8/query-database/query-modeler-overview" text="クエリモデラーの操作"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting_selection"
>title="ターゲティングディメンションの選択"
>abstract="紐付けするインバウンドデータのターゲティングディメンションを選択します。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/gs-audiences-recipients.html?lang=ja#targeting-dimensions" text="ターゲティングディメンション"

>[!CONTEXTUALHELP]
>id="acw_orchestration_keep_unreconciled_data"
>title="紐付けられていないデータの保持"
>abstract="デフォルトでは、紐付けされていないデータはアウトバウンドトランジションに保持され、今後の使用のためにワークテーブルで使用できます。 紐付けられていないデータを削除するには、「**紐付けられていないデータを保存** オプションを非アクティブにします。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_attribute"
>title="紐付け属性"
>abstract="データの紐付けに使用する属性を選択し、「確認」をクリックします。"

**紐付け**&#x200B;アクティビティを設定するには、次の手順に従います。

1. **紐付け** アクティビティをワークフローに追加します。 このアクティビティは、ターゲティングディメンションがAdobe Campaignから直接取得されない母集団を含むトランジションの後に続きます。

1. 新しいターゲティングディメンションを選択します。ディメンションは、ターゲット母集団（受信者、アプリの購読者、オペレーター、購読者など）を定義します。 [詳しくは、ターゲティングディメンションを参照してください](../../audience/about-recipients.md#targeting-dimensions)。

1. 紐付けに使用するフィールドを選択します。1 つまたは複数の紐付け条件を使用できます。

   1. 属性を使用してデータを紐付けするには、「**単純な属性**」オプションを選択します。**Source** フィールドには、入力トランジションで使用可能な、紐付けするフィールドが一覧表示されます。 「**宛先**」フィールドは、選択したターゲティングディメンションのフィールドに対応します。ソースと宛先が等しい場合、データは紐付けされます。 例えば、メールアドレスに基づいてプロファイルの重複を排除するには、「**メール**」フィールドを選択します。

      別の紐付け条件を追加するには、「**ルールを追加**」ボタンをクリックします。 複数の結合条件を指定する場合は、データをリンクするためにすべての条件を検証する必要があります。

      ![ 紐付け条件の例 ](../assets/workflow-reconciliation-criteria.png)

   1. 他の属性を使用してデータを紐付けするには、「**高度な紐付け条件**」オプションを選択します。その後、クエリモデラーを使用して独自の紐付け条件を作成できます。[詳しくは、クエリモデラーの操作方法を参照してください](../../query/query-modeler-overview.md)。

1. 「**フィルターを作成**」ボタンを使用して、紐付けるデータをフィルターします。 これにより、クエリモデラーを使用してカスタム条件を作成できます。[詳しくは、クエリモデラーの操作方法を参照してください](../../query/query-modeler-overview.md)。

デフォルトでは、紐付けされていないデータはアウトバウンドトランジションに保持され、今後の使用のためにワークテーブルで使用できます。 紐付けられていないデータを削除するには、「**紐付けられていないデータを保存** オプションを非アクティブにします。

## 例 {#reconciliation-example}

次の例は、新しいクライアントを含むインポート済みのファイルから直接プロファイルのオーディエンスを作成するワークフローを示しています。これには、次のアクティビティが含まれます。

ワークフローは、次のように設計されています。

![ ワークフローの例 ](../assets/workflow-reconciliation-sample-1.0.png)

これは、次のアクティビティを使用して作成されます。

* [ ファイルを読み込み ](load-file.md) アクティビティは、外部ツールから抽出されたプロファイルデータを含むファイルをアップロードします。

  例：

  ```
  lastname;firstname;email;birthdate;
  JACKMAN;Megan;megan.jackman@testmail.com;07/08/1975;
  PHILLIPS;Edward;phillips@testmail.com;09/03/1986;
  WEAVER;Justin;justin_w@testmail.com;11/15/1990;
  MARTIN;Babe;babeth_martin@testmail.net;11/25/1964;
  REESE;Richard;rreese@testmail.com;02/08/1987;
  ```

* **紐付け** アクティビティは、「電子メール **** フィールドと **生年月日** フィールドを紐付け条件として使用して、受信データをプロファイルとして識別します。

  ![ 紐付けアクティビティの例 ](../assets/workflow-reconciliation-sample-1.1.png)

* [ オーディエンスを保存 ](save-audience.md) アクティビティは、これらの更新に基づいて新しいオーディエンスを作成します。 また、特定のオーディエンスを作成または更新する必要がない場合は、**オーディエンスを保存** アクティビティを **終了** アクティビティに置き換えることもできます。 受信者プロファイルは、ワークフローを実行すると常に更新されます。

## 互換性 {#reconciliation-compat}

「**紐付け**」アクティビティは、クライアントコンソールには存在しません。紐付けオプションを有効にしてクライアントコンソールで作成したすべての **エンリッチメント** アクティビティは、Campaign web ユーザーインターフェイスに **紐付け** アクティビティとして表示されます。