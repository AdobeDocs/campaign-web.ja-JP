---
title: 最新のリリースノート
description: Campaign web ユーザーインターフェイスに含まれる新機能を確認
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: f6a1ebcb5a77798f738e2a4ac0b45454d941d7c7
workflow-type: tm+mt
source-wordcount: '1137'
ht-degree: 25%

---

# リリースノート {#latest-release}

<!--Last update: **March 19, 2024**-->

Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対するより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。したがって、これらのリリースノートは月に数回更新されます。定期的に確認してください。

## 4 月のリリースノート {#april-24-4-release}

**リリース日**: 2024 年 5 月 2 日（PT）

### 新機能 {#new-24-4}

次の機能は、4 月のリリース以降、すべてのユーザーが使用できます。

**新しいワークフローアクティビティ**

* **データを更新**  – このアクティビティを使用すると、データベース内のフィールドを一括更新できます。 データ更新をパーソナライズできるオプションがいくつかあります。 [詳細情報](../workflows/activities/update-data.md)
* **購読サービス**  – このアクティビティを使用すると、1 回のアクションで複数のプロファイルをサービスに登録またはサービスから登録解除できます。 [詳細情報](../workflows/activities/subscription-services.md)
* **ファイルを抽出**  – このアクティビティを使用すると、Adobe Campaignから別のシステムに外部ファイルとしてデータをエクスポートできます。 [詳細情報](../workflows/activities/extract-file.md)
* **ファイルを転送**  – このアクティビティを使用して、ファイルの送受信、ファイルの有無の確認、サーバー上のファイルの一覧表示を行います。 使用されるプロトコルは、サーバー間プロトコルまたは HTTP プロトコルのいずれかです。 [詳細情報](../workflows/activities/transfer-file.md)
* **テスト**  – このアクティビティを使用すると、指定した条件に基づいたトランジションを有効にできます。 [詳細情報](../workflows/activities/test.md)
* **JavaScript コード**  – このアクティビティを使用すると、ワークフローのコンテキストで JavaScript コードスニペットを実行できます。 [詳細情報](../workflows/activities/javascript-code.md)
* **外部シグナル**  – このアクティビティを使用すると、別のワークフローからのワークフローの実行や、API 呼び出しをトリガーできます。 [詳細情報](../workflows/activities/external-signal.md)
* **増分クエリ**  – このアクティビティを使用して、スケジュールに従ってデータベースに対してクエリを実行します。 このアクティビティが実行されるたびに、以前の実行結果が除外されます。これにより、新しい要素のみをターゲットにすることができます。 [詳細情報](../workflows/activities/incremental-query.md)

**リッチなプッシュ通知テンプレート**

Android を介してリッチなプッシュ通知を送信できるようになりました。 リッチプッシュ通知は、画像、インタラクティブボタン、その他のリッチメディアコンテンツなどのマルチメディア要素を組み込むことで、単純なテキストメッセージ以上の機能を持つモバイル通知の拡張形式です。 [詳細情報](../push/rich-push.md)

この機能はにあります。 **限定提供（LA）** （LA）

<!--
* **Audit Trail**

The Audit trail feature constantly records a detailed log of actions and events taking place within the Adobe Campaign instance in real-time. It offers a convenient method to access a chronological record of data, addressing queries such as: the status of workflows, the latest individuals to modify them, or the activities performed by users within the instance.
-->

### 限定提供（LA）の新機能 {#acs-24-4}

>[!AVAILABILITY]
>
>次の機能は、限定提供（LA）で提供されています。 移行するお客様に限定されています **Adobe Campaign StandardからAdobe Campaign v8 へ**、および他の環境にデプロイすることはできません。
>
>次のドキュメントページを参照してください。 [Campaign v8 へのCampaign Standardの移行](../rn/acs-migration.md) および [Campaign Standardユーザー向けの機能](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html).

* **ブランド化** -Campaign Standardに移行したユーザーは、技術管理者が 1 つまたは複数のブランドを定義して、ブランドの ID に影響を与えるパラメーターを一元化できるようになりました。 ブランドのロゴ、ランディングページのアクセス URL のドメイン、メッセージトラッキングの設定などが含まれます。これらのブランドを作成し、メッセージやランディングページにリンクさせることができます。 この設定は、テンプレートで管理されます。 [詳細情報](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html)

* **Rest API** -Campaign Standardに移行したユーザーは、Rest API を使用してAdobe Campaignとの統合を作成し、Adobe Campaignに使用するテクノロジーのパネルをインターフェイスで接続することで独自のエコシステムを構築できます。 [詳細情報](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html)

* **動的レポート** -Campaign Standardが移行したユーザーは、完全にカスタマイズ可能なリアルタイムのレポートを提供する、動的レポートにアクセスして、マーケティングアクティビティの影響を測定できます。 プロファイルデータへのアクセスを追加し、開封数やクリック数などの機能的なメールキャンペーンデータに加えて、性別、市区町村、年齢などのプロファイルディメンション別の人口統計学的分析を可能にします。 [詳細情報](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html)

* **ランディングページ** - ランディングページの次の機能強化は、Campaign Standardから移行するユーザーのみが使用できます：

   * サービスの設定時に、デフォルトの購読/購読解除ランディングページを参照できるようになりました。 メールをデザインする際に、そのランディングページへのリンクを定義すると、ランディングページフォームを送信したユーザーは、このサービスに自動的に登録または登録解除されます。 [詳細情報](../audience/manage-services.md#create-service)
   * ランディングページ設定の新しいオプションでは、匿名訪問者がランディングページにアクセスできるようになりました。 このオプションを選択解除すると、識別されたユーザーのみがフォームにアクセスして送信できます。 [詳細情報](../landing-pages/create-lp.md#create-landing-page)
   * ランディングページ設定の新しいオプションを使用すると、ランディングページの送信時に追加の内部データを保存できます。 [詳細情報](../landing-pages/create-lp.md#create-landing-page)
   * 新しいオプションを使用すると、複数のサービスでランディングページを使用し、動的にすることができます。 メールへのリンクを追加する際に、動的ランディングページを選択すると、任意のサービスを選択できます。 特定のサービスが関連付けられているランディングページを選択すると、このサービスが自動的に使用されます（別のサービスを選択することはできません）。 [詳細情報](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * ランディングページで条件付きコンテンツがサポートされるようになりました。 [詳細情報](../landing-pages/lp-content.md)

### 一般的な改善点 {#improvements-24-4}

以下の機能強化は、4 月のリリース以降、すべてのお客様が利用できます。
<!--**Workflow - Copy/Paste into another tab**: -->

* この **ファイルをロード** アクティビティが強化され、いくつかの節が追加されました。これにより、サンプルファイルのアップロード、エラーと却下の管理、アクティビティの実行後にアップロードしたファイルの削除をおこなえるようになりました。 [詳細情報](../workflows/activities/load-file.md)


* これで、 **アクティビティのコピー/貼り付け** 異なるブラウザータブから別のワークフローに。 [詳細情報](../workflows/orchestrate-activities.md#copy-activities-copy)

<!--**Workflow - Execution options**: -->

* すべてのワークフローアクティビティで、ワークフローの **実行オプション**. これにより、アクティビティの実行モードと、エラーが発生した場合の動作を定義できます。 [詳細情報](../workflows/orchestrate-activities.md#execution-options-execution)

<!-- **Workflow - Split Activity - Support Skipping Empty Transition**: -->

* の「母集団が空の場合はトランジションを有効化しない」オプション **分割アクティビティ** セグメント結果が空の場合、ワークフローを次のアクティビティに移行するかどうかを選択できます。 [詳細情報](../workflows/activities/split.md)

<!--* **Support of custom fields**-->

* **カスタムフィールド** は、Adobe Campaign コンソールを使用して標準のスキーマに追加された追加の属性です。 Campaign web ユーザーインターフェイスでは、これらのカスタムフィールドは、プロファイルやテストプロファイルの詳細など、様々な画面に表示されるようになりました。 Web ユーザーインターフェイスではカスタムフィールドを作成できませんが、表示方法を変更できるようになりました。 [詳細情報](../administration/custom-fields.md)


## 3月リリースノート {#24-3-release}

>[!AVAILABILITY]
>
>このバージョンは、[Campaign（コンソール）v8.6 リリース](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=ja)以降のすべてのユーザーが利用できます。Adobe Campaign クライアントコンソールのリリースとアップグレードについて詳しくは、[Campaign v8（コンソール）ドキュメント](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html?lang=ja){target="_blank"}を参照してください。

**リリース日**：2024年3月19～20日（PT）

### ダイレクトメールチャネル {#24-3-dm}

**ダイレクトメール**&#x200B;チャネルがワークフロー内およびスタンドアロン配信として使用できるようになりました。ダイレクトメールは、抽出ファイルを作成、カスタマイズ、生成し、ダイレクトメールプロバイダーと共有して顧客にメールを送信できるオフラインチャネルです。

### 新しい「データソースを変更」ワークフローアクティビティ {#24-3-change-data-source}

「**データソースを変更**」ターゲティングアクティビティを使用すると、ワークフローの作業用テーブルで使用するデータソースを変更できます。このアクティビティによって、様々なデータベース間でデータを管理できるようになり、パフォーマンスが向上するため、柔軟性が高まります。

### ワークフローアクティビティの機能強化の分割 {#24-3-split}

これで、を使用できます **同じテーブルにすべてのサブセットを生成** のオプション **分割** ワークフローアクティビティ：すべてのサブセットを 1 つの出力トランジションにグループ化します。

### クエリモデラー {#24-3-query-modeler}

* クエリモデラーがメールデザイナーで使用できるようになりました。これにより、条件付きコンテンツを作成する際に条件を作成できます。
* カスタム条件を作成する際に、日付タイプ属性に事前定義済みの値を使用できるようになりました。
* ダイアグラム内の新しいトランジションにオペレーターを追加できなくなりました。コンポーネントをフィルタリングしてグループ化する前に、既存のトランジションにのみ追加できます。
