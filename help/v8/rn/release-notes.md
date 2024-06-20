---
title: Campaign v8 web ユーザーインターフェイスリリースノート
description: 最新の Campaign web ユーザーインターフェイスリリースで提供される新機能について説明します
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: bb61fdb34fecb4131d4069965cda8a3a5099b6bc
workflow-type: tm+mt
source-wordcount: '1623'
ht-degree: 90%

---

# リリースノート {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="リリースノート"
>abstract="Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。これにより、Campaign リリースノートは月に数回更新され、最新の機能、改善点、修正が含まれます。定期的に確認することをお勧めします。"

Adobe Campaign web ユーザーインターフェイスのリリースは、機能のデプロイメントに対してより拡張性の高い、段階的なアプローチを可能にする継続的な配信モデルに基づいて動作します。したがって、これらのリリースノートは月に数回更新されます。定期的に確認してください。

## 6 月リリースノート {#24-6-release}

**リリース日**:2024 年 6 月 18～19 日

6 月リリース以降、すべてのユーザーが次の機能および機能強化を利用できるようになります。
<!--
### Visual fragments {#24-6-1}

You can now author, use, and manage **visual** fragments to quickly assemble your emails and content templates. A fragment is a prebuilt reusable component that can be referenced in multiple emails across Adobe Campaign for an improved and accelerated design process.

### Seed lists {#24-6-2}

A seed list, aka. **Trap group**, is a list of seed addresses. It is used to include specific addresses in your deliveries, and then target profiles who do not match the defined target criteria. This way, recipients who are out of the delivery audience can receive the delivery, as any other target recipient would. You can use seed addresses when sending proofs, or to protect your mailing list.-->

### 配信アラート {#24-6-3}

配信アラート機能は、ユーザーのグループが配信の実行に関する情報を含んだ通知を自動的に受信できるようにするアラート管理システムです。 [詳細情報](../msg/delivery-alerting.md)

### プランとプログラム {#24-6-4}

これで、キャンペーンを整理するプランとプログラムを作成できます。 フォルダー階層を定義すると、キャンペーンをプログラムに、プログラムをプランに整理できます。 [詳細情報](../administration/plans-programs.md)

### 改善点 {#improvements-24-6}

* **エンリッチメントアクティビティでの紐付け**：です **エンリッチメント** アクティビティを使用して、Campaign データベーススキーマからのデータを別のスキーマからのデータや、一時スキーマからのデータ（ファイルの読み込みアクティビティを使用してアップロードされたデータなど）と紐付けることができるようになりました。 例えば、このオプションを使用して、アップロードされたファイルで指定されたプロファイルの国を、Campaign データベースの専用テーブルで使用できる国の 1 つと紐付けることができます。 [詳細情報](../workflows/activities/enrichment.md)

## 5月リリースノート {#24-5-release}

**リリース日**：2024年5月21日（PT）

次の機能と改善点は、5月のリリース以降、すべてのユーザーが使用できます。

### 監査記録  {#24-5-1}

新しい&#x200B;**監査記録**&#x200B;機能では、Adobe Campaign インスタンスに対して行われたすべてのアクションとイベントの詳細かつ時系列のレコードをリアルタイムで取得できます。これには、ワークフローのステータス、ワークフローを最後に変更したユーザー、インスタンス内でユーザーが実行したアクティビティなどのクエリに対応する、Campaign データへのすべての変更を追跡する便利なメソッドが用意されています。[詳細情報](../reporting/audit-trail.md)

### カスタムフィールド {#24-5-2}

**カスタムフィールド**&#x200B;は、Adobe Campaign コンソールを通じて標準スキーマに追加される追加属性です。Campaign web ユーザーインターフェイスでは、これらのカスタムフィールドが、プロファイルやテストプロファイルの詳細など、様々な画面に表示されるようになりました。Web ユーザーインターフェイスでは、カスタムフィールドを作成できませんが、表示方法を変更できるようになりました。[詳細情報](../administration/custom-fields.md)

### テーブル間のリンクの作成 {#24-5-3}

「**エンリッチメント**」ワークフローアクティビティで別のテーブルとのリンクを作成できるようになりました。アクティビティパラメーターの新しい「**リンクの定義**」セクションを使用して、作業用テーブルデータと Adobe Campaign データベース間のリンクを作成します。例えば、受信者のアカウント番号、国およびメールが含まれるファイルからデータを読み込む場合、プロファイル内のこの情報を更新するために国テーブルへのリンクを作成できるようになりました。[詳細情報](../workflows/activities/enrichment.md#create-links)

<!--
### Content fragments {#24-5-4}

* You can now author, use, and save **visual fragments** to quickly assemble your emails and content templates. A fragment is a prebuilt reusable component that can be referenced in multiple emails across Adobe Campaign for an improved and accelerated design process. [Learn more](../email/fragments.md)

* You can now author, use, and manage **expression fragments** to quickly build personalized content. A fragment is a prebuilt reusable component that can be referenced in multiple contents across Adobe Campaign for an improved and accelerated design process.-->


### 一般的な改善点 {#improvements-24-5}

* **ダイレクトメール** - 式エディターを活用して、ダイレクトメール抽出ファイルに表示する属性を選択できるようになりました。[詳細情報](../direct-mail/content-direct-mail.md)

* **フォルダー管理** - 親フォルダーとは異なるタイプのサブフォルダーを作成できるようになりました。[詳細情報](../get-started/permissions.md#folders)


<!--* **Execution options for workflows** - You can now define execution options for your workflows, such as the maximum duration, the affinity, or the time zone.-->

* **グローバライゼーション** - 統一されたユーザーエクスペリエンスを提供するための継続的な取り組みの一環として、Adobe Experience Cloud 製品とアプリで使用される用語を統一します。これは、オブジェクトの名前に関連する場合に「ラベル」に変更されるドイツ語の用語「Titel」に影響します。変更は、UI とドキュメントに段階的にロールアウトされます。


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
