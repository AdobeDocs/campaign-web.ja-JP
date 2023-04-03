---
audience: end-user
title: Campaign Web v8 リリースノート
description: Campaign Web v8 リリースノート
exl-id: 3d8c07be-665e-46af-ba5d-f04b25b40880
badge: label="Alpha" type="Positive"
source-git-commit: b5af5099d62e0e424fffdd8eb74d67f12777b0f2
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 99%

---


# リリースノート {#release-notes}

このページでは、Campaign Web v8 の最新の機能と改善点をすべて掲載しています。

## アルファリリース{#alpha-release}

この新しい Campaign Web インターフェイスは、現在、**アルファ実務担当者**&#x200B;のみが使用でき、次の機能が搭載されています。

**現代的で直感的な統一されたエクスペリエンス**

Campaign の新しい web UI は、すべての Adobe Experience Cloud ソリューションおよびアプリと連携して、新しいユーザーエクスペリエンスを提供します。提供される機能は次のとおりです。

* 単一の共有ユーザーセッションで新しいインターフェイスや他のアドビソリューションにアクセス
* 左側のパネルからすべてのメニューとフォルダーにアクセスできる、新しいナビゲーションエクスペリエンス
* 上部バーのソリューションと組織の切り替えボタン
* コミュニティ、ヘルプセンター、サポートへの直接アクセスを備えた統合シェルの統合
<!--
No search and pulse notifications in Alpha
-->

新しい UI について詳しくは、[このページ](../get-started/user-interface.md)を参照してください。

**メールキャンペーンの作成、開始、測定**

新しい Campaign Web UI を使用すると、次の操作を実行できます。

* パーソナライズされたメールコンテンツを電子メールデザイナーでデザイン - [詳細情報](../content/edit-content.md)
* ルールビルダーでターゲットオーディエンスを定義 - [詳細情報](../audience/about-audiences.md)
* メールメッセージのプレビュー、テスト、送信 - [詳細情報](../monitor/prepare-send.md)
* ビルトインレポートを使用した送信の監視および結果の測定 - [詳細情報](../reporting/reports.md)

<!--
add info somewhere to remind users that
* they still have access to their console (+ link to v8 console doc)
* they keep their existing data (example: will be able to use their existing delivery templates to create deliveries)
-->


## 用語の更新{#terminology-updates}

既存の Campaign ユーザーとして、一部の概念は最新の用語標準に合わせて名前が変更されています。これらの変更は Campaign Web UI にのみ適用され、クライアントコンソールには反映されません。以下を参照してください。

* 配達確認は、**テストメール**&#x200B;になりました。配達確認を送信するには、メール配信 UI の「**テスト**」ボタンを使用します。配達確認ターゲットのターゲットは、**テストプロファイル**&#x200B;と呼ばれるようになりました。
* シードアドレスは **テストプロファイル** として使用されるようになりました。データベース内の追加の架空受信者シードアドレスにテストメールを送信します。
* 配信分析は、**配信準備**&#x200B;になりました。分析を開始する必要がある場合は、「**準備**」ボタンをクリックします。
* メールのプレビューは、「**コンテンツをシミュレート**」ボタンから使用できるようになりました。
* リストは、**オーディエンス**&#x200B;になりました。

## 制限事項{#limitations-alpha}

クロスチャネルキャンペーンやワークフロー管理など、一部の Campaign 主要機能は、ベータ版リリースで利用できるようになります。

このアルファ版には、以下の制限が適用されます。

* 編集可能なオブジェクトは配信のみです。その他は読み取り専用です。フィルターを使用してすべてを参照します。
* このバージョンは、1 回限りのメールキャンペーン用に設計されています。その他のチャネルはまだサポートされていません。
* 管理ユーザーインターフェイスは使用できません。
* レポート指標（開封数やトラッキングデータなど）は、1 時間ごとに更新されます。
* 配信ダッシュボードの KPI は 5 分ごとに更新されます。- ただし、配信の準備はリアルタイムです。
* 上部のバーにある Adobe Experience Cloud 通知と統合ヘルプは、まだ統合されていません。

