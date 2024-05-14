---
title: 最新のリリースノート
description: Campaign web ユーザーインターフェイスに含まれる新機能を確認
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: d50dfc4ea433fa48301707b40164e2fdf9fa64fd
workflow-type: tm+mt
source-wordcount: '1185'
ht-degree: 100%

---

# リリースノート {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="リリースノート"
>abstract="Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対するより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。これにより、Campaign リリースノートは月に数回更新され、最新の機能、改善点、修正が含まれます。定期的に確認することをお勧めします。"

<!--Last update: **March 19, 2024**-->

Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対するより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。したがって、これらのリリースノートは月に数回更新されます。定期的に確認してください。

## 4月リリースノート {#april-24-4-release}

**リリース日**：2024年5月2日（PT）

### 新機能 {#new-24-4}

次の機能は、4月のリリース以降、すべてのユーザーが使用できます。

**新しいワークフローアクティビティ**

* **データを更新** - このアクティビティを使用すると、データベースのフィールドを一括更新できます。いくつかのオプションを使用して、データ更新をパーソナライズできます。[詳細情報](../workflows/activities/update-data.md)
* **購読サービス** - このアクティビティを使用すると、1 回のアクションで複数のプロファイルをサービスに購読またはサービスから登録解除できます。[詳細情報](../workflows/activities/subscription-services.md)
* **ファイルを抽出** - このアクティビティを使用すると、Adobe Campaign から別のシステムに外部ファイルとしてデータをエクスポートできます。[詳細情報](../workflows/activities/extract-file.md)
* **ファイルを転送** - このアクティビティを使用すると、ファイルの送受信、ファイルの有無の確認、サーバー上のファイルをリストにすることができます。使用されるプロトコルは、サーバー間プロトコルまたは HTTP プロトコルのいずれかです。[詳細情報](../workflows/activities/transfer-file.md)
* **テスト** - このアクティビティを使用すると、指定した条件に基づいたトランジションを有効にできます。[詳細情報](../workflows/activities/test.md)
* **JavaScript コード** - このアクティビティを使用すると、ワークフローのコンテキストで JavaScript コードスニペットを実行できます。[詳細情報](../workflows/activities/javascript-code.md)
* **外部シグナル** - このアクティビティを使用すると、別のワークフローからのワークフローの実行や、API 呼び出しをトリガーできます。[詳細情報](../workflows/activities/external-signal.md)
* **増分クエリ** - このアクティビティを使用すると、スケジュールに従ってデータベースに対してクエリを実行できます。このアクティビティが実行されるたびに、以前の実行結果が除外されます。これにより、新しい要素だけをターゲットにすることができます。[詳細情報](../workflows/activities/incremental-query.md)

**リッチプッシュ通知テンプレート**

Android 経由でリッチプッシュ通知を送信できるようになりました。リッチプッシュ通知は、画像、インタラクティブボタン、その他のリッチメディアコンテンツなどのマルチメディア要素を組み込むことで、単純なテキストメッセージを超えたモバイル通知の拡張形式です。[詳細情報](../push/rich-push.md)

この機能は、**限定提供**（LA）です。

<!--
* **Audit Trail**

The Audit trail feature constantly records a detailed log of actions and events taking place within the Adobe Campaign instance in real-time. It offers a convenient method to access a chronological record of data, addressing queries such as: the status of workflows, the latest individuals to modify them, or the activities performed by users within the instance.
-->

### 限定提供の新機能 {#acs-24-4}

>[!AVAILABILITY]
>
>次の機能は、限定提供（LA）です。**Adobe Campaign Standard から Adobe Campaign v8** に移行するお客様に限定され、他の環境にはデプロイできません。
>
>ドキュメントページの [Campaign v8 への Campaign Standard の移行](../rn/acs-migration.md)および [Campaign Standard ユーザー向けの機能](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=ja)を参照してください。

* **ブランディング** - Campaign Standard で移行したユーザーは、技術管理者が 1 つまたは複数のブランドを定義して、ブランドの ID に影響を与えるパラメーターを一元化できるようになりました。ブランドのロゴ、ランディングページのアクセス URL のドメイン、メッセージトラッキングの設定などが含まれます。これらのブランドを作成して、メッセージやランディングページにリンクできます。こうした設定はテンプレートで管理されます。[詳細情報](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html?lang=ja)

* **Rest API** - Campaign Standard に移行したユーザーは、Rest API を使用して Adobe Campaign との統合を作成し、Adobe Campaign と使用するテクノロジーのパネルを連携させて独自のエコシステムを構築できます。[詳細情報](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html?lang=ja)

* **動的レポート** - Campaign Standard に移行したユーザーは、完全にカスタマイズ可能なリアルタイムのレポートを提供する、動的レポートにアクセスして、マーケティングアクティビティの影響を測定できます。プロファイルデータへのアクセスが追加され、開封数やクリック数などの機能的なメールキャンペーンデータに加えて、性別、市区町村、年齢などのプロファイルディメンション別のデモグラフィック分析を可能にします。[詳細情報](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html?lang=ja)

* **ランディングページ** - ランディング ページの次の機能強化は、Campaign Standard から移行するユーザーのみが利用できます。

   * サービスの設定時に、デフォルトの購読／購読解除のランディングページを参照できるようになりました。メールのデザイン時に、そのランディングページへのリンクを定義すると、ランディングページフォームを送信したユーザーは、このサービスに自動的に購読または登録解除されます。[詳細情報](../audience/manage-services.md#create-service)
   * ランディングページ設定の新しいオプションでは、匿名訪問者がランディングページにアクセスできます。このオプションを選択解除すると、識別されたユーザーのみがフォームにアクセスして送信できます。[詳細情報](../landing-pages/create-lp.md#create-landing-page)
   * ランディングページ設定の新しいオプションでは、ランディングページの送信時に追加の内部データを保存できます。[詳細情報](../landing-pages/create-lp.md#create-landing-page)
   * 新しいオプションでは、複数のサービスにランディングページを使用し、動的にすることができます。メールへのリンクの追加時に、動的ランディングページを選択すると、任意のサービスを選択できます。特定のサービスが関連付けられているランディングページを選択すると、このサービスが自動的に使用されます（別のサービスは選択できません）。[詳細情報](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * ランディングページで条件付きコンテンツがサポートされるようになりました。[詳細情報](../landing-pages/lp-content.md)

### 一般的な改善点 {#improvements-24-4}

以下の機能強化は、4月のリリース以降、すべてのお客様が利用できます。
<!--**Workflow - Copy/Paste into another tab**: -->

* 「**ファイルを読み込み**」アクティビティが強化され、いくつかのセクションが追加されました。これにより、サンプルファイルのアップロード、エラーや拒否の管理、アクティビティの実行後にアップロードされたファイルの削除を行うことができます。[詳細情報](../workflows/activities/load-file.md)


* 別のブラウザータブで、ワークフローから別のワークフローに&#x200B;**アクティビティをコピー＆ペースト**&#x200B;できるようになりました。[詳細情報](../workflows/orchestrate-activities.md#copy-activities-copy)

<!--**Workflow - Execution options**: -->

* すべてのワークフローアクティビティで、**実行オプション**&#x200B;を管理できるようになりました。これにより、アクティビティの実行モードとエラー時の動作を定義できます。[詳細情報](../workflows/orchestrate-activities.md#execution-options-execution)

<!-- **Workflow - Split Activity - Support Skipping Empty Transition**: -->

* **「分割」アクティビティ**&#x200B;の「母集団が空の場合はトランジションをアクティブ化しない」オプションを使用すると、セグメント結果が空の場合にワークフローを次のアクティビティに移行するかどうかを選択できます。[詳細情報](../workflows/activities/split.md)

<!--* **Support of custom fields**-->

* **カスタムフィールド**&#x200B;は、Adobe Campaign コンソールを通じて標準スキーマに追加される追加属性です。Campaign web ユーザーインターフェイスでは、これらのカスタムフィールドが、プロファイルやテストプロファイルの詳細など、様々な画面に表示されるようになりました。Web ユーザーインターフェイスでは、カスタムフィールドを作成できませんが、表示方法を変更できるようになりました。[詳細情報](../administration/custom-fields.md)


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

「**分割**」ワークフローアクティビティの「**同じテーブル内のすべてのサブセットを生成**」オプションを使用して、すべてのサブセットを 1 つの出力トランジションにグループ化できるようになりました。

### クエリモデラー {#24-3-query-modeler}

* クエリモデラーがメールデザイナーで使用できるようになりました。条件付きコンテンツを作成する際に、条件を作成できます。
* カスタム条件を作成する際に、日付タイプの属性に定義済みの値を使用できるようになりました。
* ダイアグラム内の新しいトランジションにオペレーターを追加できなくなりました。コンポーネントをフィルタリングしてグループ化する前にのみ、既存のトランジションに追加できます。
