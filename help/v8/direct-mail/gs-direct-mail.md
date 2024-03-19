---
audience: end-user
title: ダイレクトメール配信の概要
description: Adobe Campaign Web でダイレクトメール配信を作成して送信する方法を説明します
source-git-commit: 980c19561c9f82a22a59b626d95d72981781af54
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 1%

---


# ダイレクトメール配信の概要 {#gs-direct-mail}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="ダイレクトメール"
>abstract="ダイレクトメールチャネルは、ワークフローで、またはスタンドアロン配信として使用できるようになりました。 ダイレクトメールは、抽出ファイルの作成、パーソナライズ、生成、ダイレクトメールプロバイダーとの間での共有、顧客へのメール送信を可能にするオフラインチャネルです。"
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/release-notes/release-notes" text="リリースノートを参照してください"


ダイレクトメールは、ファイルを作成して、はがき、チラシ、カタログなどのパーソナライズされたレターを顧客に大量配信できるオフラインチャネルです。

ダイレクトメール配信を作成する際、Adobe Campaignは、すべてのターゲットプロファイルと、選択したデータ（郵送先住所、プロファイル属性など）を含む抽出ファイルを自動的に生成します。 このファイルは、選択したサーバーに送信され、選択したダイレクトメールプロバイダーがアクセスできるようになります。このプロバイダーは、実際の郵送プロセスを処理します。

ダイレクトメール配信を作成するには、次の 3 つのオプションがあります。

* **ワークフロー**：ワークフローに「ダイレクトメールチャネル」アクティビティを追加し、基本設定を指定した後、右側のウィンドウメニューからダイレクトメール配信のコンテンツを作成できます。 ワークフローの設定方法について詳しくは、 [このページ](../workflows/gs-workflow-creation.md).
* **キャンペーン**：キャンペーンを作成したら、ダイレクトメール配信を作成できます。 キャンペーンの設定について詳しくは、 [このページ](../campaigns/gs-campaigns.md).
* **スタンドアロン配信**：ワークフローやキャンペーンを使用せずに、個々のダイレクトメール配信で顧客を直接、即座にエンゲージメントします。 [配信の作成方法を説明します](../msg/gs-deliveries.md)

<!--
<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="create-push.md">
<img alt="Lead" src="assets/do-not-localize/push_create.jpeg">
</a>
<div><a href="create-push.md"><strong>Create a push delivery</strong>
</div>
<p>
</td>
<td>
<a href="content-push.md">
<img alt="Infrequent" src="assets/do-not-localize/push_design.jpeg">
</a>
<div>
<a href="content-push.md"><strong>Design a push delivery<strong></strong></a>
</div>
<p></td>
<td>
<a href="send-push.md">
<img alt="Validation" src="assets/do-not-localize/push_send.jpeg">
</a>
<div>
<a href="send-push.md"><strong>Send a push delivery</strong></a>
</div>
<p>
</td>
<td>
<a href="send-push.md">
<img alt="Validation" src="assets/do-not-localize/push_report.jpeg">
</a>
<div>
<a href="send-push.md"><strong>Push delivery report</strong></a>
</div>
<p>
</td>
</tr></table>
-->
